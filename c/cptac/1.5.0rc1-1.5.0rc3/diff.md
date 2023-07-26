# Comparing `tmp/cptac-1.5.0rc1.tar.gz` & `tmp/cptac-1.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cptac-1.5.0rc1.tar", last modified: Mon Aug  8 22:10:36 2022, max compression
+gzip compressed data, was "cptac-1.5.0rc3.tar", last modified: Wed Jul 26 22:22:56 2023, max compression
```

## Comparing `cptac-1.5.0rc1.tar` & `cptac-1.5.0rc3.tar`

### file list

```diff
@@ -1,265 +1,107 @@
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.734805 cptac-1.5.0rc1/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     3490 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     8266 2022-08-08 22:10:36.734426 cptac-1.5.0rc1/PKG-INFO
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     7114 2021-08-24 21:00:29.000000 cptac-1.5.0rc1/README.md
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.639645 cptac-1.5.0rc1/cptac/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     7286 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/__init__.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.646921 cptac-1.5.0rc1/cptac/cancers/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/__init__.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.652056 cptac-1.5.0rc1/cptac/cancers/awg/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    23610 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awgbrca.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    29485 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awgccrcc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    13300 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awgcoad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    20289 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awggbm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    16810 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awghnscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    34780 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awglscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    29996 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awgluad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    12112 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awgov.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    15260 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awgpdac.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    25523 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awg/awgucec.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.653476 cptac-1.5.0rc1/cptac/cancers/awgconf/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awgconf/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    21008 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awgconf/awgconfgbm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    27487 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/awgconf/awgconfucec.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.658249 cptac-1.5.0rc1/cptac/cancers/bcm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     4718 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmbrca.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6149 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmccrcc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     4546 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmcoad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6084 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmgbm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6187 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmhnscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6186 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmlscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6191 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmluad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     4328 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmov.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6235 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmpdac.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6195 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/bcm/bcmucec.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1962 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/brca.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.662599 cptac-1.5.0rc1/cptac/cancers/broad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6405 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadbrca.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6104 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadccrcc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6107 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadcoad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6092 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadgbm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6095 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadhnscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6106 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadlscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     7097 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadluad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6092 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadov.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6098 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broadpdac.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6999 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/broad/broaducec.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    93098 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/cancer.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1993 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/ccrcc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1962 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/coad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     2084 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/gbm.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.663611 cptac-1.5.0rc1/cptac/cancers/harmonized/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/harmonized/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     4723 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/harmonized/harmonized.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1993 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/hnscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1970 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/lscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1970 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/luad.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.664548 cptac-1.5.0rc1/cptac/cancers/mssm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/mssm/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    15760 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/mssm/mssm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1924 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/ov.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1962 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdac.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.669885 cptac-1.5.0rc1/cptac/cancers/pdc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10093 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdcbrca.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6325 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdcccrcc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     5961 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdccoad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     7505 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdcgbm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     9768 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdchnscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     9111 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdclscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10877 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdcluad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6422 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdcov.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     7514 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdcpdac.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     7402 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/pdc/pdcucec.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6850 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/source.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     2110 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/ucec.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.675366 cptac-1.5.0rc1/cptac/cancers/umich/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    12919 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichbrca.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10262 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichccrcc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    11539 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichcoad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10458 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichgbm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    12827 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichhnscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    11676 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichlscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    13199 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichluad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10620 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichov.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10273 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichpdac.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    12257 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/umich/umichucec.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.681246 cptac-1.5.0rc1/cptac/cancers/washu/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10432 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washubrca.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    14747 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washuccrcc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10625 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washucoad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    13245 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washugbm.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    15359 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washuhnscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    14634 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washulscc.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    14797 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washuluad.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    10548 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washuov.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    15372 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washupdac.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    13956 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/cancers/washu/washuucec.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.634994 cptac-1.5.0rc1/cptac/data/
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.681711 cptac-1.5.0rc1/cptac/data/data_awg_brca/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_brca/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.683143 cptac-1.5.0rc1/cptac/data/data_awg_ccrcc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_ccrcc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.683724 cptac-1.5.0rc1/cptac/data/data_awg_coad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_coad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.684162 cptac-1.5.0rc1/cptac/data/data_awg_gbm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_gbm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.684589 cptac-1.5.0rc1/cptac/data/data_awg_hnscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_hnscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.684987 cptac-1.5.0rc1/cptac/data/data_awg_lscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_lscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.685416 cptac-1.5.0rc1/cptac/data/data_awg_luad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_luad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.685813 cptac-1.5.0rc1/cptac/data/data_awg_ov/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_ov/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.686232 cptac-1.5.0rc1/cptac/data/data_awg_pdac/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_pdac/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.686645 cptac-1.5.0rc1/cptac/data/data_awg_ucec/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awg_ucec/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.687072 cptac-1.5.0rc1/cptac/data/data_awgconf_gbm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awgconf_gbm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.687487 cptac-1.5.0rc1/cptac/data/data_awgconf_ucec/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_awgconf_ucec/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.689995 cptac-1.5.0rc1/cptac/data/data_bcm_brca/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_brca/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.690483 cptac-1.5.0rc1/cptac/data/data_bcm_ccrcc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_ccrcc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.690978 cptac-1.5.0rc1/cptac/data/data_bcm_coad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_coad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.691429 cptac-1.5.0rc1/cptac/data/data_bcm_gbm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_gbm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.691890 cptac-1.5.0rc1/cptac/data/data_bcm_hnscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_hnscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.692327 cptac-1.5.0rc1/cptac/data/data_bcm_lscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_lscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.693798 cptac-1.5.0rc1/cptac/data/data_bcm_luad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_luad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.694345 cptac-1.5.0rc1/cptac/data/data_bcm_ov/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_ov/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.694817 cptac-1.5.0rc1/cptac/data/data_bcm_pdac/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_pdac/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.695246 cptac-1.5.0rc1/cptac/data/data_bcm_ucec/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_bcm_ucec/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.695664 cptac-1.5.0rc1/cptac/data/data_broad_brca/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_brca/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.696069 cptac-1.5.0rc1/cptac/data/data_broad_ccrcc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_ccrcc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.696529 cptac-1.5.0rc1/cptac/data/data_broad_coad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_coad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.696990 cptac-1.5.0rc1/cptac/data/data_broad_gbm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_gbm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.697418 cptac-1.5.0rc1/cptac/data/data_broad_hnscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_hnscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.697815 cptac-1.5.0rc1/cptac/data/data_broad_lscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_lscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.701245 cptac-1.5.0rc1/cptac/data/data_broad_luad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_luad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.702033 cptac-1.5.0rc1/cptac/data/data_broad_ov/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_ov/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.702531 cptac-1.5.0rc1/cptac/data/data_broad_pdac/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_pdac/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.703085 cptac-1.5.0rc1/cptac/data/data_broad_ucec/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      168 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_broad_ucec/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.703575 cptac-1.5.0rc1/cptac/data/data_harmonized/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_harmonized/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.703978 cptac-1.5.0rc1/cptac/data/data_mssm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_mssm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.704393 cptac-1.5.0rc1/cptac/data/data_pdc_brca/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_brca/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.705026 cptac-1.5.0rc1/cptac/data/data_pdc_ccrcc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_ccrcc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.705541 cptac-1.5.0rc1/cptac/data/data_pdc_coad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_coad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.705979 cptac-1.5.0rc1/cptac/data/data_pdc_gbm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_gbm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.706389 cptac-1.5.0rc1/cptac/data/data_pdc_hnscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_hnscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.706817 cptac-1.5.0rc1/cptac/data/data_pdc_lscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_lscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.707296 cptac-1.5.0rc1/cptac/data/data_pdc_luad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_luad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.707773 cptac-1.5.0rc1/cptac/data/data_pdc_ov/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_ov/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.708220 cptac-1.5.0rc1/cptac/data/data_pdc_pdac/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_pdac/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.708650 cptac-1.5.0rc1/cptac/data/data_pdc_ucec/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      166 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_pdc_ucec/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.709062 cptac-1.5.0rc1/cptac/data/data_umich_brca/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_brca/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.709674 cptac-1.5.0rc1/cptac/data/data_umich_ccrcc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_ccrcc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.710078 cptac-1.5.0rc1/cptac/data/data_umich_coad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_coad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.710486 cptac-1.5.0rc1/cptac/data/data_umich_gbm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_gbm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.710883 cptac-1.5.0rc1/cptac/data/data_umich_hnscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_hnscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.711338 cptac-1.5.0rc1/cptac/data/data_umich_lscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_lscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.711808 cptac-1.5.0rc1/cptac/data/data_umich_luad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_luad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.712240 cptac-1.5.0rc1/cptac/data/data_umich_ov/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_ov/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.712673 cptac-1.5.0rc1/cptac/data/data_umich_pdac/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_pdac/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.713093 cptac-1.5.0rc1/cptac/data/data_umich_ucec/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_umich_ucec/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.713504 cptac-1.5.0rc1/cptac/data/data_washu_brca/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_brca/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.713911 cptac-1.5.0rc1/cptac/data/data_washu_ccrcc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_ccrcc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.714316 cptac-1.5.0rc1/cptac/data/data_washu_coad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_coad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.714710 cptac-1.5.0rc1/cptac/data/data_washu_gbm/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_gbm/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.715124 cptac-1.5.0rc1/cptac/data/data_washu_hnscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_hnscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.715539 cptac-1.5.0rc1/cptac/data/data_washu_lscc/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_lscc/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.715981 cptac-1.5.0rc1/cptac/data/data_washu_luad/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_luad/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.716397 cptac-1.5.0rc1/cptac/data/data_washu_ov/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_ov/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.716814 cptac-1.5.0rc1/cptac/data/data_washu_pdac/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_pdac/index_urls.tsv
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.717237 cptac-1.5.0rc1/cptac/data/data_washu_ucec/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      167 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/data/data_washu_ucec/index_urls.tsv
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     5184 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/exceptions.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    20203 2022-08-08 20:22:28.000000 cptac-1.5.0rc1/cptac/gbmconf.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     5185 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/options.tsv
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    18606 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/pancan_download.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.717942 cptac-1.5.0rc1/cptac/tools/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/__init__.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.718746 cptac-1.5.0rc1/cptac/tools/auth_tools/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/auth_tools/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     3710 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/auth_tools/box_auth.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    23379 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/dataframe_tools.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.720465 cptac-1.5.0rc1/cptac/tools/download_tools/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/download_tools/__init__.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    22926 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/download_tools/box_download.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     4259 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/download_tools/download.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    13297 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/tools/download_tools/pdc_download.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.722249 cptac-1.5.0rc1/cptac/utils/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1585 2021-08-25 00:17:19.000000 cptac-1.5.0rc1/cptac/utils/__init__.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.733496 cptac-1.5.0rc1/cptac/utils/data/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)  5188159 2021-08-24 21:00:29.000000 cptac-1.5.0rc1/cptac/utils/data/BioPlex_293T_Network_10K_Dec_2019.tsv.gz
--rw-r--r--   0 robertoldroyd   (501) staff       (20)   142967 2021-08-24 21:00:29.000000 cptac-1.5.0rc1/cptac/utils/data/WikiPathwaysDataframe.tsv.gz
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    24809 2021-08-25 00:17:19.000000 cptac-1.5.0rc1/cptac/utils/other_utils.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    35798 2021-08-25 00:17:19.000000 cptac-1.5.0rc1/cptac/utils/pathway_utils.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)    16150 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/utils/stats_utils.py
--rw-r--r--   0 robertoldroyd   (501) staff       (20)       25 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/cptac/version.py
-drwxr-xr-x   0 robertoldroyd   (501) staff       (20)        0 2022-08-08 22:10:36.642070 cptac-1.5.0rc1/cptac.egg-info/
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     8266 2022-08-08 22:10:36.000000 cptac-1.5.0rc1/cptac.egg-info/PKG-INFO
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     6025 2022-08-08 22:10:36.000000 cptac-1.5.0rc1/cptac.egg-info/SOURCES.txt
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        1 2022-08-08 22:10:36.000000 cptac-1.5.0rc1/cptac.egg-info/dependency_links.txt
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        1 2021-08-25 18:59:36.000000 cptac-1.5.0rc1/cptac.egg-info/not-zip-safe
--rw-r--r--   0 robertoldroyd   (501) staff       (20)      203 2022-08-08 22:10:36.000000 cptac-1.5.0rc1/cptac.egg-info/requires.txt
--rw-r--r--   0 robertoldroyd   (501) staff       (20)        6 2022-08-08 22:10:36.000000 cptac-1.5.0rc1/cptac.egg-info/top_level.txt
--rw-r--r--   0 robertoldroyd   (501) staff       (20)       80 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/pyproject.toml
--rw-r--r--   0 robertoldroyd   (501) staff       (20)       38 2022-08-08 22:10:36.734936 cptac-1.5.0rc1/setup.cfg
--rw-r--r--   0 robertoldroyd   (501) staff       (20)     1779 2022-08-08 21:35:26.000000 cptac-1.5.0rc1/setup.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.582083 cptac-1.5.0rc3/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    10722 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/LICENSE.md
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2386 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/MANIFEST.in
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     7892 2023-07-26 22:22:56.581922 cptac-1.5.0rc3/PKG-INFO
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     7220 2023-07-21 20:36:43.000000 cptac-1.5.0rc3/README.md
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.559515 cptac-1.5.0rc3/cptac/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     6239 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/__init__.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.562837 cptac-1.5.0rc3/cptac/cancers/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/cancers/__init__.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.564749 cptac-1.5.0rc3/cptac/cancers/bcm/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/cancers/bcm/__init__.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     3581 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmbrca.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5477 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmccrcc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     3472 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmcoad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5224 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmgbm.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     4455 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmhnscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5477 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmlscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5445 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmluad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     3421 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmov.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     4590 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmpdac.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5352 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/bcm/bcmucec.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     1817 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/brca.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.566398 cptac-1.5.0rc3/cptac/cancers/broad/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/cancers/broad/__init__.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     4397 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadbrca.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5395 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadccrcc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5009 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadcoad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     4992 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadgbm.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5001 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadhnscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5195 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadlscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5934 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadluad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5323 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadov.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5659 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broadpdac.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     5285 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/broad/broaducec.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    86896 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/cancer.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2392 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/ccrcc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2363 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/coad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2347 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/gbm.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.566636 cptac-1.5.0rc3/cptac/cancers/harmonized/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/cancers/harmonized/__init__.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     4148 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/harmonized/harmonized.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2297 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/hnscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2275 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/lscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2266 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/luad.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.566864 cptac-1.5.0rc3/cptac/cancers/mssm/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/cancers/mssm/__init__.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     3605 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/mssm/mssm.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2238 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/ov.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2306 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/pdac.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     6817 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/source.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2206 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/ucec.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.568666 cptac-1.5.0rc3/cptac/cancers/umich/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/cancers/umich/__init__.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    14904 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichbrca.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    12302 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichccrcc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    13607 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichcoad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    12259 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichgbm.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    14708 2023-07-26 22:22:07.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichhnscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    13955 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichlscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    15153 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichluad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    12053 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichov.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    12315 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichpdac.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    14211 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/umich/umichucec.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.570390 cptac-1.5.0rc3/cptac/cancers/washu/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/cancers/washu/__init__.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    10735 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washubrca.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    15262 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washuccrcc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    10903 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washucoad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    13587 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washugbm.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    15936 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washuhnscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    15133 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washulscc.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    15315 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washuluad.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    11369 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washuov.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    15960 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washupdac.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    14886 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/cancers/washu/washuucec.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     4205 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/exceptions.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.570782 cptac-1.5.0rc3/cptac/tools/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        0 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/tools/__init__.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    15390 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/tools/dataframe_tools.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     7540 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/tools/download_tools.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.571721 cptac-1.5.0rc3/cptac/utils/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     1585 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/utils/__init__.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.577624 cptac-1.5.0rc3/cptac/utils/data/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)  5188159 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/utils/data/BioPlex_293T_Network_10K_Dec_2019.tsv.gz
+-rw-r--r--   0 blakemcgee   (501) staff       (20)   142967 2023-07-01 23:26:52.000000 cptac-1.5.0rc3/cptac/utils/data/WikiPathwaysDataframe.tsv.gz
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    26222 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/utils/other_utils.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    34070 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/utils/pathway_utils.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)    16178 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/cptac/utils/stats_utils.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)       25 2023-07-21 20:36:00.000000 cptac-1.5.0rc3/cptac/version.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.560407 cptac-1.5.0rc3/cptac.egg-info/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     7892 2023-07-26 22:22:56.000000 cptac-1.5.0rc3/cptac.egg-info/PKG-INFO
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     2591 2023-07-26 22:22:56.000000 cptac-1.5.0rc3/cptac.egg-info/SOURCES.txt
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        1 2023-07-26 22:22:56.000000 cptac-1.5.0rc3/cptac.egg-info/dependency_links.txt
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        1 2023-07-01 23:27:33.000000 cptac-1.5.0rc3/cptac.egg-info/not-zip-safe
+-rw-r--r--   0 blakemcgee   (501) staff       (20)      126 2023-07-26 22:22:56.000000 cptac-1.5.0rc3/cptac.egg-info/requires.txt
+-rw-r--r--   0 blakemcgee   (501) staff       (20)        6 2023-07-26 22:22:56.000000 cptac-1.5.0rc3/cptac.egg-info/top_level.txt
+-rw-r--r--   0 blakemcgee   (501) staff       (20)       80 2023-07-11 18:06:05.000000 cptac-1.5.0rc3/pyproject.toml
+-rw-r--r--   0 blakemcgee   (501) staff       (20)       38 2023-07-26 22:22:56.582135 cptac-1.5.0rc3/setup.cfg
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     1681 2023-07-21 20:44:54.000000 cptac-1.5.0rc3/setup.py
+drwxr-xr-x   0 blakemcgee   (501) staff       (20)        0 2023-07-26 22:22:56.581707 cptac-1.5.0rc3/tests/
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     1030 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/tests/test_all_datasets.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)      429 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/tests/test_consistency.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)      534 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/tests/test_data_format_and_output.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)      559 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/tests/test_datasets.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)      700 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/tests/test_error_handling.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)      184 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/tests/test_imports.py
+-rw-r--r--   0 blakemcgee   (501) staff       (20)     1418 2023-07-18 20:32:04.000000 cptac-1.5.0rc3/tests/test_join.py
```

### Comparing `cptac-1.5.0rc1/MANIFEST.in` & `cptac-1.5.0rc3/MANIFEST.in`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 # General files
 include README.md
 include cptac/options.tsv
 include cptac/utils/data/BioPlex_293T_Network_10K_Dec_2019.tsv.gz
 include cptac/utils/data/Uniprot_Proteome.tsv.gz
 include cptac/utils/data/WikiPathwaysDataframe.tsv.gz
 
-# awg files
-include cptac/data/data_awg_brca/index_urls.tsv
-include cptac/data/data_awg_ccrcc/index_urls.tsv
-include cptac/data/data_awg_coad/index_urls.tsv
-include cptac/data/data_awg_gbm/index_urls.tsv
-include cptac/data/data_awg_hnscc/index_urls.tsv
-include cptac/data/data_awg_lscc/index_urls.tsv
-include cptac/data/data_awg_luad/index_urls.tsv
-include cptac/data/data_awg_ov/index_urls.tsv
-include cptac/data/data_awg_pdac/index_urls.tsv
-include cptac/data/data_awg_ucec/index_urls.tsv
-
-# awgconf files
-include cptac/data/data_awgconf_ucec/index_urls.tsv
-include cptac/data/data_awgconf_gbm/index_urls.tsv
-
 # bcm files
 include cptac/data/data_bcm_brca/index_urls.tsv
 include cptac/data/data_bcm_ccrcc/index_urls.tsv
 include cptac/data/data_bcm_coad/index_urls.tsv
 include cptac/data/data_bcm_gbm/index_urls.tsv
 include cptac/data/data_bcm_hnscc/index_urls.tsv
 include cptac/data/data_bcm_lscc/index_urls.tsv
@@ -45,26 +29,14 @@
 include cptac/data/data_broad_pdac/index_urls.tsv
 include cptac/data/data_broad_ucec/index_urls.tsv
 
 # harmonized and mssm files
 include cptac/data/data_harmonized/index_urls.tsv
 include cptac/data/data_mssm/index_urls.tsv
 
-# pdc files
-include cptac/data/data_pdc_brca/index_urls.tsv
-include cptac/data/data_pdc_ccrcc/index_urls.tsv
-include cptac/data/data_pdc_coad/index_urls.tsv
-include cptac/data/data_pdc_gbm/index_urls.tsv
-include cptac/data/data_pdc_hnscc/index_urls.tsv
-include cptac/data/data_pdc_lscc/index_urls.tsv
-include cptac/data/data_pdc_luad/index_urls.tsv
-include cptac/data/data_pdc_ov/index_urls.tsv
-include cptac/data/data_pdc_pdac/index_urls.tsv
-include cptac/data/data_pdc_ucec/index_urls.tsv
-
 # umich files
 include cptac/data/data_umich_brca/index_urls.tsv
 include cptac/data/data_umich_ccrcc/index_urls.tsv
 include cptac/data/data_umich_coad/index_urls.tsv
 include cptac/data/data_umich_gbm/index_urls.tsv
 include cptac/data/data_umich_hnscc/index_urls.tsv
 include cptac/data/data_umich_lscc/index_urls.tsv
```

### Comparing `cptac-1.5.0rc1/PKG-INFO` & `cptac-1.5.0rc3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 Metadata-Version: 2.1
 Name: cptac
-Version: 1.5.0rc1
+Version: 1.5.0rc3
 Summary: Python packaging for CPTAC data
 Home-page: http://github.com/PayneLab/cptac
 Author: Dr. Samuel Payne
 Author-email: sam_payne@byu.edu
 License: Apache 2.0
 Project-URL: Documentation, https://paynelab.github.io/cptac/
-Description: # Easy access to CPTAC data
-        This software provides easy access to cancer data from the National Cancer Institute's CPTAC program, which characterizes and studies the proteogenomic landscape of tumors. We implement the software as a Python package called `cptac`, but you can seamlessly use it in an R environment with the help of the `reticulate` package (demonstrated in [Tutorial 6](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)). Our package is installed in one step with `pip`:
-        ```
-        pip install cptac
-        ```
-        See the [Installation section below](https://paynelab.github.io/cptac/#installation) if you have further questions.
-        
-        The package gives you the data as `pandas` `DataFrame` objects in Python. If you are using R, `reticulate` converts the tables to `data.frame` objects. By providing the tables natively in your programming environment, we eliminate the need for parsing and formatting, allowing you to quickly feed the data into whatever analysis code you have written. Follow our walkthrough tutorials and use cases for examples of how to use the software.
-        
-        Additionally, the software automatically handles data downloading, storage, and updates. You need only to tell it which datasets you want downloaded, and it will automatically get the data without requiring you to write any HTTP requests or database queries.
-        
-        ## Installation
-        This package is intended to run on Python 3.6 or greater. If you plan on interfacing with it from R via `reticulate`, you must still have Python installed on your computer, and download the package into that Python environment.
-        
-        ### Installing Python
-        If you do not already have Python installed on your computer, we suggest using either the [standard Python distribution](https://www.python.org/downloads/) or the [Anaconda distribution](https://www.anaconda.com/distribution/). Follow the installation instructions at the respective links. The Anaconda distribution allows you to set up multiple distinct Python environments and comes with many useful Python packages pre-installed. For more information, see the Ananconda documentation.
-        
-        ### Installing the cptac package
-        We distribute the package [through the Python Package Index (PyPI)](https://pypi.org/project/cptac/), so regardless of which Python distribution you are using, you install the package using the `pip` program:
-        ```
-        pip install cptac
-        ```
-        If you are using the Anaconda distribution of Python, this will install `cptac` to the currently active environment as long as `pip` is available in that environment, which it would be by default. If `pip` is not installed in your environment, you can install it with `conda install -c anaconda pip`. Then, you can use `pip` to install the `cptac` package. We plan on making `cptac` directly available through `conda` in the near future.
-        
-        The package depends on several other Python libraries including `numpy`, `pandas`, `requests`, and others. Normally, `pip` will automatically handle these dependencies when it installs `cptac` and you don't have to worry about any of it. However, if you have a special use case or are interested in exactly which versions of which packages are needed, you can consult the `install_requires` list in the [setup.py file](https://github.com/PayneLab/cptac/blob/master/setup.py).
-        
-        ## Documentation
-        Our goal is that our documentation will make this software and data accessible both to people without a computer science background, and people without a biology background. We provide two types of documentation to accomplish this: tutorials and use cases. The tutorials give a basic introduction to the software as well as conventions for storing and accessing the data. The use cases are short examples focused on a biological question and show practical uses of the software and data for biological discovery. Each use case works with a different combination of data types and explores meaningful cancer research hypotheses. 
-        
-        You can access the tutorials and use cases as static webpages using the links below. They were originally written in Python as interactive Jupyter notebooks, so if you want to run them interactively with Jupyter you can download the notebooks from the [notebooks folder](https://github.com/PayneLab/cptac/tree/master/notebooks) on the GitHub repository. If you are unfamiliar with Jupyter, follow the installation and usage instructions given [here](https://jupyter.org/install) on the Jupyter website. You will then be able to run our tutorials as interactive, exploratory data analyses. If you want to run them interactively without installing anything, please visit our Binder site which hosts the notebooks [here](https://mybinder.org/v2/gh/PayneLab/cptac/master?filepath=%2Fnotebooks).
-        
-        ### Tutorials
-        - [Tutorial 1: CPTAC data introduction](https://paynelab.github.io/cptac/tutorial01_data_intro.html)
-        - [Tutorial 2: Using pandas to work with cptac dataframes](https://paynelab.github.io/cptac/tutorial02_pandas.html)
-        - [Tutorial 3: Joining dataframes with cptac](https://paynelab.github.io/cptac/tutorial03_joining_dataframes.html)
-        - [Tutorial 4: Understanding multi-indexes](https://paynelab.github.io/cptac/tutorial04_multiindex.html)
-        - [Tutorial 5: How to keep up to date with new package and data releases](https://paynelab.github.io/cptac/tutorial05_updates.html)
-        - [Tutorial 6: Easy integration with R](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)
-        
-        ### Use cases
-        - [Use Case 1: Comparing transcriptomics and proteomics](https://paynelab.github.io/cptac/usecase01_omics.html)
-        - [Use Case 2: Correlation between clinical attributes](https://paynelab.github.io/cptac/usecase02_clinical_attributes.html)
-        - [Use Case 3: Associating clinical variables with omics data](https://paynelab.github.io/cptac/usecase03_clinical_and_acetylation.html)
-        - [Use Case 4: How Do Mutations Affect Protein Abundance?](https://paynelab.github.io/cptac/usecase04_mutations_and_omics.html)
-        - [Use Case 5: Gene Set Enrichment Analysis](https://paynelab.github.io/cptac/usecase05_enrichment_analysis.html)
-        - [Use Case 6: Comparing Derived Molecular Data with Proteomics](https://paynelab.github.io/cptac/usecase06_derived_molecular.html)
-        - [Use Case 7: Trans Genetics Effects](https://paynelab.github.io/cptac/usecase07_trans_genetic_effect.html)
-        - [Use Case 8: Outliers](https://paynelab.github.io/cptac/usecase08_outliers.html)
-        - [Use Case 9: Clinical Outcomes](https://paynelab.github.io/cptac/usecase09_clinical_outcomes.html)
-        - [Use Case 10: Pathway diagram overlay](https://paynelab.github.io/cptac/usecase10_pathway_overlay.html)
-        
-        ## Developer documentation
-        Documentation for anyone wanting to understand the internal workings of the package is available on the GitHub repository in the [devdocs folder](https://github.com/PayneLab/cptac/tree/master/devdocs).
-        
-        ## License
-        See the [LICENSE.md](https://github.com/PayneLab/cptac/blob/master/LICENSE.md) document on the GitHub repository. Please note the difference between the license as it applies to code versus data.
-        
-        ## Contact
-        This package is maintained by [the Payne lab](https://payne.byu.edu) at Brigham Young University.
-        
 Keywords: bioinformatics cancer proteomics genomics open science open data
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# CPTAC v.1.5 Release Candidate is now available
+Please report any bugs or possible improvements. Enjoy!
+
+# Easy access to CPTAC data
+This software provides easy access to cancer data from the National Cancer Institute's CPTAC program, which characterizes and studies the proteogenomic landscape of tumors. We implement the software as a Python package called `cptac`, but you can seamlessly use it in an R environment with the help of the `reticulate` package (demonstrated in [Tutorial 6](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)). Our package is installed in one step with `pip`:
+```
+pip install cptac
+```
+See the [Installation section below](https://paynelab.github.io/cptac/#installation) if you have further questions.
+
+The package gives you the data as `pandas` `DataFrame` objects in Python. If you are using R, `reticulate` converts the tables to `data.frame` objects. By providing the tables natively in your programming environment, we eliminate the need for parsing and formatting, allowing you to quickly feed the data into whatever analysis code you have written. Follow our walkthrough tutorials and use cases for examples of how to use the software.
+
+Additionally, the software automatically handles data downloading, storage, and updates. You need only to tell it which datasets you want downloaded, and it will automatically get the data without requiring you to write any HTTP requests or database queries.
+
+## Installation
+This package is intended to run on Python 3.6 or greater. If you plan on interfacing with it from R via `reticulate`, you must still have Python installed on your computer, and download the package into that Python environment.
+
+### Installing Python
+If you do not already have Python installed on your computer, we suggest using either the [standard Python distribution](https://www.python.org/downloads/) or the [Anaconda distribution](https://www.anaconda.com/distribution/). Follow the installation instructions at the respective links. The Anaconda distribution allows you to set up multiple distinct Python environments and comes with many useful Python packages pre-installed. For more information, see the Ananconda documentation.
+
+### Installing the cptac package
+We distribute the package [through the Python Package Index (PyPI)](https://pypi.org/project/cptac/), so regardless of which Python distribution you are using, you install the package using the `pip` program:
+```
+pip install cptac
+```
+If you are using the Anaconda distribution of Python, this will install `cptac` to the currently active environment as long as `pip` is available in that environment, which it would be by default. If `pip` is not installed in your environment, you can install it with `conda install -c anaconda pip`. Then, you can use `pip` to install the `cptac` package. We plan on making `cptac` directly available through `conda` in the near future.
+
+The package depends on several other Python libraries including `numpy`, `pandas`, `requests`, and others. Normally, `pip` will automatically handle these dependencies when it installs `cptac` and you don't have to worry about any of it. However, if you have a special use case or are interested in exactly which versions of which packages are needed, you can consult the `install_requires` list in the [setup.py file](https://github.com/PayneLab/cptac/blob/master/setup.py).
+
+## Documentation
+Our goal is that our documentation will make this software and data accessible both to people without a computer science background, and people without a biology background. We provide two types of documentation to accomplish this: tutorials and use cases. The tutorials give a basic introduction to the software as well as conventions for storing and accessing the data. The use cases are short examples focused on a biological question and show practical uses of the software and data for biological discovery. Each use case works with a different combination of data types and explores meaningful cancer research hypotheses. 
+
+You can access the tutorials and use cases as static webpages using the links below. They were originally written in Python as interactive Jupyter notebooks, so if you want to run them interactively with Jupyter you can download the notebooks from the [notebooks folder](https://github.com/PayneLab/cptac/tree/master/notebooks) on the GitHub repository. If you are unfamiliar with Jupyter, follow the installation and usage instructions given [here](https://jupyter.org/install) on the Jupyter website. You will then be able to run our tutorials as interactive, exploratory data analyses. If you want to run them interactively without installing anything, please visit our Binder site which hosts the notebooks [here](https://mybinder.org/v2/gh/PayneLab/cptac/master?filepath=%2Fnotebooks).
+
+### Tutorials
+- [Tutorial 1: CPTAC data introduction](https://paynelab.github.io/cptac/tutorial01_data_intro.html)
+- [Tutorial 2: Using pandas to work with cptac dataframes](https://paynelab.github.io/cptac/tutorial02_pandas.html)
+- [Tutorial 3: Joining dataframes with cptac](https://paynelab.github.io/cptac/tutorial03_joining_dataframes.html)
+- [Tutorial 4: Understanding multi-indexes](https://paynelab.github.io/cptac/tutorial04_multiindex.html)
+- [Tutorial 5: How to keep up to date with new package and data releases](https://paynelab.github.io/cptac/tutorial05_updates.html)
+- [Tutorial 6: Easy integration with R](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)
+
+### Use cases
+- [Use Case 1: Comparing transcriptomics and proteomics](https://paynelab.github.io/cptac/usecase01_omics.html)
+- [Use Case 2: Correlation between clinical attributes](https://paynelab.github.io/cptac/usecase02_clinical_attributes.html)
+- [Use Case 3: Associating clinical variables with omics data](https://paynelab.github.io/cptac/usecase03_clinical_and_acetylation.html)
+- [Use Case 4: How Do Mutations Affect Protein Abundance?](https://paynelab.github.io/cptac/usecase04_mutations_and_omics.html)
+- [Use Case 5: Gene Set Enrichment Analysis](https://paynelab.github.io/cptac/usecase05_enrichment_analysis.html)
+- [Use Case 6: Comparing Derived Molecular Data with Proteomics](https://paynelab.github.io/cptac/usecase06_derived_molecular.html)
+- [Use Case 7: Trans Genetics Effects](https://paynelab.github.io/cptac/usecase07_trans_genetic_effect.html)
+- [Use Case 8: Outliers](https://paynelab.github.io/cptac/usecase08_outliers.html)
+- [Use Case 9: Clinical Outcomes](https://paynelab.github.io/cptac/usecase09_clinical_outcomes.html)
+- [Use Case 10: Pathway diagram overlay](https://paynelab.github.io/cptac/usecase10_pathway_overlay.html)
+
+## Developer documentation
+Documentation for anyone wanting to understand the internal workings of the package is available on the GitHub repository in the [devdocs folder](https://github.com/PayneLab/cptac/tree/master/devdocs).
+
+## License
+See the [LICENSE.md](https://github.com/PayneLab/cptac/blob/master/LICENSE.md) document on the GitHub repository. Please note the difference between the license as it applies to code versus data.
+
+## Contact
+This package is maintained by [the Payne lab](https://payne.byu.edu) at Brigham Young University.
```

### Comparing `cptac-1.5.0rc1/README.md` & `cptac-1.5.0rc3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# CPTAC v.1.5 Release Candidate is now available
+Please report any bugs or possible improvements. Enjoy!
+
 # Easy access to CPTAC data
 This software provides easy access to cancer data from the National Cancer Institute's CPTAC program, which characterizes and studies the proteogenomic landscape of tumors. We implement the software as a Python package called `cptac`, but you can seamlessly use it in an R environment with the help of the `reticulate` package (demonstrated in [Tutorial 6](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)). Our package is installed in one step with `pip`:
 ```
 pip install cptac
 ```
 See the [Installation section below](https://paynelab.github.io/cptac/#installation) if you have further questions.
```

### Comparing `cptac-1.5.0rc1/cptac/__init__.py` & `cptac-1.5.0rc3/cptac/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,167 +7,140 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import os.path as path
 import sys
-import threading
 import warnings
-import webbrowser
 import pandas as pd
 
 # cptac base path
 CPTAC_BASE_DIR = path.abspath(path.dirname(__file__))
 
 # Function imports
-from cptac.tools.download_tools.download import download
-from cptac.tools.download_tools.box_download import download_text as _download_text
-from cptac.exceptions import CptacError, CptacWarning, InvalidParameterError, NoInternetError, OldPackageVersionWarning
+from cptac.tools.download_tools import download, init_files
+from cptac.exceptions import CptacError, CptacWarning, NoInternetError
+from cptac.utils.other_utils import df_to_tree
 
 # Dataset imports
 from cptac.cancers.brca import Brca
 from cptac.cancers.ccrcc import Ccrcc
 from cptac.cancers.coad import Coad
 from cptac.cancers.gbm import Gbm
 from cptac.cancers.hnscc import Hnscc
 from cptac.cancers.lscc import Lscc
 from cptac.cancers.luad import Luad
 from cptac.cancers.ov import Ov
 from cptac.cancers.pdac import Pdac
 from cptac.cancers.ucec import Ucec
 
-# auth import
-from cptac.tools.auth_tools.box_auth import BoxAuth
-box_auth = BoxAuth()
 
-#### This code generates the __OPTIONS__ dataframe which shows all possible cancer, source, datatype combinations
+#### Create custom exception and warning hooks to simplify error messages for new users
+def _exception_handler(exception_type, exception, traceback, default_hook=sys.excepthook): 
+    """Catch cptac-generated exceptions, and make them prettier."""
+    if issubclass(type(exception), CptacError):
+        print(f"cptac error: {str(exception)} ({traceback.tb_frame.f_code.co_filename}, line {traceback.tb_lineno})", file=sys.stderr)
+    else:
+        default_hook(exception_type, exception, traceback)
+
+def _warning_displayer(message, category, filename, lineno, file=None, line=None, default_displayer=warnings.showwarning):
+    """Catch cptac-generated warnings and make them prettier."""
+    if issubclass(category, CptacWarning):
+        print(f"cptac warning: {str(message)} ({filename}, line {lineno})", file=sys.stderr)
+    else:
+        default_displayer(message, category, filename, lineno, file, line)
+
+sys.excepthook = _exception_handler
+warnings.showwarning = _warning_displayer
+warnings.simplefilter("always", category=CptacWarning)
+
+#### Create the index for the data files (file lookup table)
+try:
+    init_files()
+except NoInternetError:
+    if path.exists(path.join(CPTAC_BASE_DIR, 'data', 'index.tsv')):
+        pass
+    else:
+        raise NoInternetError("Unable to initialize cptac without index file. Please run the package at least once with an internet connection.")
+INDEX = pd.read_csv(path.join(CPTAC_BASE_DIR, 'data', 'index.tsv'), sep='\t')
+
+#### Generates the OPTIONS dataframe which shows all possible cancer, source, datatype combinations
 def _load_options():
     """Load the tsv file with all the possible cancer, source, datatype combinations"""
-    options_file = path.join(CPTAC_BASE_DIR, "options.tsv")
-    df = pd.read_csv(options_file, sep="\t")
-    return df
-
-__OPTIONS__ = _load_options()
+    options_df = pd.DataFrame(INDEX['description'].str.split('-').tolist())
+    options_df.columns = ['Source', 'Cancer', 'Datatype']
+    options_df = options_df[['Cancer', 'Source', 'Datatype']]
+    # options_df.loc[options_df.iloc[:2].str.contains('miRNA')] = 'miRNA' # condense all forms of micro RNA
+    # options_df = options_df.unique().reset_index(drop=True)
+    return options_df
+
+OPTIONS = _load_options()
+
+def list_datasets(*, condense_on = None, column_order = None, print_tree=False):
+    """
+    List all available datasets.
+    
+    :param condense_on (list): A list of column names. Values in selected columns will be aggregated into a list.
+    :param print_tree (bool): If True, returns the database split in a pretty tree.
+    """
+    df = OPTIONS.copy()
+    df = df[df['Datatype'] != 'mapping'].reset_index(drop=True)
+    if column_order is None:
+        column_order = df.columns
+    if type(condense_on) == list:
+        group_on_cols = [col for col in column_order if col not in condense_on]
+        df = df.groupby(group_on_cols).agg({col: lambda x: list(set(x)) for col in condense_on})
+    else:
+        df = df[column_order]
 
-def get_options():
-    return __OPTIONS__.copy()
+    return df if not print_tree else df_to_tree(df)
 
 def get_cancer_options():
-    df = __OPTIONS__.copy()
-    return df["Cancers"].unique()
+    return list_datasets(condense_on=['Datatype'])
 
+def get_cancer_info():
+    cancer_abbreviations = {
+        "brca": "Breast invasive carcinoma",
+        "ccrcc": "Clear cell renal cell carcinoma",
+        "coad": "Colon adenocarcinoma",
+        "gbm": "Glioblastoma multiforme",
+        "hnscc": "Head and Neck squamous cell carcinoma",
+        "lscc": "Lung squamous cell carcinoma",
+        "luad": "Lung adenocarcinoma",
+        "ov": "Ovarian serous cystadenocarcinoma",
+        "pda": "Pancreatic ductal adenocarcinoma",
+        "pdac": "Pancreatic ductal adenocarcinoma",
+        "ucec": "Uterine Corpus Endometrial Carcinoma",
+        # Add more if needed
+    }
+    return cancer_abbreviations
+    
 def get_source_options():
-    df = __OPTIONS__.copy()
-    return df["Sources"].unique()
-
-def list_datasets():
-    """List all available datasets."""
-    df = __OPTIONS__.\
-    copy().\
-    drop("Loadable datatypes", axis=1)
-
-    df = df.\
-    assign(Datatypes=df["Datatypes"].str.split("\ *,\ *", expand=False, regex=True)).\
-    explode("Datatypes").\
-    reset_index(drop=True)
-
-    # Print our dataframe as a pretty tree structure
-    info = {}
-    for row in df.set_index(["Cancers", "Sources", "Datatypes"]).index.values:
-        if row[0] not in info.keys():
-            info[row[0]] = {}
-        if row[1] not in info[row[0]].keys():
-            info[row[0]][row[1]] = []
-        info[row[0]][row[1]].append(row[2])
-
-    df_tree = _tree(info)
-    print(df_tree)
-
-    #if the dataframe is needed it can be returned. If not,
-    #the python interpreter will print anything that is returned, so no return for now
-    #return df
-
-def _tree(nest, prepend=""):
-    """Recursively build a formatted string to represent a dictionary"""
-    tree_str = ""
-    if isinstance(nest, dict):
-        for i, (k, v) in enumerate(nest.items()):
-            if i == len(nest.keys()) - 1:
-                branch = "└"
-                newprepend = prepend + "    "
-            else:
-                branch = "├"
-                newprepend = prepend + "│   "
-            tree_str += f"{prepend}{branch}── {k}\n"
-            tree_str += _tree(nest=v, prepend=newprepend)
-    elif isinstance(nest, list):
-        for i, v in enumerate(nest):
-            if i == len(nest) - 1:
-                branch = "└"
-            else:
-                branch = "├"
-            tree_str += f"{prepend}{branch}── {v}\n"
-    else:
-        raise ValueError(f"Unexpected type '{type(nest)}'")
+    return list_datasets(condense_on=['Cancer'], column_order=['Source', 'Datatype', 'Cancer'])
 
-    return tree_str
+def get_datatype_options():
+    return list_datasets(condense_on=['Cancer'], column_order=['Datatype', 'Source', 'Cancer'])
 
 #### End __OPTIONS__ code
 
-def embargo():
-    """Open CPTAC embargo details in web browser."""
-    message = "Opening embargo details in web browser..."
-    print(message, end = '\r')
-    webbrowser.open("https://proteomics.cancer.gov/data-portal/about/data-use-agreement")
-    print(" " * len(message), end='\r') # Erase the message
+# This website no longer works
+# def embargo():
+#     """Open CPTAC embargo details in web browser."""
+#     message = "Opening embargo details in web browser..."
+#     print(message, end = '\r')
+#     webbrowser.open("https://proteomics.cancer.gov/data-portal/about/data-use-agreement")
+#     print(" " * len(message), end='\r') # Erase the message
 
 def version():
     """Return version number of cptac package."""
     version = {}
     version_path = path.join(CPTAC_BASE_DIR, "version.py")
     with open(version_path) as fp:
         exec(fp.read(), version)
     return version['__version__']
 
 def how_to_cite():
     """Give instructions for citing CPTAC datasets."""
     print("If you use the API to generate results, please cite our manuscript describing the API - Lindgren et al. 2021, PMID:33560848, https://pubs.acs.org/doi/10.1021/acs.jproteome.0c00919")
     print('\n')
-    print("For instructions on how to cite a specific dataset, please call its how_to_cite method, e.g. cptac.Endometrial().how_to_cite()")
-
-#### Helper functions for handling exceptions and warnings
-
-# Because Python binds default arguments when the function is defined,
-# default_hook's default will always refer to the original sys.excepthook
-def _exception_handler(exception_type, exception, traceback, default_hook=sys.excepthook): 
-    """Catch cptac-generated exceptions, and make them prettier."""
-    if issubclass(type(exception), CptacError):
-        print(f"cptac error: {str(exception)} ({traceback.tb_frame.f_code.co_filename}, line {traceback.tb_lineno})", file=sys.stderr) # We still send to stderr
-    else:
-        default_hook(exception_type, exception, traceback) # This way, exceptions from other packages will still be treated the same way
-
-def _warning_displayer(message, category, filename, lineno, file=None, line=None, default_displayer=warnings.showwarning): # Python binds default arguments when the function is defined, so default_displayer's default will always refer to the original warnings.showwarning
-    """Catch cptac-generated warnings and make them prettier."""
-    if issubclass(category, CptacWarning):
-        print(f"cptac warning: {str(message)} ({filename}, line {lineno})", file=sys.stderr) # We still send to stderr
-    else:
-        default_displayer(message, category, filename, lineno, file, line) # This way, warnings from other packages will still be displayed the same way
-
-sys.excepthook = _exception_handler # Set our custom exception hook
-warnings.showwarning = _warning_displayer # And our custom warning displayer
-warnings.simplefilter("always", category=CptacWarning) # Edit the warnings filter to show multiple occurences of cptac-generated warnings
-
-def check_version():
-    """Check in background whether the package is up-to-date"""
-    version_url = "https://byu.box.com/shared/static/kbwivmqnrdnn5im2gu6khoybk5a3rfl0.txt"
-    try:
-        remote_version = _download_text(version_url)
-    except NoInternetError:
-        pass
-    else:
-        local_version = version()
-        if remote_version != local_version:
-            warnings.warn(f"Your version of cptac ({local_version}) is out-of-date. Latest is {remote_version}. Please run 'pip install --upgrade cptac' to update it.", OldPackageVersionWarning, stacklevel=2)
-
-version_check_thread = threading.Thread(target=check_version)
-version_check_thread.start() # We don't join because we want this to just finish in the background and not block the main thread
+    print("For instructions on how to cite a specific dataset, please call its how_to_cite method, e.g. cptac.Endometrial().how_to_cite()")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/awg/awgcoad.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washuluad.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,252 +6,316 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
 import os
-import warnings
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, ReindexMapError
+from cptac.cancers.mssm.mssm import Mssm
 
-class AwgCoad(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Load all of the colon dataframes as values in the self._data dict variable, with names as keys, and format them properly.
+class WashuLuad(Source):
+    def __init__(self, no_internet=False):
+        """Load all of the washuluad dataframes as values in the self._data dict variable, with names as keys, and format them properly.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        self.valid_versions = ["0.0", "0.0.1"] # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-
         self.data_files = {
-            "0.0": {
-                "annotation"              : "clinical.tsi.gz",
-                "miRNA"                   : "miRNA.cct.gz",
-                "somatic_mutation_binary" : "mutation_binary.cbt.gz",
-                "somatic_mutation"        : "mutation.txt.gz",
-                "phosphoproteomics"       : ["phosphoproteomics_normal.gz", "phosphoproteomics_tumor.gz"],
-                "proteomics"              : ["proteomics_normal.cct.gz", "proteomics_tumor.cct.gz"],
-                "transcriptomics"         : "transcriptomics.gz"},
-            "0.0.1": {
-                "annotation"              : "clinical.tsi.gz",
-                "followup"                : "Colon_One_Year_Clinical_Data_20160927.xls",
-                "CNV"                     : "Human__CPTAC_COAD__VU__SCNA__ExomeSeq__01_28_2016__BCM__Gene__BCM_CopyWriteR_GISTIC2.cct.gz",
-                "miRNA"                   : "miRNA.cct.gz",
-                "somatic_mutation_binary" : "mutation_binary.cbt.gz",
-                "somatic_mutation"        : "mutation.txt.gz",
-                "phosphoproteomics"       : ["phosphoproteomics_normal.gz", "phosphoproteomics_tumor.gz"],
-                "proteomics"              : ["proteomics_normal.cct.gz", "proteomics_tumor.cct.gz"],
-                "transcriptomics"         : "transcriptomics.gz"},
+            "cibersort"         : "CIBERSORT.Output_Abs_LUAD.txt.gz",
+            "CNV"               : "LUAD.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            "miRNA"             : ["LUAD_mature_miRNA_combined.tsv.gz","LUAD_precursor_miRNA_combined.tsv.gz","LUAD_total_miRNA_combined.tsv.gz"],
+            # "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
+            "somatic_mutation"  : "LUAD_discovery.dnp.annotated.exonic.maf.gz",
+            "transcriptomics"   : ["LUAD_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz", "LUAD_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "LUAD_xCell.txt.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
+        #self._readme_files = {}
+
         self.load_functions = {
-            "clinical"                  : self.load_annotation,
-            "CNV"                       : self.load_CNV,
-            "derived_molecular"         : self.load_annotation,
-            "followup"                  : self.load_followup,
-            "miRNA"                     : self.load_miRNA,
-            "phosphoproteomics"         : self.load_phosphoproteomics,
-            "proteomics"                : self.load_proteomics,
-            "somatic_mutation"          : self.load_somatic_mutation,
-            "somatic_mutation_binary"   : self.load_somatic_mutation_binary,
-            "transcriptomics"           : self.load_transcriptomics,
+            'transcriptomics'   : self.load_transcriptomics,
+            'somatic_mutation'  : self.load_somatic_mutation,
+            'miRNA'             : self.load_miRNA,
+            'xcell'             : self.load_xcell,
+            'cibersort'         : self.load_cibersort,
+            'CNV'               : self.load_CNV,
+            'tumor_purity'      : self.load_tumor_purity,
+            # 'readme'            : self.load_readme,
+            "hla_typing": self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
-        super().__init__(cancer_type="coad", source='awg', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-
-    # Overload the default how_to_cite function, to provide the specific publication information for the Colon dataset
-    def how_to_cite(self):
-        """Print instructions for citing the data."""
-        super().how_to_cite(cancer_type='colorectal cancer', pmid=31031003)
-
-    def load_annotation(self):
-        if 'clinical' not in self._data or 'derived_molecular' not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files('annotation')
-
-            df = pd.read_csv(file_path, sep='\t',index_col=0)
-            df = df.sort_index()
-            df = df.transpose()
-
-            # Separate clinical and derived molecular dataframes
-            clinical = df.drop(columns=['StromalScore', 'ImmuneScore', 'ESTIMATEScore', 'TumorPurity','immuneSubtype', 'CIN', 'Integrated.Phenotype', 'Transcriptomic_subtype', 'Proteomic_subtype', 'mutation_rate', 'Mutation_Phenotype'])
-            derived_molecular = df[['StromalScore', 'ImmuneScore', 'ESTIMATEScore', 'TumorPurity', 'immuneSubtype', 'CIN', 'Integrated.Phenotype', 'Transcriptomic_subtype', 'Proteomic_subtype', 'mutation_rate', 'Mutation_Phenotype']]
-
-            # Format the dataframes
-            clinical = clinical.apply(pd.to_numeric, errors="ignore")
-            derived_molecular = derived_molecular.apply(pd.to_numeric, errors="ignore")
-            derived_molecular = derived_molecular.sort_index(axis="columns")
-
-            # save dataframes into self._data
-            self.save_df('clinical', clinical)
-            self.save_df('derived_molecular', derived_molecular)
+        # Call the parent class __init__ function
+        super().__init__(cancer_type="luad", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-    def load_CNV(self):
-        df_type = 'CNV'
+    def load_transcriptomics(self):
+        df_type = 'transcriptomics'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files(df_type)
+            file_path_list = self.locate_files(df_type)
+            # loop over list of file paths
+            for file_path in file_path_list:
+                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
+                file_name = os.path.basename(file_path)
 
-            df = pd.read_csv(file_path, sep='\t',index_col=0)
-            df = df.sort_index()
-            df = df.transpose()
-            # save df in self._data
-            self.save_df(df_type, df)
+                if file_name == "LUAD_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df = pd.read_csv(file_path, sep="\t")
+                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+                    df = df.set_index(["Name", "Database_ID"])
+                    df = df.sort_index()
+                    df = df.T
+                    df.index.name = "Patient_ID"
+                    df.index = df.index.str.replace(r"-T", "", regex=True) #remove label for tumor samples
+                    self._helper_tables["transcriptomics_tumor"] = df
+                    
+                if file_name == "LUAD_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df = pd.read_csv(file_path, sep="\t")
+                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+                    df = df.set_index(["Name", "Database_ID"])
+                    df = df.sort_index()
+                    df = df.T
+                    df.index.name = "Patient_ID"
+                    df.index = df.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
+                    self._helper_tables["transcriptomics_normal"] = df
+            
+            # Combine the two transcriptomics dataframes
+            rna_tumor = self._helper_tables.get("transcriptomics_tumor")
+            rna_normal = self._helper_tables.get("transcriptomics_normal") # Normal entries are already marked with 'N' on the end of the ID
+            if rna_tumor is None or rna_normal is None:
+                print("rna_tumor or rna_normal is None")
+                return
+            if not isinstance(rna_tumor, pd.DataFrame) or not isinstance(rna_normal, pd.DataFrame):
+                print("rna_tumor or rna_normal is not a DataFrame")
+                return
+       
+            rna_combined = pd.concat([rna_tumor, rna_normal])
 
-    def load_followup(self):
-        df_type = 'followup'
+            # save df in self._data
+            self.save_df(df_type, rna_combined)
+    
+    def load_somatic_mutation(self):
+        df_type = 'somatic_mutation'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            # parse followup file
-            df = pd.read_excel(file_path)
-            # Replace redundant values for "not reported" with NaN
-            nan_equivalents = ['Not Reported/ Unknown', 'Reported/ Unknown', 'Not Applicable',
-                'na', 'unknown', 'Not Performed', 'Unknown tumor status']
+            df = pd.read_csv(file_path, sep='\t', dtype={"PUBMED": "O"})    
+            # Rename the columns we want to keep to the appropriate names
+            df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
+            df = df.rename(columns={
+                        "Hugo_Symbol":"Gene",
+                        "Gene":"Gene_Database_ID",
+                        "Variant_Classification":"Mutation",
+                        "HGVSp_Short":"Location"})
 
-            df = df.replace(nan_equivalents, np.nan)
-
-            # Rename and set index
-            df = df.rename(columns={'PPID': 'Patient_ID'})
             df = df.set_index("Patient_ID")
-            df = df.sort_index()
-
+            df = df[ ['Gene'] + ["Mutation"] + ["Location"] + [ col for col in df.columns if col not in ["Gene","Mutation","Location"] ] ]
+            df.index = df.index.str.replace(r"_T", "", regex=True)     
             # save df in self._data
             self.save_df(df_type, df)
 
     def load_miRNA(self):
-        df_type = 'miRNA'
+        self.load_precursor_miRNA()
+        self.load_mature_miRNA()
+        self.load_total_mRNA()
+
+    def load_precursor_miRNA(self):
+        df_type = 'precursor_miRNA'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t',index_col=0)
-            df = df.sort_index()
+            df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
+            df.index = df.index.str.replace('\.T$','', regex = True)
+            df.index = df.index.str.replace('\.A$','.N', regex = True)
+            df.index.name = 'Patient_ID'                
+            # Sort
+            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
+            normal = normal.sort_values(by=["Patient_ID"])
+            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
+            tumor = tumor.sort_values(by=["Patient_ID"])
+            all_df = pd.concat([tumor, normal])
             # save df in self._data
-            self.save_df(df_type, df)
+            self.save_df(df_type, all_df)
 
-    def load_phosphoproteomics(self):
-        df_type = 'phosphoproteomics'
+    def load_mature_miRNA(self):
+        df_type = 'mature_miRNA'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
-            file_paths = self.locate_files(df_type)
-
-            phosphoproteomics_dfs = {}
-            for file_path in file_paths:
-                file_name = file_path.split(os.sep)[-1]
-                df = pd.read_csv(file_path, sep='\t',index_col=0)
-                df = df.sort_index()
-                df = df.transpose()
-
-                if file_name == "phosphoproteomics_normal.gz":
-                    phosphoproteomics_dfs["normal"] = df
-                else:
-                    phosphoproteomics_dfs["tumor"] = df
-
-            # Get phosphoproteomics dataframes, so we can process and combine them
-            phos_tumor = phosphoproteomics_dfs["tumor"]
-            phos_normal = phosphoproteomics_dfs["normal"]
-
-            # Mark entries in phosphoproteomics_normal dataframe with .N at the end of the ID
-            phos_normal = phos_normal.set_index(phos_normal.index + '.N')
-
-            # Combine the two phosphoproteomics dataframes into one dataframe
-            phos_combined = pd.concat([phos_tumor, phos_normal])
-
-            # Create our phosphoproteomics columns multiindex
-            multiindex = phos_combined.columns.str.split('[_:]', expand=True) # Split the column names into their constituent parts
-            multiindex = multiindex.droplevel([2, 4]) # The third level is just empty strings, and the fifth is a duplicate of the second
-            multiindex = multiindex.set_names(["Name", "Site", "Database_ID"])
-            phos_combined.columns = multiindex
-            phos_combined = phos_combined.sort_index(axis=1) # Put all the columns in alphabetical order
+            file_path = self.locate_files(df_type)
+            
+            df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias', 'Derives_from'])
+            df = df.transpose()
+            df.index = df.index.str.replace('\.T$','', regex = True)
+            df.index = df.index.str.replace('\.A$','.N', regex = True)
+            df.index.name = 'Patient_ID'                
+            # Sort
+            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
+            normal = normal.sort_values(by=["Patient_ID"])
+            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
+            tumor = tumor.sort_values(by=["Patient_ID"])
+            all_df = pd.concat([tumor, normal])
+            # save df in self._data
+            self.save_df(df_type, all_df)
 
-            # save dataframe in self._data
-            self.save_df(df_type, phos_combined)
+    def load_total_mRNA(self):
+        df_type = 'total_miRNA'
+        if df_type not in self._data:
+            file_path = self.locate_files(df_type)
+            
+            df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
+            df = df.transpose()
+            df.index = df.index.str.replace('\.T$','', regex = True)
+            df.index = df.index.str.replace('\.A$','.N', regex = True)
+            df.index.name = 'Patient_ID'                
+            # Sort
+            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
+            normal = normal.sort_values(by=["Patient_ID"])
+            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
+            tumor = tumor.sort_values(by=["Patient_ID"])
+            all_df = pd.concat([tumor, normal])
+            # save df in self._data
+            self.save_df(df_type, all_df)
 
-    def load_proteomics(self):
-        df_type = 'proteomics'
+    def load_xcell(self):
+        df_type = 'xcell'
         if df_type not in self._data:
+            file_path = self.locate_files(df_type)
 
-            file_path_list = self.locate_files(df_type)
+            df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
+            df = df.transpose()
+            df.columns.name = 'Name'
+            df.index.name = 'Patient_ID'
+            df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
+            df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
+            # save df in self._data
+            self.save_df(df_type, df)
 
-            for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+    def load_cibersort(self):
+        df_type = 'cibersort'
+        if df_type not in self._data:
+            file_path = self.locate_files(df_type)
 
-                if file_name == "proteomics_normal.cct.gz":
-                    df_normal = pd.read_csv(file_path, sep='\t', index_col=0)
-                    df_normal = df_normal.sort_index()
-                    df_normal = df_normal.transpose()
-                    # append .N to patient ids from the normal table
-                    df_normal = df_normal.rename(index=lambda s: s + ".N")
-
-                if file_name == "proteomics_tumor.cct.gz":
-                    df_tumor = pd.read_csv(file_path, sep='\t', index_col=0)
-                    df_tumor = df_tumor.sort_index()
-                    df_tumor = df_tumor.transpose()
-
-            # merge tumor and normal data
-            df_combined = pd.concat([df_normal, df_tumor])
-            df_combined.index.name = "Patient_ID"
-            df_combined.columns.name = "Name"
+            df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
+            df.index.name = 'Patient_ID'
+            df.columns.name = 'Name'
+            df.index = df.index.str.replace(r'-T$', '', regex=True) 
+            df.index = df.index.str.replace(r'-A$', '.N', regex=True)
+            # save df in self._data
+            self.save_df(df_type, df)
 
-            # save dataframe in self._data
-            self.save_df(df_type, df_combined)
+    def load_mapping(self):
+        df_type = 'mapping'
+        if "CNV_gene_ids" not in self._helper_tables:
+            file_path = self.locate_files(df_type)
 
-    def load_somatic_mutation(self):
-        df_type = 'somatic_mutation'
+            df = read_gtf(file_path)
+            df = df.as_df()
+            df = df[["gene_name","gene_id"]]
+            df = df.drop_duplicates()
+            df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+            df = df.set_index("Name")
+            self._helper_tables["CNV_gene_ids"] = df 
+
+    def load_CNV(self):
+        df_type = 'CNV'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t',index_col=0)
-            df = df.sort_index()
-            df = df.sort_values(by="SampleID")
+            df = pd.read_csv(file_path, sep="\t")
+            df = df.rename(columns={"Gene": "Name"})
+            df = df.set_index("Name")
+            cnv = df
+
+            self.load_mapping()
+            gene_ids = self._helper_tables["CNV_gene_ids"]
+            df = cnv.join(gene_ids,how = "left") #merge in gene_ids 
             df = df.reset_index()
-            df = df[["SampleID","Gene","Variant_Type","Protein_Change"]]
-            df = df.drop_duplicates(keep="first") # Get rid of rows that are now duplicates since we didn't keep the mRNA column. We do this before setting the index, because drop_duplicates doesn't consider the index.
-            df = df.rename(columns={"SampleID":"Patient_ID", "Variant_Type":"Mutation", "Protein_Change":"Location"})
-            df = df.sort_values(by=["Patient_ID", "Gene"])
-            df = df.set_index("Patient_ID") # We only do this after the drop_duplicates call above because drop_duplicates doesn't consider the index, but we of course want the Patient_ID to be considered when identifying duplicate rows to drop.
-
+            df = df.set_index(["Name", "Database_ID"]) #create multi-index
+            df = df.T
+            df.index.name = 'Patient_ID'
             # save df in self._data
             self.save_df(df_type, df)
 
-    def load_somatic_mutation_binary(self):
-        df_type = 'somatic_mutation_binary'
+    def load_tumor_purity(self):
+        df_type = 'tumor_purity'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t',index_col=0)
-            df = df.sort_index()
-            df = df.transpose()
+            df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
+            df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
+            df = df.set_index('Sample_ID') 
+            df.index.name = 'Patient_ID'
+
+            # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
+            mssmclin = Mssm(filter_type='luad', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')               
+            patient_ids = clinical_df.index.to_list()
+            df = df.loc[df.index.isin(patient_ids)]
 
             # save df in self._data
             self.save_df(df_type, df)
 
-    def load_transcriptomics(self):
-        df_type = 'transcriptomics'
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
+            # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t',index_col=0)
-            df = df.sort_index()
-            df = df.transpose()
-            # save df in self._data
-            self.save_df(df_type, df)
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
+
+    # def load_readme(self):
+    #     df_type = 'readme'
+    #     if not self._readme_files:
+    #         file_path_list = self.locate_files(df_type)
+    #         # loop over list of file paths
+    #         for file_path in file_path_list:
+    #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
+    #             file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+
+    #             if file_name == "README_miRNA":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_miRNA"] = reader.read()
+                        
+    #             elif file_name == "README_CIBERSORT":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_cibersort"] = reader.read()
+                        
+    #             elif file_name == "README_xCell":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_xcell"] = reader.read()
+                
+    #             elif file_name == "README_somatic_mutation_WXS":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_somatic_mutation"] = reader.read()
+                        
+    #             elif file_name == "README_gene_expression":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_transcriptomics"] = reader.read()
+                
+    #             elif file_name == "README.boxnote":
+    #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
+
+    #             elif file_name == "README_ESTIMATE_WashU":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/awg/awghnscc.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washuccrcc.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,342 +6,314 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
 import os
-import warnings
-import datetime
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, ReindexMapError, PublicationEmbargoWarning
+from cptac.cancers.mssm.mssm import Mssm
 
-class AwgHnscc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Load all of the hnscc dataframes as values in the self._data dict variable, with names as keys, and format them properly.
+class WashuCcrcc(Source):
+    def __init__(self, no_internet=False):
+        """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        self.valid_versions = ["0.1", "2.0"] # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-
         self.data_files = {
-            "0.1": {
-                "somatic_mutation"  : "HNSCC.strelka.sorted.filtered.annovar.hg19_multianno_filtered.maf.txt.gz",
-                "proteomics"        : ["Proteomics_DIA_Gene_level_Normal.cct.gz", "Proteomics_DIA_Gene_level_Tumor.cct.gz"],
-                "transcriptomics"   : "RNAseq_RSEM_UQ_log2.cct.gz",
-                "circular_RNA"      : "RNAseq_circ_RSEM_UQ_log2.cct.gz",
-                "CNV"               : "SCNA_gene_level.cct.gz",
-                "annotation"        : "clinic.tsi.gz"},
-            "2.0": {
-                "circular_RNA"      : "circRNAseq_RSEM_UQ_log2_Combined.cct.gz",
-                "followup"          : "HN_followUp_9_24.xlsx",
-                "annotation"        : "Meta_table.tsv.gz",
-                "miRNA"             : "microRNA_log2_Combined.cct.gz",
-                "phosphoproteomics" : "Phosphoproteomics_TMT_site_level_combined_all.cct.gz",
-                "proteomics"        : "Proteomics_TMT_gene_level_combined_all.cct.gz",
-                "transcriptomics"   : "RNAseq_RSEM_UQ_Combined.cct.gz",
-                "CNV"               : "SCNA_log2_gene_level.cct.gz",
-                "somatic_mutation"  : "SomaticMutations_maf.tsv.gz"},
+            "cibersort"         : "CIBERSORT.Output_Abs_ccRCC.txt.gz",
+            "CNV"               : "ccRCC.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            "miRNA"             : ["ccRCC_precursor_miRNA_combined.tsv.gz", "ccRCC_mature_miRNA_combined.tsv.gz", "ccRCC_total_miRNA_combined.tsv.gz"],
+            # "readme"            : ["README_miRNA", "README_CIBERSORT", "README_xCell", "README_somatic_mutation_WXS", "README_gene_expression", "README.boxnote", "README_ESTIMATE_WashU"],
+            "somatic_mutation"  : "ccRCC_discovery.dnp.annotated.exonic.maf.gz",
+            "transcriptomics"   : ["ccRCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz", "ccRCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "ccRCC_xCell.txt.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
+        # self._readme_files = {}
+
         self.load_functions = {
-            'clinical'                : self.load_clinical,
-            'derived_molecular'       : self.load_derived_molecular,
-            'CNV'                     : self.load_CNV,
-            'followup'                : self.load_followup,
-            'circular_RNA'            : self.load_circular_RNA,
-            'miRNA'                   : self.load_miRNA,
-            'phosphoproteomics'       : self.load_phosphoproteomics,
-            'proteomics'              : self.load_proteomics,
-            'somatic_mutation'        : self.load_somatic_mutation,
-            'transcriptomics'         : self.load_transcriptomics,
+            'transcriptomics'   : self.load_transcriptomics,
+            'somatic_mutation'  : self.load_somatic_mutation,
+            'miRNA'             : self.load_miRNA,
+            'xcell'             : self.load_xcell,
+            'cibersort'         : self.load_cibersort,
+            'CNV'               : self.load_CNV,
+            'tumor_purity'      : self.load_tumor_purity,
+            #'readme'            : self.load_readme,
+            "hla_typing": self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
+        # Call the parent class __init__ function
+        super().__init__(cancer_type="ccrcc", source="washu", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        super().__init__(cancer_type="hnscc", source='awg', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+    def load_transcriptomics(self):
+        df_type = 'transcriptomics'
+        if df_type not in self._data:
+            file_path_list = self.locate_files(df_type)
+            # loop over list of file paths
+            for file_path in file_path_list:
+                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
+                file_name = os.path.basename(file_path)
+
+                if file_name == "ccRCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df = pd.read_csv(file_path, sep="\t")
+                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+                    df = df.set_index(["Name", "Database_ID"])
+                    df = df.sort_index()
+                    df = df.T
+                    df.index.name = "Patient_ID"
+                    df.index = df.index.str.replace(r"-T", "", regex=True) #remove label for tumor samples
+                    self._helper_tables["transcriptomics_tumor"] = df
+                    
+                if file_name == "ccRCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df = pd.read_csv(file_path, sep="\t")
+                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+                    df = df.set_index(["Name", "Database_ID"])
+                    df = df.sort_index()
+                    df = df.T
+                    df.index.name = "Patient_ID"
+                    df.index = df.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
+                    self._helper_tables["transcriptomics_normal"] = df
+
+            # Combine the two transcriptomics dataframes
+            rna_tumor = self._helper_tables.get("transcriptomics_tumor")
+            rna_normal = self._helper_tables.get("transcriptomics_normal") # Normal entries are already marked with 'N' on the end of the ID
+            if rna_tumor is None or rna_normal is None:
+                print("rna_tumor or rna_normal is None")
+                return
+            if not isinstance(rna_tumor, pd.DataFrame) or not isinstance(rna_normal, pd.DataFrame):
+                print("rna_tumor or rna_normal is not a DataFrame")
+                return
+       
+            rna_combined = pd.concat([rna_tumor, rna_normal])
 
+            # save df in self._data
+            self.save_df(df_type, rna_combined)
 
-    def load_CNV(self):
-        df_type = 'CNV'
+    def load_somatic_mutation(self):
+        df_type = 'somatic_mutation'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            df = pd.read_csv(file_path, sep='\t')
 
-            if self.version == "2.0":
-                df = df.set_index('gene_symbol')
-
-            df = df.sort_index()
-            df = df.transpose()
-            df = df.sort_index()
-            df.columns.name=None
-            df.index.name = "Patient_ID"
+            df = pd.read_csv(file_path, sep='\t')    
+            df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
+            df = df.rename(columns={
+                        "Hugo_Symbol":"Gene",
+                        "Gene":"Gene_Database_ID",
+                        "Variant_Classification":"Mutation",
+                        "HGVSp_Short":"Location"})
 
+            df = df.set_index("Patient_ID")
+            df = df[ ['Gene'] + ["Mutation"] + ["Location"] + [ col for col in df.columns if col not in ["Gene","Mutation","Location"] ] ]
+            df.index = df.index.str.replace(r"_T", "", regex=True)     
             # save df in self._data
             self.save_df(df_type, df)
 
-
     def load_miRNA(self):
-        df_type = 'miRNA'
+        self.load_precursor_miRNA()
+        self.load_mature_miRNA()
+        self.load_total_mRNA()
+
+    def load_precursor_miRNA(self):
+        df_type = 'precursor_miRNA'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            df = pd.read_csv(file_path, sep='\t', index_col=0)
-            df = df.sort_index()
-            df = df.transpose()
-
-            # Reformat patient ids
-            df.index = df.index.str.replace(r'-T$', '', 1, regex=True)
-            df.index = df.index.str.replace(r'-N$', '.N', 1, regex=True)
 
+            df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
+            df = df.transpose()
+            df.index = df.index.str.replace('\.T$','', regex = True)
+            df.index = df.index.str.replace('\.A$','.N', regex = True)
+            df.index.name = 'Patient_ID'                
+            # Sort
+            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
+            normal = normal.sort_values(by=["Patient_ID"])
+            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
+            tumor = tumor.sort_values(by=["Patient_ID"])
+            all_df = pd.concat([tumor, normal])
             # save df in self._data
-            self.save_df(df_type, df)
-
+            self.save_df(df_type, all_df)
 
-    def load_transcriptomics(self):
-        df_type = 'transcriptomics'
+    def load_mature_miRNA(self):
+        df_type = 'mature_miRNA'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            df = pd.read_csv(file_path, sep='\t')
-
-            if self.version == "2.0":
-                df = df.set_index('Idx')
-
-            df = df.sort_index()
+            
+            df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias', 'Derives_from'])
             df = df.transpose()
-            df = df.sort_index()
-            df.columns.name=None
-
-            if self.version == "0.1":
-                df.index = df.index.str.replace(r'\.', '-', 1, regex=True)
-                df.index = df.index.str.replace(r'\.T$', '', 1, regex=True)
-            elif self.version == "2.0":
-                df.index = df.index.str.replace(r'-T$', '', 1, regex=True)
-                df.index = df.index.str.replace(r'-N$', '.N', 1, regex=True)
-
-            df.index.name = "Patient_ID"
-
+            df.index = df.index.str.replace('\.T$','', regex = True)
+            df.index = df.index.str.replace('\.A$','.N', regex = True)
+            df.index.name = 'Patient_ID'                
+            # Sort
+            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
+            normal = normal.sort_values(by=["Patient_ID"])
+            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
+            tumor = tumor.sort_values(by=["Patient_ID"])
+            all_df = pd.concat([tumor, normal])
             # save df in self._data
-            self.save_df(df_type, df)
-
+            self.save_df(df_type, all_df)
 
-    def load_circular_RNA(self):
-        df_type = 'circular_RNA'
+    def load_total_mRNA(self):
+        df_type = 'total_miRNA'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-
-            df = pd.read_csv(file_path, sep='\t')
-            df = df.sort_index()
+            
+            df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
-            df = df.sort_index()
-            df.columns.name=None
-
-            if self.version == "0.1":
-                # We want all the patientIDs to have the the format C3L-00977, and these have the form C3L.00977.N, so we need to replace the first "." with a "-"
-                df.index = df.index.str.replace(r'\.', '-', 1, regex=True)
-                df.index = df.index.str.replace(r'\.T$', '', 1, regex=True)
-
-            elif self.version == "2.0":
-                df.index = df.index.str.replace(r'-T$', '', 1, regex=True)
-                df.index = df.index.str.replace(r'-N$', '.N', 1, regex=True)
-
-            df.index.name = "Patient_ID"
+            df.index = df.index.str.replace('\.T$','', regex = True)
+            df.index = df.index.str.replace('\.A$','.N', regex = True)
+            df.index.name = 'Patient_ID'                
+            # Sort
+            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
+            normal = normal.sort_values(by=["Patient_ID"])
+            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
+            tumor = tumor.sort_values(by=["Patient_ID"])
+            all_df = pd.concat([tumor, normal])
+            # save df in self._data
+            self.save_df(df_type, all_df)
 
+    def load_xcell(self):
+        df_type = 'xcell'
+        if df_type not in self._data:
+            file_path = self.locate_files(df_type)
+        
+            df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
+            df = df.transpose()
+            df.columns.name = 'Name'
+            df.index.name = 'Patient_ID'
+            df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
+            df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_followup(self):
-        df_type = 'followup'
+    def load_cibersort(self):
+        df_type = 'cibersort'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            df = pd.read_excel(file_path)
-
-            # Rename, set, and sort by index
-            df = df.rename(columns={"CASE_ID": "Patient_ID"})
-            df = df.set_index("Patient_ID")
-            df = df.sort_index()
 
+            df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
+            df.index.name = 'Patient_ID'
+            df.columns.name = 'Name'
+            df.index = df.index.str.replace(r'-T$', '', regex=True) 
+            df.index = df.index.str.replace(r'-A$', '.N', regex=True)
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_mapping(self):
+        df_type = 'mapping'
+        if "CNV_gene_ids" not in self._helper_tables:
+            file_path = self.locate_files(df_type)
+
+            df = read_gtf(file_path)
+            df = df.as_df()
+            df = df[["gene_name","gene_id"]]
+            df = df.drop_duplicates()
+            df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+            df = df.set_index("Name")
+            self._helper_tables["CNV_gene_ids"] = df 
 
-    def load_phosphoproteomics(self):
-        df_type = 'phosphoproteomics'
+    def load_CNV(self):
+        df_type = 'CNV'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            df = pd.read_csv(file_path, sep='\t')
-            df = df.rename(columns={"Gene": "Name"})
 
-            # Drop unlocalized sites
-            unlocalized_sites = (df["Index"].str.rsplit("_", n=1, expand=True)[1] == '0')
-            df = df[~unlocalized_sites]
-
-            # Parse a few columns out of the "Index" column that we'll need for our multiindex
-            split_ids = df["Index"].str.split('_', expand=True)
-            df = df.drop(columns="Index")
-            sites = split_ids.iloc[:, -1]
-            database_ids = split_ids[0].str.cat(split_ids[1], sep='_')
-            df = df.assign(**{"Site": sites, "Database_ID": database_ids})
-
-            # Some rows have at least one localized phosphorylation site, but also have other phosphorylations that aren't localized. We'll drop those rows, if their localized sites are duplicated in another row, to avoid creating duplicates, because we only preserve information about the localized sites in a given row. However, if the localized sites aren't duplicated in another row, we'll keep the row.
-            unlocalized_to_drop = df.index[~split_ids[4].eq(split_ids[5]) & df.duplicated(["Name", "Site", "Peptide", "Database_ID"], keep=False)] # Column 4 of the split "Index" column is number of phosphorylations detected, and column 5 is number of phosphorylations localized, so if the two values aren't equal, the row has at least one unlocalized site
-            df = df.drop(index=unlocalized_to_drop)
-
-            # Give it a multiindex
-            df = df.set_index(["Name", "Site", "Peptide", "Database_ID"]) # This will create a multiindex from these columns, in this order.
-            df = df.sort_index()
-            df = df.transpose()
-            df.index = df.index.str.replace(r'-T$', '', 1, regex=True)
-            df.index = df.index.str.replace(r'-N$', '.N', 1, regex=True)
-            df.index = df.index.str.replace(r'-C$', '.C', 1, regex=True) #-C is cored NAT samples
-            df = df.sort_index()
+            df = pd.read_csv(file_path, sep="\t")
+            df = df.rename(columns={"Gene": "Name"})
+            df = df.set_index("Name")
+            cnv = df
 
+            self.load_mapping()
+            gene_ids = self._helper_tables["CNV_gene_ids"]
+            df = cnv.join(gene_ids,how = "left") #merge in gene_ids 
+            df = df.reset_index()
+            df = df.set_index(["Name", "Database_ID"]) #create multi-index
+            df = df.T
+            df.index.name = 'Patient_ID'
             # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_proteomics(self):
-        df_type = 'proteomics'
+    def load_tumor_purity(self):
+        df_type = 'tumor_purity'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-
-            if self.version == "0.1":
-                for file in file_path:
-                    path_elements = file.split(os.sep) # Get a list of the levels of the path
-                    file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
-
-                    # Combine the two proteomics dataframes
-                    if file_name == "Proteomics_DIA_Gene_level_Normal.cct.gz":
-                        df_normal = pd.read_csv(file, sep='\t')
-                        df_normal = df_normal.transpose()
-                        df_normal.columns.name=None
-                        df_normal.index.name = "Patient_ID"
-
-                    elif file_name == "Proteomics_DIA_Gene_level_Tumor.cct.gz":
-                        df_tumor = pd.read_csv(file, sep='\t')
-                        df = df.transpose()
-                        df.columns.name=None
-                        df.index.name = "Patient_ID"
-
-                df_normal.index = df_normal.index + ".N" #concatenate a ".N" onto the end of the normal data so we can identify it as normal after it's appended to tumor
-                prot_combined = pd.concat([df_tumor, df_normal]) #append the normal data onto the end of the tumor data
-                prot_combined = prot_combined.sort_index(axis='columns') # Put all the columns in alphabetical order
-                prot_combined = prot_combined.sort_index()
-                df = prot_combined
-
-            if self.version == "2.0":
-                df = pd.read_csv(file_path, sep='\t')
-                df = df.set_index('Index')
-
-                df = df.transpose()
-                df.columns.name=None
-                df.index.name = "Patient_ID"
-
-                df.index = df.index.str.replace(r'-T$', '', 1, regex=True)
-                df.index = df.index.str.replace(r'-N$', '.N', 1, regex=True)
-                df.index = df.index.str.replace(r'-C$', '.C', 1, regex=True) #-C is cored NAT samples
-
+        
+            df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
+            df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
+            df = df.set_index('Sample_ID') 
+            df.index.name = 'Patient_ID'
+
+            # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
+            mssmclin = Mssm(filter_type='ccrcc', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')              
+            patient_ids = clinical_df.index.to_list()
+            df = df.loc[df.index.isin(patient_ids)]     
+                       
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
 
-    def load_somatic_mutation(self):
-        df_type = 'somatic_mutation'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
+            # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            df = pd.read_csv(file_path, sep='\t')
 
-            if self.version == "0.1":
-                #Rename the columns we want to keep to the appropriate names
-                df = df.rename(columns={"Tumor_Sample_Barcode":"Patient_ID","Hugo_Symbol_Annovar":"Gene","Variant_Classification_Annovar":"Mutation"})
-                df['Location'] = df['Annovar_Info_protein'].str.extract(r'([^:]+$)') #The location that we care about is stored after the last colon
-                df = df[['Patient_ID', 'Gene', 'Mutation', 'Location']]
-
-            elif self.version == "2.0":
-                df = df[['Tumor_Sample_Barcode','Hugo_Symbol','Variant_Classification','HGVSp_Short']]
-                df = df.rename(columns={
-                    "Tumor_Sample_Barcode":"Patient_ID",
-                    "Hugo_Symbol":"Gene",
-                    "Variant_Classification":"Mutation",
-                    "HGVSp_Short":"Location"}) #Rename the columns we want to keep to the appropriate names
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
 
-            df = df.sort_values(by=["Patient_ID", "Gene"])
-            df = df.set_index("Patient_ID")
-            df = df.sort_index()
-            df.columns.name=None
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
 
-            # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_annotation(self):
-        # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
-        file_path = self.locate_files('annotation')
-        df = pd.read_csv(file_path, sep='\t')
-
-        if self.version == "2.0":
-            df = df.set_index('case_id')
-        elif self.version == "0.1":
-            df = df.set_index('CASE_ID')
-
-        df.columns.name=None
-        df.index.name="Patient_ID"
-
-        # Split the clinical data in to clinical data and derived molecular data
-        if self.version == "0.1":
-            derived_molecular_cols = ['P53GENE_ANALYSIS', 'EGFR_AMP_STATUS']
-
-        elif self.version == "2.0":
-            derived_molecular_cols = ['NAT_pathology_review', 'tumor_pathology_review',
-               'ESTIMATE_stromal_score', 'ESTIMATE_immune_score', 'stemness_score',
-               'mutation_count', 'TP53_mutation', 'CDKN2A_mutation', 'FAT1_mutation',
-               'NOTCH1_mutation', 'CSMD3_mutation', 'DNAH5_mutation', 'KMT2D_mutation',
-               'transcriptomic_subtype', 'chr_instability_idx', 'tumor_proportion',
-               'normal_epithelial_proportion', 'immune_proportion',
-               'muscle_proportion', 'fibroblast_proportion', 'EGFR_pathway',
-               'Hypoxia_pathway', 'JAK.STAT_pathway', 'MAPK_pathway', 'NFkB_pathway',
-               'PI3K_pathway', 'TGFb_pathway', 'TNFa_pathway', 'Trail_pathway',
-               'VEGF_pathway', 'p53_pathway']
-
-        derived_molecular_df = df[derived_molecular_cols]
-        derived_molecular_df = derived_molecular_df.sort_index(axis='columns')
-        derived_molecular_df = derived_molecular_df.sort_index()
-
-        df = df.drop(columns=derived_molecular_cols)
-        df = df.sort_index()
-        df = df.sort_index(axis='columns')
-
-        # save dfs in self._data
-        self.save_df("clinical", df)
-        self.save_df("derived_molecular", derived_molecular_df)
-
-    # load_annotation takes care of the data for these datatypes
-    def load_clinical(self):
-        if 'clinical' not in self._data:
-            self.load_annotation()
-
-    def load_derived_molecular(self):
-        if 'derived_molecular' not in self._data:
-            self.load_annotation()
-
-
-    def how_to_cite(self):
-        return super().how_to_cite(cancer_type='head and neck squamous cell carcinoma', pmid=33417831)
+        return self._data[df_type]
+    # def load_readme(self):
+    #     df_type = 'readme'
+    #     if not self._readme_files:
+    #         file_path_list = self.locate_files(df_type)
+    #         # loop over list of file paths
+    #         for file_path in file_path_list:
+    #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
+    #             file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+
+    #             if file_name == "README_miRNA":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_miRNA"] = reader.read()
+                        
+    #             elif file_name == "README_CIBERSORT":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_cibersort"] = reader.read()
+                        
+    #             elif file_name == "README_xCell":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_xcell"] = reader.read()
+                
+    #             elif file_name == "README_somatic_mutation_WXS" in file_path:
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_somatic_mutation"] = reader.read()
+                        
+    #             elif file_name == "README_gene_expression":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_transcriptomics"] = reader.read()
+                
+    #             elif file_name == "README.boxnote":
+    #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
+
+    #             elif file_name == "README_ESTIMATE_WashU":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/awg/awgov.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washuov.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,253 +6,240 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, ReindexMapError
+from cptac.cancers.mssm.mssm import Mssm
 
-class AwgOv(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Load all of the ovarian dataframes as values in the self._data dict variable, with names as keys, and format them properly.
+class WashuOv(Source):
+    def __init__(self, no_internet=False):
+        """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
-
+        
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        self.valid_versions = ["0.0", "0.0.1"] # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-
         self.data_files = {
-            "0.0": {
-                "clinical"          : "clinical.csv.gz",
-                "CNV"               : "cnv.tsv.gz",
-                "definitions"       : "definitions.txt",
-                "phosphoproteomics" : "phosphoproteomics.txt.gz",
-                "proteomics"        : "proteomics.txt.gz",
-                "somatic_mutation"  : "somatic_38.maf.gz",
-                "transcriptomics"   : "transcriptomics.tsv.gz",
-                "treatment"         : "treatment.csv.gz"},
-            "0.0.1": {
-                "clinical"          : "clinical.csv.gz",
-                "CNV"               : "cnv.tsv.gz",
-                "definitions"       : "definitions.txt",
-                "followup"          : "Ovary_One_Year_Clinical_Data_20160927.xls",
-                "phosphoproteomics" : "phosphoproteomics.txt.gz",
-                "proteomics"        : "proteomics.txt.gz",
-                "somatic_mutation"  : "somatic_38.maf.gz",
-                "transcriptomics"   : "transcriptomics.tsv.gz",
-                "treatment"         : "treatment.csv.gz"},
+            "cibersort"             : "CIBERSORT.Output_Abs_OV.txt.gz",
+            "CNV"                   : "OV.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"               : "gencode.v22.annotation.gtf.gz",
+            "miRNA"                : ["OV_precursor_miRNA_combined.tsv.gz","OV_mature_miRNA_combined.tsv.gz","OV_total_miRNA_combined.tsv.gz"], # waiting for data
+            # "readme"                : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
+            "somatic_mutation"      : "OV_prospective.dnp.annotated.exonic.addrecovercases.maf.gz",
+            "transcriptomics"       : "OV_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz",
+            "tumor_purity"          : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"                 : "OV_xCell.txt.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
+        #self._readme_files = {}
+
         self.load_functions = {
-            'clinical'                : self.load_clinical,
-            'CNV'                     : self.load_CNV,
-            'followup'                : self.load_followup,
-            'phosphoproteomics'       : self.load_phosphoproteomics,
-            'proteomics'              : self.load_proteomics,
-            'somatic_mutation'        : self.load_somatic_mutation,
-            'transcriptomics'         : self.load_transcriptomics,
-            'treatment'               : self.load_treatment,
+            'transcriptomics'   : self.load_transcriptomics,
+            'somatic_mutation'  : self.load_somatic_mutation,
+            'miRNA'             : self.load_miRNA,
+            'xcell'             : self.load_xcell,
+            'cibersort'         : self.load_cibersort,
+            'CNV'               : self.load_CNV,
+            'tumor_purity'      : self.load_tumor_purity,
+            #'readme'            : self.load_readme,
+            "hla_typing"        : self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
-        super().__init__(cancer_type="ov", source='awg', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-
-
-    def load_clinical(self):
-        df_type = 'clinical'
-        if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files(df_type)
+        # Call the parent class __init__ function
+        super().__init__(cancer_type="ov", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-            df = pd.read_csv(file_path, sep=',', index_col=0)
-            df = df.rename(columns={"Participant_ID":"Patient_ID"})
-            df = df.set_index("Patient_ID")
-
-            # save df in self._data
-            self.save_df(df_type, df)
-
-
-    def load_CNV(self):
-        df_type = 'CNV'
+    def load_transcriptomics(self):
+        df_type = 'transcriptomics'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t', index_col=0)
-            df = df.sort_index()
-            df = df.transpose()
+            df = pd.read_csv(file_path, sep="\t")
+            df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+            df = df.set_index(["Name", "Database_ID"])
             df = df.sort_index()
-
+            df = df.T
+            df.index.name = "Patient_ID"
+            #remove label for tumor samples. All samples are tumors 
+            df.index = df.index.str.replace(r"-T", "", regex=True) 
             # save df in self._data
             self.save_df(df_type, df)
 
-
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t', index_col=0)
-            df = df.reset_index()
-            # The first part of the barcode is the patient id, which we need to make a Patient_ID column
-            split_barcode = df["Tumor_Sample_Barcode"].str.split("_", n=1, expand=True)
-            df["Tumor_Sample_Barcode"] = split_barcode[0]
-            df = df[["Tumor_Sample_Barcode","Hugo_Symbol","Variant_Classification","HGVSp_Short"]] # We only want these columns
-            df = df.rename(columns={"Tumor_Sample_Barcode":"Patient_ID","Hugo_Symbol":"Gene","Variant_Classification":"Mutation","HGVSp_Short":"Location"})
-            df = df.sort_values(by=["Patient_ID", "Gene"])
-            df = df.set_index("Patient_ID")
+            df = pd.read_csv(file_path, sep='\t')    
+            # Rename the columns we want to keep to the appropriate names
+            df = pd.read_csv(file_path, sep='\t')    
+            df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
+            df = df.rename(columns={
+                        "Hugo_Symbol":"Gene",
+                        "Gene":"Gene_Database_ID",
+                        "Variant_Classification":"Mutation",
+                        "HGVSp_Short":"Location"})
 
+            df = df.set_index("Patient_ID")
+            df = df[ ['Gene'] + ["Mutation"] + ["Location"] + [ col for col in df.columns if col not in ["Gene","Mutation","Location"] ] ]
+            df.index = df.index.str.replace(r"_T", "", regex=True)     
             # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_transcriptomics(self):
-        df_type = 'transcriptomics'
+    
+    def load_xcell(self):
+        df_type = 'xcell'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t', index_col=0)
-            df = df.sort_index()
+            df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df = df.transpose()
-            df = df.sort_index()
-            date_cols = ['1-Dec', '1-Sep', '10-Mar', '10-Sep', '11-Sep', '12-Sep',
-                         '14-Sep', '15-Sep', '2-Mar', '2-Sep', '3-Mar', '3-Sep', '4-Mar',
-                         '4-Sep', '5-Mar', '6-Mar', '6-Sep', '7-Mar', '7-Sep', '8-Mar',
-                         '8-Sep', '9-Mar', '9-Sep']
-            df = df.drop(columns=date_cols) # Drop all date values until new data is uploaded
-
+            df.columns.name = 'Name'
+            df.index.name = 'Patient_ID'
+            df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
+            df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_followup(self):
-        df_type = 'followup'
+    def load_cibersort(self):
+        df_type = 'cibersort'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_excel(file_path)
-            # Replace redundant values for "not reported" with NaN
-            nan_equivalents = ['Not Reported/ Unknown', 'Reported/ Unknown', 'Not Applicable',
-                'na', 'unknown', 'Not Performed', 'Unknown tumor status', 'Unknown',
-                'Unknown Tumor Status', 'Not specified']
-            df = df.replace(nan_equivalents, np.nan)
-
-            # Rename PPID to Patient_ID and set as index
-            df = df.rename(columns={'PPID': 'Patient_ID'})
-            df = df.set_index("Patient_ID")
-            df = df.sort_index()
-
+            df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
+            df.index.name = 'Patient_ID'
+            df.columns.name = 'Name'
+            df.index = df.index.str.replace(r'-T$', '', regex=True) 
+            df.index = df.index.str.replace(r'-A$', '.N', regex=True)
             # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_phosphoproteomics(self):
-        df_type = 'phosphoproteomics'
-        if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
+    def load_mapping(self):
+        df_type = 'mapping'
+        if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t')
-            df = df[df["site"].notnull()] # Drops all rows with nan values in site column
-
-            # Create our column multiindex
-            # Split the genes from the sites, splitting from the right since some genes have hyphens in their names, but the genes and sites are also separated by hyphens
-            split_genes = df["site"].str.rsplit("-", n=1, expand=True)
-            # hgnc_symbol is a duplicate of split_genes[0], and site is now in split_genes and will be re-inserted differently
-            df = df.drop(columns=["hgnc_symbol", "site"])
-            df = df.assign(Name=split_genes[0], Site=split_genes[1])
-            # Get rid of all lowercase s, t, and y delimeters in the sites
-            df["Site"] = df["Site"].str.replace(r"[sty]", r"", regex=True)
-            df = df.rename(columns={"refseq_peptide": "Database_ID"})
-            df = df.set_index(["Name", "Site", "Peptide", "Database_ID"]) # Turn these columns into a multiindex
+            df = read_gtf(file_path)
+            df = df.as_df()
+            df = df[["gene_name","gene_id"]]
+            df = df.drop_duplicates()
+            df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+            df = df.set_index("Name")
+            self._helper_tables["CNV_gene_ids"] = df  
 
-            df = df.sort_index()
-            df = df.transpose()
+    def load_CNV(self):
+        df_type = 'CNV'
+        if df_type not in self._data:
+            file_path = self.locate_files(df_type)
 
+            df = pd.read_csv(file_path, sep="\t")
+            df = df.rename(columns={"Gene": "Name"})
+            df = df.set_index("Name")
+            cnv = df
+
+            self.load_mapping()
+            gene_ids = self._helper_tables["CNV_gene_ids"]
+            df = cnv.join(gene_ids,how = "left") #merge in gene_ids 
+            df = df.reset_index()
+            df = df.set_index(["Name", "Database_ID"]) #create multi-index
+            df = df.T
+            df.index.name = 'Patient_ID'
             # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_proteomics(self):
-        df_type = 'proteomics'
+    def load_tumor_purity(self):
+        df_type = 'tumor_purity'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t')
-            df = df[df["hgnc_symbol"].notnull()] # Drops all nan values in hgnc_symbol column
+            df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
+            df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
+            df = df.set_index('Sample_ID') 
+            df.index.name = 'Patient_ID' 
 
-            # Create our column multiindex
-            df = df.rename(columns={"hgnc_symbol": "Name", "refseq_peptide": "Database_ID"})
-            df = df.set_index(["Name", "Database_ID"])
-            df = df.sort_index()
-            df = df.transpose()
+            # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
+            mssmclin = Mssm(filter_type='ov', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')               
+            patient_ids = clinical_df.index.to_list()
+            df = df.loc[df.index.isin(patient_ids)]    
 
             # save df in self._data
             self.save_df(df_type, df)
 
-
-    def load_treatment(self):
-        df_type = 'treatment'
+    def load_miRNA(self):
+        df_type = 'miRNA'
         if df_type not in self._data:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files(df_type)
+            file_paths = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep=',', index_col=0)
-            df = df.rename(columns={"Participant_ID":"Patient_ID"})
-            df = df.set_index("Patient_ID")
+            # This is just an example; the actual loading will depend on your data
+            df = pd.concat([pd.read_csv(file_path, sep='\t') for file_path in file_paths])
+            df = df.rename(columns={"YourColumnName": "NewColumnName"})
+            df = df.set_index("NewColumnName")
+
+            # Further processing here, if necessary
 
-            # save df in self._data
             self.save_df(df_type, df)
 
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
 
-    def load_definitions(self):
-        df_type = 'definitions'
-        # TODO: low priority, make sure this actually works later
-        if not self._definitions:
-            # verify the df_type is valid for the current version and get file path (defined in source.py, the parent class)
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            with open(file_path, "r", errors="ignore") as definitions_file:
-                for line in definitions_file.readlines():
-                    line = line.strip()
-                    line = line.split("\t")
-                    term = line[0]
-                    definition = line[1]
-                    self._definitions[term] = definition
-
-
-    # Override the save_df function from source.py so we can mark normal ov samples
-    def save_df(self, datatype, df):
-
-        # Take C prefix off of indices for those samples that have them (tumor samples have C, normal have N)
-        df.index = df.index.where(~df.index.str.startswith('C'), df.index.str[1:])
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
 
-        # Move the prepended N to a .N at the end to match other normal sample labeling in cptac
-        df.index = df.index.where(~df.index.str.startswith('N'), df.index.str[1:] + ".N")
-
-        # Drop all OV_QC samples--they're quality control samples not relevant for data analysis
-        df = df.drop(index=df.index[df.index.str.startswith("OV_QC")])
-
-        # Inherit the parent event
-        super().save_df(datatype, df)
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
 
+            self.save_df(df_type, df)
 
-    def how_to_cite(self):
-        return super().how_to_cite(cancer_type='high grade serous ovarian cancer', pmid=27372738)
+        return self._data[df_type]
+    # def load_readme(self):
+    #     df_type = 'readme'
+    #     if not self._readme_files:
+    #         file_path_list = self.locate_files(df_type)
+    #         # loop over list of file paths
+    #         for file_path in file_path_list:
+    #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
+    #             file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+                
+    #             if file_name == "README_miRNA":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_miRNA"] = reader.read()
+                    
+    #             elif file_name == "README_CIBERSORT":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_cibersort"] = reader.read()
+                        
+    #             elif file_name == "README_xCell":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_xcell"] = reader.read()
+                
+    #             elif file_name == "README_somatic_mutation_WXS":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_somatic_mutation"] = reader.read()
+                        
+    #             elif file_name == "README_gene_expression":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_transcriptomics"] = reader.read()
+                    
+    #             elif file_name == "README.boxnote":
+    #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
+                
+    #             elif file_name == "README_ESTIMATE_WashU":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/bcm/bcmbrca.py` & `cptac-1.5.0rc3/cptac/cancers/bcm/bcmgbm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,125 @@
-#   Copyright 2018 Samuel Payne sam_payne@byu.edu
+#   Copyright 2023 Samuel Payne sam_payne@byu.edu
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Importing necessary libraries
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-
-class BcmBrca(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which bcmbrca dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
+class BcmGbm(Source):
+    def __init__(self, no_internet=False):
+        """
+        Define bcmgbm dataframes available in self.load_functions with names as keys.
+        
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): If set to True, skips the index update step which requires an internet connection.
+        Default is False.
         """
-
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        
+        # Define the needed variables and pass them to the parent Dataset class __init__ function
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "BRCA-gene_RSEM_tumor_normal_UQ_log2(x+1)_BCM.txt", 
-                "mapping" : "gencode.v34.basic.annotation-mapping.txt"
-            }
+            "transcriptomics" : "GBM-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt.gz",
+            "mapping" : "gencode.v34.basic.annotation-mapping.txt.gz",
+            "circular_RNA" : "GBM-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt.gz"
         }
-        
+
         self.load_functions = {
+            'circular_RNA' : self.load_circular_RNA,
             'transcriptomics' : self.load_transcriptomics,
         }
-        
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
 
         # Call the parent class __init__ function
-        super().__init__(cancer_type="brca", source='bcm', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="gbm", source='bcm', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
+
+    def load_circular_RNA(self):
+        """
+        Load and parse all files for bcm gbm circular RNA data.
+        """
+        df_type = 'circular_RNA'
         
+        # Check if data is already loaded
+        if df_type not in self._data:
+            # Get file path to the correct data
+            file_path = self.locate_files(df_type)
+
+            # Load and parse the file 
+            df = pd.read_csv(file_path, sep="\t")
+            df = df.rename_axis('INDEX').reset_index()
+            df[["circ","chrom","start","end","gene"]] = df.INDEX.str.split('_', expand=True)
+            df["circ_chromosome"] = df["circ"] +"_" + df["chrom"]
+            df = df.set_index('gene')
+
+            # Load mapping information and add it to circular RNA data
+            self.load_mapping()
+            gene_key = self._helper_tables["gene_key"]
+            df = gene_key.join(df, how = "inner")
+            df = df.reset_index()
+            df = df.rename(columns= {"gene_name": "Name","gene":"Database_ID"}) # change names to match cptac package
+            df = df.set_index(["Name","circ_chromosome", "start","end","Database_ID"]) #create multi-index
+            df.drop(['INDEX', 'circ', 'chrom'], axis=1, inplace=True) 
+            df = df.sort_index()
+            df = df.T
+            df.index = df.index.str.replace(r"_T", "", regex=True) # remove Tumor label. All samples are tumor samples
+            df.index.name = "Patient_ID"
+
+            # Save df in data
+            self.save_df(df_type, df)
+
+
     def load_mapping(self):
+        """
+        Load and parse all files for mapping. These will be used for circular RNA and transcriptomics loading.
+        """
         df_type = 'mapping'
-        # self._helper_tables is a dictionary of helpful dataframes that the user does not need to access
-        # dataframes here are used to load the other data types, but don't show up when the user lists available data
-        # this way mapping only needs to be loaded once and all other types can use it when they are loaded
+        
+        # Check if helper tables have already been loaded
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep='\t')
-            df = df[["gene","gene_name"]] #only need gene (database gene id) and gene_name (common gene name)
+
+            # Load the file, select needed columns, set index, remove duplicates
+            df = pd.read_csv(file_path, sep="\t")
+            df = df[["gene","gene_name"]] 
             df = df.set_index("gene")
             df = df.drop_duplicates()
+
+            # Save mapping in helper tables
             self._helper_tables["gene_key"] = df 
-            
-        
+
+
     def load_transcriptomics(self):
-        """Load and parse all files for bcm brca transcriptomics data
-           Populates self._data with transcriptomics data in a Pandas dataframe
+        """
+        Load and parse all files for bcm gbm transcriptomics data.
         """
         df_type = 'transcriptomics'
+        
+        # Check if data is already loaded
         if df_type not in self._data:
-            # get file path to the correct data (defined in source.py, the parent class)
+            # Get file path to the correct data
             file_path = self.locate_files(df_type)
 
-            # process the file and add it to self._data
-            df = pd.read_csv(file_path, sep='\t')
+            # Load the file 
+            df = pd.read_csv(file_path, sep="\t")
             df.index.name = 'gene'
-            # in order to finish parsing the file we need mapping information (the gene_key)
-            # make sure self._helper_tables has gene_key parsed and loaded
+
+            # Load mapping information and add it to transcriptomics data
             self.load_mapping()
-            # get gene key to use for transcriptomics
             gene_key = self._helper_tables["gene_key"]
-            transcript = gene_key.join(df,how = "inner") #keep only gene_ids with gene names
+            transcript = gene_key.join(df, how="inner") 
             transcript = transcript.reset_index()
             transcript = transcript.rename(columns={"gene_name":"Name","gene":"Database_ID"})
             transcript = transcript.set_index(["Name", "Database_ID"])
-            transcript = transcript.sort_index() #alphabetize
+            transcript = transcript.sort_index() 
             transcript = transcript.T
-            transcript.index.name = "Patient_ID"
+            transcript.index = transcript.index.str.replace(r"_T", "", regex=True)
+            transcript.index.name = "Patient_ID" 
 
-            df = transcript
-            # save df in self._data
-            self.save_df(df_type, df)
+            # Save transcriptomics in data
+            self.save_df(df_type, transcript)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/bcm/bcmccrcc.py` & `cptac-1.5.0rc3/cptac/cancers/bcm/bcmccrcc.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,124 +5,126 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Importing necessary libraries
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
 
 class BcmCcrcc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which bcmccrcc dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+    def __init__(self, no_internet=False):
+        """
+        Define which bcmccrcc dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): If set to True, skips the index update step which requires an internet connection.
+        Default is False.
         """
 
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        # Define the needed variables and pass them to the parent Dataset class __init__ function
         self.data_files = {
-            "1.0": {
-                "circular_RNA" : "CCRCC-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt",
-                "mapping" : "gencode.v34.basic.annotation-mapping.txt",
-                "transcriptomics" : "CCRCC-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt"
-            }
+            "circular_RNA" : "CCRCC-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt.gz",
+            "mapping" : "gencode.v34.basic.annotation-mapping.txt.gz",
+            "transcriptomics" : "CCRCC-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt.gz"
         }
 
         self.load_functions = {
             'circular_RNA' : self.load_circular_RNA,
             'transcriptomics' : self.load_transcriptomics,
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ccrcc", source='bcm', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="ccrcc", source='bcm', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
 
     def load_circular_RNA(self):
+        """
+        Load and parse all files for circular RNA data.
+        """
         df_type = 'circular_RNA'
 
+        # Check if data is already loaded
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Get file path to the correct data
             file_path = self.locate_files(df_type)
 
+            # Load, process the file and save it in data
             df = pd.read_csv(file_path, sep="\t")
             df = df.rename_axis('INDEX').reset_index()
             df[["circ","chrom","start","end","gene"]] = df.INDEX.str.split('_', expand=True)
             df["circ_chromosome"] = df["circ"] +"_" + df["chrom"]
             df = df.set_index('gene')
             self._data["circular_RNA"] = df
 
-            # Add gene names to circular RNA data
+            # Load mapping information and add it to circular RNA data
             self.load_mapping()
             gene_key = self._helper_tables["gene_key"]
 
             df = gene_key.join(df, how = "inner")
             df = df.reset_index()
             df = df.rename(columns= {"gene_name": "Name","gene":"Database_ID"}) # change names to match cptac package
             df = df.set_index(["Name","circ_chromosome", "start","end","Database_ID"]) #create multi-index
             df.drop(['INDEX', 'circ', 'chrom'], axis=1, inplace=True)
             df = df.sort_index()
             df = df.T
             df.index = df.index.str.replace(r"_T", "", regex=True) # remove Tumor label
             df.index = df.index.str.replace(r"_A", ".N", regex=True)# Normal samples labeled with .N
             df.index.name = "Patient_ID"
 
-            # save df in self._data
+            # Save df in self._data
             self.save_df(df_type, df)
 
     def load_mapping(self):
+        """
+        Load and parse all files for mapping.
+        """
         df_type = 'mapping'
-        # self._helper_tables is a dictionary of helpful dataframes that the user does not need to access
-        # dataframes here are used to load the other data types, but don't show up when the user lists available data
-        # this way mapping only needs to be loaded once and all other types can use it when they are loaded
-        if "gene_key" not in self._helper_tables:
 
+        # Check if helper tables have already been loaded
+        if "gene_key" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
+            # Load the file, select needed columns, set index, remove duplicates
             df = pd.read_csv(file_path, sep="\t")
-            df = df[["gene","gene_name"]] #only need gene (database gene id) and gene_name (common gene name)
+            df = df[["gene","gene_name"]] 
             df = df.set_index("gene")
             df = df.drop_duplicates()
+
+            # Save mapping in helper tables
             self._helper_tables["gene_key"] = df
 
 
     def load_transcriptomics(self):
+        """
+        Load and parse all files for bcm ccrcc transcriptomics data.
+        """
         df_type = 'transcriptomics'
 
+        # Check if data is already loaded
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Get file path to the correct data
             file_path = self.locate_files(df_type)
 
+            # Load and process the file
             df = pd.read_csv(file_path, sep="\t")
             df.index.name = 'gene'
 
-            # Add gene names to transcriptomic data
+            # Load mapping information and add it to transcriptomics data
             self.load_mapping()
             gene_key = self._helper_tables["gene_key"]
-            transcript = gene_key.join(df,how = "inner") #keep only gene_ids with gene names
+            transcript = gene_key.join(df,how = "inner") 
             transcript = transcript.reset_index()
             transcript = transcript.rename(columns={"gene_name":"Name","gene":"Database_ID"})
             transcript = transcript.set_index(["Name", "Database_ID"])
             transcript = transcript.sort_index() #alphabetize
             transcript = transcript.T
             transcript.index = transcript.index.str.replace(r"_T", "", regex=True)
             transcript.index = transcript.index.str.replace(r"_A", ".N", regex=True)# Normal samples labeled with .N
             transcript.index.name = "Patient_ID"
+
             df = transcript
             
-            # save df in self._data
+            # Save df in self._data
             self.save_df(df_type, df)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/bcm/bcmcoad.py` & `cptac-1.5.0rc3/cptac/cancers/bcm/bcmpdac.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,88 +6,102 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
 
-class BcmCoad(Source):
+class BcmPdac(Source):
+    """
+    The BcmPdac class inherits from the Source class and is used to handle and load PDAC data from BCM
+    """
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which bcmcoad dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+    def __init__(self, no_internet=False):
+        """
+        Initializes BcmPdac class. Defines the available bcmpdac dataframes, sets some required variables and
+        calls the parent Dataset class __init__ function.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): Whether to skip the index update step because it requires an internet 
+        connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "CRC-gene_RSEM_tumor_normal_UQ_log2(x+1)_BCM.txt", 
-                "mapping" : "gencode.v34.basic.annotation-mapping.txt" # This kinda goes along with the transcriptomics, but when you figure out brca it will solve this too
-            }
+            "transcriptomics" : "PDAC-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt.gz",
+            "mapping" : "gencode.v34.basic.annotation-mapping.txt.gz",
+            "circular_RNA" : "PDAC-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt.gz",
         }
         
         self.load_functions = {
+            'circular_RNA' : self.load_circular_RNA,
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
+        super().__init__(cancer_type="pdac", source='bcm', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        # Call the parent class __init__ function
-        super().__init__(cancer_type="coad", source='bcm', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+    def load_circular_RNA(self):
+        """Loads the circular RNA data."""
+
+        df_type = 'circular_RNA'
+        if df_type not in self._data:
+            file_path = self.locate_files(df_type)
+            
+            df = pd.read_csv(file_path, sep="\t")
+            df = df.rename_axis('INDEX').reset_index()
+            df[["circ","chrom","start","end","gene"]] = df.INDEX.str.split('_', expand=True)
+            df["circ_chromosome"] = df["circ"] +"_" + df["chrom"]
+            df = df.set_index('gene')
+            
+            self.load_mapping()
+            gene_key = self._helper_tables["gene_key"]
+            df = gene_key.join(df, how = "inner")
+            df = df.reset_index()
+            df = df.rename(columns= {"gene_name": "Name","gene":"Database_ID"}) 
+            df = df.set_index(["Name","circ_chromosome", "start","end","Database_ID"]) 
+            df.drop(['INDEX', 'circ', 'chrom'], axis=1, inplace=True) 
+            df = df.sort_index()
+            df = df.T
+            df.index = df.index.str.replace(r"_T", "", regex=True) # remove Tumor label. All samples are tumor samples
+            df.index.name = "Patient_ID"
 
+            self.save_df(df_type, df)
         
     def load_mapping(self):
+        """Loads the mapping data."""
+
         df_type = 'mapping'
-        # self._helper_tables is a dictionary of helpful dataframes that the user does not need to access
-        # dataframes here are used to load the other data types, but don't show up when the user lists available data
-        # this way mapping only needs to be loaded once and all other types can use it when they are loaded
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
-            df = df[["gene","gene_name"]] #only need gene (database gene id) and gene_name (common gene name)
+            df = df[["gene","gene_name"]]
             df = df.set_index("gene")
             df = df.drop_duplicates()
-            self._helper_tables["gene_key"] = df 
-            
+            self._helper_tables["gene_key"] = df
             
     def load_transcriptomics(self):
+        """Loads the transcriptomics data."""
+        
         df_type = 'transcriptomics'
-
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df.index.name = 'gene'
-            self._data["transcriptomics"] = df
-                
-            # Add gene names to transcriptomic data
+
             self.load_mapping()
             gene_key = self._helper_tables["gene_key"]
-            transcript = gene_key.join(df,how = "inner") #keep only gene_ids with gene names
+            transcript = gene_key.join(df, how = "inner")
             transcript = transcript.reset_index()
-            transcript = transcript.rename(columns={
-             "gene_name":"Name","gene":"Database_ID"})
+            transcript = transcript.rename(columns={"gene_name":"Name","gene":"Database_ID"})
             transcript = transcript.set_index(["Name", "Database_ID"])
-            transcript = transcript.sort_index() #alphabetize
+            transcript = transcript.sort_index() 
             transcript = transcript.T
+            transcript.index = transcript.index.str.replace(r"_T", "", regex=True)  
+            transcript.index = transcript.index.str.replace(r"_A", ".N", regex=True)
             transcript.index.name = "Patient_ID"
-            df = transcript
-            
-            # save df in self._data
-            self.save_df(df_type, df)
+
+            self.save_df(df_type, transcript)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/bcm/bcmgbm.py` & `cptac-1.5.0rc3/cptac/cancers/bcm/bcmucec.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,119 +6,112 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
 
-class BcmGbm(Source):
+class BcmUcec(Source):
+    """Define the BcmUcec class, inherited from the Source class. This class will manage the loading of the UCEC data from the BCM source."""
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which bcmgbm dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+    def __init__(self, no_internet=False):
+        """
+        Initialize the BcmUcec object with the specified parameters.
+        This object represents the UCEC data from the BCM source.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): If True, skip the index update step. Useful when internet connection is spotty or not available. Default is False.
         """
 
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        # Define the data files associated with this dataset
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "GBM-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt",
-                "mapping" : "gencode.v34.basic.annotation-mapping.txt",
-                "circular_RNA" : "GBM-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt",
-                # "not_used" : "CPTAC_GBM_discovery_CNV_gene_level_log2ratio.tsv.gz"
-            }
+            "mapping" : "gencode.v34.basic.annotation-mapping.txt.gz",
+            "circular_RNA" : "UCEC-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt.gz",
+            "transcriptomics" : "UCEC-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt.gz"
         }
         
+        # Define the load functions for each data type
         self.load_functions = {
             'circular_RNA' : self.load_circular_RNA,
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
+        # Initialize the Source parent class
+        super().__init__(cancer_type="ucec", source='bcm', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        # Call the parent class __init__ function
-        super().__init__(cancer_type="gbm", source='bcm', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-    
-    
     def load_circular_RNA(self):
+        """Load the circular RNA dasta from the defined file."""
+
         df_type = 'circular_RNA'
         
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # If the data is not already loaded, load it
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df = df.rename_axis('INDEX').reset_index()
             df[["circ","chrom","start","end","gene"]] = df.INDEX.str.split('_', expand=True)
             df["circ_chromosome"] = df["circ"] +"_" + df["chrom"]
             df = df.set_index('gene')
-
+            
             # Add gene names to circular RNA data
             self.load_mapping()
             gene_key = self._helper_tables["gene_key"]
             df = gene_key.join(df, how = "inner")
             df = df.reset_index()
             df = df.rename(columns= {"gene_name": "Name","gene":"Database_ID"}) # change names to match cptac package
             df = df.set_index(["Name","circ_chromosome", "start","end","Database_ID"]) #create multi-index
             df.drop(['INDEX', 'circ', 'chrom'], axis=1, inplace=True) 
             df = df.sort_index()
             df = df.T
-            df.index = df.index.str.replace(r"_T", "", regex=True) # remove Tumor label. All samples are tumor samples
+            df.index = df.index.str.replace(r"_T", "", regex=True) # remove Tumor label
+            df.index = df.index.str.replace(r"_A", ".N", regex=True)# Normal samples labeled with .N
             df.index.name = "Patient_ID"
-            
+
             # save df in self._data
             self.save_df(df_type, df)
 
-
     def load_mapping(self):
+        """Load the mapping data from the defined file."""
+
         df_type = 'mapping'
-        # self._helper_tables is a dictionary of helpful dataframes that the user does not need to access
-        # dataframes here are used to load the other data types, but don't show up when the user lists available data
-        # this way mapping only needs to be loaded once and all other types can use it when they are loaded
+
         if not self._helper_tables:
+            # If the mapping data is not already loaded, load it
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df = df[["gene","gene_name"]] #only need gene (database gene id) and gene_name (common gene name)
             df = df.set_index("gene")
             df = df.drop_duplicates()
-            self._helper_tables["gene_key"] = df 
-            
-            
+            self._helper_tables["gene_key"] = df
+
     def load_transcriptomics(self):
+        """Load the transcriptomics data from the defined file."""
+
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # If the data is not already loaded, load it
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df.index.name = 'gene'
             
             # Add gene names to transcriptomic data
             self.load_mapping()
             gene_key = self._helper_tables["gene_key"]
-            transcript = gene_key.join(df, how="inner") #keep only gene_ids with gene names
+            transcript = gene_key.join(df, how = "inner") #keep only gene_ids with gene names
             transcript = transcript.reset_index()
             transcript = transcript.rename(columns={"gene_name":"Name","gene":"Database_ID"})
             transcript = transcript.set_index(["Name", "Database_ID"])
             transcript = transcript.sort_index() #alphabetize
             transcript = transcript.T
             transcript.index = transcript.index.str.replace(r"_T", "", regex=True)
-            transcript.index.name = "Patient_ID" 
+            transcript.index = transcript.index.str.replace(r"_A", ".N", regex=True)# Normal samples labeled with .N
+            transcript.index.name = "Patient_ID"
+
             df = transcript
             # save df in self._data
             self.save_df(df_type, df)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/bcm/bcmlscc.py` & `cptac-1.5.0rc3/cptac/cancers/bcm/bcmlscc.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,64 +5,52 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Import necessary modules
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
 
 class BcmLscc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which bcmlscc dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+    def __init__(self, no_internet=False):
+        """Initializes the BcmLscc class by defining which bcmlscc dataframes are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): If True, skips the index update step because it requires an internet connection. Default is False.
         """
 
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        # Define data files
         self.data_files = {
-            "1.0": {
-                "circular_RNA" : "LSCC-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt",
-                "mapping" : "gencode.v34.basic.annotation-mapping.txt",
-                "transcriptomics" : "LSCC-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt"
-            }
+            "circular_RNA" : "LSCC-circRNA_rsem_tumor_normal_UQ_log2(x+1)_BCM.txt.gz",
+            "mapping" : "gencode.v34.basic.annotation-mapping.txt.gz",
+            "transcriptomics" : "LSCC-gene_rsem_removed_circRNA_tumor_normal_UQ_log2(x+1)_BCM.txt.gz"
         }
         
+        # Define load functions
         self.load_functions = {
             'circular_RNA' : self.load_circular_RNA,
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="lscc", source='bcm', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-
+        super().__init__(cancer_type="lscc", source='bcm', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_circular_RNA(self):
-        df_type = 'circular_RNA'
+        """Load circular RNA data."""
 
+        df_type = 'circular_RNA'
+        # Check if data is not loaded
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
+            # Load data and apply necessary transformations
             df = pd.read_csv(file_path, sep='\t')
             df = df.rename_axis('INDEX').reset_index()
             df[["circ","chrom","start","end","gene"]] = df.INDEX.str.split('_', expand=True)
             df["circ_chromosome"] = df["circ"] +"_" + df["chrom"]
             df = df.set_index('gene')
             
             # Add gene names to circular RNA data
@@ -78,37 +66,40 @@
             df.index = df.index.str.replace(r"_T", "", regex=True) # remove Tumor label
             df.index = df.index.str.replace(r"_A", ".N", regex=True)# Normal samples labeled with .N
             df.index.name = "Patient_ID"
 
             # save df in self._data
             self.save_df(df_type, df)
 
-        
     def load_mapping(self):
+        """Load mapping data. This method is used by other loading methods to map gene names."""
+
         df_type = 'mapping'
-        # self._helper_tables is a dictionary of helpful dataframes that the user does not need to access
-        # dataframes here are used to load the other data types, but don't show up when the user lists available data
-        # this way mapping only needs to be loaded once and all other types can use it when they are loaded
+        # Check if helper tables are not loaded
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
+            # Load data and apply necessary transformations
             df = pd.read_csv(file_path, sep='\t')
             df = df[["gene","gene_name"]] #only need gene (database gene id) and gene_name (common gene name)
             df = df.set_index("gene")
             df = df.drop_duplicates()
             self._helper_tables["gene_key"] = df
-            
-            
+
     def load_transcriptomics(self):
+        """Load transcriptomics data."""
+
         df_type = 'transcriptomics'
 
+        # Check if data is not loaded
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
+            # Load data and apply necessary transformations
             df = pd.read_csv(file_path, sep='\t')
             df.index.name = 'gene'
             
             # Add gene names to transcriptomic data
             self.load_mapping()
             gene_key = self._helper_tables["gene_key"]
             transcript = gene_key.join(df, how = "inner") #keep only gene_ids with gene names
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/bcm/bcmov.py` & `cptac-1.5.0rc3/cptac/cancers/bcm/bcmcoad.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-#   Copyright 2018 Samuel Payne sam_payne@byu.edu
+#   Copyright 2023 Samuel Payne sam_payne@byu.edu
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Importing necessary libraries
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-
-class BcmOv(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which bcmov dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
+class BcmCoad(Source):
+    def __init__(self, no_internet=False):
+        """
+        Define bcmcoad dataframes available in self.load_functions with names as keys.
+        
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): If set to True, skips the index update step which requires an internet connection.
+        Default is False.
         """
-
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        
+        # Define the needed variables and pass them to the parent Dataset class __init__ function
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "OV-gene_RSEM_tumor_normal_UQ_log2(x+1)_BCM.txt", 
-                "mapping" : "gencode.v34.basic.annotation-mapping.txt"
-            }
+            "transcriptomics" : "CRC-gene_RSEM_tumor_normal_UQ_log2(x+1)_BCM.txt.gz",
+            "mapping" : "gencode.v34.basic.annotation-mapping.txt.gz"
         }
-        
+
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
-        
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
 
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ov", source='bcm', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="coad", source='bcm', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+
 
-        
     def load_mapping(self):
+        """
+        Load and parse all files for mapping. These will be used for transcriptomics loading.
+        """
         df_type = 'mapping'
-        # self._helper_tables is a dictionary of helpful dataframes that the user does not need to access
-        # dataframes here are used to load the other data types, but don't show up when the user lists available data
-        # this way mapping only needs to be loaded once and all other types can use it when they are loaded
+        
+        # Check if helper tables have already been loaded
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
-            
+
+            # Load the file, select needed columns, set index, remove duplicates
             df = pd.read_csv(file_path, sep="\t")
-            df = df[["gene","gene_name"]] #only need gene (database gene id) and gene_name (common gene name)
+            df = df[["gene","gene_name"]] 
             df = df.set_index("gene")
             df = df.drop_duplicates()
+
+            # Save mapping in helper tables
             self._helper_tables["gene_key"] = df
-            
-        
+
+
     def load_transcriptomics(self):
+        """
+        Load and parse all files for bcm coad transcriptomics data.
+        """
         df_type = 'transcriptomics'
-
+        
+        # Check if data is already loaded
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Get file path to the correct data
             file_path = self.locate_files(df_type)
-            
+
+            # Load the file 
             df = pd.read_csv(file_path, sep="\t")
             df.index.name = 'gene'
-            
-            # Add gene names to transcriptomic data
+
+            # Load mapping information and add it to transcriptomics data
             self.load_mapping()
             gene_key = self._helper_tables["gene_key"]
-            transcript = gene_key.join(df, how = "inner") #keep only gene_ids with gene names
+            transcript = gene_key.join(df,how = "inner") 
             transcript = transcript.reset_index()
             transcript = transcript.rename(columns={"gene_name":"Name","gene":"Database_ID"})
             transcript = transcript.set_index(["Name", "Database_ID"])
-            transcript = transcript.sort_index() #alphabetize
+            transcript = transcript.sort_index() 
             transcript = transcript.T
             transcript.index.name = "Patient_ID"
 
-            # save df in self._data
+            df = transcript
+
+            # Save df in data
             self.save_df(df_type, df)
+
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/broad/broadbrca.py` & `cptac-1.5.0rc3/cptac/cancers/broad/broadluad.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,107 @@
-#   Copyright 2018 Samuel Payne sam_payne@byu.edu
-#   Licensed under the Apache License, Version 2.0 (the "License");
-#   you may not use this file except in compliance with the License.
-#   You may obtain a copy of the License at
-#       http://www.apache.org/licenses/LICENSE-2.0
-#   Unless required by applicable law or agreed to in writing, software
-#   distributed under the License is distributed on an "AS IS" BASIS,
-#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#   See the License for the specific language governing permissions and
-#   limitations under the License.
+# Copyright 2018 Samuel Payne sam_payne@byu.edu
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#     http://www.apache.org/licenses/LICENSE-2.0
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-from gtfparse import read_gtf
-
+from pyranges import read_gtf
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-
-
-class BroadBrca(Source):
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which broadbrca dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+class BroadLuad(Source):
+    def __init__(self, no_internet=False):
+        """Defines the available dataframes in the self.load_functions dictionary variable with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): If True, the index update step which requires an internet connection is skipped. Default is False.
         """
         
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        # Initialize necessary variables and pass them to the parent Dataset class __init__ function
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "BRCA.rsem_transcripts_tpm.txt.gz",
-                "mapping" : ["sample_descriptions.tsv", "gencode.v34.GRCh38.genes.collapsed_only.gtf"]
-            }
+            "transcriptomics" : "LUAD.rsem_transcripts_tpm.txt.gz",
+            "mapping" : ["sample_descriptions.tsv.gz", "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz", "aliquot_to_patient_ID.tsv.gz"]
         }
-        
-        # If we end up needing to declare all this stuff, this is how and where we would do it
-        # I think it's taken care of in the parent class though when we call super, so it shouldn't be needed here
-        # self._data = {}
-        # self._helper_files = {}
-        
+
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
-        
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
 
-        # Call the parent class __init__ function
-        super().__init__(cancer_type="brca", source='broad', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="luad", source='broad', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
+        """Loads and preprocesses the mapping files. Generates helper tables for later use."""
         df_type = 'mapping'
         
-        # Since this is the only location where things are added to _helper_tables, just check if they are empty
-        # If they are empty, populate them
+        # If _helper_tables is empty, populate them
         if not self._helper_tables:
             file_path_list = self.locate_files(df_type)
             for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+                file_name = file_path.split('/')[-1] # The last element will be the name of the file
                 
-                if file_name == "sample_descriptions.tsv":
+                # Sample descriptions mapping
+                if file_name == "sample_descriptions.tsv.gz":
                     broad_key = pd.read_csv(file_path, sep="\t")
-                    broad_key = broad_key.loc[broad_key['cohort'] == "BRCA"] # get only BRCA keys
+                    broad_key = broad_key.loc[broad_key['cohort'] == "LUAD"] #get only LUAD keys
                     broad_key = broad_key[["sample_id","GDC_id","tissue_type"]]
-                    broad_key = broad_key.set_index("sample_id") # set broad id as index
-                    # add tumor type identification to end
+                    broad_key = broad_key.set_index("sample_id")#set broad id as index
+                    #key only the main Patient IDs (first 9 characters) and remove the -0N aliqout IDs
+                    broad_key['GDC_id'] = broad_key['GDC_id'].str[:9]
+                    #add tumor type identification to end
                     broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
-                    # change so tumor samples have nothing on end of id and .N for normal samples
+                    #change so tumor samples have nothing on end of id and .N for normal samples
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
-                    # convert df to dictionary
+                    #covert df to dictionary
                     broad_dict = broad_key.to_dict()["Patient_ID"]
                     self._helper_tables["broad_key"] = broad_dict
                     
-                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf":
+                # Gene name mapping   
+                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz":
                     broad_gene_names = read_gtf(file_path)
+                    broad_gene_names = broad_gene_names.as_df()
                     broad_gene_names = broad_gene_names[["gene_name","gene_id"]]
                     broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) #change name to merge 
                     broad_gene_names = broad_gene_names.set_index("gene_id")
-                    broad_gene_names = broad_gene_names.drop_duplicates()                
+                    broad_gene_names = broad_gene_names.drop_duplicates()
                     self._helper_tables["broad_gene_names"] = broad_gene_names
-
+                    
+                # Aliquot to patient ID mapping    
+                elif file_name == "aliquot_to_patient_ID.tsv.gz":
+                    df = pd.read_csv(file_path, sep = "\t", index_col = 0)
+                    self._helper_tables["map_ids"] = df
 
     def load_transcriptomics(self):
+        """Loads and preprocesses the transcriptomics data."""
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df = df.set_index(["transcript_id","gene_id"])
             
             # Add gene names to transcriptomic data
             self.load_mapping()
             broad_gene_names = self._helper_tables["broad_gene_names"]
-            broad_dict = self._helper_tables["broad_key"]        
-            df = broad_gene_names.join(df, how = "left") #merge in gene names keep transcripts that have a gene name
+            broad_dict = self._helper_tables["broad_key"]
+            mapping_df = self._helper_tables["map_ids"]
+            aliquot_dict = mapping_df.to_dict()["patient_ID"]        
+            df = broad_gene_names.join(df,how = "left") #merge in gene names keep transcripts that have a gene name
             df = df.reset_index()
             df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"})
             df = df.set_index(["Name","Transcript_ID","Database_ID"])
             df = df.rename(columns = broad_dict)# rename columns with CPTAC IDs
-            df = df.sort_index() 
+            df = df.rename(columns = aliquot_dict) 
             df = df.T
-            df.index.name = "Patient_ID"
+            # average duplicates: C3N-00545-03 and C3N-00545-01 were seperated out as two different aliqout ids. 
+            # They are from the same sample, so we average them. 
+            df = df.groupby("index", level = 0).mean() 
+            df.index.name = "Patient_ID"     
             # save df in self._data
             self.save_df(df_type, df)
-
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/broad/broadccrcc.py` & `cptac-1.5.0rc3/cptac/cancers/broad/broadccrcc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,112 +1,106 @@
-#   Copyright 2018 Samuel Payne sam_payne@byu.edu
-#   Licensed under the Apache License, Version 2.0 (the "License");
-#   you may not use this file except in compliance with the License.
-#   You may obtain a copy of the License at
-#       http://www.apache.org/licenses/LICENSE-2.0
-#   Unless required by applicable law or agreed to in writing, software
-#   distributed under the License is distributed on an "AS IS" BASIS,
-#   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#   See the License for the specific language governing permissions and
-#   limitations under the License.
+# Copyright 2018 Samuel Payne sam_payne@byu.edu
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#     http://www.apache.org/licenses/LICENSE-2.0
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 import pandas as pd
-import numpy as np
 import os
-import warnings
-from gtfparse import read_gtf
-
+from pyranges import read_gtf
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-
 
 class BroadCcrcc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which broadccrcc dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+    def __init__(self, no_internet=False):
+        """
+        Initialize the BroadCcrcc object.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. 
+        This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. 
+        Default is False.
         """
-        
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "CCRCC.rsem_transcripts_tpm.txt.gz",
-                "mapping" : ["sample_descriptions.tsv", "gencode.v34.GRCh38.genes.collapsed_only.gtf"]
-            }
+            "transcriptomics" : "CCRCC.rsem_transcripts_tpm.txt.gz",
+            "mapping" : ["sample_descriptions.tsv.gz", "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz"]
         }
         
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ccrcc", source='broad', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="ccrcc", source='broad', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
+        """
+        Load mapping from the provided files.
+        """
         df_type = 'mapping'
         
-        # Since this is the only location where things are added to _helper_tables, just check if they are empty
-        # If they are empty, populate them
+        # If _helper_tables are empty, populate them
         if not self._helper_tables:
             file_path_list = self.locate_files(df_type)
             for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
+                path_elements = file_path.split('/') # Get a list of the levels of the path
                 file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
                 
-                if file_name == "sample_descriptions.tsv":
+                if file_name == "sample_descriptions.tsv.gz":
+                    # Load broad keys specific for CCRCC
                     broad_key = pd.read_csv(file_path, sep="\t")
-                    broad_key = broad_key.loc[broad_key['cohort'] == "CCRCC"] #get only CCRCC keys
+                    broad_key = broad_key.loc[broad_key['cohort'] == "CCRCC"]
                     broad_key = broad_key[["sample_id","GDC_id","tissue_type"]]
-                    broad_key = broad_key.set_index("sample_id")#set broad id as index
-                    #add tumor type identification to end
-                    broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
-                    #change so tumor samples have nothing on end of id and .N for normal samples
+                    broad_key = broad_key.set_index("sample_id") # set broad id as index
+                    
+                    # Add tumor type identification to end and standardize patient id format
+                    broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"]
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
-                    #convert df to dictionary
+                    
+                    # Convert df to dictionary
                     broad_dict = broad_key.to_dict()["Patient_ID"]
                     self._helper_tables["broad_key"] = broad_dict
                     
-                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf":
+                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz":
+                    # Load broad gene names
                     broad_gene_names = read_gtf(file_path)
+                    broad_gene_names = broad_gene_names.as_df()
                     broad_gene_names = broad_gene_names[["gene_name","gene_id"]]
-                    broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) #change name to merge 
+                    broad_gene_names = broad_gene_names.rename(columns = {"gene_name":"Name"}) #change name to merge 
                     broad_gene_names = broad_gene_names.set_index("gene_id")
-                    broad_gene_names = broad_gene_names.drop_duplicates()
+                    broad_gene_names = broad_gene_names.drop_duplicates()                
                     self._helper_tables["broad_gene_names"] = broad_gene_names
         
     def load_transcriptomics(self):
+        """
+        Load transcriptomics data from the provided file.
+        """
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Perform initial checks and get file path
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df = df.set_index(["transcript_id","gene_id"])
             
             # Add gene names to transcriptomic data
             self.load_mapping()
             broad_gene_names = self._helper_tables["broad_gene_names"]
             broad_dict = self._helper_tables["broad_key"]        
-            df = broad_gene_names.join(df, how = "left") #merge in gene names keep transcripts that have a gene name
+            df = broad_gene_names.join(df, how = "left") # Merge in gene names, keep transcripts that have a gene name
             df = df.reset_index()
             df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"})
             df = df.set_index(["Name","Transcript_ID","Database_ID"])
-            df = df.rename(columns = broad_dict)# rename columns with CPTAC IDs
+            df = df.rename(columns = broad_dict) # Rename columns with CPTAC IDs
             df = df.sort_index() 
             df = df.T
             df.index.name = "Patient_ID"
-            # save df in self._data
-            self.save_df(df_type, df)
+            
+            # Save df in self._data
+            self.save_df(df_type, df)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/broad/broadcoad.py` & `cptac-1.5.0rc3/cptac/cancers/broad/broadlscc.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,108 +6,91 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
 import os
-import warnings
-from gtfparse import read_gtf
-
+from pyranges import read_gtf
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-
-
-class BroadCoad(Source):
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which broadcoad dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+class BroadLscc(Source):
+    def __init__(self, no_internet=False):
+        """Define which broadlscc dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
         
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        # Define data files and their corresponding loading functions
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "Colon.rsem_transcripts_tpm.txt.gz",
-                "mapping" : ["sample_descriptions.tsv", "gencode.v34.GRCh38.genes.collapsed_only.gtf"]
-            }
+            "transcriptomics" : "LSCC.rsem_transcripts_tpm.txt.gz",
+            "mapping" : ["sample_descriptions.tsv.gz", "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz"]
         }
         
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="coad", source='broad', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="lscc", source='broad', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
+        """Load the mapping data, if it has not been loaded yet"""
         df_type = 'mapping'
         
-        # Since this is the only location where things are added to _helper_tables, just check if they are empty
-        # If they are empty, populate them
         if not self._helper_tables:
             file_path_list = self.locate_files(df_type)
             for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+                path_elements = file_path.split('/') # Split the path into components
+                file_name = path_elements[-1] # Extract the file name
                 
-                if file_name == "sample_descriptions.tsv":
+                # Load and process sample description
+                if file_name == "sample_descriptions.tsv.gz":
                     broad_key = pd.read_csv(file_path, sep="\t")
-                    broad_key = broad_key.loc[broad_key['cohort'] == "Colon"] #get only HNSCC keys
+                    broad_key = broad_key.loc[broad_key['cohort'] == "LSCC"] # Filter LSCC keys
                     broad_key = broad_key[["sample_id","GDC_id","tissue_type"]]
-                    broad_key = broad_key.set_index("sample_id")#set broad id as index
-                    #add tumor type identification to end
+                    broad_key = broad_key.set_index("sample_id") # Set broad id as index
+                    # Add tissue type to patient ID
                     broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
-                    #change so tumor samples have nothing on end of id and .N for normal samples
+                    # Standardize patient ID format
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
-                    #covert df to dictionary
+                    # Convert dataframe to dictionary
                     broad_dict = broad_key.to_dict()["Patient_ID"]
                     self._helper_tables["broad_key"] = broad_dict
                     
-                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf":
+                # Load and process gene names
+                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz":
                     broad_gene_names = read_gtf(file_path)
+                    broad_gene_names = broad_gene_names.as_df()
                     broad_gene_names = broad_gene_names[["gene_name","gene_id"]]
-                    broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) #change name to merge 
+                    broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) # Change column name for merging
                     broad_gene_names = broad_gene_names.set_index("gene_id")
                     broad_gene_names = broad_gene_names.drop_duplicates()
                     self._helper_tables["broad_gene_names"] = broad_gene_names
-        
-      
+
     def load_transcriptomics(self):
+        """Load transcriptomics data, if it has not been loaded yet"""
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df = df.set_index(["transcript_id","gene_id"])
             
             # Add gene names to transcriptomic data
             self.load_mapping()
             broad_gene_names = self._helper_tables["broad_gene_names"]
             broad_dict = self._helper_tables["broad_key"]        
-            df = broad_gene_names.join(df, how = "left") #merge in gene names keep transcripts that have a gene name
+            df = broad_gene_names.join(df, how = "left") # Merge in gene names, keep transcripts that have a gene name
             df = df.reset_index()
             df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"})
             df = df.set_index(["Name","Transcript_ID","Database_ID"])
-            df = df.rename(columns = broad_dict)# rename columns with CPTAC IDs
+            df = df.rename(columns = broad_dict) # Rename columns with CPTAC IDs
             df = df.sort_index() 
             df = df.T
             df.index.name = "Patient_ID"
-            # save df in self._data
-            self.save_df(df_type, df)
+            # Save dataframe in self._data
+            self.save_df(df_type, df)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/broad/broadgbm.py` & `cptac-1.5.0rc3/cptac/cancers/broad/broaducec.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,108 +6,109 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-from gtfparse import read_gtf
-
+from pyranges import read_gtf
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-
 
-class BroadGbm(Source):
+class BroadUcec(Source):
+    """
+    This class handles the loading and providing of data for the Uterine Corpus Endometrial Carcinoma (UCEC) from the Broad Institute.
+    It inherits from the Source parent class.
+    """
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which broadgbm dataframes as are available in the self.load_functions dictionary variable, with names as keys.
-
-        Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+    def __init__(self, no_internet=False):
         """
+        Initializes the BroadUcec object. It specifies the available dataframes and their respective load functions.
         
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
+        Parameters:
+        no_internet (bool): If True, the index update step (which requires internet connection) will be skipped. Defaults to False.
+        """
 
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "GBM.rsem_transcripts_tpm.txt.gz",
-                "mapping" : ["sample_descriptions.tsv", "gencode.v34.GRCh38.genes.collapsed_only.gtf"]
-            }
+            "transcriptomics" : "UCEC.rsem_transcripts_tpm.txt.gz",
+            "mapping" : ["sample_descriptions.tsv.gz", "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz", "aliquot_to_patient_ID.tsv.gz"]
         }
         
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
-        # Call the parent class __init__ function
-        super().__init__(cancer_type="gbm", source='broad', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="ucec", source='broad', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
-        df_type = 'mapping'
-        
-        # Since this is the only location where things are added to _helper_tables, just check if they are empty
-        # If they are empty, populate them
+        """
+        This method populates the _helper_tables dictionary with dataframes necessary for mapping and identifying data.
+        It loads three types of mapping data - broad_keys, broad_gene_names, and map_ids.
+        """
         if not self._helper_tables:
-            file_path_list = self.locate_files(df_type)
-            for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
-                
-                if file_name == "sample_descriptions.tsv":
-                    broad_key = pd.read_csv(file_path, sep="\t")
-                    broad_key = broad_key.loc[broad_key['cohort'] == "GBM"] #get only GBM keys
-                    broad_key = broad_key[["sample_id","GDC_id","tissue_type"]]
-                    broad_key = broad_key.set_index("sample_id")#set broad id as index
-                    #add tumor type identification to end
-                    broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
-                    #change so tumor samples have nothing on end of id and .N for normal samples
-                    broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
-                    broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
-                    #covert df to dictionary
-                    broad_dict = broad_key.to_dict()["Patient_ID"]
-                    self._helper_tables["broad_key"] = broad_dict
-                    
-                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf":
-                    broad_gene_names = read_gtf(file_path)
-                    broad_gene_names = broad_gene_names[["gene_name","gene_id"]]
-                    broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) #change name to merge 
-                    broad_gene_names = broad_gene_names.set_index("gene_id")
-                    broad_gene_names = broad_gene_names.drop_duplicates()
-                    self._helper_tables["broad_gene_names"] = broad_gene_names
-        
+            self._load_broad_keys()
+            self._load_broad_gene_names()
+            self._load_map_ids()
 
     def load_transcriptomics(self):
+        """
+        This method loads the transcriptomics data and combines it with the mapping data to create a dataframe with appropriate gene and patient identifiers.
+        """
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep="\t")
-            df = df.set_index(["transcript_id","gene_id"])
+            df = pd.read_csv(file_path, sep="\t").set_index(["transcript_id","gene_id"])
             
             # Add gene names to transcriptomic data
             self.load_mapping()
-            broad_gene_names = self._helper_tables["broad_gene_names"]
-            broad_dict = self._helper_tables["broad_key"]        
-            df = broad_gene_names.join(df, how = "left") #merge in gene names keep transcripts that have a gene name
-            df = df.reset_index()
-            df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"})
-            df = df.set_index(["Name","Transcript_ID","Database_ID"])
-            df = df.rename(columns = broad_dict)# rename columns with CPTAC IDs
-            df = df.sort_index() 
-            df = df.T
-            df.index.name = "Patient_ID"
-            # save df in self._data
-            self.save_df(df_type, df)
+            df = self._add_gene_names(df)
+            df = self._rename_with_identifiers(df)
+            self.save_df(df_type, df)
+
+    # Additional methods to split the loading process
+    def _load_broad_keys(self):
+        """
+        Helper method to load the broad keys dataframe.
+        """
+        file_path = self.locate_files("sample_descriptions.tsv.gz")
+        broad_key = pd.read_csv(file_path, sep="\t")
+        broad_key = broad_key.loc[broad_key['cohort'] == "UCEC"][["sample_id","GDC_id","tissue_type"]].set_index("sample_id")
+        broad_key['GDC_id'] = broad_key['GDC_id'].str[:9]
+        broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"]
+        broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
+        broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
+        self._helper_tables["broad_key"] = broad_key.to_dict()["Patient_ID"]
+
+    def _load_broad_gene_names(self):
+        """
+        Helper method to load the broad gene names dataframe.
+        """
+        file_path = self.locate_files("gencode.v34.GRCh38.genes.collapsed_only.gtf.gz")
+        broad_gene_names = read_gtf(file_path).as_df()
+        broad_gene_names = broad_gene_names[["gene_name","gene_id"]].rename(columns= {"gene_name":"Name"}).set_index("gene_id").drop_duplicates()
+        self._helper_tables["broad_gene_names"] = broad_gene_names
+
+    def _load_map_ids(self):
+        """
+        Helper method to load the map ids dataframe.
+        """
+        file_path = self.locate_files("aliquot_to_patient_ID.tsv.gz")
+        self._helper_tables["map_ids"] = pd.read_csv(file_path, sep = "\t", index_col = 0)
+
+    def _add_gene_names(self, df):
+        """
+        Helper method to join the dataframe with the broad gene names.
+        """
+        df = self._helper_tables["broad_gene_names"].join(df, how = "left").reset_index()
+        df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"}).set_index(["Name","Transcript_ID","Database_ID"])
+        return df
+
+    def _rename_with_identifiers(self, df):
+        """
+        Helper method to rename the dataframe with the identifiers.
+        """
+        broad_dict = self._helper_tables["broad_key"]
+        aliquot_dict = self._helper_tables["map_ids"].to_dict()["patient_ID"]
+        df = df.rename(columns = broad_dict).rename(columns = aliquot_dict).sort_index()
+        df = df.T.groupby("index", level = 0).mean()  # Average duplicates 
+        df.index.name = "Patient_ID"
+        return df
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/broad/broadhnscc.py` & `cptac-1.5.0rc3/cptac/cancers/broad/broadpdac.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,97 +6,98 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
 import os
-import warnings
-from gtfparse import read_gtf
-
+from pyranges import read_gtf
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-
-
-class BroadHnscc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which broadhnscc dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
+class BroadPdac(Source):
+    """
+    The class BroadPdac manages the transcriptomics and mapping data for pancreatic ductal adenocarcinoma (PDAC)
+    sourced from the Broad institute. It is a child class of the Source class.
+    """
+    
+    def __init__(self, no_internet=False):
+        """
+        Initializes the BroadPdac object with necessary attributes and calls the __init__ method of the parent class.
+        
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection.
+        Default is False.
         """
-
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        
+        # File paths for the transcriptomics and mapping data
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "HNSCC.rsem_transcripts_tpm.txt.gz",
-                "mapping" : ["sample_descriptions.tsv", "gencode.v34.GRCh38.genes.collapsed_only.gtf"]
-            }
+            "transcriptomics" : "PDAC.rsem_transcripts_tpm.txt.gz",
+            "mapping" : ["sample_descriptions.tsv.gz", "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz"]
         }
         
+        # Define the load functions for the different data types
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="hnscc", source='broad', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="pdac", source='broad', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
+        """
+        Populates the _helper_tables attribute with mapping data, if it is not already populated.
+        """
+        
         df_type = 'mapping'
         
-        # Since this is the only location where things are added to _helper_tables, just check if they are empty
-        # If they are empty, populate them
+        # Populate _helper_tables if it's empty
         if not self._helper_tables:
             file_path_list = self.locate_files(df_type)
             for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+                path_elements = file_path.split('/') # Get a list of the levels of the path
+                file_name = path_elements[-1] # Identify files for parsing
                 
-                if file_name == "sample_descriptions.tsv":
+                if file_name == "sample_descriptions.tsv.gz":
+                    # Load, filter and format sample descriptions data
                     broad_key = pd.read_csv(file_path, sep="\t")
-                    broad_key = broad_key.loc[broad_key['cohort'] == "HNSCC"] #get only HNSCC keys
+                    broad_key = broad_key.loc[broad_key['cohort'] == "PDAC"] #get only PDAC keys
                     broad_key = broad_key[["sample_id","GDC_id","tissue_type"]]
                     broad_key = broad_key.set_index("sample_id")#set broad id as index
                     #add tumor type identification to end
                     broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
                     #change so tumor samples have nothing on end of id and .N for normal samples
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
                     #covert df to dictionary
                     broad_dict = broad_key.to_dict()["Patient_ID"]
                     self._helper_tables["broad_key"] = broad_dict
                     
-                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf":
+                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz":
+                    # Load and format gene names data
                     broad_gene_names = read_gtf(file_path)
+                    broad_gene_names = broad_gene_names.as_df()
                     broad_gene_names = broad_gene_names[["gene_name","gene_id"]]
                     broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) #change name to merge 
                     broad_gene_names = broad_gene_names.set_index("gene_id")
                     broad_gene_names = broad_gene_names.drop_duplicates()
                     self._helper_tables["broad_gene_names"] = broad_gene_names
-        
+
     def load_transcriptomics(self):
+        """
+        Loads and processes transcriptomics data, and saves it in the _data attribute.
+        """
+        
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Perform initial checks and get file path
             file_path = self.locate_files(df_type)
             
+            # Load and process transcriptomics data
             df = pd.read_csv(file_path, sep="\t")
             df = df.set_index(["transcript_id","gene_id"])
             
             # Add gene names to transcriptomic data
             self.load_mapping()
             broad_gene_names = self._helper_tables["broad_gene_names"]
             broad_dict = self._helper_tables["broad_key"]        
@@ -104,9 +105,9 @@
             df = df.reset_index()
             df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"})
             df = df.set_index(["Name","Transcript_ID","Database_ID"])
             df = df.rename(columns = broad_dict)# rename columns with CPTAC IDs
             df = df.sort_index() 
             df = df.T
             df.index.name = "Patient_ID"
-            # save df in self._data
+            # Save df in self._data
             self.save_df(df_type, df)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/broad/broadlscc.py` & `cptac-1.5.0rc3/cptac/cancers/broad/broadov.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,96 +6,79 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
 import os
-import warnings
-from gtfparse import read_gtf
-
+from pyranges import read_gtf
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-
-
-class BroadLscc(Source):
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which broadlscc dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+class BroadOv(Source):
+    def __init__(self, no_internet=False):
+        """Define which BroadOv dataframes are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
-        
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "LSCC.rsem_transcripts_tpm.txt.gz",
-                "mapping" : ["sample_descriptions.tsv", "gencode.v34.GRCh38.genes.collapsed_only.gtf"]
-            }
+            "transcriptomics" : "Ovary.rsem_transcripts_tpm.txt.gz",
+            "mapping" : ["sample_descriptions.tsv.gz", "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz"]
         }
         
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="lscc", source='broad', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="ov", source='broad', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
+        """Loads and preprocesses the mapping files. Generates helper tables for later use."""
         df_type = 'mapping'
         
-        # Since this is the only location where things are added to _helper_tables, just check if they are empty
-        # If they are empty, populate them
+        # If _helper_tables is empty, populate them
         if not self._helper_tables:
             file_path_list = self.locate_files(df_type)
             for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+                file_name = file_path.split('/')[-1] # The last element will be the name of the file
                 
-                if file_name == "sample_descriptions.tsv":
+                # Sample descriptions mapping
+                if file_name == "sample_descriptions.tsv.gz":
                     broad_key = pd.read_csv(file_path, sep="\t")
-                    broad_key = broad_key.loc[broad_key['cohort'] == "LSCC"] #get only LSCC keys
+                    broad_key = broad_key.loc[broad_key['cohort'] == "Ovary"] #get only OV keys
                     broad_key = broad_key[["sample_id","GDC_id","tissue_type"]]
                     broad_key = broad_key.set_index("sample_id")#set broad id as index
                     #add tumor type identification to end
                     broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
                     #change so tumor samples have nothing on end of id and .N for normal samples
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
                     broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
                     #covert df to dictionary
                     broad_dict = broad_key.to_dict()["Patient_ID"]
                     self._helper_tables["broad_key"] = broad_dict
                     
-                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf":
+                # Gene name mapping   
+                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz":
                     broad_gene_names = read_gtf(file_path)
+                    broad_gene_names = broad_gene_names.as_df()
                     broad_gene_names = broad_gene_names[["gene_name","gene_id"]]
                     broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) #change name to merge 
                     broad_gene_names = broad_gene_names.set_index("gene_id")
                     broad_gene_names = broad_gene_names.drop_duplicates()
                     self._helper_tables["broad_gene_names"] = broad_gene_names
-        
-        
+
     def load_transcriptomics(self):
+        """Loads and preprocesses the transcriptomics data."""
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep="\t")
             df = df.set_index(["transcript_id","gene_id"])
             
             # Add gene names to transcriptomic data
             self.load_mapping()
@@ -106,8 +89,8 @@
             df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"})
             df = df.set_index(["Name","Transcript_ID","Database_ID"])
             df = df.rename(columns = broad_dict)# rename columns with CPTAC IDs
             df = df.sort_index() 
             df = df.T
             df.index.name = "Patient_ID"
             # save df in self._data
-            self.save_df(df_type, df)
+            self.save_df(df_type, df)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/broad/broadov.py` & `cptac-1.5.0rc3/cptac/cancers/broad/broadbrca.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,108 +6,87 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
 import os
-import warnings
-from gtfparse import read_gtf
-
+from pyranges import read_gtf
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-
-
-class BroadOv(Source):
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which broadov dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+class BroadBrca(Source):
+    def __init__(self, no_internet=False):
+        """Initialization of BroadBrca class.
 
-        Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        Args:
+            no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. Default is False.
         """
-        
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "transcriptomics" : "Ovary.rsem_transcripts_tpm.txt.gz",
-                "mapping" : ["sample_descriptions.tsv", "gencode.v34.GRCh38.genes.collapsed_only.gtf"]
-            }
+            "transcriptomics" : "BRCA.rsem_transcripts_tpm.txt.gz",
+            "mapping" : ["sample_descriptions.tsv.gz", "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz"]
         }
-        
+
         self.load_functions = {
             'transcriptomics' : self.load_transcriptomics,
         }
-        
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
 
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ov", source='broad', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="brca", source='broad', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
+        """Load mapping file."""
+
         df_type = 'mapping'
-        
-        # Since this is the only location where things are added to _helper_tables, just check if they are empty
-        # If they are empty, populate them
+
+        # Check if helper tables are empty, if so, populate them
         if not self._helper_tables:
             file_path_list = self.locate_files(df_type)
             for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
-                
-                if file_name == "sample_descriptions.tsv":
-                    broad_key = pd.read_csv(file_path, sep="\t")
-                    broad_key = broad_key.loc[broad_key['cohort'] == "Ovary"] #get only OV keys
-                    broad_key = broad_key[["sample_id","GDC_id","tissue_type"]]
-                    broad_key = broad_key.set_index("sample_id")#set broad id as index
-                    #add tumor type identification to end
-                    broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
-                    #change so tumor samples have nothing on end of id and .N for normal samples
-                    broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
-                    broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
-                    #covert df to dictionary
-                    broad_dict = broad_key.to_dict()["Patient_ID"]
-                    self._helper_tables["broad_key"] = broad_dict
+                path_elements = file_path.split('/') # Split path into components
+                file_name = path_elements[-1] # Last element will be the file name
+
+                # Parse files based on file name
+                if file_name == "sample_descriptions.tsv.gz":
+                    # Processing for the sample descriptions file
+                    self._process_sample_descriptions(file_path)
                     
-                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf":
-                    broad_gene_names = read_gtf(file_path)
-                    broad_gene_names = broad_gene_names[["gene_name","gene_id"]]
-                    broad_gene_names = broad_gene_names.rename(columns= {"gene_name":"Name"}) #change name to merge 
-                    broad_gene_names = broad_gene_names.set_index("gene_id")
-                    broad_gene_names = broad_gene_names.drop_duplicates()
-                    self._helper_tables["broad_gene_names"] = broad_gene_names
-        
+                elif file_name == "gencode.v34.GRCh38.genes.collapsed_only.gtf.gz":
+                    # Processing for the gtf file
+                    self._process_gtf(file_path)
+
+    def _process_sample_descriptions(self, file_path):
+        """Process the sample descriptions file."""
+        broad_key = pd.read_csv(file_path, sep="\t")
+        broad_key = broad_key.loc[broad_key['cohort'] == "BRCA"]
+        broad_key = broad_key[["sample_id","GDC_id","tissue_type"]].set_index("sample_id")
+        broad_key["Patient_ID"] = broad_key["GDC_id"] + broad_key["tissue_type"] 
+        broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Tumor", "", regex=True)
+        broad_key.Patient_ID = broad_key.Patient_ID.str.replace(r"Normal", ".N", regex=True)
+        broad_dict = broad_key.to_dict()["Patient_ID"]
+        self._helper_tables["broad_key"] = broad_dict
+
+    def _process_gtf(self, file_path):
+        """Process the gtf file."""
+        broad_gene_names = read_gtf(file_path)
+        broad_gene_names = broad_gene_names.as_df()
+        broad_gene_names = broad_gene_names[["gene_name","gene_id"]].rename(columns = {"gene_name":"Name"}).set_index("gene_id")
+        broad_gene_names = broad_gene_names.drop_duplicates()                
+        self._helper_tables["broad_gene_names"] = broad_gene_names
 
     def load_transcriptomics(self):
+        """Load transcriptomics data."""
         df_type = 'transcriptomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep="\t")
-            df = df.set_index(["transcript_id","gene_id"])
-            
-            # Add gene names to transcriptomic data
+            df = pd.read_csv(file_path, sep="\t").set_index(["transcript_id","gene_id"])
+
             self.load_mapping()
             broad_gene_names = self._helper_tables["broad_gene_names"]
             broad_dict = self._helper_tables["broad_key"]        
-            df = broad_gene_names.join(df, how = "left") #merge in gene names keep transcripts that have a gene name
-            df = df.reset_index()
-            df = df.rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"})
-            df = df.set_index(["Name","Transcript_ID","Database_ID"])
-            df = df.rename(columns = broad_dict)# rename columns with CPTAC IDs
-            df = df.sort_index() 
+            df = broad_gene_names.join(df, how = "left")
+            df = df.reset_index().rename(columns= {"transcript_id": "Transcript_ID","gene_id":"Database_ID"}).set_index(["Name","Transcript_ID","Database_ID"])
+            df = df.rename(columns = broad_dict).sort_index() 
             df = df.T
             df.index.name = "Patient_ID"
-            # save df in self._data
-            self.save_df(df_type, df)
+            self.save_df(df_type, df)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/cancer.py` & `cptac-1.5.0rc3/cptac/cancers/cancer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,97 +6,84 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import logging
-import pandas as pd
 import numpy as np
 import re
 import warnings
+import pandas as pd
 
 from functools import reduce
 
 import cptac.utils as ut
 
 from cptac.exceptions import *
-from cptac.tools.dataframe_tools import add_index_levels, join_col_to_dataframe, sort_df_by_sample_status
-from cptac.tools.dataframe_tools import unionize_indices, generate_sample_status_col
+from cptac.tools.dataframe_tools import add_index_levels, join_col_to_dataframe
 
 class Cancer:
-    """Note that all cancer datasets are class objects that inherit from cptac.dataset. Therefore
-    the same function calls exist for cptac.Brca, cptac.Gbm, etc.
+    NORMAL_ENDINGS = ('.N', '.C') # HNSCC data has cored normal samples marked .C
+    """Note that all cancer datasets are class objects that inherit 
+        from cptac.cancer.
+    Therefore the same function calls exist for cptac.Brca, cptac.Gbm, etc.
     """
 
-    def __init__(self, cancer_type, attempt_update_index=True, skip_init=False):
+    def __init__(self, cancer_type: str):
         """Initialize variables for a Cancer object.
 
         Parameters:
         cancer_type (str): The cancer type requested for this dataset
-
         """
 
         self._cancer_type = cancer_type
         self._sources = {} # Child class __init__ needs to fill this
 
-        self._valid_omics_dfs = [
+        self._valid_omics_dfs = {
             'acetylproteomics',
             'circular_RNA',
             'CNV',
-            'lincRNA',
-            'lipidomics',
-            'metabolomics',
             'miRNA',
             'phosphoproteomics',
-            'phosphoproteomics_gene',
             'proteomics',
             'somatic_mutation_binary',
-            'transcriptomics', 
-            'CNV_log2ratio',
-            'CNV_gistic'
-             ]
+            'transcriptomics',
+            }   
 
-        self._valid_metadata_dfs = [
+        self._valid_metadata_dfs = {
             "clinical",
+            "medical_history",
             "derived_molecular",
-            "experimental_design",
-            #"followup", # Right now there are duplicate rows, so don't include follow up tables for joins.
-            ] # We don't allow the treatment df, as in Ovarian, or medical_history df, as in Ccrcc, because they both have multiple rows for each sample.
-
+            "cibersort",
+            "xcell",
+            "ancestry_prediction",
+            "hla_typing",
+            "followup",
+            } 
 
         #ignore logging messages
         logger = logging.getLogger()
         logger.setLevel(logging.CRITICAL)
 
-    def set_source_version(self, source, version):
-        """Set the data version you wish to use for a single source
-
-        Parameters:
-        source (string): the desired source (e.g. 'broad' or 'washu')
-        version (string): the desired version (e.g. '3.1' or 'latest')
-        """
-        self._sources[source].set_version(version)
-        print(f"{self._cancer_type} cancer data from source {source} now using data freeze {self._sources[source].get_version()}")
-
-    def delete_df(self, df_type, source='all'):
+    def delete_df(self, df_type: str, source: str='all'):
         '''This function enables users to delete dataframes they no longer need to free up RAM
 
         Parameters:
-        df_type (string): The type of dataframe to delete. For example, if the proteomics dataframe was loaded 
-            with get_proteomics() then they would pass 'proteomics' to this function to delete it.
+        df_type (string): The type of dataframe to delete. For example, if the proteomics dataframe
+            was loaded with get_proteomics() then they would pass 'proteomics' to this function to delete it.
         source (string): The source from which to delete the dataframe of type df_type
             Default: 'all' loops through all sources, checks for that df_type and deletes it if present
         '''
         # list of sources from which the df_type was deleted
         deleted_from = None
 
         if source == 'all':
             deleted_from = list()
-            for key in self._sources.keys():
+            for key in self._sources:
                 if df_type in self._sources[key]._data:
                     del self._sources[key]._data[df_type]
                     deleted_from.append(key)
         else:
             if df_type in self._sources[source]._data:
                 del self._sources[source]._data[df_type]
                 deleted_from = source
@@ -104,187 +91,143 @@
         if deleted_from:
             print(f"{df_type} deleted from {deleted_from}.")
         else:
             warnings.warn(f"{df_type} not found for deletion. Perhaps you misspelled the df_type ({df_type}) or meant to delete a different dataframe?")
 
 
     # Clinical table getters
-    def get_clinical(self, source=None, tissue_type="both", imputed=False):
+    def get_clinical(self, source: str= None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get the clinical dataframe from the specified data source."""
-        return self.get_dataframe("clinical", source, tissue_type, imputed=imputed)
-
-    def get_demographic(self, source=None, tissue_type="both", imputed=False):
-        """Get the demographic dataframe from the specified data source."""
-        return self.get_dataframe("demographic", source, tissue_type, imputed=imputed)
-
-    def get_derived_molecular(self, source=None, tissue_type="both"):
-        """Get the derived_molecular dataframe."""
-        return self.get_dataframe("derived_molecular", source, tissue_type)
-
-    def get_experimental_design(self, source=None, tissue_type="both"):
-        """Get the experimental_design dataframe."""
-        return self.get_dataframe("experimental_design", source, tissue_type)
-
-    def get_medical_conditions(self, source=None, tissue_type="both", imputed=False):
-        """Get the medical_conditions dataframe from the specified data source."""
-        return self.get_dataframe("medical_conditions", source, tissue_type, imputed=imputed)
+        df = self.get_dataframe("clinical", source, tissue_type, imputed=imputed)
+        df.columns = df.columns.str.split('/').str[-1] # Keep only the part after the slash
+        return df
 
     def get_medical_history(self, source=None, tissue_type="both"):
         """Get the medical_history dataframe."""
-        return self.get_dataframe("medical_history", source, tissue_type)
-
-    def get_previous_cancer(self, source=None, tissue_type="both", imputed=False):
-        """Get the previous_cancer dataframe from the specified data source."""
-        return self.get_dataframe("previous_cancer", source, tissue_type, imputed=imputed)
-
-    def get_cancer_diagnosis(self, source=None, tissue_type="both", imputed=False):
-        """Get the cancer_diagnosis dataframe from the specified data source."""
-        return self.get_dataframe("cancer_diagnosis", source, tissue_type, imputed=imputed)
+        df = self.get_dataframe("medical_history", source, tissue_type)
+        df.columns = df.columns.str.split('/').str[-1]  # Keep only the part after the slash
+        return df
 
     def get_followup(self, source=None, tissue_type="both", imputed=False):
         """Get the followup dataframe from the specified data source."""
-        return self.get_dataframe("followup", source, tissue_type, imputed=imputed)
+        df = self.get_dataframe("follow-up", source, tissue_type)
+        df.columns = df.columns.str.split('/').str[-1]  # Keep only the part after the slash
+        return df
 
+    def get_derived_molecular(self, type, source=None, tissue_type="both", imputed=False):
+        """Get type of derived_molecular dataframe. Valid types are cibersort, xcell, hla_typing, and ancestry_prediction"""
+        df = self.get_dataframe(type, source, tissue_type)
+        return df
 
+    # derived_molecular get functions to use in joining
+    def get_cibersort(self, source=None, tissue_type="both", imputed=False):
+        """Get cibersort data from the specified data source"""
+        df = self.get_dataframe("cibersort", source, tissue_type)
+        return df
 
+    def get_xcell(self, source=None, tissue_type="both", imputed=False):
+        """Get xcell data from the specified data source"""
+        df = self.get_dataframe("xcell", source, tissue_type)
+        return df
+    
+    def get_ancestry_prediction(self, source=None, tissue_type="both", imputed=False):
+        """Get ancestry_prediction data from the specified data source"""
+        df = self.get_dataframe("ancestry_prediction", source, tissue_type)
+        return df
+    
+    def get_hla_typing(self, source=None, tissue_type="both", imputed=False):
+        """Get hla_typing data from the specified data source"""
+        df = self.get_dataframe("hla_typing", source, tissue_type)
+        return df
+    
     # Quantitative table getters
-    def get_acetylproteomics(self, source, tissue_type="both", imputed=False):
-        """Get the acetylproteomics dataframe from the specified data source."""
-        return self.get_dataframe("acetylproteomics", source, tissue_type, imputed=imputed)
-
-    def get_acetylproteomics_gene(self, source=None, tissue_type="both"):
-        """Get the acetylproteomics_gene dataframe. The gene level acetylation measurement is an aggregate metric which potentially averages together individual measurements of different sites. Use get_acetylproteomics() to view the data for individual sites."""
-        return self.get_dataframe("acetylproteomics_gene", source, tissue_type)
-
-    def get_circular_RNA(self, source=None, tissue_type="both", imputed=False):
+    def get_circular_RNA(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get a circular RNA dataframe from the specified data source."""
         return self.get_dataframe("circular_RNA", source, tissue_type, imputed=imputed)
 
-    def get_CNV(self, source=None, tissue_type="both", imputed=False):
+    def get_CNV(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get a CNV dataframe from the specified data source."""
         return self.get_dataframe("CNV", source, tissue_type, imputed=imputed)
 
-    def get_deconvolution_cibersort(self, source=None, tissue_type="both", imputed=False):
-        """Get a deconvolution dataframe from the specified data source using the cibersort algorithm."""
-        return self.get_dataframe('xcell', source, tissue_type, imputed=imputed)
-
-    def get_deconvolution_xcell(self, source=None, tissue_type="both", imputed=False):
-        """Get a deconvolution dataframe from the specified data source using the cibersort algorithm."""
-        return self.get_dataframe('cibersort', source, tissue_type, imputed=imputed)
-
-    def get_deconvolution(self, deconv_algorithm=None, source=None, tissue_type="both", imputed=False):
-        """Get a deconvolution dataframe from the specified data source.
-
-        Parameters:
-        deconv_algorithm (str):  Choose an alorithm. Acceptable values are ['cibersort', 'xcell']. 
-        source (str): Select data generated by a certain institution. Available sources are ['washu']. Defaults to 'washu'. 
-        """
-        valid_algs = ['cibersort', 'xcell']
-        if deconv_algorithm is None or deconv_algorithm not in valid_algs:
-            raise InvalidParameterError(f"Please pass a valid value to the 'deconv_algorithm' parameter to specify which algorithm you want deconvolution data from. Valid options are {valid_algs}.")
-
-        return self.get_dataframe(deconv_algorithm, source, tissue_type, imputed=imputed)
-
-    def get_lincRNA(self, source=None, tissue_type="both"):
-        """Get the lincRNA dataframe."""
-        return self.get_dataframe("lincRNA",source, tissue_type)
-
-    def get_lipidomics(self, source=None, tissue_type="both"):
-        """Get the lipidomics dataframe."""
-        return self.get_dataframe("lipidomics", source, tissue_type)
-
-    def get_gene_fusion(self, source=None):
-        """Get the gene_fusion dataframe."""
-        return self.get_dataframe("gene_fusion", source)
-
-    def get_metabolomics(self, source=None, tissue_type="both"):
-        """Get the metabolomics dataframe."""
-        return self.get_dataframe("metabolomics", source, tissue_type)
-
-    def get_methylation(self, source=None, tissue_type="both"):
-        """Get the methylation dataframe."""
-        return self.get_dataframe("methylation", source, tissue_type)
-
-    def get_miRNA(self, source=None, miRNA_type='total', tissue_type="both", imputed=False):
+    def get_miRNA(self, source: str=None, miRNA_type: str='total', tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get miRNA dataframe from the specified data source.
 
         Parameters:
         source (str): Select data generated by a certain institution. Available sources are ['washu']. Defaults to 'washu'.
         miRNA_type (str): Choose the type of miRNA molecules measured. Acceptable values are ['total', 'precursor', 'mature'].
         """
         return self.get_dataframe(miRNA_type+'_miRNA', source, tissue_type, imputed=imputed)
 
-    def get_phosphoproteomics(self, source=None, tissue_type="both", imputed=False):
+    def get_phosphoproteomics(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get the phosphoproteomics dataframe from the specified data source."""
         return self.get_dataframe("phosphoproteomics", source, tissue_type, imputed=imputed)
 
-    def get_phosphoproteomics_gene(self, source=None, tissue_type="both"):
-        """Get the phosphoproteomics_gene dataframe. The gene level phosphorylation measurement is an aggregate metric which potentially averages together individual measurements of different sites. Use get_phosphoproteomics() to view the data for individual sites."""
-        return self.get_dataframe("phosphoproteomics_gene", source, tissue_type)
-
-    def get_phosphosites(self, genes, source=None):
-        """Returns dataframe with all phosphosites of specified gene or list of genes.
+    #def get_phosphosites(self, genes, source=None):
+        # """Returns dataframe with all phosphosites of specified gene or list of genes.
 
-        Parameters:
-        genes (str, or list or array-like of str): gene or list of genes to use to select phosphosites. str if single, list or array-like of str if multiple.
+        # Parameters:
+        # genes (str, or list or array-like of str): gene or list of genes to use to select phosphosites. str if single, list or array-like of str if multiple.
 
-        Returns:
-        pandas.DataFrame: The phosphoproteomics for the specified gene(s).
-        """
-        return self._get_omics_cols("phosphoproteomics", genes, source)
+        # Returns:
+        # pandas.DataFrame: The phosphoproteomics for the specified gene(s).
+        # """
+        # return self._get_omics_cols("phosphoproteomics", genes, source)
 
-    def get_proteomics(self, source=None, tissue_type="both", imputed=False):
+    def get_proteomics(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get the proteomics dataframe from the specified data source."""
         return self.get_dataframe("proteomics", source, tissue_type, imputed=imputed)
+    
+    def get_acetylproteomics(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
+        """Get the acetylproteomics dataframe from the specified data source."""
+        return self.get_dataframe("acetylproteomics", source, tissue_type, imputed=imputed)
 
-    def get_somatic_mutation(self, source=None, tissue_type="both", imputed=False):
+    def get_somatic_mutation(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get the somatic mutation dataframe from the specified data source."""
         return self.get_dataframe("somatic_mutation", source, tissue_type, imputed=imputed)
 
-    def get_somatic_mutation_binary(self, source=None):
+    def get_somatic_mutation_binary(self, source: str=None) -> pd.DataFrame:
         """Get the somatic_mutation_binary dataframe, which has a binary value indicating, for each location on each gene, whether there was a mutation in that gene at that location, for each sample."""
         return self.get_dataframe("somatic_mutation_binary", source)
 
-    def get_targeted_phosphoproteomics(self, source=None, tissue_type="both"):
+    def get_targeted_phosphoproteomics(self, source: str=None, tissue_type: str="both") -> pd.DataFrame:
         """Get the targeted_phosphoproteomics dataframe."""
         return self.get_dataframe("targeted_phosphoproteomics", source, tissue_type)
 
-    def get_targeted_proteomics(self, source=None, tissue_type="both"):
+    def get_targeted_proteomics(self, source: str=None, tissue_type: str="both") -> pd.DataFrame:
         """Get the targeted_proteomics dataframe."""
         return self.get_dataframe("targeted_proteomics", source, tissue_type)
 
-    def get_transcriptomics(self, source=None, tissue_type="both", imputed=False):
+    def get_transcriptomics(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get the transcriptomics dataframe from the specified data source."""
-        """source (str): Select data generated by a certain institution. Available sources are ['washu','bcm','broad']."""
         return self.get_dataframe("transcriptomics", source, tissue_type, imputed=imputed)
 
-    def get_treatment(self, source=None, tissue_type="both"):
-        """Get the treatment dataframe."""
-        return self.get_dataframe("treatment", source, tissue_type)
+    # def get_treatment(self, source=None, tissue_type="both"):
+        # """Get the treatment dataframe."""
+        # return self.get_dataframe("treatment", source, tissue_type)
 
-    def get_tumor_purity(self, source=None, tissue_type="both", imputed=False):
+    def get_tumor_purity(self, source: str=None, tissue_type: str="both", imputed: bool=False) -> pd.DataFrame:
         """Get the tumor purity dataframe from the specified data source."""
         return self.get_dataframe("tumor_purity", source, tissue_type, imputed=imputed)
 
-    def get_ubiquitylomics(self, source=None, tissue_type="both", imputed=False):
-        """Get the ubiquitylomics dataframe from the specified data source."""
-        return self.get_dataframe("ubiquitylomics", source, tissue_type, imputed=imputed)
+    # def get_ubiquitylomics(self, source=None, tissue_type="both", imputed=False):
+        # """Get the ubiquitylomics dataframe from the specified data source."""
+        # return self.get_dataframe("ubiquitylomics", source, tissue_type, imputed=imputed)
 
-    def get_docs(self, data, source=None, tissue_type="both", imputed=False):
+    def get_docs(self, data: str, source: str=None, tissue_type: str="both", imputed: bool=False):
         """Get the readme docs for the specified data type and source."""
         if source in self._datasets.keys():
-            obj = self._datasets[source] 
+            obj = self._datasets[source]
             print('README file for ' + data, '\n')
             print(obj._readme_files['readme_'+data])
             return 0
         else:
             raise DataSourceNotFoundError(f"Data source {source} not found for the {self._cancer_type} dataset.")
 
-    def define(self, term):
-        """Print the definition a term, if it is in the dataset's list of definitions.
+    def define(self, term: str):
+        """Print the definition of a term, if it is in the dataset's list of definitions.
 
         Parameters:
         term (str): term to be defined
 
         Returns: None
         """
         if len(self._definitions.keys()) == 0:
@@ -299,318 +242,405 @@
         if len(self._definitions.keys()) > 0:
             for term in sorted(self._definitions.keys(), key=str.lower):
                 print(term)
         else:
             raise NoDefinitionsError("No definitions provided for this dataset.")
 
     # Join functions
-    # Note: These are now helper functions that call multi_join on awg data by default
-    def join_omics_to_omics(self, df1_name, df2_name, df1_source=None, df2_source=None, genes1=None, genes2=None, how="outer", quiet=False, tissue_type="both"):
+    def quick_join(self, left_df_name: str, right_df_name: str, left_df_source: str=None, right_df_source: str=None, genes1: str=None, genes2: str=None, how: str='outer') -> pd.DataFrame:
+        """
+        Quickly join two specified cptac dataframes; optimized for speed.
+
+        Parameters:
+        left_df_name : str
+            Name of first dataframe. Must be in the form 'source name' if left_df_source is not provided. (ex. 'washu proteomics')
+        right_df_name : str
+            Name of the second dataframe. Must be in the form 'source name' if right_df_source is not provided.
+        left_df_source : str, optional
+            Name of source for the first dataframe. If left_df_name was in the form 'source name', this parameter is ignored.
+        right_df_source : str, optional
+            Name of source for the second dataframe. If right_df_name was in the form 'source name', this parameter is ignored.
+        genes1 : str or list of str, optional
+            Gene(s) for column(s) to select from the first dataframe. str if one key, list or array-like of str if multiple.
+            Default of None will select entire dataframe.
+        genes2 : str or list of str, optional
+            Gene(s) for column(s) to select from the second dataframe. str if one key, list or array-like of str if multiple.
+            Default of None will select entire dataframe.
+        how : str, optional
+            How to perform the join; see Pandas.DataFrame.join. Default is 'outer'.
+
+        Returns:
+        pandas.DataFrame
+            The selected columns from the two dataframes, joined into one dataframe.
+        """
+
+        if ' ' in left_df_name:
+            left_df_source, left_df_name = left_df_name.split(' ')
+        if ' ' in right_df_name:
+            right_df_source, right_df_name = right_df_name.split(' ')
+
+        if isinstance(genes1, str):
+            genes1 = [genes1]
+        if isinstance(genes2, str):
+            genes2 = [genes2]
+
+        try:
+            left_df = self.get_dataframe(left_df_name, left_df_source)
+            logging.info('Got first dataframe.')
+            right_df = self.get_dataframe(right_df_name, right_df_source)
+            logging.info('Got second dataframe.')
+        except Exception as e:
+            logging.error(f"Error occurred while fetching dataframes: {str(e)}")
+            raise e
+
+        if isinstance(left_df.columns, pd.MultiIndex):
+            left_df.columns = left_df.columns.droplevel('Database_ID')
+        if isinstance(right_df.columns, pd.MultiIndex):
+            right_df.columns = right_df.columns.droplevel('Database_ID')
+
+        left_df = left_df.add_prefix(left_df_name.title()+'_')
+        right_df = right_df.add_prefix(right_df_name.title()+'_')
+
+        try:
+            result = left_df.merge(right_df, left_index=True, right_index=True, how=how)
+            logging.info('Dataframes successfully merged.')
+        except Exception as e:
+            logging.error(f"Error occurred while merging dataframes: {str(e)}")
+            raise e
+
+        return result
+    
+
+    # Note: These are now helper functions that call multi_join
+    def join_omics_to_omics(self, df1_name: str, df2_name: str, df1_source: str=None, df2_source: str=None, genes1: str=None, genes2: str=None, how: str="outer", quiet:bool=False, tissue_type: str="both"
+                            ) -> pd.DataFrame:
         """Take specified column(s) from one omics dataframe, and join to specified columns(s) from another omics dataframe. Intersection (inner join) of indices is used.
 
         Parameters:
         df1_name (str): Name of first omics dataframe to select columns from.
         df2_name (str): Name of second omics dataframe to select columns from.
-        genes1 (str, or list or array-like of str, optional): Gene(s) for column(s) to select from df1_name. str if one key, list or array-like of str if multiple. Default of None will select entire dataframe.
-        genes2 (str, or list or array-like of str, optional): Gene(s) for Column(s) to select from df2_name. str if one key, list or array-like of str if multiple. Default of None will select entire dataframe.
+        df1_source (str): Name of source for the first omics dataframe.
+        df2_source (str): Name of source for the second omics dataframe.
+        genes1 (str, or list or array-like of str, optional): Gene(s) for column(s) to select from df1_name. str if one key, list or array-like of str if multiple.
+            Default of None will select entire dataframe.
+        genes2 (str, or list or array-like of str, optional): Gene(s) for Column(s) to select from df2_name. str if one key, list or array-like of str if multiple.
+            Default of None will select entire dataframe.
         how (str, optional): How to perform the join, acceptable values are from ['outer', 'inner', 'left', 'right']. Defaults to 'outer'.
         quiet (bool, optional): Whether to warn when inserting NaNs. Defaults to False.
-        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type desired in the dataframe. Defaults to "both".
+        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type for the dataframe. Defaults to "both".
 
         Returns:
         pandas.DataFrame: The selected columns from the two omics dataframes, joined into one dataframe.
         """
         # Check to make sure that the "how" parameter is valid
         self._check_how_parameter(how)
 
-        if df1_source is None:
-            df1_source = "awg"
-            warnings.warn(f"No source specified for {df1_name} data. Source awg used, pass a source to the df1_source parameter to prevent this warning", stacklevel=3)
-        if df2_source is None:
-            df2_source = "awg"
-            warnings.warn(f"No source specified for {df1_name} data. Source awg used, pass a source to the df2_source parameter to prevent this warning", stacklevel=3)
-
         # Set up parameters to work with multi_join
         df1_name = f"{df1_source} {df1_name}"
         df2_name = f"{df2_source} {df2_name}"
 
         if genes1 is None:
             genes1 = []
         if genes2 is None:
             genes2 = []
 
-        return self.multi_join({df1_name:genes1, df2_name:genes2}, how=how, tissue_type=tissue_type)
+        return self.multi_join({df1_name:genes1, df2_name:genes2}, how=how, tissue_type=tissue_type, flatten=True)
 
-    def join_omics_to_mutations(self, omics_name, mutations_genes, omics_source=None, mutations_source=None, omics_genes=None, mutations_filter=None, show_location=True, how="outer", quiet=False, tissue_type="both",mutation_cols=["Mutation","Location"]):
+    def join_omics_to_mutations(
+                self,
+				omics_name: str,
+				mutations_genes: str or list[str],
+				omics_source: str,
+				mutations_source: str,
+				omics_genes: str=None,
+				mutations_filter: str=None,
+				show_location: bool=True,
+				how: str="outer",
+				quiet: bool=False,
+				tissue_type: str="both",
+				mutation_cols: str or list=["Mutation","Location"]
+        ) -> pd.DataFrame:
         """Select all mutations for specified gene(s), and joins them to all or part of the given omics dataframe. Intersection (inner join) of indices is used. Each location or mutation cell contains a list, which contains the one or more location or mutation values corresponding to that sample for that gene, or a value indicating that the sample didn't have a mutation in that gene.
 
         Parameters:
         omics_df (str): Name of omics dataframe to join the mutation data to.
         mutations_genes (str, or list or array-like of str): The gene(s) to get mutation data for. str if one gene, list or array-like of str if multiple.
-        omics_genes (str, or list or array-like of str, optional): Gene(s) to select from the omics dataframe. str if one gene, list or array-like of str if multiple. Default will select entire dataframe.
-        mutations_filter (list, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority. If none of the multiple mutations in a sample are included in mutations_filter, the function will automatically prioritize truncation over missense mutations, and then mutations earlier in the sequence over later mutations. Passing an empty list will cause this default hierarchy to be applied to all samples. Default parameter of None will cause no filtering to be done, and all mutation data will be included, in a list.
+        omics_source (str, optional): Name of source for the omics data.
+        mutations_source (str, optional): Name of source for the mutations data.
+        omics_genes (str, or list or array-like of str, optional): Gene(s) to select from the omics dataframe.
+            str if one gene, list or array-like of str if multiple.
+            Default will select entire dataframe.
+        mutations_filter (list, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority.
+            If none of the multiple mutations in a sample are included in mutations_filter, the function will automatically prioritize
+                truncation over missense mutations, and then mutations earlier in the sequence over later mutations.
+            Passing an empty list will cause this default hierarchy to be applied to all samples.
+            Default parameter of None will cause no filtering to be done, and all mutation data will be included, in a list.
         show_location (bool, optional): Whether to include the Location column from the mutation dataframe. Defaults to True.
         how (str, optional): How to perform the join, acceptable values are from ['outer', 'inner', 'left', 'right']. Defaults to 'outer'.
         quiet (bool, optional): Whether to warn when inserting NaNs. Defaults to False.
-        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type desired in the dataframe. Defaults to "both".
+        tissue_type (str, optional): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type for the dataframe. Defaults to "both".
 
         Returns:
         pandas.DataFrame: The mutations for the specified gene, joined to all or part of the omics dataframe. Each location or mutation cell contains a list, which contains the one or more location or mutation values corresponding to that sample for that gene, or a value indicating that the sample didn't have a mutation in that gene.
         """
 
         # Check to make sure that the "how" parameter is valid
         self._check_how_parameter(how)
 
-        # Figure out sources, default to awg
-        if omics_source is None:
-            omics_source = "awg"
-            warnings.warn(f"No source specified for {omics_name} data. Source awg used, pass a source to the omics_source parameter to prevent this warning", stacklevel=3)
-        if mutations_source is None:
-            mutations_source = "awg"
-            warnings.warn(f"No source specified for mutations data. Source awg used, pass a source to the mutations_source parameter to prevent this warning", stacklevel=3)
-
         # Set up parameters to work with multi_join
         df1_name = f"{omics_source} {omics_name}"
         df2_name = f"{mutations_source} somatic_mutation"
 
         if omics_genes is None:
             genes1 = []
         else:
             genes1 = omics_genes
 
-        return self.multi_join({df1_name:genes1, df2_name:mutations_genes}, mutations_filter=mutations_filter, how=how, tissue_type=tissue_type)
+        return self.multi_join({df1_name:genes1, df2_name:mutations_genes}, mutations_filter=mutations_filter, how=how, tissue_type=tissue_type, flatten=True)
 
-    def join_metadata_to_metadata(self, df1_name, df2_name, df1_source=None, df2_source=None, cols1=None, cols2=None, how="outer", quiet=False, tissue_type="both"):
+    def join_metadata_to_metadata(self, df1_name: str, df2_name: str, df1_source: str=None, df2_source: str=None, cols1: str=None, cols2: str=None, how: str="outer", quiet: bool =False, tissue_type: str="both"
+                                  ) -> pd.DataFrame:
         """Take specified column(s) from one metadata dataframe, and join to specified columns(s) from another metadata dataframe. Intersection (inner join) of indices is used.
 
         Parameters:
         df1_name (str): Name of first metadata dataframe to select columns from.
         df2_name (str): Name of second metadata dataframe to select columns from.
-        cols1 (str, or list or array-like of str, optional): Column(s) to select from df1_name. str if one key, list or array-like of str if multiple. Default of None will select entire dataframe.
-        cols2 (str, or list or array-like of str, optional): Column(s) to select from df2_name. str if one key, list or array-like of str if multiple. Default of None will select entire dataframe.
+        df1_source (str, optional): Name of source for the first dataframe.
+        df2_source (str, optional): Name of source for the second dataframe.
+        cols1 (str, or list or array-like of str, optional): Column(s) to select from df1_name.
+            str if one key, list or array-like of str if multiple.
+            Default of None will select entire dataframe.
+        cols2 (str, or list or array-like of str, optional): Column(s) to select from df2_name.
+            str if one key, list or array-like of str if multiple.
+            Default of None will select entire dataframe.
         how (str, optional): How to perform the join, acceptable values are from ['outer', 'inner', 'left', 'right']. Defaults to 'outer'.
         quiet (bool, optional): Whether to warn when inserting NaNs. Defaults to False.
-        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type desired in the dataframe. Defaults to "both".
+        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type for the dataframe. Defaults to "both".
 
         Returns:
         pandas.DataFrame: The selected columns from the two metadata dataframes, joined into one dataframe.
         """
 
         # Check to make sure that the "how" parameter is valid
         self._check_how_parameter(how)
 
-        # Figure out sources, default to awg
-        if df1_source is None:
-            df1_source = "awg"
-            warnings.warn(f"No source specified for {df1_name} data. Source awg used, pass a source to the df1_source parameter to prevent this warning", stacklevel=3)
-        if df2_source is None:
-            df2_source = "awg"
-            warnings.warn(f"No source specified for {df1_name} data. Source awg used, pass a source to the df2_source parameter to prevent this warning", stacklevel=3)
-
         # Set up parameters to work with multi_join
         df1_name = f"{df1_source} {df1_name}"
         df2_name = f"{df2_source} {df2_name}"
 
         if cols1 is None:
             cols1 = []
         if cols2 is None:
             cols2 = []
 
-        return self.multi_join({df1_name:cols1, df2_name:cols2}, how=how, tissue_type=tissue_type)
+        return self.multi_join({df1_name:cols1, df2_name:cols2}, how=how, tissue_type=tissue_type, flatten=True)
 
-    def join_metadata_to_omics(self, metadata_name, omics_name, omics_source=None, metadata_source=None, metadata_cols=None, omics_genes=None, how="outer", quiet=False, tissue_type="both"):
+    def join_metadata_to_omics(self, metadata_name: str, omics_name: str, omics_source: str=None, metadata_source:str=None, metadata_cols: str=None, omics_genes: str=None, how: str="outer", quiet: bool=False, tissue_type: str="both"
+                               ) -> pd.DataFrame:
         """Joins columns from a metadata dataframe (clinical, derived_molecular, or experimental_design) to part or all of an omics dataframe. Intersection (inner join) of indices is used.
 
         Parameters:
         metadata_name (str): Name of metadata dataframe to select columns from.
         omics_name (str): Name of omics dataframe to join the metadata columns to.
-        metadata_cols (str, or list or array-like of str, optional): Column(s) to select from the metadata dataframe. str if one gene, list or array-like of str if multiple. Default is None, which will select the entire metadata dataframe.
-        omics_genes (str, or list or array-like of str, optional): Gene(s) to select data for from the omics dataframe. str if one gene, list or array-like of str if multiple. Default is None, which will select entire dataframe.
+        metadata_cols (str, or list or array-like of str, optional): Column(s) to select from the metadata dataframe.
+            str if one gene, list or array-like of str if multiple.
+            Default is None, which will select the entire metadata dataframe.
+        omics_genes (str, or list or array-like of str, optional): Gene(s) to select data for from the omics dataframe.
+            str if one gene, list or array-like of str if multiple.
+            Default is None, which will select entire dataframe.
         how (str, optional): How to perform the join, acceptable values are from ['outer', 'inner', 'left', 'right']. Defaults to 'outer'.
         quiet (bool, optional): Whether to warn when inserting NaNs. Defaults to False.
-        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type desired in the dataframe. Defaults to "both".
+        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type for the dataframe. Defaults to "both".
 
         Returns:
         pandas.DataFrame: The selected metadata columns, joined with all or part of the omics dataframe.
         """
 
         # Check to make sure that the "how" parameter is valid
         self._check_how_parameter(how)
 
-        # Figure out sources, default to awg
-        if omics_source is None:
-            omics_source = "awg"
-            warnings.warn(f"No source specified for {omics_name} data. Source awg used, pass a source to the omics_source parameter to prevent this warning", stacklevel=3)
-        if metadata_name is None:
-            metadata_name = "awg"
-            warnings.warn(f"No source specified for {metadata_name} data. Source awg used, pass a source to the mutations_source parameter to prevent this warning", stacklevel=3)
-
         # Set up parameters to work with multi_join
         df1_name = f"{metadata_source} {metadata_name}"
         df2_name = f"{omics_source} {omics_name}"
 
         if metadata_cols is None:
             genes1 = []
         else:
             genes1 = metadata_cols
         if omics_genes is None:
             genes2 = []
         else:
             genes2 = omics_genes
 
-        return self.multi_join({df1_name:genes1, df2_name:genes2}, how=how, tissue_type=tissue_type)
+        return self.multi_join({df1_name:genes1, df2_name:genes2}, how=how, tissue_type=tissue_type, flatten=True)
 
-    def join_metadata_to_mutations(self, metadata_name, mutations_genes, metadata_source=None, mutations_source=None,  metadata_cols=None, mutations_filter=None, show_location=True, how="outer", quiet=False, tissue_type="both"):
+    def join_metadata_to_mutations(self, metadata_name: str, mutations_genes: str or list[str], metadata_source: str=None, mutations_source: str=None,  metadata_cols: str=None, mutations_filter: str=None, show_location: bool=True, how: str="outer", quiet: bool=False,
+                                    tissue_type: str="both") -> pd.DataFrame:
         """Select all mutations for specified gene(s), and joins them to all or part of the given metadata dataframe. Intersection (inner join) of indices is used. Each location or mutation cell contains a list, which contains the one or more location or mutation values corresponding to that sample for that gene, or a value indicating that the sample didn't have a mutation in that gene.
 
         Parameters:
         metadata_name (str): Name of metadata dataframe to join the mutation data to.
         mutations_genes (str, or list or array-like of str): The gene(s) to get mutation data for. str if one gene, list or array-like of str if multiple.
-        metadata_cols (str, or list or array-like of str, optional): Gene(s) to select from the metadata dataframe. str if one gene, list or array-like of str if multiple. Default will select entire dataframe.
-        mutations_filter (list, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority. If none of the multiple mutations in a sample are included in mutations_filter, the function will automatically prioritize truncation over missense mutations, and then mutations earlier in the sequence over later mutations. Passing an empty list will cause this default hierarchy to be applied to all samples. Default parameter of None will cause no filtering to be done, and all mutation data will be included, in a list.
+        metadata_source (str, optional): Name of source for metadata.
+        mutations_source (str, optional): Name of source for mutations data.
+        metadata_cols (str, or list or array-like of str, optional): Gene(s) to select from the metadata dataframe. str if one gene, list or array-like of str if multiple.
+            Default will select entire dataframe.
+        mutations_filter (list, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority.
+            If none of the multiple mutations in a sample are included in mutations_filter, the function will automatically prioritize truncation over missense mutations, and then mutations earlier in the sequence over later mutations.
+            Passing an empty list will cause this default hierarchy to be applied to all samples.
+            Default parameter of None will cause no filtering to be done, and all mutation data will be included, in a list.
         show_location (bool, optional): Whether to include the Location column from the mutation dataframe. Defaults to True.
         how (str, optional): How to perform the join, acceptable values are from ['outer', 'inner', 'left', 'right']. Defaults to 'outer'.
         quiet (bool, optional): Whether to warn when inserting NaNs. Defaults to False.
-        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type desired in the dataframe. Defaults to "both".
+        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type for the dataframe. Defaults to "both".
 
         Returns:
         pandas.DataFrame: The mutations for the specified gene, joined to all or part of the metadata dataframe. Each location or mutation cell contains a list, which contains the one or more location or mutation values corresponding to that sample for that gene, or a value indicating that the sample didn't have a mutation in that gene.
         """
 
         # Check to make sure that the "how" parameter is valid
         self._check_how_parameter(how)
 
-        # Figure out sources, default to awg
-        if metadata_source is None:
-            metadata_source = "awg"
-            warnings.warn(f"No source specified for {metadata_name} data. Source awg used, pass a source to the metadata_source parameter to prevent this warning", stacklevel=3)
-        if mutations_source is None:
-            mutations_source = "awg"
-            warnings.warn(f"No source specified for mutations data. Source awg used, pass a source to the mutations_source parameter to prevent this warning", stacklevel=3)
-
         # Set up parameters to work with multi_join
         df1_name = f"{metadata_source} {metadata_name}"
         df2_name = f"{mutations_source} somatic_mutation"
 
         if metadata_cols is None:
             metadata_cols = []
 
-        return self.multi_join({df1_name:metadata_cols, df2_name:mutations_genes}, how=how, tissue_type=tissue_type, mutations_filter=mutations_filter)
-
-    def multi_join(self, join_dict, mutations_filter=None, flatten=False, levels_to_drop=[], how="outer", tissue_type="both"):    
-        """Takes a dictionary where keys include a source and datatype (either in a ('source', 'datatype') tuple or as a space separated string "source datatype"), and values are columns from those dataframes. Joins all the columns into one dataframe. If the value is an empty list it will join the entire dataframe
-
-        Parameters:
-        join_dict (dict): A dictionary with the dataframe and columns to join. Keys are the names of the dataframes and the value is a list of string with the name of the columns corresponding to each dataframe. Example: {('awg', 'phosphoproteomics'):['A2M', 'AAAS'],'awg proteomics':['AAAS', 'ZZZ3'], 'awg somatic_mutation':['AHCTF1', 'ZFHX3']}.
-
-            Valid dataframes are: acetylproteomics, CNV, phosphoproteomics, phosphoproteomics_gene, proteomics,
-            somatic_mutation_binary, somatic_mutation, transcriptomics, clinical, derived_molecular and experimental_design.
+        return self.multi_join({df1_name:metadata_cols, df2_name:mutations_genes}, how=how, tissue_type=tissue_type, mutations_filter=mutations_filter, flatten=True)
 
-            For somatic_mutation_binary it joins all columns that match a gene. Example {'awg somatic_mutation_binary' : ['A1CF', 'ZYG11B']} It returns a dataframe with all columns that contain those genes.
 
-        mutations_filter (list, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority. If none of the multiple mutations in a sample are included in mutations_filter, the function will automatically prioritize truncation over missense mutations, and then mutations earlier in the sequence over later mutations. Passing an empty list will cause this default hierarchy to be applied to all samples. Default parameter of None will cause no filtering to be done, and all mutation data will be included, in a list.
+    def _get_columns(self, datatype, source, data_key, tissue_type, mutations_filter=None):
+        """
+        Helper function to get the relevant columns for the join operation.
 
-        flatten (bool, optional): Defaults to False and will flatten the multiindexes if set to True.
+        Parameters:
+        datatype (str): Type of data to be joined. This can be one of several types, including 'omics' data and metadata.
+        source (str): Source of the data. For example, this could be 'bcm', 'phosphoproteomics', etc.
+        data_key (list): List of keys from the join_dict dictionary.
+        tissue_type (str): The type of tissue data to be retrieved. Can be "tumor","normal", or "both" if we're still doing that lol
+        mutations_filter (list, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority.
+            If none of the multiple mutations in a sample are included in mutations_filter, the function will automatically prioritize
+            truncation over missense mutations, and then mutations earlier in the sequence over later mutations.
+            Passing an empty list will cause this default hierarchy to be applied to all samples.
+            Default parameter of None will cause no filtering to be done, and all mutation data will be included, in a list.
+            
+        Returns:
+        pandas.DataFrame: A DataFrame that contains the relevant columns to be joined.
+        """
+        # If key belongs to omics
+        if datatype in self._valid_omics_dfs:
+            # If key is somatic_mutation_binary it will join all columns that match a gene
+            if datatype == "somatic_mutation_binary":
+                binary_data = "\n".join(list(self.get_somatic_mutation_binary(source).columns))
+                found_genes = [re.findall((gene + ".+\n"), binary_data) for gene in data_key] if data_key else []
+                found_genes = list(map(lambda x: x.strip("\n"), found_genes))
+                columns = self._get_omics_cols(datatype, source, found_genes or None, tissue_type=tissue_type)
+            else:
+                columns = self._get_omics_cols(datatype, source, data_key or None, tissue_type=tissue_type)
+        # If key belongs to metadata
+        elif datatype in self._valid_metadata_dfs:
+            columns = self._get_metadata_cols(datatype, source, data_key or None, tissue_type=tissue_type)
+        # If key is somatic_mutation
+        elif datatype == "somatic_mutation":
+            columns = self._get_genes_mutations(source, data_key, mutations_filter=mutations_filter)
+        else:
+            raise ValueError(f"Invalid datatype: {datatype}")
+        return columns
 
-        levels_to_drop (list, optional): Defaults to empty list. Takes a list of strings. Strings are levels to be dropped. If empty it will not drop any.
 
-        tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the desired tissue type desired in the dataframe. Defaults to "both"
+    def multi_join(self, join_dict: dict, mutations_filter: list = None, flatten: bool = False,
+                   levels_to_drop: list = [], how: str = "outer", tissue_type: str = "both") -> pd.DataFrame:
+        """
+        Joins multiple dataframes into a single dataframe based on the join_dict.
 
-        Returns: pandas.DataFrame
+        Parameters:
+        join_dict (dict): A dictionary with the dataframe and columns to join. Keys are the names of the dataframes and the value is a list of string with the name of the columns corresponding to each dataframe.
+        mutations_filter (list, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority.
+        flatten (bool, optional): If set to True, the multiindexes will be flattened. Defaults to False.
+        levels_to_drop (list, optional): List of level names to drop from the dataframe. If empty it will not drop any. Defaults to an empty list.
+        how (str, optional): Method of join. Can be one of 'outer', 'inner', 'left', 'right'. Defaults to 'outer'.
+        ?tissue_type (str): The type of tissue data to be retrieved. Can be "tumor","normal", or "both".
+        
+        Returns:
+        pandas.DataFrame: The resulting DataFrame after performing all the joins.
         """
-        column_names = []
-        to_join=[]
 
-        # a flag for if mutations data is included, for formatting later
+        column_names = set()
+        to_join = []
         format_mutations = False
 
-        for source_data_key in join_dict.keys():
-            if isinstance(source_data_key, tuple):
-                source, datatype = source_data_key
-            else:
-                # TODO: remind user to input "source datatype" for dictionary keys in error
-                source, datatype = source_data_key.split()
+        for source_data_key, data_key in join_dict.items():
+            # Split key into source and datatype
+            source, datatype = source_data_key if isinstance(source_data_key, tuple) else source_data_key.split()
 
-            # Make sure all requested data exists and is valid
+            # Raise error if datatype is invalid
             if datatype not in self._sources[source].load_functions:
-                raise DataFrameNotIncludedError(f"{source} {datatype} is not a valid dataframe in the {self.get_cancer_type()} dataset.")
+                raise DataFrameNotIncludedError(
+                    f"{source} {datatype} is not a valid dataframe in the {self.get_cancer_type()} dataset.")
 
-            ## If key belongs to omics
-            if datatype in self._valid_omics_dfs:
-                # If key is somatic_mutation_binary it will join all columns that match a gene
-                if datatype == "somatic_mutation_binary":
-                    binary_data = self.get_somatic_mutation_binary(source)
-                    binary_data = "\n".join(list(binary_data.columns))
-                    found_genes = []
-                    if len(join_dict[source_data_key]) != 0:
-                        for gene in join_dict[source_data_key]:
-                            found_genes += (re.findall((gene+".+\n"), binary_data))
-                        found_genes = list(map(lambda x: x.strip("\n"), found_genes))#returns a list of columns that match the given gene
-                        columns = self._get_omics_cols(datatype, source, found_genes, tissue_type= tissue_type)
-                    else:
-                        columns = self._get_omics_cols(datatype, source, None, tissue_type= tissue_type)
-                else:
-                    if len(join_dict[source_data_key]) != 0:# If there are values to join it will get the columns
-                        columns = self._get_omics_cols(datatype, source, join_dict[source_data_key], tissue_type = tissue_type)
-                    else:# Else join all the dataframe
-                        columns = self._get_omics_cols(datatype, source, None, tissue_type = tissue_type)
-            ## If key belongs to metadata 
-            elif datatype in self._valid_metadata_dfs:
-                if len(join_dict[source_data_key]) != 0:# If there are values to join it will get the columns
-                    columns = self._get_metadata_cols(datatype, source, join_dict[source_data_key], tissue_type = tissue_type)
-                else:# Else join all the dataframe
-                    columns = self._get_metadata_cols(datatype, source, None, tissue_type = tissue_type)
-            ## If key is somatic_mutation 
-            elif datatype == "somatic_mutation":
-                columns = self._get_genes_mutations(source, join_dict[source_data_key], mutations_filter = mutations_filter)
-                # Set flag that mutations data in join_dict
+            # Get the relevant columns
+            columns = self._get_columns(datatype, source, data_key, tissue_type, mutations_filter)
+
+            # Set flag that mutations data in join_dict
+            if datatype == "somatic_mutation":
                 format_mutations = True
 
-            ### Checks if there are columns with the same name and adds the name of the
-            for i in columns.columns:
-                if type(i) == tuple:
-                    i = reduce(lambda  x, y: str(x)+str(y), i)#returns a flattened column name
-                if i in column_names:
-                    columns = columns.rename(columns={i: str(i)+'_'+source+'_'+datatype})
-                column_names.append(i)
-            ###
+            # Checks if there are columns with the same name and renames them
+            for column in columns:
+                if column in column_names:
+                    columns = columns.rename(columns={column: str(column) + '_' + source + '_' + datatype})
+                column_names.add(column)
 
             to_join.append(columns)
 
         joined, how = reduce(self._join_dataframe, to_join, how)
 
+        if flatten and isinstance(joined.columns, pd.MultiIndex):
+            joined.columns = joined.columns.droplevel('Database_ID')
+
         # Format any included mutations data
         if format_mutations:
             mutations_were_filtered = mutations_filter is not None
             joined = self._format_mutations_data(joined, mutations_were_filtered, how=how, tissue_type=tissue_type)
 
-        if len(levels_to_drop) != 0:
+        if levels_to_drop:
             joined = ut.reduce_multiindex(joined, levels_to_drop=levels_to_drop)
 
-        if flatten == True:
-            joined = ut.reduce_multiindex(joined, flatten=flatten)
+        # Sort the dataframe for good measure (based off sample status (tumor or normal), then alphabetically)
+        joined = joined.sort_index()
+
+        # Tempted to get rid of this since it seems outdated, but I'll keep it in for now
+        # '.N' for normal, '.C' for cored normals (in HNSCC)
+        normal = joined[joined.index.str.contains(r'\.[NC]$', regex=True, na=False)]
+        # Tumor samples don't have any special endings for now
+        tumor = joined[~joined.index.str.contains(r'\.[NC]$', regex=True, na=False)]
+        joined = pd.concat([tumor, normal])
+
         return joined
 
+
     # Help functions
-    def get_cancer_type(self):
+    def get_cancer_type(self) -> str:
         """Return the cancer type for this dataset, as a string."""
         return self._cancer_type
 
-    def get_data_list(self):
+    def get_data_list(self) -> list:
         """Return a list of all data currently loaded into memory"""
         complete_list = {}
         for source in self._sources.keys():
             data_list = {}
             for name in sorted(self._sources[source]._data.keys(), key=str.lower):
                 df = self._sources[source]._data[name]
                 data_list[name] = {'rows': df.shape[0], 'columns': df.shape[1]}
             complete_list[source] = data_list
         return complete_list
 
-    def how_to_cite(self, cancer_type='', pmid='', unpublished=False):
+    def how_to_cite(self, cancer_type: str='', pmid: str = '', unpublished: bool=False):
         """Print instructions for citing the data."""
 
         # current main message
         main_message = ('Please include the following statement(s) in publications using data '
          'accessed through this module:\n"Data used in this publication were generated '
          'by the Clinical Proteomic Tumor Analysis Consortium (NCI/NIH). '
          'Data were accessed through the Python module cptac, PMID: 33560848."')
@@ -622,200 +652,225 @@
             print(cancer_specific_message)
         elif (cancer_type and unpublished):
             print(f"Data for {cancer_type} has not been published yet.")
         else:
             # no additional message will be printed if we have not passed in parameters
             pass
 
-    def list_data_sources(self):
+    def list_data_sources(self, source_filter: str or list[str]="all"):
         """Print which sources provide each data type.
 
         Parameters:
-        print_list (bool, optional): Whether to print the list. Default is True. Otherwise, it's returned as a string.
+        source_filter (str or list[str], optional): filter which sources are shown in the table, default "all" returns all sources and datatypes.
+            If a source is specified, only datatypes with data from that source will be shown.
         """
 
         # This dict will be keyed by data type, and the values will be each source that provides that data type
         data_sources = {}
+        datatypes_to_keep = []
+
+        # handle sources filter parameter
+        if source_filter == "all":
+            source_filter = self._sources.keys()
+        elif isinstance(source_filter, str): # If it's a single source, make it a list so we can treat everything the same
+            source_filter = [source_filter]
+        for src in source_filter:
+            if src not in self._sources.keys():
+                raise InvalidParameterError(f"{src} is not a valid source for the {self._cancer_type} datatset. Valid sources are: {list(self._sources.keys())}")
 
+
+        # Get each datatype and its sources
         for source in sorted(self._sources.keys()):
             for df_name in sorted(self._sources[source].load_functions.keys()):
-                if df_name in ["cibersort", "xcell"]:
-                    df_name = f"deconvolution_{df_name}" # For clarity
+
+                if source in source_filter:
+                    datatypes_to_keep.append(df_name)
 
                 if df_name in data_sources.keys():
                     data_sources[df_name][0] += f", {source}"
                 else:
                     data_sources[df_name] = [source]
 
+        # Filter based on user parameter
+        kept_data = {k: data_sources[k] for k in datatypes_to_keep}
+        data_sources = kept_data
+
         data_sources = pd.\
         DataFrame(data_sources).\
         transpose().\
         sort_index().\
         reset_index()
 
         data_sources.columns=["Data type", "Available sources"]
 
         return data_sources
+    
 
-    def version(self, source):
-        """Return the dataset version of this instance, as a string."""
-        return self._sources[source]
-
-    def get_dataframe(self, name, source=None, tissue_type="both", imputed=False):
-        """Check that a given dataframe from a given source exists, and return a copy if it does.
-
-        Parameters:
-        name (str): The datatype for which you want the dataframe.
-        source (str): The source of the dataframe.
-        tissue_type (str, optional): Acceptable values in ["tumor","normal","both"]. Specifies the tissue type desired in the dataframe. Defaults to "both".
-        imputed (bool, optional): whether the data is imputed. Defaults to False.
+    def get_dataframe(
+        self,
+        data_type: str,
+        source: str = None,
+        tissue_type: str = "both",
+        imputed: bool = False
+    ) -> pd.DataFrame:
+        """
+        Check if a given dataframe from a specific source exists and return a copy if it does.
+
+        Parameters:
+        data_type (str): The data type of the desired dataframe.
+        source (str, optional): The source of the dataframe. Defaults to None.
+        tissue_type (str, optional): Desired tissue type in the dataframe. Acceptable values are ["tumor", "normal", "both"]. Defaults to "both".
+        imputed (bool, optional): Specifies whether the data is imputed. Defaults to False.
 
-        Returns: pandas.DataFrame
+        Returns:
+        pandas.DataFrame: A dataframe containing the requested data.
         """
 
         if imputed:
-            name = name + "_imputed"
+            data_type += "_imputed"
 
-        # If no source specified, tell user what sources are available for that datatype
         if source is None:
-            sources_for_data = []
-            for src in self._sources.keys():
-                if name in self._sources[src].load_functions.keys():
-                    sources_for_data.append(src)
-            if len(sources_for_data) == 0:
-                # Desired datatype does not exist
-                raise DataFrameNotIncludedError(f"{name} datatype not included in the {self._cancer_type} dataset. Use <cancer object>.list_data_sources() to see which data are available.")
-            elif len(sources_for_data) == 1:
-                # Warn the user that a default value is being used
+            sources_for_data = [src for src in self._sources if data_type in self._sources[src].load_functions]
+
+            if not sources_for_data:
+                raise DataFrameNotIncludedError(
+                    f"{data_type} datatype is not included in the {self._cancer_type} dataset. Use <cancer object>.list_data_sources() to see which data are available.")
+
+            if len(sources_for_data) == 1:
                 source = sources_for_data[0]
-                warnings.warn(f"Using source {source} for {name} data as no other sources provide this data. To remove this warning, pass {source} as the source parameter.", ParameterWarning, stacklevel=3)
+                warnings.warn(
+                    f"Using source {source} for {data_type} data as no other sources provide this data. To remove this warning, pass {source} as the source parameter.",
+                    ParameterWarning, stacklevel=3)
             else:
-                # Raise error and let user know what sources are available
-                raise DataSourceNotFoundError(f"No source selected. Available sources for {self._cancer_type} {name} data are: {sources_for_data}.")
+                raise DataSourceNotFoundError(
+                    f"No source selected. Available sources for {self._cancer_type} {data_type} data are: {sources_for_data}.")
 
-        if source in self._sources.keys():
-            df = self._sources[source].get_df(name)
+        if source not in self._sources:
+            raise DataSourceNotFoundError(f"Data source {source} not found for the {self._cancer_type} dataset.")
 
-            # Handle tissue type and filter df as specified
-            if tissue_type == "normal":
-                df = self._normal_only(df)
-            elif tissue_type == "tumor":
-                df = self._tumor_only(df)
+        df = self._sources[source].get_df(data_type)
 
-            return df
-        else:
-            raise DataSourceNotFoundError(f"Data source {source} not found for the {self._cancer_type} dataset.")
+        if tissue_type == "normal":
+            df = self._normal_only(df)
+        elif tissue_type == "tumor":
+            df = self._tumor_only(df)
+
+        if data_type == 'clinical':
+            df.columns = df.columns.str.split('/').str[-1]  # Keep only the part after the slash
+
+        return df
+
+    
 
     # "Private" methods
-    def _check_df_valid(self, df_name, source, df_type):
-        """Checks whether a dataframe with this name is valid for use as an omics or metadata dataframe in one of the utilties functions. Throws an InvalidParameterError if it isn't.
+    def _check_df_valid(self, df_name: str, source: str, df_type: str):
+        """
+        Checks whether a dataframe with this name is valid for use as an omics or metadata dataframe in one of the utilties functions.
+        Throws an InvalidParameterError if it isn't.
 
         Parameters:
         df_name (str): The dataframe name to check.
         source (str): The source of the dataframe.
         df_type (str): Which type of dataframe we're validating--either "omics" or "metadata"
 
         Returns: None
         """
         if not isinstance(df_name, str): # Check that they passed a str, since utilities functions used to directly accept dataframes
             raise InvalidParameterError(f"Please pass a str for dataframe name parameter. You passed {df_name}, which is a {type(df_name)}")
 
-        if df_type == "omics":
-            valid_dfs = self._valid_omics_dfs
-        elif df_type == "metadata":
-            valid_dfs = self._valid_metadata_dfs
-        else:
+        valid_df_types = {"omics": self._valid_omics_dfs, "metadata": self._valid_metadata_dfs}
+
+        try:
+            valid_dfs = valid_df_types[df_type]
+        except KeyError:
             raise CptacDevError(f"Invalid df_type of {df_type} passed to cptac.Dataset._check_df_valid.")
 
         if df_name not in self._sources[source].load_functions:
             raise DataFrameNotIncludedError(f"{source} {df_name} dataframe not included in the {self.get_cancer_type()} dataset.")
-        elif df_name not in valid_dfs:
-            error_msg = f"{df_name} is not a valid {df_type} dataframe for this function in this dataset. Valid options:"
-            for valid_name in valid_dfs:
-                if valid_name in self._sources[source].load_functions: # Only print it if it's included in this dataset
-                    error_msg = error_msg + '\n\t' + valid_name
+
+        if df_name not in valid_dfs:
+            valid_options = '\n\t'.join([valid_name for valid_name in valid_dfs if valid_name in self._sources[source].load_functions])
+            error_msg = f"{df_name} is not a valid {df_type} dataframe for this function in the dataset. Valid options: \n\t{valid_options}"
             raise InvalidParameterError(error_msg)
 
-    def _tumor_only(self, df):
+    def _tumor_only(self, df: pd.DataFrame):
         """For a given dataframe, keep only the tumor samples."""
-        normal_endings = ('.N', '.C') # HNSCC data has cored normal samples marked .C
-        tumor_df = df[~df.index.str.endswith(normal_endings)]
+        tumor_df = df[~df.index.str.endswith(self.NORMAL_ENDINGS)]
         return tumor_df
 
-    def _normal_only(self, df):
+    def _normal_only(self, df: pd.DataFrame):
         """For a given dataframe, keep only the normal samples."""
-        normal_endings = ('.N', '.C') # HNSCC data has cored normal samples marked .C
-        normal_df = df[df.index.str.endswith(normal_endings)]
+        normal_df = df[df.index.str.endswith(self.NORMAL_ENDINGS)]
         return normal_df
 
     def _get_omics_cols(self, omics_df_name, source, genes, tissue_type="both"):
-        """Based on a single gene, or a list or array-like of genes, select multiple columns from an omics dataframe, and return the selected columns as one dataframe.
+        """
+        Based on a single gene, or a list or array-like of genes, select multiple columns from an omics dataframe, and return the selected columns as one dataframe.
 
         Parameters:
         omics_df_name (str): Name of omics dataframe to select column(s) from.
         source (str): Source for data to select column(s) from.
-        genes (str, or list or array-like of str): Gene(s) to use to select columns from omics_df. str if one gene, list or array-like if multiple. Passing None will select the entire omics dataframe.
+        genes (str or list or array-like of str): Gene(s) to use to select columns from omics_df. str if one gene, list or array-like if multiple. Passing None will select the entire omics dataframe.
         tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the tissue type desired in the dataframe. Defaults to "both".
 
         Returns:
         pandas.DataFrame: The selected columns from the dataframe.
         """
+
         # Check that they passed a valid omics df
         self._check_df_valid(omics_df_name, source, "omics")
 
         # Get our omics df, using get_dataframe to catch invalid requests
         omics_df = self.get_dataframe(omics_df_name, source, tissue_type).copy()
 
         # Process genes parameter
-        if isinstance(genes, str): # If it's a single gene, make it a list so we can treat everything the same
+        if isinstance(genes, str): 
             genes = [genes]
-        elif isinstance(genes, (list, pd.Series, pd.Index)): # If it's already a list or array-like, we're all good
+        elif isinstance(genes, (list, pd.Series, pd.Index)): 
             pass
-        elif genes is None: # If it's the default of None, rename columns and return the entire dataframe
-            # Add the gene name to end beginning of each column header, to preserve info when we join dataframes.
+        elif genes is None: 
             if isinstance(omics_df.columns, pd.MultiIndex):
                 omics_df.columns = omics_df.columns.set_levels(omics_df.columns.levels[0] + '_' + source + '_' + omics_df_name, level=0)
             else:
                 omics_df = omics_df.add_suffix('_' + source + '_' + omics_df_name)
             return omics_df
-        else: # If it's none of those, they done messed up. Tell 'em.
+        else: 
             raise InvalidParameterError("Genes parameter \n{}\nis of invalid type {}. Valid types: str, list or array-like of str, or NoneType.".format(genes, type(genes)))
 
         genes = pd.Index(genes, name="Name")
 
         if isinstance(omics_df.columns, pd.MultiIndex):
-            contained = genes.intersection(omics_df.columns.get_level_values("Name")).drop_duplicates() # Get the genes that actually exist in the dataframe's columns
+            contained = genes.intersection(omics_df.columns.get_level_values("Name")).drop_duplicates() 
             mi_contained = omics_df.columns[omics_df.columns.get_level_values("Name").isin(genes)]
 
-            not_contained = genes.difference(contained).drop_duplicates() # So we can warn the user later
+            not_contained = genes.difference(contained).drop_duplicates() 
             arrays = [not_contained] + [[np.nan] for i in range(omics_df.columns.nlevels - 1)]
             mi_not_contained = pd.MultiIndex.from_product(arrays, names=omics_df.columns.names)
 
-            genes = mi_contained.union(mi_not_contained) # To use for reindexing the dataframe
+            genes = mi_contained.union(mi_not_contained)
         else:
-            contained = genes.intersection(omics_df.columns).drop_duplicates() # Get the genes that actually exist in the dataframe's columns
-            not_contained = genes.difference(contained).drop_duplicates() # So we can warn the user later
+            contained = genes.intersection(omics_df.columns).drop_duplicates() 
+            not_contained = genes.difference(contained).drop_duplicates()
 
         selected = omics_df[contained]
-        selected = selected.reindex(columns=genes) # This will add the columns not included in the dataframe, and fill them with NaN.
+        selected = selected.reindex(columns=genes) 
 
-        # Warn the user about columns filled with NaN
         if len(not_contained) > 0:
             warnings.warn(f"The following columns were not found in the {source} {omics_df_name} dataframe, so they were inserted into joined table, but filled with NaN: {', '.join(not_contained)}", ParameterWarning, stacklevel=3)
 
-        # Append dataframe name to end of each column header, to preserve info when we merge dataframes
         if isinstance(omics_df.columns, pd.MultiIndex):
             selected.columns = selected.columns.set_levels(selected.columns.levels[0] + '_' + source + '_' + omics_df_name, level=0)
         else:
             selected = selected.add_suffix('_' + source + '_' + omics_df_name)
 
         selected.columns.name = "Name"
         return selected
 
-    def _get_metadata_cols(self, df_name, source, cols, tissue_type="both"):
+
+    def _get_metadata_cols(self, df_name: str, source: str, cols: str or list[str], tissue_type: str="both") -> pd.DataFrame:
         """Select a single column or several columns from a metadata dataframe.
 
         Parameters:
         df_name (str): The name of the metadata dataframe to select the column(s) from.
         source (str): The source for the metadata.
         cols (str, or list or array-like of str): The column(s) to select from the dataframe. str if single, list or array-like of str if multiple. Passing None will select the entire dataframe.
         tissue_type (str): Acceptable values in ["tumor","normal","both"]. Specifies the tissue type desired in the dataframe. Defaults to "both".
@@ -845,149 +900,156 @@
         not_contained = cols.difference(df.columns)
         if len(not_contained) > 0:
             raise InvalidParameterError(f'The following columns were not found in the {source} {df_name} dataframe: {", ".join(not_contained)}')
 
         selected = df[cols]
         return selected
 
-    def _get_genes_mutations(self, source, genes, mutations_filter, mutation_cols = ["Mutation","Location"]):
-            """Gets all the mutations for one or multiple genes, for all patients.
+    def _get_genes_mutations(self, source: str, genes: str or list[str], mutations_filter: str or list[str], mutation_cols: list or str = ["Mutation","Location"]) -> pd.DataFrame:
+        """Gets all the mutations for one or multiple genes, for all patients.
+
+        Parameters:
+        genes (str, or list or array-like of str): The gene(s) to grab mutations for. str if one, list or array-like of str if multiple.
+        mutations_filter (list[str] or str, optional):
+            List of mutations to prioritize when filtering out multiple mutations, in order of priority.
+            If none of the multiple mutations in a sample are included in mutations_filter, the function
+            will automatically prioritize truncation over missense mutations, and then mutations earlier
+            in the sequence over later mutations.
+            Passing an empty list will cause this default hierarchy to be applied to all samples.
+            Passing None will cause no filtering to be done, and all mutation data will be included, in a list.
+        mutation_cols (list or str): List of columns to include in joined df.
+            Default is the Mutation and Location column. The str "all" returns all mutation columns.
+
+        Returns:
+        pandas.DataFrame: The mutations in each patient for the specified gene(s).
+        """
+
+        somatic_mutation = self.get_somatic_mutation(source)
+
+        # Process genes parameter
+        if isinstance(genes, str): # If it's a single gene, make it a list so we can treat everything the same
+            genes = [genes]
+        elif isinstance(genes, (list, pd.Series, pd.Index)): # If it's already a list or array-like, we're all good
+            pass
+        else: # If it's neither of those, they done messed up. Tell 'em.
+            raise InvalidParameterError("Genes parameter {} is of invalid type {}. Valid types: str, or list or array-like of str.".format(genes, type(genes)))
 
-            Parameters:
-            genes (str, or list or array-like of str): The gene(s) to grab mutations for. str if one, list or array-like of str if multiple.
-            mutations_filter (list[str] or str, optional): List of mutations to prioritize when filtering out multiple mutations, in order of priority. If none of the multiple mutations in a sample are included in mutations_filter, the function will automatically prioritize truncation over missense mutations, and then mutations earlier in the sequence over later mutations. Passing an empty list will cause this default hierarchy to be applied to all samples. Passing None will cause no filtering to be done, and all mutation data will be included, in a list.
-            mutation_cols (list or str): List of columns to include in joined df. Default is the Mutation and Location column. The str "All" returns all mutation columns. 
-
-            Returns:
-            pandas.DataFrame: The mutations in each patient for the specified gene(s).
-            """
-
-            somatic_mutation = self.get_somatic_mutation(source)
-
-            # Process genes parameter
-            if isinstance(genes, str): # If it's a single gene, make it a list so we can treat everything the same
-                genes = [genes]
-            elif isinstance(genes, (list, pd.Series, pd.Index)): # If it's already a list or array-like, we're all good
+        # Process mutations_filter parameter
+        if mutations_filter is not None:
+            if isinstance(mutations_filter, str): # If it's a single gene, make it a list so we can treat everything the same
+                mutations_filter = [mutations_filter]
+            elif isinstance(mutations_filter, (list, pd.Series, pd.Index)): # If it's already a list or array-like, we're all good
                 pass
-            else: # If it's neither of those, they done messed up. Tell 'em.
-                raise InvalidParameterError("Genes parameter {} is of invalid type {}. Valid types: str, or list or array-like of str.".format(genes, type(genes)))
+            else: # Again, let them know if their parameter is not going to cut it
+                raise InvalidParameterError("mutations_filter parameter {} is of invalid type {}. Valid types: str, or list or array-like of str.".format(mutations_filter, type(mutations_filter)))
 
-            # Process mutations_filter parameter
-            if mutations_filter is not None:
-                if isinstance(mutations_filter, str): # If it's a single gene, make it a list so we can treat everything the same
-                    mutations_filter = [mutations_filter]
-                elif isinstance(mutations_filter, (list, pd.Series, pd.Index)): # If it's already a list or array-like, we're all good
-                    pass
-                else: # Again, let them know if their parameter is not going to cut it
-                    raise InvalidParameterError("mutations_filter parameter {} is of invalid type {}. Valid types: str, or list or array-like of str.".format(mutations_filter, type(mutations_filter)))
-
-            # Set some column names for use later
-            gene_col = "Gene"
-            mutation_col = "Mutation"
-            location_col = "Location"
-            mutation_status_col = "Mutation_Status"
+        # Set some column names for use later
+        gene_col = "Gene"
+        mutation_col = "Mutation"
+        location_col = "Location"
+        mutation_status_col = "Mutation_Status"
+
+        # Check that they didn't make any typos in specifying filter values
+        invalid_filter = False
+        if mutations_filter is not None:
+            for filter_val in mutations_filter:
+                if (filter_val not in somatic_mutation[mutation_col].values) and (filter_val not in somatic_mutation[location_col].values):
+                    raise InvalidParameterError(f"Filter value {filter_val} does not exist in the mutations dataframe for this dataset. Check for typos and existence. Merge aborted.")
+
+        # Create an empty dataframe, which we'll fill with the columns we select using our genes, and then return.
+        df = pd.DataFrame(index=somatic_mutation.index.copy().drop_duplicates())
+        genes = pd.Series(genes).drop_duplicates()
+        for gene in genes:
+            gene_mutations = somatic_mutation[somatic_mutation[gene_col] == gene] # Get all the mutations for that gene
+            if len(gene_mutations) == 0: # If the gene doesn't match any genes in the dataframe, tell them
+                raise InvalidParameterError("{} gene not found in somatic_mutation data.".format(gene))
+            gene_mutations = gene_mutations.drop(columns=[gene_col]) # Gene column is same for every sample, so we don't need it anymore.
 
-            # Check that they didn't make any typos in specifying filter values
-            invalid_filter = False
+            # Check whether all filter values exist for this particular gene. If not, that's fine, we just want to warn the user.
             if mutations_filter is not None:
                 for filter_val in mutations_filter:
-                    if (filter_val not in somatic_mutation[mutation_col].values) and (filter_val not in somatic_mutation[location_col].values):
-                        raise InvalidParameterError(f"Filter value {filter_val} does not exist in the mutations dataframe for this dataset. Check for typos and existence. Merge aborted.")
+                    if (filter_val not in gene_mutations[mutation_col].values) and (filter_val not in gene_mutations[location_col].values):
+                        warnings.warn(f"Filter value {filter_val} does not exist in the mutations data for the {gene} gene, though it exists for other genes.", ParameterWarning, stacklevel=3)
 
-            # Create an empty dataframe, which we'll fill with the columns we select using our genes, and then return.
-            df = pd.DataFrame(index=somatic_mutation.index.copy().drop_duplicates())
-            genes = pd.Series(genes).drop_duplicates()
-            for gene in genes:
-                gene_mutations = somatic_mutation[somatic_mutation[gene_col] == gene] # Get all the mutations for that gene
-                if len(gene_mutations) == 0: # If the gene doesn't match any genes in the dataframe, tell them
-                    raise InvalidParameterError("{} gene not found in somatic_mutation data.".format(gene))
-                gene_mutations = gene_mutations.drop(columns=[gene_col]) # Gene column is same for every sample, so we don't need it anymore.
-
-                # Check whether all filter values exist for this particular gene. If not, that's fine, we just want to warn the user.
-                if mutations_filter is not None:
-                    for filter_val in mutations_filter:
-                        if (filter_val not in gene_mutations[mutation_col].values) and (filter_val not in gene_mutations[location_col].values):
-                            warnings.warn(f"Filter value {filter_val} does not exist in the mutations data for the {gene} gene, though it exists for other genes.", ParameterWarning, stacklevel=3)
-
-                # Create another empty dataframe, which we'll fill with the mutation and location data for this gene, as lists
-                prep_index = gene_mutations.index.copy().drop_duplicates()
-                prep_columns = gene_mutations.columns.copy()
-                mutation_status_idx = pd.Index([mutation_status_col]) # Prep mutation_status_col to be joined
-                prep_cols_with_mut_status = prep_columns.append(mutation_status_idx) # Add a mutation_status column, which will indicate if there are 1 or multiple mutations
-                mutation_lists = pd.DataFrame(index=prep_index, columns=prep_cols_with_mut_status)
-
-                if mutation_cols == "All":
-                    mutation_cols = somatic_mutation.columns.to_list()
-                    mutation_cols = mutation_cols[1:] #drop column name "Gene"  
-
-                # Get the mutation(s), mutation status, and location information for this gene and sample
-                # Yes, I know I'm doing that horrible thing, using nested for loops to work with dataframes. However, I tried refactoring it to use DataFrame.groupby and DataFrame.apply, and both actually made it slower. Go figure.
-                for sample in mutation_lists.index: # samples ids with mutation
-
-                    sample_data = gene_mutations.loc[sample] # Get slice of dataframe for the sample
-
-                    for col in mutation_cols:
-
-                        sliced_col = sample_data[col] # Get single col 
-
-                        #Make Mutations List 
-                        if col == mutation_col:
-                            if isinstance(sliced_col, pd.Series):
-                                sample_mutations_list = sliced_col.tolist()
-                            else:
-                                sample_mutations_list = [sliced_col] 
-
-                            # Figure out what our mutation status is (either single_mutation or multiple_mutation)
-                            if len(sample_mutations_list) > 1:
-                                sample_mutation_status = "Multiple_mutation"
-                            else:
-                                sample_mutation_status = "Single_mutation"
-                        #Make Location List        
-                        if col == location_col:
-                            if isinstance(sliced_col, pd.Series):
-                                sample_locations_list = sliced_col.tolist()
-                            else:
-                                sample_locations_list = [sliced_col]
+            # Create another empty dataframe, which we'll fill with the mutation and location data for this gene, as lists
+            prep_index = gene_mutations.index.copy().drop_duplicates()
+            prep_columns = gene_mutations.columns.copy()
+            mutation_status_idx = pd.Index([mutation_status_col]) # Prep mutation_status_col to be joined
+            prep_cols_with_mut_status = prep_columns.append(mutation_status_idx) # Add a mutation_status column, which will indicate if there are 1 or multiple mutations
+            mutation_lists = pd.DataFrame(index=prep_index, columns=prep_cols_with_mut_status)
+
+            if mutation_cols == "all":
+                mutation_cols = somatic_mutation.columns.to_list()
+                mutation_cols = mutation_cols[1:] #drop column name "Gene"
+
+            # Get the mutation(s), mutation status, and location information for this gene and sample
+            # Yes, I know I'm doing that horrible thing, using nested for loops to work with dataframes. However, I tried refactoring it to use DataFrame.groupby and DataFrame.apply, and both actually made it slower. Go figure.
+            for sample in mutation_lists.index: # samples ids with mutation
+
+                sample_data = gene_mutations.loc[sample] # Get slice of dataframe for the sample
+
+                for col in mutation_cols:
+
+                    sliced_col = sample_data[col] # Get single col
+
+                    #Make Mutations List
+                    if col == mutation_col:
+                        if isinstance(sliced_col, pd.Series):
+                            sample_mutations_list = sliced_col.tolist()
                         else:
-                            if isinstance(sliced_col, pd.Series):
-                                sample_mut_col_list = sliced_col.tolist()
-                            else:
-                                sample_mut_col_list = [sliced_col]
-
-                            mutation_lists.at[sample, col] = sample_mut_col_list  
-
-                    necessary_cols = ["Mutation","Location"] #must be included in order to filter mutations                   
-                    if mutations_filter is not None: # Filter multiple mutations down to just one
-                        #Check that Mutation and Location is mutation_cols so mutations_filter can work 
-                        if (all(x in mutation_cols for x in necessary_cols)):
-                            chosen_mutation, chosen_location = self._filter_multiple_mutations(mutations_filter, sample_mutations_list, sample_locations_list)
-                            mutation_lists.at[sample, mutation_col] = chosen_mutation
-                            mutation_lists.at[sample, location_col] = chosen_location
-
-                    else: # Include all the mutations!
-                        if (all(x in mutation_cols for x in necessary_cols)):
-                            mutation_lists.at[sample, mutation_col] = sample_mutations_list
-                            mutation_lists.at[sample, location_col] = sample_locations_list 
-
-
-                    # Also add the mutations status column
-                    mutation_lists.at[sample, mutation_status_col] = sample_mutation_status
-
-                # Print warning if either Location and Mutation not provided and mutation_filter provided                       
-                if (mutations_filter is not None) & ((all(x in mutation_cols for x in necessary_cols)) == False):
-                    warnings.warn(f"mutations_filter was not applied because columns 'Location' and 'Mutation' were not included in mutation_cols.", ParameterWarning, stacklevel=3)                        
-
-                mutation_lists = mutation_lists[mutation_cols + [mutation_status_col]] #only include user specified columns and Mutation_Status 
-                mutation_lists = mutation_lists.add_prefix(gene + '_') # Add the gene name to end beginning of each column header, to preserve info when we join dataframes.
-                df = df.join(mutation_lists, how='outer') # Append the columns to our dataframe we'll return.
-                df.columns.name = "Name"
+                            sample_mutations_list = [sliced_col]
 
-            return df
+                        # Figure out what our mutation status is (either single_mutation or multiple_mutation)
+                        if len(sample_mutations_list) > 1:
+                            sample_mutation_status = "Multiple_mutation"
+                        else:
+                            sample_mutation_status = "Single_mutation"
+                    #Make Location List
+                    if col == location_col:
+                        if isinstance(sliced_col, pd.Series):
+                            sample_locations_list = sliced_col.tolist()
+                        else:
+                            sample_locations_list = [sliced_col]
+                    else:
+                        if isinstance(sliced_col, pd.Series):
+                            sample_mut_col_list = sliced_col.tolist()
+                        else:
+                            sample_mut_col_list = [sliced_col]
+
+                        mutation_lists.at[sample, col] = sample_mut_col_list
+
+                necessary_cols = ["Mutation","Location"] #must be included in order to filter mutations
+                if mutations_filter is not None: # Filter multiple mutations down to just one
+                    #Check that Mutation and Location is mutation_cols so mutations_filter can work
+                    if all(x in mutation_cols for x in necessary_cols):
+                        chosen_mutation, chosen_location = self._filter_multiple_mutations(mutations_filter, sample_mutations_list, sample_locations_list)
+                        mutation_lists.at[sample, mutation_col] = chosen_mutation
+                        mutation_lists.at[sample, location_col] = chosen_location
+
+                else: # Include all the mutations!
+                    if all(x in mutation_cols for x in necessary_cols):
+                        mutation_lists.at[sample, mutation_col] = sample_mutations_list
+                        mutation_lists.at[sample, location_col] = sample_locations_list
+
+                # Also add the mutations status column
+                mutation_lists.at[sample, mutation_status_col] = sample_mutation_status
+
+            # Print warning if either Location and Mutation not provided and mutation_filter provided
+            if (mutations_filter is not None) & ((all(x in mutation_cols for x in necessary_cols)) == False):
+                warnings.warn("mutations_filter was not applied because columns 'Location' and 'Mutation' were not included in mutation_cols.", ParameterWarning, stacklevel=3)
+
+            mutation_lists = mutation_lists[mutation_cols + [mutation_status_col]] #only include user specified columns and Mutation_Status
+            mutation_lists = mutation_lists.add_prefix(gene + '_') # Add the gene name to end beginning of each column header, to preserve info when we join dataframes.
+            df = df.join(mutation_lists, how='outer') # Append the columns to our dataframe we'll return.
+            df.columns.name = "Name"
 
-    def _format_mutations_data(self, mutations, mutations_were_filtered, show_location=True, how="outer", quiet=False, tissue_type="both", mutation_cols=["Mutation","Location"]):
+        return df
+
+    def _format_mutations_data(self, mutations: pd.DataFrame, mutations_were_filtered: bool, show_location: bool=True, how: str="outer", quiet: bool=False, tissue_type: str="both", mutation_cols: list[str] or str=["Mutation","Location"]
+                               ) -> pd.DataFrame:
         """Format mutations data. Add a Sample_Status column, fill in NaNs with Wildtype_Normal or Wildtype_Tumor.
         Note: This is mostly so that the multi_join function can behave the same way as the old join functions.
         join_other_to_mutations does this same formatting, and should probably be refactored to use this.
         Or, since none of those old functions work currently anyway, they could be removed. Or become helper functions that call multi_join
 
         Parameters:
         mutations (pandas.DataFrame): The selected mutations data to format.
@@ -1047,15 +1109,15 @@
         location_regex = r'^.*_Location$' # Construct regex to find all location columns
         location_cols = mutations.columns[mutations.columns.get_level_values("Name").str.match(location_regex)] # Get a list of all location columns
         for location_col in location_cols:
             if show_location: # If we're including the location column, fill NaN with "No_mutation", since that's what it means, so things are clearer to the user.
 
                 # Make sure Sample Status is not NaN, though--if it is, we have no mutation data at all for that sample, so we can't say "No_mutation".
                 # It must have been a sample that was in the other dataframe, but not the mutations.
-                mutations.loc[(pd.isnull(mutations[location_col])) & (pd.notnull(sample_status_map)), location_col] = no_mutation_fill 
+                mutations.loc[(pd.isnull(mutations[location_col])) & (pd.notnull(sample_status_map)), location_col] = no_mutation_fill
 
                 # If we didn't filter mutations, encapsulate the fill values in lists, to match the other values in the column
                 if not mutations_were_filtered:
                     mutations[location_col] = mutations[location_col].apply(lambda x: x if isinstance(x, list) else [x])
             else:
                 mutations = mutations.drop(columns=[location_col]) # Drop the location column, if the caller wanted us to.
 
@@ -1067,15 +1129,15 @@
             mutations.loc[(sample_status_map == "Normal") & (pd.isnull(mutations[mutation_status_col])), mutation_status_col] = wildtype_normal_fill
             # Change all NaN mutation status values for Tumor samples to Wildtype_Tumor
             mutations.loc[(sample_status_map == "Tumor") & (pd.isnull(mutations[mutation_status_col])), mutation_status_col] = wildtype_tumor_fill
 
         return mutations
 
 
-    def _join_other_to_mutations(self, other, mutations, mutations_were_filtered, show_location, how, quiet):
+    def _join_other_to_mutations(self, other: pd.DataFrame, mutations: pd.DataFrame, mutations_were_filtered: bool, show_location: bool, how: str, quiet: bool) -> pd.DataFrame:
         """Join selected mutations data to selected other omics or metadata, add a Sample_Status column, fill in NaNs with Wildtype_Normal or Wildtype_Tumor, and name the dataframe.
 
         Parameters:
         other (pandas.DataFrame): The selected data from the other type of dataframe (omics or metadata) to join with the selected mutations.
         mutations (pandas.DataFrame): The selected mutations data to join with.
         mutations_were_filtered (bool): Whether multiple mutations in the mutations data were filtered down to just one, or not. Determines whether fill values are in lists or not.
         show_location (bool): Whether to include the Location column from the mutation dataframe.
@@ -1129,15 +1191,15 @@
         # Depending on show_location, either fill NaN values in the joined dataframe location columns with "No_mutation", or just drop the location columns altogether
         location_regex = r'^.*_Location$' # Construct regex to find all location columns
         location_cols = joined.columns[joined.columns.get_level_values("Name").str.match(location_regex)] # Get a list of all location columns
         for location_col in location_cols:
             if show_location: # If we're including the location column, fill NaN with "No_mutation", since that's what it means, so things are clearer to the user.
 
                 # Make sure Sample Status is not NaN, though--if it is, we have no mutation data at all for that sample, so we can't say "No_mutation". It must have been a sample that was in the other dataframe, but not the mutations.
-                joined.loc[(pd.isnull(joined[location_col])) & (pd.notnull(sample_status_map)), location_col] = no_mutation_fill 
+                joined.loc[(pd.isnull(joined[location_col])) & (pd.notnull(sample_status_map)), location_col] = no_mutation_fill
 
                 # If we didn't filter mutations, encapsulate the fill values in lists, to match the other values in the column
                 if not mutations_were_filtered:
                     joined[location_col] = joined[location_col].apply(lambda x: x if isinstance(x, list) else [x])
             else:
                 joined = joined.drop(columns=[location_col]) # Drop the location column, if the caller wanted us to.
 
@@ -1146,15 +1208,15 @@
         mutation_status_cols = joined.columns[joined.columns.get_level_values("Name").str.match(mutation_status_regex)] # Get a list of all Mutation_Status columns
         for mutation_status_col in mutation_status_cols:
             joined.loc[(sample_status_map == "Normal") & (pd.isnull(joined[mutation_status_col])), mutation_status_col] = "Wildtype_Normal" # Change all NaN mutation status values for Normal samples to Wildtype_Normal
             joined.loc[(sample_status_map == "Tumor") & (pd.isnull(joined[mutation_status_col])), mutation_status_col] = "Wildtype_Tumor" # Change all NaN mutation status values for Tumor samples to Wildtype_Tumor
 
         return joined
 
-    def _filter_multiple_mutations(self, mutations_filter, sample_mutations_list, sample_locations_list):
+    def _filter_multiple_mutations(self, mutations_filter: list[str], sample_mutations_list: list[str], sample_locations_list: list[str]) -> str and str:
         """Based on a mutations filter, choose one mutation and its location from two lists of mutations and locations.
 
         Parameters:
         mutations_filter (list of str): A list of mutations to prioritize, in order of priority. Passing an empty list will cause truncations to be chosen over missense, and mutations earlier in the sequence over later ones.
         sample_mutations_list (list of str): The mutations to filter.
         sample_locations_list (list of str): The locations to filter, in the same order as the mutations.
 
@@ -1162,17 +1224,17 @@
         str: The chosen mutation
         str: The chosen location
         """
         # Based on the cancer type, define which mutation types are truncations, for sorting later
         if self._cancer_type == 'colon':
             truncations = ['frameshift deletion', 'frameshift insertion', 'frameshift substitution', 'stopgain', 'stoploss']
             missenses = ['nonframeshift deletion', 'nonframeshift insertion', 'nonframeshift substitution', 'nonsynonymous SNV']
-        elif self._cancer_type == 'hnscc' and self.version() == "0.1":
-            truncations =["stopgain", "stoploss"]
-            missenses = ["nonframeshift insertion", "nonframeshift deletion"]
+        # elif self._cancer_type == 'hnscc' and self.version() == "0.1":
+        #     truncations =["stopgain", "stoploss"]
+        #     missenses = ["nonframeshift insertion", "nonframeshift deletion"]
         else:
             truncations = ['Frame_Shift_Del', 'Frame_Shift_Ins', 'Nonsense_Mutation', 'Nonstop_Mutation', 'Splice_Site']
             missenses = ['In_Frame_Del', 'In_Frame_Ins', 'Missense_Mutation']
 
         if self._cancer_type == "gbm":
             noncodings = ["Intron", "RNA", "3'Flank", "Splice_Region", "5'UTR", "5'Flank", "3'UTR"]
 
@@ -1224,15 +1286,15 @@
             num_location = self._parse_mutation_location(location) # Here, we're parsing the numerical position out of the location strings, for comparisons
             num_soonest_location = self._parse_mutation_location(soonest_location)
             if num_location < num_soonest_location:
                 soonest_location = location
                 soonest_mutation = mutation
         return soonest_mutation, soonest_location
 
-    def _parse_mutation_location(self, location):
+    def _parse_mutation_location(self, location: str) -> int:
         """Parse the number out of the location for a mutation.
 
         Parameters:
         location (str): The location to parse.
 
         Returns:
         int: The numerical part of the location.
@@ -1246,247 +1308,181 @@
                 num = num + char
                 found_digits = True
             else:
                 if found_digits: # We only want the first block of numbers
                     return int(num)
         return int(num) # We get here if the location ended with a digit
 
-    def _check_how_parameter(self, given_how):
+    def _check_how_parameter(self, given_how: str):
         possible_values = ['outer', 'inner', 'left', 'right']
         if given_how not in possible_values:
             raise InvalidParameterError("'{}' is not a valid value for 'how'. Possible values are 'outer', 'inner', 'left', 'right'.".format(given_how))
 
-    def _join_dataframe(self, df1, df2):
+    def _join_dataframe(self, df1: pd.DataFrame, df2: pd.DataFrame) -> pd.DataFrame:
         """Joins a dataframe to another dataframe.
 
         Returns: pandas.DataFrame
         """
         if type(df1) == str:
             return [df2, df1]
         elif type(df1) == list:
             how = df1[1]
             if df1[0].columns.names != df2.columns.names:
-                    df1[0].columns = add_index_levels(to=df1[0].columns, source=df2.columns)
-                    df2.columns = add_index_levels(to=df2.columns, source=df1[0].columns)
+                df1[0].columns = add_index_levels(to=df1[0].columns, source=df2.columns)
+                df2.columns = add_index_levels(to=df2.columns, source=df1[0].columns)
 
             joined = df1[0].join(df2, how= how)
         return [joined,how]
 
-    def _pancan_unionize_indices(self):
-        '''Gets a master index of all IDs, adds IDs to clinical (clinical will have all IDs in other data), 
-        adds Sample_Tumor_Normal column, and sorts clinical rows'''
-        master_index = pd.Index([])
-
-        for name, ds in self._datasets.items():
-            ds_index = unionize_indices(ds._data) # unionize_indices takes 
-
-            master_index = master_index.\
-            union(ds_index).\
-            drop_duplicates()
-
-        # For some cases, there needs to be a multiindex with patient and aliquot IDs. In this case, we drop
-        # tuples so they are not included in the master index
-        master_index = [x for x in master_index if not isinstance(x, tuple)] # drop tuples from index (Patient_ID, Aliquot)
-
-        new_clinical = self._datasets["mssm"]._data["clinical"] # Get the clinical dataframe
-        new_clinical = new_clinical.reindex(master_index) # Take the big, comprehensive index generated by unionize_indices and use it to reindex the clinical dataframe. This will insert empty rows for any samples in the master index that weren't in the clinical dataframe before.
-        sample_status_col = generate_sample_status_col(new_clinical, normal_test=lambda sample: sample[-2:] == '.N') # Parse the patient IDs and based on that generate a column that says which rows are tumor or normal. Note that if the normal IDs are marked by some format other than a ".N" at the end, you'll need to edit the "normal_test" parameter. But otherwise you're fine.
-        new_clinical.insert(0, "Sample_Tumor_Normal", sample_status_col) # Add this new column into the clinical dataframe
-        self._datasets["mssm"]._data['clinical'] = new_clinical # Save the edited clinical dataframe
-
-        #TODO don't forget this sorting in whatever save_df does. We won't be unionizing indices at all though.
-        #This will no longer work since we deprecated the sort_all_rows_pancan function
-        #self._datasets["mssm"]._data = sort_all_rows_pancan(self._datasets["mssm"]._data) # sort clinical after adding master
-
     def _get_sample_status_map(self):
         """Get a pandas Series from the clinical dataframe, with sample ids as the index, and each sample's status (tumor or normal) as the values."""
         clinical = self.get_clinical()
         status_map = clinical["Sample_Tumor_Normal"]
         status_map.name = "Sample_Status"
         return status_map
 
-    def get_genotype_all_vars(self, mutations_genes, omics_source, mutations_filter=None, show_location=True, mutation_hotspot=None):
-        """Return a dataframe that has the mutation type and wheather or not it is a multiple mutation
+    def get_genotype_all_vars(self, mutations_gene: str or list[str], omics_source: str, mutations_source: str, mutations_filter: list=None, show_location: bool=True, mutation_hotspot: str=None
+                              ) -> pd.DataFrame:
+        """Return a dataframe that has the mutation type and whether or not it is a multiple mutation
         Parameters:
         mutation_genes (str, or list or array-like of str): The gene(s) to get mutation data for.
         mutations_filter (list, optional):  List of mutations to prioritize when filtering out multiple mutations, in order of priority.
         omics_source(str): Source of omics data ex "bcm", "washu", "broad", "umich"
+        mutations_source(str): Source of mutations data ex "bcm", "washu", "broad", "umich"
         show_location (bool, optional): Whether to include the Location column from the mutation dataframe. Defaults to True.
-        mutation_hotspot (optional): a list of hotspots
+        mutation_hotspot (optional): a list of hotspot locations
+        
+        Returns:
+        A dataframe specifying the primary mutation type (as specified by mutations_filter), its location (optional), and whether there is one or multiple mutations
         """
 
-        #If they don't give us a filter, this is the default.
-
-        mutations_filter = ["Deletion",
-                                    'Frame_Shift_Del', 'Frame_Shift_Ins', 'Nonsense_Mutation', 'Nonstop_Mutation', #tuncation
-                                    'Missense_Mutation_hotspot',
-                                    'Missense_Mutation',
-                                    'Amplification',
-                                    'In_Frame_Del', 'In_Frame_Ins', 'Splice_Site' ,
-                                    'De_Novo_Start_Out_Frame' ,'De_Novo_Start_In_Frame', 
-                                    'Start_Codon_Ins', 'Start_Codon_SNP', 
-                                    'Silent',
-                                    'Wildtype']
-
-        truncations = ['Frame_Shift_Del', 'Frame_Shift_Ins', 'Nonsense_Mutation', 'Nonstop_Mutation', 'Splice_Site']
-        missenses = ['In_Frame_Del', 'In_Frame_Ins', 'Missense_Mutation']
-        noncodings = ["Intron", "RNA", "3'Flank", "Splice_Region", "5'UTR", "5'Flank", "3'UTR"]
-
-
-
         #check that gene is in the somatic_mutation DataFrame
-        somatic_mutation = self.get_somatic_mutation()
-        if mutations_genes not in somatic_mutation["Gene"].unique(): #if the gene isn't in the somacic mutations df it will still have CNV data that we want
-            def add_del_and_amp_no_somatic(row):
-                if row[mutations_genes] <= -.2:
-                    mutations = 'Deletion'
-
-                elif row[mutations_genes] >= .2:
-                    mutations = 'Amplification'
-                else:
-                    mutations = "No_Mutation"
-
-                return mutations
-
+        somatic_mutation = self.get_somatic_mutation(source=omics_source)
+        #if the gene isn't in the somatic mutations df it will still have CNV data that we want          
+        if mutations_gene not in somatic_mutation["Gene"].unique(): 
             cnv = self.get_CNV(source = omics_source)
-            #drop the database index from ccrcc and brca
             if isinstance(cnv.keys(), pd.core.indexes.multi.MultiIndex):
-                drop = ['Database_ID']
-                cnv = ut.reduce_multiindex(df=cnv, levels_to_drop=drop)       
-            gene_cnv = cnv[[mutations_genes]]
-            mutation_col = gene_cnv.apply(add_del_and_amp_no_somatic, axis=1)
-            df = gene_cnv.assign(Mutation = mutation_col)
-            return df
+                cnv = ut.reduce_multiindex(df=cnv, levels_to_drop=['Database_ID'])       
+            gene_cnv = cnv[[mutations_gene]]
+            gene_cnv["Mutation"] = np.select(
+                    [gene_cnv[mutations_gene] <= -.2, gene_cnv[mutations_gene] >= .2], 
+                    ['Deletion', 'Amplification'], 
+                    'Wildtype_Tumor'
+            )
+            gene_cnv['Location'] = gene_cnv['Mutation']
+            gene_cnv['Mutation_Status'] = 'Single_mutation'
+            gene_cnv.loc[gene_cnv['Mutation'] == 'Wildtype_Tumor'] = 'Wildtype_Tumor'
+            gene_cnv = gene_cnv.drop(mutations_gene, axis=1)
+            return gene_cnv
 
 
         #combine the cnv and mutations dataframe
-        combined = self.join_omics_to_mutations(omics_df_name="CNV", mutations_genes=mutations_genes, omics_genes=mutations_genes, omics_source = omics_source)
-
-
-        #drop the database index 
-        drop = ['Database_ID']
-        combined = ut.reduce_multiindex(df=combined, levels_to_drop=drop)
-
-
-        #If there are hotspot mutations, append 'hotspot' to the mutation type so that it's prioritized correctly
-        def mark_hotspot_locations(row):
-            #iterate through each location in the current row
-            mutations = []
-            for location in row[mutations_genes+'_Location']:
-                if location in mutation_hotspot: #if it's a hotspot mutation
-                    #get the position of the location
-                    position = row[mutations_genes+'_Location'].index(location)
-                    #use that to change the correct mutation
-                    mutations.append(row[mutations_genes+"_Mutation"][position] + "_hotspot")
-                else:
-                    # get the position of the location
-                    position = row[mutations_genes+'_Location'].index(location)
-                    mutations.append(row[mutations_genes+"_Mutation"][position])
-            return mutations
-
+        combined = self.join_omics_to_mutations(
+                omics_name="CNV",
+                mutations_genes=mutations_gene,
+                omics_source=omics_source,
+                mutations_source=mutations_source,
+                omics_genes=mutations_gene,
+                mutations_filter=mutations_filter
+        )
+        if isinstance(combined.index, pd.MultiIndex):
+            combined.columns = combined.columns.droplevel(0)
+        combined["mutations_list"] = np.empty((len(combined), 0)).tolist()
+        
+        #Load the mutation types
+        CNV_col = mutations_gene+ "_" + omics_source + "_CNV"
+        isAmplification = lambda row: row[CNV_col] >= .2
+        isDeletion = lambda row: row[CNV_col] <= -.2
+        mut_type = lambda row: row[mutations_gene + "_Mutation"]
+        
+        combined["mutations_list"] = combined.apply(lambda row: 
+                row["mutations_list"] + ['Deletion'] if isDeletion(row) 
+                else row["mutations_list"] + ['Amplification'] if isAmplification(row) >= .2 
+                else row["mutations_list"], 
+            axis = 1)
+        combined["locations_list"] = combined["mutations_list"]
+
+        combined["mutations_list"] = combined.apply(lambda row: 
+                row["mutations_list"] if (mut_type(row) == ["Wildtype_Tumor"] 
+                        and (isAmplification(row) or isDeletion(row))) 
+                else row["mutations_list"] + row[mutations_gene + "_Mutation"],
+            axis = 1)
+        combined["locations_list"] = combined.apply(lambda row: 
+                row["locations_list"] if (mut_type(row) == ["Wildtype_Tumor"] 
+                        and (isAmplification(row) or isDeletion(row))) 
+                else row["locations_list"] + row[mutations_gene + "_Location"],
+            axis = 1)
+        
+        # Determine hotspots
         if mutation_hotspot is not None:
-            combined['hotspot'] = combined.apply(mark_hotspot_locations, axis=1)
-            combined[mutations_genes+"_Mutation"] = combined['hotspot']
-            combined = combined.drop(columns='hotspot')
-
-
-        # Based on cnv make a new column with mutation type that includes deletions and amplifications
-        def add_del_and_amp(row):
-            if row[mutations_genes+ "_" + omics_source + "_CNV"] <= -.2:
-                mutations = row[mutations_genes+"_Mutation"] + ['Deletion']
-                locations = row[mutations_genes+'_Location']+['Deletion']
-
-            elif row[mutations_genes + "_" + omics_source+"_CNV"] >= .2:
-                mutations = row[mutations_genes+"_Mutation"] + ['Amplification']
-                locations = row[mutations_genes+'_Location']+['Amplification']
-            else:
-                mutations = row[mutations_genes+"_Mutation"]
-                locations = row[mutations_genes+"_Location"]
-
-            return mutations, locations
-
-
-        combined['mutations'], combined['locations'] = zip(*combined.apply(add_del_and_amp, axis=1))
-
-        #now that we have the deletion and amplifications, we need to prioritize the correct mutations.
-        def sort(row):
-            sortedcol = []
-            location = []
-            chosen_indices = []
-            sample_mutations_list = row['mutations']
-            sample_locations_list = row['locations']
-            if len(sample_mutations_list) == 1: #if there's only one mutation in the list
-                sortedcol.append(sample_mutations_list[0])
-                location.append(sample_locations_list[0])
-
-            else:
-                for filter_val in mutations_filter: # This will start at the beginning of the filter list, thus filters earlier in the list are prioritized, like we want
-                    if filter_val in sample_mutations_list:
-                        chosen_indices = [index for index, value in enumerate(sample_mutations_list) if value == filter_val]
-                    if len(chosen_indices) > 0: # We found at least one mutation from the filter to prioritize, so we don't need to worry about later values in the filter priority list
-                        break
-
-                if len(chosen_indices) == 0: # None of the mutations for the sample were in the filter, so we're going to have to use our default hierarchy
-                    for mutation in sample_mutations_list:
-                        if mutation in truncations:
-                            chosen_indices += [index for index, value in enumerate(sample_mutations_list) if value == mutation]
-
-                if len(chosen_indices) == 0: # None of them were in the filter, nor were truncations, so we'll grab all the missenses
-                    for mutation in sample_mutations_list:
-                        if mutation in missenses:
-                            chosen_indices += [index for index, value in enumerate(sample_mutations_list) if value == mutation]
-
-                if len(chosen_indices) == 0: # None of them were in the filter, nor were truncations, nor missenses, so we'll grab all the noncodings
-                    for mutation in sample_mutations_list:
-                        if mutation in noncodings:
-                            chosen_indices += [index for index, value in enumerate(sample_mutations_list) if value == mutation]
-
-                soonest_mutation = sample_mutations_list[chosen_indices[0]]
-                soonest_location = sample_locations_list[chosen_indices[0]]
-                chosen_indices.clear()
-                sortedcol.append(soonest_mutation)
-                location.append(soonest_location)
-
-            return pd.Series([sortedcol, location],index=['mutations', 'locations'])
-
-        df = combined.apply(sort, axis=1)
-        combined['Mutation'] = df['mutations']
-        combined['Location'] = df['locations']
-
-        #get a sample_status column that says if the gene has multiple mutations (including dletion and amplification)
-        def sample_status(row):
-            if len(row['mutations']) > 1: #if there's more than one mutation
-                if len(row['mutations']) == 2 and "Wildtype_Tumor" in row['mutations']: #one of the mutations might be a "wildtype tumor"
-                    status ="Single_mutation"
-
-                elif len(row['mutations']) == 2 and "Wildtype_Normal" in row['mutations']:
-                    status ="Single_mutation"
-
-                else:
-                    status = "Multiple_mutation"
-            else:
-                if row["mutations"] == ["Wildtype_Normal"]:
-                    status = "Wildtype_Normal"
-                elif row['mutations'] == ['Wildtype_Tumor']:
-                    status = "Wildtype_Tumor"
-                else:
-                    status = "Single_mutation"
-
-            return status
-        combined['Mutation_Status'] = combined.apply(sample_status, axis=1)
-
-        #drop all the unnecessary Columns
-        df = combined.drop(columns=[mutations_genes+ "_" + omics_source +"_CNV", mutations_genes+"_Mutation", mutations_genes+"_Location", mutations_genes+"_Mutation_Status", 'Sample_Status', 'mutations','locations'])
-        df['Mutation'] = [','.join(map(str, l)) for l in df['Mutation']]
-        df['Location'] = [','.join(map(str, l)) for l in df['Location']]
-        if show_location == False: df = df.drop(columns="Location") #if they don't want us to show the location, drop it
-
-        return df
+            combined["mutations_list"] = combined.apply(lambda row: 
+                    [
+                        mut + "_hotspot" if row["locations_list"][i] in mutation_hotspot 
+                        else mut 
+                        for i, mut in enumerate(row["mutations_list"])], 
+                axis = 1
+            )
+        
+        #Sort mutation types
+        if mutations_filter == None:
+            mutations_filter = [
+                'Deletion',
+                'Frame_Shift_Del', 'Frame_Shift_Ins', 'Nonsense_Mutation', 'Nonstop_Mutation',
+                'Missense_Mutation',
+                'Amplification',
+                'In_Frame_Del', 'In_Frame_Ins', 'Splice_Site' ,
+                'De_Novo_Start_Out_Frame' ,'De_Novo_Start_In_Frame', 
+                'Start_Codon_Ins', 'Start_Codon_SNP', 
+                'Silent',
+                'Wildtype_Tumor'
+            ]
+        mutations_filter = {
+            mutation : 2 * rank + 1 for rank, mutation in enumerate(mutations_filter)
+        }
+        if mutation_hotspot != None:
+            hotspot_filter = {
+                mutation + "_hotspot" : rank for rank, mutation in enumerate(mutations_filter)
+            }
+            mutations_filter.update(hotspot_filter)
+
+        # Although seemingly complex, the following five lines do the following:
+        # 1. For each row, link (zip) the items in the ["mutations_list"] and ["locations_list"] columns together
+        # 2. Sort the ["mutations_list"] column based on its position in mutations_filter, including its respective location
+        # 3. Unlink the lists using list comprehension (last 4 lines)
+        sorted_mut_loc = combined.apply(lambda row: 
+                sorted(
+                    zip(row["mutations_list"], row["locations_list"]), 
+                    key = lambda pair: mutations_filter[pair[0]]
+                ), 
+            axis = 1)
+        sorted_mut_loc = sorted_mut_loc.tolist()
+        sorted_mut_loc = list(sorted_mut_loc)
+        combined["mutations_list"] = [[items[0] for items in row] for row in sorted_mut_loc]
+        combined["locations_list"] = [[items[1] for items in row] for row in sorted_mut_loc]
+        
+
+        combined["Mutation"] = combined.apply(lambda row: row["mutations_list"][0], axis = 1)
+        combined["Location"] = combined.apply(lambda row: row["locations_list"][0], axis = 1)
+        combined["Mutation_Status"] = combined.apply(lambda row: 
+                "Wildtype_Tumor" if row["mutations_list"][0] == "Wildtype_Tumor" 
+                else "Single_mutation" if len(row["mutations_list"]) == 1 
+                else "Multiple_mutation", 
+            axis = 1
+            )
+        result = combined[["Mutation", "Location", "Mutation_Status"]]
+        if not show_location:
+            result.drop("Location", inplace = True)
+        return result
+    
+#     Additional information for some datasets, not applicable to pancan
+#     truncations = ['Frame_Shift_Del', 'Frame_Shift_Ins', 'Nonsense_Mutation', 'Nonstop_Mutation', 'Splice_Site']
+#     missenses = ['In_Frame_Del', 'In_Frame_Ins', 'Missense_Mutation']
+#     noncodings = ["Intron", "RNA", "3'Flank", "Splice_Region", "5'UTR", "5'Flank", "3'UTR"]
 
-    def _warn_inserted_nans(self, name1, name2, index1, index2):
+    def _warn_inserted_nans(self, name1: str, name2: str, index1: pd.Index, index2: pd.Index):
         """Compare two indices from two dataframes, and warn the user that any rows with index values not in both indices were filled with NaNs in a join function.
 
         Parameters:
         name1 (str): Name of the dataframe the first index came from
         name2 (str): Name of the dataframe the second index came from
         index1 (pandas.Index): First index to compare
         index2 (pandas.Index): Second index to compare
@@ -1495,20 +1491,20 @@
         """
         unique1 = index1.difference(index2)
         unique2 = index2.difference(index1)
 
         self._issue_inserted_nans_warning(unique1, name2)
         self._issue_inserted_nans_warning(unique2, name1)
 
-    def _issue_inserted_nans_warning(self, unique, other_name):
+    def _issue_inserted_nans_warning(self, unique: list[str], other_name: str):
         """Issue a warning that the samples in unique were not found in the other_name dataframe, and those column(s) were filled with NaN.
 
         Parameters:
         unique (list or array-like of str): The samples that weren't in the other_name dataframe.
         other_name (str): The name of the dataframe the samples weren't found in.
 
         Returns: None
         """
         if other_name == "somatic_mutation":
             return # This will have separate fill warnings printed, because we use different fill values.
         elif len(unique) > 0:
-            warnings.warn(f"{other_name} data was not found for the following samples, so {other_name} data columns were filled with NaN for these samples: {', '.join(unique)}", InsertedNanWarning, stacklevel=4)
+            warnings.warn(f"{other_name} data was not found for the following samples, so {other_name} data columns were filled with NaN for these samples: {', '.join(unique)}", InsertedNanWarning, stacklevel=4)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/ccrcc.py` & `cptac-1.5.0rc3/cptac/cancers/ccrcc.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,34 +5,47 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Imports from the cptac.cancers package
 from cptac.cancers.cancer import Cancer
 
-from cptac.cancers.awg.awgccrcc import AwgCcrcc
+# Imports from the cptac.cancers sub-packages
 from cptac.cancers.bcm.bcmccrcc import BcmCcrcc
 from cptac.cancers.broad.broadccrcc import BroadCcrcc
-from cptac.cancers.pdc.pdcccrcc import PdcCcrcc
 from cptac.cancers.umich.umichccrcc import UmichCcrcc
 from cptac.cancers.washu.washuccrcc import WashuCcrcc
 from cptac.cancers.mssm.mssm import Mssm
 from cptac.cancers.harmonized.harmonized import Harmonized
 
 
 class Ccrcc(Cancer):
+    """
+    The Ccrcc class is a subclass of the Cancer class and provides an interface to
+    various data sources with ccRCC (clear cell renal cell carcinoma) data.
+
+    Attributes:
+        _sources (dict): A dictionary that holds instances of data source objects.
+    """
 
     def __init__(self, no_internet=False):
-        """Load all the data sources with ccRCC data and provide an interface to them."""
-
+        """
+        Constructor for the Ccrcc class. It initializes instances of various data source
+        classes and adds them to the _sources attribute.
+
+        Parameters:
+            no_internet (bool): A flag indicating whether to download data or not. If True,
+                                the data source objects are initialized without downloading
+                                data. Defaults to False.
+        """
         super().__init__(cancer_type="ccrcc")
-        
-        self._sources["awg"] = AwgCcrcc(version="latest", no_internet=no_internet)
-        self._sources["bcm"] = BcmCcrcc(version="latest", no_internet=no_internet)
-        self._sources["broad"] = BroadCcrcc(version="latest", no_internet=no_internet)
-        self._sources["mssm"] = Mssm(filter_type='ccrcc', version="latest", no_internet=no_internet)
-        self._sources["pdc"] = PdcCcrcc(version="latest", no_internet=no_internet)
-        self._sources["umich"] = UmichCcrcc(version="latest", no_internet=no_internet)
-        self._sources["washu"] = WashuCcrcc(version="latest", no_internet=no_internet)
-        self._sources["harmonized"] = Harmonized(filter_type='ccrcc', version="latest", no_internet=no_internet)
+
+        # Initialize data sources and add them to the _sources dictionary
+        self._sources["bcm"] = BcmCcrcc(no_internet=no_internet)
+        self._sources["broad"] = BroadCcrcc(no_internet=no_internet)
+        self._sources["mssm"] = Mssm(filter_type='ccrcc', no_internet=no_internet)
+        self._sources["umich"] = UmichCcrcc(no_internet=no_internet)
+        self._sources["washu"] = WashuCcrcc(no_internet=no_internet)
+        self._sources["harmonized"] = Harmonized(filter_type='ccrcc', no_internet=no_internet)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/coad.py` & `cptac-1.5.0rc3/cptac/cancers/lscc.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,34 +5,46 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Importing the base Cancer class
 from cptac.cancers.cancer import Cancer
 
-from cptac.cancers.awg.awgcoad import AwgCoad
-from cptac.cancers.bcm.bcmcoad import BcmCoad
-from cptac.cancers.broad.broadcoad import BroadCoad
-from cptac.cancers.pdc.pdccoad import PdcCoad
-from cptac.cancers.umich.umichcoad import UmichCoad
-from cptac.cancers.washu.washucoad import WashuCoad
+# Importing data sources for LSCC
+from cptac.cancers.bcm.bcmlscc import BcmLscc
+from cptac.cancers.broad.broadlscc import BroadLscc
+from cptac.cancers.umich.umichlscc import UmichLscc
+from cptac.cancers.washu.washulscc import WashuLscc
 from cptac.cancers.mssm.mssm import Mssm
 from cptac.cancers.harmonized.harmonized import Harmonized
 
-
-class Coad(Cancer):
+class Lscc(Cancer):
+    """
+    The Lscc class inherits from the Cancer class and provides access to various data sources 
+    for LSCC (Lung squamous cell carcinoma).
+
+    Attributes:
+        _sources (dict): A dictionary that stores instances of data source objects.
+    """
 
     def __init__(self, no_internet=False):
-        """Load all the data sources with COAD data and provide an interface to them."""
-
-        super().__init__(cancer_type="coad")
+        """
+        The constructor for the Lscc class. It initializes instances of various data source 
+        classes and adds them to the _sources attribute.
+
+        Parameters:
+            no_internet (bool): If set to True, the data source objects are initialized 
+                                without downloading data. Default is False.
+        """
+        super().__init__(cancer_type="lscc")
+        
+        # Initialize data sources and add them to the _sources dictionary
+        self._sources["bcm"] = BcmLscc(no_internet=no_internet)
+        self._sources["broad"] = BroadLscc(no_internet=no_internet)
+        self._sources["mssm"] = Mssm(filter_type='lscc', no_internet=no_internet)
+        self._sources["umich"] = UmichLscc(no_internet=no_internet)
+        self._sources["washu"] = WashuLscc(no_internet=no_internet)
+        self._sources["harmonized"] = Harmonized(filter_type='lscc', no_internet=no_internet)
 
-        self._sources["awg"] = AwgCoad(version="latest", no_internet=no_internet)
-        self._sources["bcm"] = BcmCoad(version="latest", no_internet=no_internet)
-        self._sources["broad"] = BroadCoad(version="latest", no_internet=no_internet)
-        self._sources["mssm"] = Mssm(filter_type='coad', version="latest", no_internet=no_internet)
-        self._sources["pdc"] = PdcCoad(version="latest", no_internet=no_internet)
-        self._sources["umich"] = UmichCoad(version="latest", no_internet=no_internet)
-        self._sources["washu"] = WashuCoad(version="latest", no_internet=no_internet)
-        self._sources["harmonized"] = Harmonized(filter_type='coad', version="latest", no_internet=no_internet)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/luad.py` & `cptac-1.5.0rc3/cptac/cancers/ov.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,34 +5,46 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Importing the base Cancer class
 from cptac.cancers.cancer import Cancer
 
-from cptac.cancers.awg.awgluad import AwgLuad
-from cptac.cancers.bcm.bcmluad import BcmLuad
-from cptac.cancers.broad.broadluad import BroadLuad
-from cptac.cancers.pdc.pdcluad import PdcLuad
-from cptac.cancers.umich.umichluad import UmichLuad
-from cptac.cancers.washu.washuluad import WashuLuad
+# Importing data sources for OV (Ovarian cancer)
+from cptac.cancers.bcm.bcmov import BcmOv
+from cptac.cancers.broad.broadov import BroadOv
+from cptac.cancers.umich.umichov import UmichOv
+from cptac.cancers.washu.washuov import WashuOv
 from cptac.cancers.mssm.mssm import Mssm
 from cptac.cancers.harmonized.harmonized import Harmonized
 
-
-class Luad(Cancer):
+class Ov(Cancer):
+    """
+    The Ov class inherits from the Cancer class and provides access to various data sources 
+    for OV (Ovarian cancer).
+
+    Attributes:
+        _sources (dict): A dictionary that stores instances of data source objects.
+    """
 
     def __init__(self, no_internet=False):
-        """Load all the data sources with LUAD data and provide an interface to them."""
-
-        super().__init__(cancer_type="luad")
+        """
+        The constructor for the Ov class. It initializes instances of various data source 
+        classes and adds them to the _sources attribute.
+
+        Parameters:
+            no_internet (bool): If set to True, the data source objects are initialized 
+                                without downloading data. Default is False.
+        """
+        super().__init__(cancer_type="ov")
         
-        self._sources["awg"] = AwgLuad(version="latest", no_internet=no_internet)
-        self._sources["bcm"] = BcmLuad(version="latest", no_internet=no_internet)
-        self._sources["broad"] = BroadLuad(version="latest", no_internet=no_internet)
-        self._sources["mssm"] = Mssm(filter_type='luad', version="latest", no_internet=no_internet)
-        self._sources["pdc"] = PdcLuad(version="latest", no_internet=no_internet)
-        self._sources["umich"] = UmichLuad(version="latest", no_internet=no_internet)
-        self._sources["washu"] = WashuLuad(version="latest", no_internet=no_internet)
-        self._sources["harmonized"] = Harmonized(filter_type='luad', version="latest", no_internet=no_internet)
+        # Initialize data sources and add them to the _sources dictionary
+        self._sources["bcm"] = BcmOv(no_internet=no_internet)
+        self._sources["broad"] = BroadOv(no_internet=no_internet)
+        self._sources["mssm"] = Mssm(filter_type='ov', no_internet=no_internet)
+        self._sources["umich"] = UmichOv(no_internet=no_internet)
+        self._sources["washu"] = WashuOv(no_internet=no_internet)
+        self._sources["harmonized"] = Harmonized(filter_type='ov', no_internet=no_internet)
+
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/pdac.py` & `cptac-1.5.0rc3/cptac/cancers/pdac.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,34 +5,46 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Importing the base Cancer class
 from cptac.cancers.cancer import Cancer
 
-from cptac.cancers.awg.awgpdac import AwgPdac
+# Importing data sources for PDAC (Pancreatic Ductal Adenocarcinoma)
 from cptac.cancers.bcm.bcmpdac import BcmPdac
 from cptac.cancers.broad.broadpdac import BroadPdac
-from cptac.cancers.pdc.pdcpdac import PdcPdac
 from cptac.cancers.umich.umichpdac import UmichPdac
 from cptac.cancers.washu.washupdac import WashuPdac
 from cptac.cancers.mssm.mssm import Mssm
 from cptac.cancers.harmonized.harmonized import Harmonized
 
-
 class Pdac(Cancer):
+    """
+    The Pdac class inherits from the Cancer class and provides access to various data sources 
+    for PDAC (Pancreatic Ductal Adenocarcinoma).
+
+    Attributes:
+        _sources (dict): A dictionary that stores instances of data source objects.
+    """
 
     def __init__(self, no_internet=False):
-        """Load all the data sources with PDAC data and provide an interface to them."""
-
+        """
+        The constructor for the Pdac class. It initializes instances of various data source 
+        classes and adds them to the _sources attribute.
+
+        Parameters:
+            no_internet (bool): If set to True, the data source objects are initialized 
+                                without downloading data. Default is False.
+        """
         super().__init__(cancer_type="pdac")
 
-        self._sources["awg"] = AwgPdac(version="latest", no_internet=no_internet)
-        self._sources["bcm"] = BcmPdac(version="latest", no_internet=no_internet)
-        self._sources["broad"] = BroadPdac(version="latest", no_internet=no_internet)
-        self._sources["mssm"] = Mssm(filter_type='pdac', version="latest", no_internet=no_internet)
-        self._sources["pdc"] = PdcPdac(version="latest", no_internet=no_internet)
-        self._sources["umich"] = UmichPdac(version="latest", no_internet=no_internet)
-        self._sources["washu"] = WashuPdac(version="latest", no_internet=no_internet)
-        self._sources["harmonized"] = Harmonized(filter_type='pdac', version="latest", no_internet=no_internet)
+        # Initialize data sources and add them to the _sources dictionary
+        self._sources["bcm"] = BcmPdac(no_internet=no_internet)
+        self._sources["broad"] = BroadPdac(no_internet=no_internet)
+        self._sources["mssm"] = Mssm(filter_type='pdac', no_internet=no_internet)
+        self._sources["umich"] = UmichPdac(no_internet=no_internet)
+        self._sources["washu"] = WashuPdac(no_internet=no_internet)
+        self._sources["harmonized"] = Harmonized(filter_type='pdac', no_internet=no_internet)
+
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/pdc/pdcgbm.py` & `cptac-1.5.0rc3/cptac/cancers/source.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,159 +5,131 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-import pandas as pd
-import numpy as np
 import os
-import warnings
-import datetime
-import mygene
-
-from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
+import cptac
+import pandas as pd
+from hashlib import md5
+from warnings import warn
 
-class PdcGbm(Source):
+from cptac import CPTAC_BASE_DIR
+from cptac.exceptions import DataTypeNotInSourceError, MissingFileError, FailedChecksumWarning
+from cptac.tools.dataframe_tools import standardize_axes_names
+
+class Source:
+    """
+    The Source class is a base class that provides methods to manage and interact with different data sources.
+    
+    Attributes:
+        no_internet (bool): If set to True, the data source objects are initialized
+                            without downloading data. Default is False.
+        source (str): The name of the data source.
+        cancer_type (str): The type of cancer that the data pertains to.
+        _data (dict): Dictionary to hold the loaded dataframes.
+        _helper_tables (dict): Dictionary to hold helper tables that support
+                                certain functions.
+        data_files (dict): Dictionary that holds the data file names for each
+                            data type.
+        load_functions (dict): Dictionary that holds the load function for each
+                                data type.
+    """
 
-    def __init__(self, version="latest", no_internet=False):
-        """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+    def __init__(self, cancer_type, source, data_files, load_functions, no_internet):
+        """
+        The constructor for the Source class.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+            cancer_type (str): The type of cancer that the data pertains to.
+            source (str): The name of the data source.
+            data_files (dict): Dictionary that holds cthe data file names for each
+                                data type.
+            load_functions (dict): Dictionary that holds the load function for each
+                                    data type.
+            no_internet (bool): If set to True, the data source objects are
+                                initialized without downloading data. Default is False.
         """
+        self.no_internet = no_internet
+        self.source = source
+        self.cancer_type = cancer_type
+        self._data = {}
+        self._helper_tables = {}
+        self.data_files = data_files
+        self.load_functions = load_functions
 
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
+    def get_df(self, df_type):
+        """Get the dataframe of the specified data type
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
-        self.data_files = {
-            "1.0": {
-                "acetylproteomics"     : "acetylproteomics.tsv.gz",
-                "clinical"             : "clinical.tsv.gz",
-                "phosphoproteomics"    : "phosphoproteomics.tsv.gz",
-                "proteomics"           : "proteomics.tsv.gz",
-                "mapping"              : "GBM_normal_sample_mapping.xlsx"
-            }
-        }
-        
-        self.load_functions = {
-            'acetylproteomics' : self.load_acetylproteomics,
-            'clinical' : self.load_clinical,
-            'phosphoproteomics' : self.load_phosphoproteomics,
-            'proteomics' : self.load_proteomics,
-        }
-        
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
+        Parameters:
+        df_type (str): Name of datatype to return e.g. "proteomics".
 
-        # Call the parent class __init__ function
-        super().__init__(cancer_type="gbm", source='pdc', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-        
-        
-    def load_acetylproteomics(self):
-        df_type = 'acetylproteomics'
-        
-        if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep='\t')
-            
-            # Get dictionary to map GTEX IDs to patient IDs (for GTEX normal samples)
-            self.load_mapping()
-            mapping_dict = self._helper_tables["map_ids"]
-            
-            df['Patient_ID'] = df['case_submitter_id'].replace(mapping_dict) # GTEX IDs to patient IDs for normal samples
-            df = df.set_index('Patient_ID')
-            df = df.drop(['aliquot_submitter_id', 'case_submitter_id'], axis = 'columns')
-            df = map_database_to_gene_pdc(df, 'refseq') # map refseq IDs to gene names
-            
-            # save df in self._data
-            self.save_df(df_type, df)
-            
-            
-    def load_clinical(self):
-        df_type = 'clinical'
-        
-        if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep='\t', index_col=0)
-            df = df.drop(['ref'], axis = 'index') # Drop quality control and ref intensity
-            
-            # Get dictionary to map GTEX IDs to patient IDs (for GTEX normal samples)
-            self.load_mapping()
-            mapping_dict = self._helper_tables["map_ids"]
-            
-            df = df.reset_index()
-            df['Patient_ID'] = df['case_submitter_id'].replace(mapping_dict) # GTEX IDs to patient IDs for normal samples
-            df = df.set_index('Patient_ID')
-            df = df.drop(['case_submitter_id'], axis = 'columns') 
-            
-            # save df in self._data
-            self.save_df(df_type, df)
-            
-            
-    def load_phosphoproteomics(self):
-        df_type = 'phosphoproteomics'
-        
-        if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep='\t')
-            
-            # Get dictionary to map GTEX IDs to patient IDs (for GTEX normal samples)
-            self.load_mapping()
-            mapping_dict = self._helper_tables["map_ids"]
-            
-            df['Patient_ID'] = df['case_submitter_id'].replace(mapping_dict) # GTEX IDs to patient IDs for normal samples
-            df = df.set_index('Patient_ID')
-            df = df.drop(['aliquot_submitter_id', 'case_submitter_id'], axis = 'columns')
-            df = map_database_to_gene_pdc(df, 'refseq') # map refseq IDs to gene names
-            
-            # save df in self._data
-            self.save_df(df_type, df)
-            
-            
-    def load_proteomics(self):
-        df_type = 'proteomics'
-        
+        Returns:
+        pandas.DataFrame: The dataframe of the desired datatype.
+        """
+        # if that df hasn't been loaded yet, load it
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
-            file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep='\t')
-            
-            # Get dictionary to map GTEX IDs to patient IDs (for GTEX normal samples)
-            self.load_mapping()
-            mapping_dict = self._helper_tables["map_ids"]
-            
-            # Proteomics
-            df['Patient_ID'] = df['case_submitter_id'].replace(mapping_dict) # GTEX IDs to patient IDs for normal samples
-            df = df.set_index('Patient_ID')
-            df = df.drop(['aliquot_submitter_id', 'case_submitter_id'], axis = 'columns')
-            
-            # save df in self._data
-            self.save_df(df_type, df)
-            
-    
-    def load_mapping(self):
-        df_type = 'mapping'
-        
-        if not self._helper_tables:
-            file_path = self.locate_files(df_type)
+            # check to see if the df type requested is availabe from this source
+            if df_type not in self.load_functions:
+                raise DataTypeNotInSourceError(f"The {self.source} source does not have {df_type} data for {self.cancer_type} cancer.")
+            self.load_functions[df_type]()
+        return self._data[df_type]
+
+    def save_df(self, df_type, df):
+        """Perform final formatting so all cptac data is consistent, and save the dataframe in the self._data dictionary with df_type as the key"""
+
+        # set the index name to "Patient_ID" and the columns name to "Name"
+        standardize_axes_names(df)
+
+        # Sort the dataframe based off sample status (tumor or normal), then alphabetically
+        df = df.sort_index()
+        #'.N' for normal, '.C' for cored normals (in HNSCC)
+        normal = df.loc[df.index.str.contains(r'\.[NC]$', regex = True, na = False)]
+        # Tumor samples don't have any special endings cohorts for now
+        tumor = df.loc[~ df.index.str.contains(r'\.[NC]$', regex = True, na = False)]
+        df = pd.concat([tumor, normal])
+
+        self._data[df_type] = df
+
+
+    def locate_files(self, datatype):
+        """Checks if the datatype is valid
+        If the datatype is valid, it finds the file path, downloading the files if necessary
+
+        Parameters:
+            datatype (str): The datatype to get all filepaths for.
 
-            # This file maps GTEX normal samples to our desired 'PT-' subject identifier and
-            # can be found on Box under CPTAC/cptac/pancan/helper_files
-            df = pd.read_excel(file_path, index_col = 'Original Id', usecols = ['Original Id', 'Subject ID'])
-            df['Subject ID'] = df['Subject ID'].apply(lambda x: x+'.N' if 'PT-' in x else x) # add normal identifier 
-            map_dict = df.to_dict()['Subject ID']
-            self._helper_tables["map_ids"] = map_dict
-            
+        Returns:
+            A single file path or a list of file paths to all files of the given datatype
+        """
+        # pull the file name or list of file names from the self.data_files dict
+        data_files = self.data_files[datatype]
+        # self.data_files can either contain a single string or a list of strings. Let's work with all as a list for now.
+        if type(data_files) != list:
+            data_files = [data_files]
+        file_paths = []
+        # Locate and download each data_file
+        for data_file in data_files:
+            # dataset = self.source if self.source in ['harmonized', 'mssm'] else f"{self.source}_{self.cancer_type}"
+            # This should eventually be handled within the respective sources, but this will do for now
+            cancer_type = "all_cancers" if self.source in ['mssm', 'harmonized'] or self.source in['washu'] and datatype in ['tumor_purity', 'hla_typing'] else self.cancer_type
+            dataset = f"{self.source}-{cancer_type}"
+            file_path = os.path.join(CPTAC_BASE_DIR, f"data/{dataset}/{data_file}")
+            prefixed_file = f"{self.source}-{cancer_type}-{datatype}-{data_file}"
+            # Ensure data is not corrupted, download files if needed
+            if os.path.isfile(file_path) and not self.no_internet: # It's pointless to check the checksum if we can't redownload it
+                with open(file_path, 'rb') as in_file:
+                    local_hash = f"md5:{md5(in_file.read()).hexdigest()}"
+                if local_hash != cptac.INDEX.loc[cptac.INDEX['filename']==prefixed_file, 'checksum'].item():
+                    warn(FailedChecksumWarning("Local file and online file have different checksums; redownloading data"))
+                    os.remove(file_path)
+                
+            if not os.path.isfile(file_path) and not self.no_internet:
+                cptac.download(self.cancer_type, self.source, datatype, data_file)
+            elif not os.path.isfile(file_path) and self.no_internet:
+                raise MissingFileError(f"The {self.source} {data_file} file for the {self.cancer_type} is not downloaded and you are running cptac in no_internet mode.")
+
+            file_paths.append(file_path)
+        
+        return file_paths if len(file_paths) >= 2 else file_paths[0]
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichbrca.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichbrca.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,71 +6,57 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
+import cptac.tools.dataframe_tools as df_tools
+from cptac import CPTAC_BASE_DIR
 
 
 class UmichBrca(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                # prosp-brca-all-samples.txt shows which patient IDs have normal samples and which have replicates 
-                # This file can be found on Box under CPTAC/cptac/pancan/helper_files
-                "mapping" : "prosp-brca-all-samples.txt",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-            }
+            "proteomics": "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",
+            "phosphoproteomics": "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            # prosp-brca-all-samples.txt shows which patient IDs have normal samples and which have replicates
+            "mapping": "prosp-brca-all-samples.txt.gz",
+            "acetylproteomics": "abundance_multi-site_MD.tsv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],
         }
-        
+
         self.load_functions = {
-            'phosphoproteomics' : self.load_phosphoproteomics,
-            'proteomics' : self.load_proteomics,
+            'phosphoproteomics': self.load_phosphoproteomics,
+            'proteomics': self.load_proteomics,
+            'acetylproteomics': self.load_acetylproteomics,
         }
-        
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
 
         # Call the parent class __init__ function
-        super().__init__(cancer_type="brca", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="brca", source="umich", data_files=self.data_files,
+                         load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
         df_type = 'mapping'
-        
+
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
 
-            map_df = pd.read_csv(file_path, sep = "\t")
+            map_df = pd.read_csv(file_path, sep="\t")
             map_df = map_df[['Participant', 'id', 'Type']]
             self._helper_tables["map_ids"] = map_df
 
             # Drop samples that don't correlate well with the original cptac tumor values
             # The proteomics and phosphoproteomics file contained duplicate patient IDs with unique values. 18 of these were IDs
             # with both tumor and normal samples (according to the mapping file). To find which ID contained values nearest to the
             # original cptac tumor measurements, we calculated pearson correlations and created scatterplots to compare
@@ -79,136 +65,183 @@
             # The second occurrence showed a low correlation with the flagship tumor values (average around  0.2).
             # In Brca, normal samples were dropped in downstream analysis because of quality control issues. Therefore, we dropped
             # the second occurrence of the 18 patient IDs with a normal sample because they did not correlate well with the
             # flagship tumor values and are likely normal samples. There were 7 IDs with replicates shown in the mapping file
             # (prosp-brca-all-samples.txt). The same method was used to check that these correlated well with their respective
             # flagship cptac tumor values. Replicates were averaged (consistent with the handling of other replicates in the pancan module).
             # note:  21BR010.1 had a correlation of 0.275 (so dropped), and 21BR010.2 had correlation of 0.848 (so averaged)
-            # A file containing the correlations can be downloaded at:
-            # https://byu.box.com/shared/static/jzsq69bd079oq0zbicw4w616hyicd5ev.xlsx
-
             # Get patient IDs with normal samples or replicates (from mapping file)
             # 7 IDs with replicates: '11BR031', '11BR053', '11BR036', '11BR060', '14BR005', '11BR011', '21BR010'
             # 18 IDs with normals: '11BR074', '11BR073', '20BR007', '21BR010', '11BR017', '05BR029', '18BR003', '11BR030',
             #   '01BR027','11BR025', '11BR047', '11BR028', '11BR020', '20BR008', '11BR024', '11BR023', '11BR015', '11BR006'
 
             # Get IDs with replicates
             replicate_list = list(set(map_df.loc[map_df.id.str.contains('REP')].Participant))
             replicate_list.remove('RetroIR')
             replicate_list = [x[1:] for x in replicate_list]
             self._helper_tables["replicate_list"] = replicate_list
 
             # Get IDs with normals
-            norm_df = map_df.loc[map_df.Type == 'Adjacent_Normal'] # get all patient_IDs with normal samples
-            norm_df.index = norm_df.Participant.apply(lambda x: x[1:]+'.1') #remove initial 'X' and add '.1' (did not correlate well)
+            norm_df = map_df.loc[map_df.Type == 'Adjacent_Normal']  # get all patient_IDs with normal samples
+            norm_df.index = norm_df.Participant.apply(
+                lambda x: x[1:] + '.1')  # remove initial 'X' and add '.1' (did not correlate well)
             not_tumor = norm_df.index.to_list()
             self._helper_tables["not_tumor"] = not_tumor
 
-
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
-        
+
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            df = pd.read_csv(file_path, sep = "\t")
-            
-             # Parse a few columns out of the "Index" column that we'll need for our multiindex
-            df[['Database_ID','Transcript_ID',"Gene_ID","Havana_gene","Havana_transcript","Transcript","Name","Site"]] = df.Index.str.split("\\|",expand=True)
-            df[['num1','start',"end","detected_phos","localized_phos","Site"]] = df.Site.str.split("_",expand=True) 
-
-            # Some rows have at least one localized phosphorylation site, but also have other 
-            # phosphorylations that aren't localized. We'll drop those rows, if their localized 
-            # sites are duplicated in another row, to avoid creating duplicates, because we only 
-            # preserve information about the localized sites in a given row. However, if the localized 
+            df = pd.read_csv(file_path, sep="\t")
+
+            df_mapping = pd.read_csv(f"{CPTAC_BASE_DIR}/data/brca_mapping.csv")
+            patient_dict = dict(zip(df_mapping['Hash'], df_mapping['Patient_ID']))
+
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID', 'Transcript_ID', "Gene_ID", "Havana_gene", "Havana_transcript", "Transcript", "Name",
+                "Site"]] = df.Index.str.split("\\|", expand=True)
+            df[['num1', 'start', "end", "detected_phos", "localized_phos", "Site"]] = df.Site.str.split("_",
+                                                                                                        expand=True)
+
+            # Some rows have at least one localized phosphorylation site, but also have other
+            # phosphorylations that aren't localized. We'll drop those rows, if their localized
+            # sites are duplicated in another row, to avoid creating duplicates, because we only
+            # preserve information about the localized sites in a given row. However, if the localized
             # sites aren't duplicated in another row, we'll keep the row.
-            
-            # dectected_phos of the split "Index" column is number of phosphorylations detected, 
+
+            # dectected_phos of the split "Index" column is number of phosphorylations detected,
             # and localized_phos is number of phosphorylations localized, so if the two values aren't equal, the row has at least one unlocalized site
-            unlocalized_to_drop = df.index[~df["detected_phos"].eq(df["localized_phos"]) & df.duplicated(["Name", "Site", "Peptide", "Database_ID"], keep=False)]
+            unlocalized_to_drop = df.index[~df["detected_phos"].eq(df["localized_phos"]) & df.duplicated(
+                ["Name", "Site", "Peptide", "Database_ID"], keep=False)]
             df = df.drop(index=unlocalized_to_drop)
 
-            df = df[df['Site'].notna()] # only keep columns with phospho site 
-            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # Create a multiindex in this order.
-            #drop columns not needed in df 
-            df.drop(['Gene', "Index", "num1", "start", "end", "detected_phos", "localized_phos", "Havana_gene", 
+            df = df[df['Site'].notna()]  # only keep columns with phospho site
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID'])  # Create a multiindex in this order.
+            # drop columns not needed in df
+            df.drop(['Gene', "Index", "num1", "start", "end", "detected_phos", "localized_phos", "Havana_gene",
                      "Havana_transcript", "MaxPepProb", "Gene_ID", "Transcript_ID", "Transcript"], axis=1, inplace=True)
             df = df.transpose()
-            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios 
-            df = df.subtract(ref_intensities, axis="columns") # Subtract ref intensities from all the values, to get ratios
-            df = df.iloc[1:,:] # drop ReferenceIntensity row 
+            ref_intensities = df.loc["ReferenceIntensity"]  # Get reference intensities to use to calculate ratios
+            df = df.subtract(ref_intensities,
+                             axis="columns")  # Subtract ref intensities from all the values, to get ratios
+            df = df.iloc[1:, :]  # drop ReferenceIntensity row
             # drop ending of CPT retrospective samples to match cptac
-            df = df.rename(index={'CPT0008140004':'CPT000814', 'CPT0018460005': 'CPT001846', 
-                                  '604':'CPT000814'}) # 604 mapped to CPT000814 in pdc index
+            df = df.rename(index={'CPT000814-0004': 'CPT000814', 'CPT001846-0005': 'CPT001846'})
 
-            drop_cols = ['RetroIR','RetroIR.1','RefInt_Pool01-1','RefInt_Pool02-1',
-                         'RefInt_Pool03-1','RefInt_Pool04-1','RefInt_Pool05-1','RefInt_Pool06-1',
-                         'RefInt_Pool07-1','RefInt_Pool08-1','RefInt_Pool09-1','RefInt_Pool10-1',
-                         'RefInt_Pool11-1','RefInt_Pool12-1','RefInt_Pool13-1','RefInt_Pool14-1',
-                         'RefInt_Pool15-1','RefInt_Pool16-1','RefInt_Pool17-1']
+            drop_cols = ['RetroIR-07', 'RetroIR-13', 'RefInt_Pool01', 'RefInt_Pool02',
+                         'RefInt_Pool03', 'RefInt_Pool04', 'RefInt_Pool05', 'RefInt_Pool06',
+                         'RefInt_Pool07', 'RefInt_Pool08', 'RefInt_Pool09', 'RefInt_Pool10',
+                         'RefInt_Pool11', 'RefInt_Pool12', 'RefInt_Pool13', 'RefInt_Pool14',
+                         'RefInt_Pool15', 'RefInt_Pool16', 'RefInt_Pool17']
             # Drop quality control and ref intensity cols
-            df = df.drop(drop_cols, axis = 'index')
-            
-            if self.version == "1.0":
-                self.load_mapping()
-                not_tumor = self._helper_tables["not_tumor"]
-                replicate_list = self._helper_tables["replicate_list"]
-                df = df.loc[ ~ df.index.isin(not_tumor)] # drop rows that don't correlate well with respective cptac tumor
-                df = average_replicates(df, replicate_list) # average 7 IDs with replicates
+            df = df.drop(drop_cols, axis='index')
+
+            self.load_mapping()
+            not_tumor = self._helper_tables["not_tumor"]
+            replicate_list = self._helper_tables["replicate_list"]
+            df = df.loc[~ df.index.isin(not_tumor)]  # drop rows that don't correlate well with respective cptac tumor
+            df = df_tools.average_replicates(df, replicate_list)  # average 7 IDs with replicates
+
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: patient_dict.get(x, x))
+
+            df['Patient_ID'] = df['Patient_ID'].apply(
+                lambda x: x + '.N' if 'NX' in x else x)  # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
 
             # save df in self._data
             self.save_df(df_type, df)
-            
-    
+
     def load_proteomics(self):
         df_type = 'proteomics'
-        
+
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep = "\t") 
-            df['Database_ID'] = df.Index.apply(lambda x: x.split('|')[0]) # get protein identifier 
-            df['Name'] = df.Index.apply(lambda x: x.split('|')[6]) # get protein name 
-            df = df.set_index(['Name', 'Database_ID']) # set multiindex
-            df = df.drop(columns = ['Index', 'MaxPepProb', 'NumberPSM', 'Gene']) # drop unnecessary  columns
+            df = pd.read_csv(file_path, sep="\t")
+            df['Database_ID'] = df["Index"].str.split('|').str[0]  # get protein identifier
+            df['Name'] = df["Index"].str.split('|').str[6]  # get protein name
+            df = df.set_index(['Name', 'Database_ID'])  # set multiindex
+            df = df.drop(columns=['Index', 'MaxPepProb', 'NumberPSM', 'Gene'])  # drop unnecessary  columns
             df = df.transpose()
-            ref_intensities = df.loc["ReferenceIntensity"] # get reference intensities to use to calculate ratios 
-            df = df.subtract(ref_intensities, axis="columns") # subtract reference intensities from all the values
-            df = df.iloc[1:,:] # drop ReferenceIntensity row 
+            ref_intensities = df.loc["ReferenceIntensity"]  # get reference intensities to use to calculate ratios
+            df = df.subtract(ref_intensities, axis="columns")  # subtract reference intensities from all the values
+            df = df.iloc[1:, :]  # drop ReferenceIntensity row
             df.index.name = 'Patient_ID'
-
-            # drop ending of CPT retrospective samples to match cptac 
-            df = df.rename(index={'CPT0008140004':'CPT000814', 'CPT0018460005': 'CPT001846', 
-                                  '604':'CPT000814'}) # 604 mapped to CPT000814 in the proteomics file from the PDC pipeline 
+            # drop ending of CPT retrospective samples to match cptac
+            df = df.rename(index={'CPT0008140004': 'CPT000814', 'CPT0018460005': 'CPT001846',
+                                  '604': 'CPT000814'})  # 604 mapped to CPT000814 in the proteomics file from the PDC pipeline
 
             drop_cols = ['RetroIR', 'RetroIR.1',
-               'RefInt_Pool01', 'RefInt_Pool02', 'RefInt_Pool03', 'RefInt_Pool04',
-               'RefInt_Pool05', 'RefInt_Pool06', 'RefInt_Pool07', 'RefInt_Pool08',
-               'RefInt_Pool09', 'RefInt_Pool10', 'RefInt_Pool11', 'RefInt_Pool12',
-               'RefInt_Pool13', 'RefInt_Pool14', 'RefInt_Pool15', 'RefInt_Pool16',
-               'RefInt_Pool17']                
-            df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
-            
-            if self.version == "1.0":
-                self.load_mapping()
-                not_tumor = self._helper_tables["not_tumor"]
-                replicate_list = self._helper_tables["replicate_list"]
-                df = df.loc[ ~ df.index.isin(not_tumor)] # drop rows that don't correlate well with respective cptac tumor
-                df = average_replicates(df, replicate_list) # average 7 IDs with replicates
+                         'RefInt_Pool01', 'RefInt_Pool02', 'RefInt_Pool03', 'RefInt_Pool04',
+                         'RefInt_Pool05', 'RefInt_Pool06', 'RefInt_Pool07', 'RefInt_Pool08',
+                         'RefInt_Pool09', 'RefInt_Pool10', 'RefInt_Pool11', 'RefInt_Pool12',
+                         'RefInt_Pool13', 'RefInt_Pool14', 'RefInt_Pool15', 'RefInt_Pool16',
+                         'RefInt_Pool17']
+            df = df.drop(drop_cols, axis='index')  # drop quality control and ref intensity cols
+
+            self.load_mapping()
+            not_tumor = self._helper_tables["not_tumor"]
+            replicate_list = self._helper_tables["replicate_list"]
+            df = df.loc[~ df.index.isin(not_tumor)]  # drop rows that don't correlate well with respective cptac tumor
+            df = df_tools.average_replicates(df, replicate_list)  # average 7 IDs with replicates
 
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+            df = pd.read_csv(file_path, sep="\t")
 
-        
+            df_mapping = pd.read_csv(f"{CPTAC_BASE_DIR}/data/brca_mapping.csv")
+            patient_dict = dict(zip(df_mapping['Hash'], df_mapping['Patient_ID']))
 
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID', 'Site1', "Site2", "Int1", "Int2", "Site"]] = df.Index.str.split("_", expand=True)
+            df = df[df['Site'].notna()]  # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'})  # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(
+                ['Name', 'Site', 'Peptide', 'Database_ID'])  # This will create a multiindex from these columns
+            df = df.T  # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]  # Get reference intensities to use to calculate ratios
+            df = df.iloc[1:, :]  # drop ReferenceIntensity row
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            # df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: patient_dict.get(x, x))
+
+            df['Patient_ID'] = df['Patient_ID'].apply(
+                lambda x: x + '.N' if 'NX' in x else x)  # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df,
+                                                  'index')  # add ".1" to the second ocurrence of the ID with a duplicate
+            # save df in self._data
+            self.save_df(df_type, df)
 #############################################
 
-    # TODO: Readmes
+# TODO: Readmes
 #             elif file_name == "README_v3.boxnote":
 #                 self._readme_files["readme_proteomics"] = get_boxnote_text(file_path)
-                
-#             elif file_name == "README.boxnote":
-#                 self._readme_files["readme_phosphoproteomics"] = get_boxnote_text(file_path)
 
- 
+#             elif file_name == "README.boxnote":
+#                 self._readme_files["readme_phosphoproteomics"] = get_boxnote_text(file_path)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichccrcc.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichccrcc.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,85 +6,65 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+from cptac import CPTAC_BASE_DIR
 
 class UmichCcrcc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-        
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                "mapping" : "aliquot_to_patient_ID.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-                #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
-                #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            "mapping" : "aliquot_to_patient_ID.tsv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],
+            #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
+            #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
         }
         
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ccrcc", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-
+        super().__init__(cancer_type="ccrcc", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_mapping(self):
         df_type = 'mapping'
 
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
             # aliquot_to_patient_ID.tsv contains only unique aliquots (no duplicates),
             # so there is no need to slice out cancer specific aliquots
-            # This file can be found on Box under CPTAC/cptac/pancan/helper_files
             df = pd.read_csv(file_path, sep = "\t", index_col = 'aliquot_ID', usecols = ['aliquot_ID', 'patient_ID'])
             map_dict = df.to_dict()['patient_ID'] # create dictionary with aliquot_ID as keys and patient_ID as values
             self._helper_tables["map_ids"] = map_dict
 
             # drop quality control and ref intensity cols
             drop_cols = ['NCI7-1','NCI7-2','NCI7-3','NCI7-4','NCI7-5', 'QC1', 'QC2', 'QC3', 'QC4', 'QC5', 'QC6', 'QC7', 
                     'QC8', 'RefInt_pool01', 'RefInt_pool02', 'RefInt_pool03', 'RefInt_pool04', 'RefInt_pool05', 
                     'RefInt_pool06', 'RefInt_pool07', 'RefInt_pool08', 'RefInt_pool09', 'RefInt_pool10', 'RefInt_pool11', 
                     'RefInt_pool12', 'RefInt_pool13', 'RefInt_pool14', 'RefInt_pool15', 'RefInt_pool16', 'RefInt_pool17', 
                     'RefInt_pool18', 'RefInt_pool19', 'RefInt_pool20', 'RefInt_pool21', 'RefInt_pool22', 'RefInt_pool23']
             self._helper_tables["drop_cols"] = drop_cols
-            
 
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
         
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
@@ -122,15 +102,14 @@
             map_ids = self._helper_tables["map_ids"]
             df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
             df = df.rename(index = map_ids) # replace aliquot_IDs with Patient_IDs (normal samples have .N appended)
             
             # save df in self._data
             self.save_df(df_type, df)
 
-
     def load_proteomics(self):
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
@@ -151,15 +130,60 @@
             map_ids = self._helper_tables["map_ids"]
             df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
             df = df.rename(index = map_ids) # replace aliquot_IDs with Patient_IDs (normal samples have .N appended)
 
             # save df in self._data
             self.save_df(df_type, df)
 
-        
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID', "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
+
+            # save df in self._data
+            self.save_df(df_type, df)       
+
 #############################################
 
 # TODO: Readmes
 #             elif file_name == "README_v3.boxnote":
 #                 self._readme_files["readme_proteomics"] = get_boxnote_text(file_path)
                 
 #             elif file_name == "README.boxnote":
@@ -179,8 +203,8 @@
                 df = pd.read_csv(file_path, sep="\t")
                 df = df.transpose()
                 df.index.name = 'Patient_ID'
                 df.columns.name = 'Name'
                 df = average_replicates(df)
                 df = df.sort_values(by=["Patient_ID"])
                 self._data["proteomics_imputed"] = df
-            '''
+            '''
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichcoad.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichcoad.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,86 +6,59 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+from cptac import CPTAC_BASE_DIR
 
 class UmichCoad(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
-        Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        Args:
+            no_internet (bool, optional): If true, skips the index update step because it requires an internet connection.
         """
 
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0", "1.1"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                "mapping" : "CRC_Prospective sample info.xlsx",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-                #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
-                #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
-            },
-            "1.1": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                "mapping" : "CRC_Prospective sample info.xlsx",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            "mapping" : "CRC_Prospective sample info.xlsx",
         }
         
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
-        # Call the parent class __init__ function
-        super().__init__(cancer_type="coad", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="coad", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
+        """Loads mapping from 'Label' to 'Sample Code' into _helper_tables['map_ids'].
+
+        Reads the 'CRC_Prospective sample info.xlsx' file and creates a dictionary mapping
+        'Label' to 'Sample Code'. This is used in subsequent load methods to map aliquots to patient IDs.
+        """
         df_type = 'mapping'
 
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
-            # Mapping file to convert aliquots to patient_IDs for Colon
-            # This file can be found on Box under CPTAC/cptac/pancan/helper_files
             df = pd.read_excel(file_path, index_col = 'Label', usecols = ['Label', 'Sample Code'])
-            map_dict = df.to_dict()['Sample Code'] # create dictionary with aliquots as keys and patient IDs as values
+            map_dict = df.to_dict()['Sample Code'] # Create dictionary with aliquots as keys and patient IDs as values
             self._helper_tables["map_ids"] = map_dict
 
-
     def load_phosphoproteomics(self):
+        """Loads phosphoproteomics data into _data['phosphoprotemoics']
+        
+        Reads the 'Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz' file, processes it,
+        and stores the result in _data['phosphoproteomics'].
+        """
         df_type = 'phosphoproteomics'
         
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep='\t') 
@@ -123,28 +96,34 @@
                    'RefInt_ColonRef09', 'RefInt_ColonRef10', 'RefInt_ColonRef11',
                    'RefInt_ColonRef12', 'RefInt_ColonRef13', 'RefInt_ColonRef14',
                    'RefInt_ColonRef15', 'RefInt_ColonRef16', 'RefInt_ColonRef17',
                    'RefInt_ColonRef18', 'RefInt_ColonRef19', 'RefInt_ColonRef20',
                    'RefInt_ColonRef21', 'RefInt_ColonRef22-1']
             df = df.drop(drop_cols, axis='index')
             
-            if self.version == "1.1":
-                self.load_mapping()
-                mapping_dict = self._helper_tables["map_ids"]
-
-                df = df.reset_index()
-                df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquots with Patient_IDs
-                df.Patient_ID = df.Patient_ID.apply(lambda x: x[1:]+'.N' if x[0] == 'N' else x[1:]) # change normals to have .N
-                df = df.set_index('Patient_ID')
+            # if self.version == "1.1":
+            # FIXME: The following code was inside the if block. It should work fine without it.
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquots with Patient_IDs
+            df.Patient_ID = df.Patient_ID.apply(lambda x: x[1:]+'.N' if x[0] == 'N' else x[1:]) # change normals to have .N
+            df = df.set_index('Patient_ID')
+            # /FIXME
             
             # save df in self._data
             self.save_df(df_type, df)
 
-
     def load_proteomics(self):
+        """Loads proteomics data into _data['proteomics']
+        
+        Reads the 'Report_abundance_groupby=protein_protNorm=MD_gu.tsv.gz' file, processes it,
+        and stores the result in _data['proteomics'].
+        """
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep='\t')
@@ -165,26 +144,78 @@
                    'RefInt_ColonRef09', 'RefInt_ColonRef10', 'RefInt_ColonRef11',
                    'RefInt_ColonRef12', 'RefInt_ColonRef13', 'RefInt_ColonRef14',
                    'RefInt_ColonRef15', 'RefInt_ColonRef16', 'RefInt_ColonRef17',
                    'RefInt_ColonRef18', 'RefInt_ColonRef19', 'RefInt_ColonRef20',
                    'RefInt_ColonRef21', 'RefInt_ColonRef22-1']
             df = df.drop(drop_cols, axis='index')
 
-            if self.version == "1.1":
-                self.load_mapping()
-                mapping_dict = self._helper_tables["map_ids"]
-
-                df = df.reset_index()
-                df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquots with Patient_IDs
-                df.Patient_ID = df.Patient_ID.apply(lambda x: x[1:]+'.N' if x[0] == 'N' else x[1:]) # change normals to have .N
-                df = df.set_index('Patient_ID')
+            # if self.version == "1.1":
+            # FIXME: The following code was inside the if block. It should work fine without it.
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquots with Patient_IDs
+            df.Patient_ID = df.Patient_ID.apply(lambda x: x[1:]+'.N' if x[0] == 'N' else x[1:]) # change normals to have .N
+            df = df.set_index('Patient_ID')
+            # /FIXME
 
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_acetylproteomics(self):
+        """Loads acetylproteomics data into _data['acetylproteomics'].
+        
+        Reads the corresponding file, processes it,
+        and stores the result in _data['acetylproteomics'].
+        """
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID', "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
+
+            # save df in self._data
+            self.save_df(df_type, df)
 
 #############################################
 
                 
 #       TODO: Readmes
 #             elif file_name == "README_v3.boxnote":
 #                 self._readme_files["readme_proteomics"] = get_boxnote_text(file_path)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichgbm.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichgbm.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,86 +6,68 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+import cptac.tools.dataframe_tools as df_tools
+from cptac import CPTAC_BASE_DIR
 
 class UmichGbm(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+    def __init__(self, no_internet=False):
+        """Initialize the class.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
-        no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
+        no_internet (bool, optional): If True, the index update step will be skipped.
+        This can be used if there is no internet connection or if the internet connection is spotty.
+        Default is False.
         """
 
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
+        # Define the file names for each type of data.
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "mapping" : "aliquot_to_patient_ID.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],                  
-                #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
-                #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",
+            "mapping" : "aliquot_to_patient_ID.tsv.gz",
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            "acetylproteomics" : "abundance_multi-site_MD.tsv.gz",
         }
         
+        # Define the function to load each type of data.
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
+            'acetylproteomics' : self.load_acetylproteomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
+        # Initialize the parent class
+        super().__init__(cancer_type="gbm", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        # Call the parent class __init__ function
-        super().__init__(cancer_type="gbm", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-        
-        
     def load_mapping(self):
+        """Load the mapping from aliquot IDs to patient IDs."""
+
         df_type = 'mapping'
 
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
-
-            # aliquot_to_patient_ID.tsv contains only unique aliquots (no duplicates), 
-            # so there is no need to slice out cancer specific aliquots
-            # This file can be found on Box under CPTAC/cptac/pancan/helper_files
             df = pd.read_csv(file_path, sep = "\t", index_col = 'aliquot_ID', usecols = ['aliquot_ID', 'patient_ID'])
-            mapping_dict = df.to_dict()['patient_ID'] # create dictionary with aliquots as keys and patient IDs as values
+            mapping_dict = df.to_dict()['patient_ID'] # Create a dictionary mapping aliquots to patient IDs.
             self._helper_tables["map_ids"] = mapping_dict
 
-
     def load_phosphoproteomics(self):
+        """Load the phosphoproteomics data."""
+
         df_type = 'phosphoproteomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Get the file path to the data.
             file_path = self.locate_files(df_type)
-            
-            df = pd.read_csv(file_path, sep='\t')                 
+            # Load the data
+            df = pd.read_csv(file_path, sep='\t') 
+
             # Parse a few columns out of the "Index" column that we'll need for our multiindex
             df[['Database_ID','Transcript_ID',"Gene_ID","Havana_gene",
                 "Havana_transcript","Transcript","Name","Site"]] = df.Index.str.split("\\|",expand=True)
             df[['num1','start',"end","detected_phos","localized_phos","Site"]] = df.Site.str.split("_",expand=True) 
 
             # Some rows have at least one localized phosphorylation site, but also have other 
             # phosphorylations that aren't localized. We'll drop those rows, if their localized 
@@ -119,25 +101,27 @@
             self.load_mapping()
             mapping_dict = self._helper_tables["map_ids"]
             df = df.reset_index()
             df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquot_IDs with Patient_IDs
             df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'PT-' in x else x) # GTEX normals start with 'PT-' 
             df = df.set_index('Patient_ID')
 
-            # save df in self._data
+            # Save the processed data.
             self.save_df(df_type, df)
-            
 
     def load_proteomics(self):
+        """Load the proteomics data."""
+
         df_type = 'proteomics'
 
         if df_type not in self._data:
-            # perform initial checks and get file path (defined in source.py, the parent class)
+            # Get the file path to the data.
             file_path = self.locate_files(df_type)
 
+            # Load the data.
             df = pd.read_csv(file_path, sep = "\t")
             df['Database_ID'] = df.Index.apply(lambda x: x.split('|')[0]) # get protein identifier 
             df['Name'] = df.Index.apply(lambda x: x.split('|')[6]) # get protein name 
             df = df.set_index(['Name', 'Database_ID']) # set multiindex
             df = df.drop(columns = ['Index', 'MaxPepProb', 'NumberPSM', 'Gene']) # drop unnecessary  columns
             df = df.transpose()
             ref_intensities = df.loc["ReferenceIntensity"] # get reference intensities to use to calculate ratios
@@ -155,19 +139,68 @@
             self.load_mapping()
             mapping_dict = self._helper_tables["map_ids"]
             df = df.reset_index()
             df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquot_IDs with Patient_IDs
             df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'PT-' in x else x) # GTEX normals start with 'PT-'
             df = df.set_index('Patient_ID')
             
-            # save df in self._data
+            # Save the processed data.
             self.save_df(df_type, df)
 
+    def load_acetylproteomics(self):
+        """Load the acetylproteomics data."""
+
+        df_type = 'acetylproteomics'
 
+        if df_type not in self._data:
+            # Get the file path to the data.
+            file_path = self.locate_files(df_type)
+
+            # Load the data
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID','Site1',"Site2","Int1","Int2", "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            
+            df = df.T # transpose
+            df = df.drop('ProteinID', axis = 'index')
+            df = df.drop('ReferenceIntensity', axis = 'index')
+            df = df.drop('Site1', axis = 'index')
+            df = df.drop('Site2', axis = 'index')
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            if 'C3N-01825.1' in df.index:
+                df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
 
+            # Save the processed data
+            self.save_df(df_type, df)
 #############################################
 
 
 
 
 
 
@@ -194,8 +227,8 @@
                 df = pd.read_csv(file_path, sep="\t")
                 df = df.transpose()
                 df.index.name = 'Patient_ID'
                 df.columns.name = 'Name'
                 df = average_replicates(df)
                 df = df.sort_values(by=["Patient_ID"])
                 self._data["proteomics_imputed"] = df
-            '''
+            '''
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichhnscc.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichucec.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,198 +6,216 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+import cptac.tools.dataframe_tools as df_tools
+from cptac import CPTAC_BASE_DIR
 
-class UmichHnscc(Source):
 
-    def __init__(self, version="latest", no_internet=False):
+class UmichUcec(Source):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-                #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
-                #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",                    
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            "acetylproteomics" : "abundance_multi-site_MD.tsv.gz",
+            "mapping" : "aliquot_to_patient_ID.tsv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],
         }
         
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
+            'acetylproteomics' : self.load_acetylproteomics,
         }
-        
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
 
         # Call the parent class __init__ function
-        super().__init__(cancer_type="hnscc", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="ucec", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+
+    def load_mapping(self):
+        df_type = 'mapping'
+
+        if not self._helper_tables:
+            file_path = self.locate_files(df_type)
+            
+            # aliquot_to_patient_ID.tsv contains only unique aliquots (no duplicates), 
+            # so there is no need to slice out cancer specific aliquots
+            df = pd.read_csv(file_path, sep = "\t", index_col = 'aliquot_ID', usecols = ['aliquot_ID', 'patient_ID'])
+            map_dict = df.to_dict()['patient_ID'] # create dictionary with aliquot_ID as keys and patient_ID as values
+            self._helper_tables["map_ids"] = map_dict
 
-        
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-
+            
             df = pd.read_csv(file_path, sep = "\t") 
             # Parse a few columns out of the "Index" column that we'll need for our multiindex
-            df[['Database_ID','Transcript_ID',"Gene_ID","Havana_gene","Havana_transcript","Transcript","Name", "Site"]] = df.Index.str.split("\\|",expand=True)
+            df[['Database_ID','Transcript_ID',"Gene_ID","Havana_gene","Havana_transcript","Transcript","Name","Site"]] = df.Index.str.split("\\|",expand=True)
             df[['num1','start',"end","detected_phos","localized_phos","Site"]] = df.Site.str.split("_",expand=True) 
 
-            # Some rows have at least one localized phosphorylation site, but also have other
-            # phosphorylations that aren't localized. We'll drop those rows, if their localized 
-            # sites are duplicated in another row, to avoid creating duplicates, because we only 
-            # preserve information about the localized sites in a given row. However, if the localized 
-            # sites aren't duplicated in another row, we'll keep the row.
-            unlocalized_to_drop = df.index[~df["detected_phos"].eq(df["localized_phos"]) & \
-                                           df.duplicated(["Name", "Site", "Peptide", "Database_ID"], keep=False)]
-            # dectected_phos of the split "Index" column is number of phosphorylations detected, and 
-            # localized_phos is number of phosphorylations localized, so if the two values aren't equal, the 
-            # row has at least one unlocalized site
+            # Some rows have at least one localized phosphorylation site, but also have other 
+            # phosphorylations that aren't localized. We'll drop those rows, if their localized sites 
+            # are duplicated in another row, to avoid creating duplicates, because we only preserve information 
+            # about the localized sites in a given row. However, if the localized sites aren't duplicated in 
+            # another row, we'll keep the row.
+            unlocalized_to_drop = df.index[~df["detected_phos"].eq(df["localized_phos"]) & df.duplicated(["Name", "Site", "Peptide", "Database_ID"], keep=False)]# dectected_phos of the split "Index" column is number of phosphorylations detected, and localized_phos is number of phosphorylations localized, so if the two values aren't equal, the row has at least one unlocalized site
             df = df.drop(index=unlocalized_to_drop)
             df = df[df['Site'].notna()] # only keep columns with phospho site 
-            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # create a multiindex, in this order.
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
             #drop columns not needed in df 
-            df.drop(['Gene', "Index", "num1", "start", "end", "detected_phos", "localized_phos", "Havana_gene", 
+            df.drop(["Gene", "Index", "num1", "start", "end", "detected_phos", "localized_phos", "Havana_gene", 
                      "Havana_transcript", "MaxPepProb", "Gene_ID", "Transcript_ID", "Transcript"], axis=1, inplace=True)
-            df = df.T #transpose df 
+            df = df.T # transpose 
             ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios 
             df = df.subtract(ref_intensities, axis="columns") # Subtract ref intensities from all the values, to get ratios
             df = df.iloc[1:,:] # drop ReferenceIntensity row
             
-            # There were 4 labels with "-duplicate" appended in proteomics and phosphoproteomics files.
-            # I ran a pearson correlation to check how well the values from each duplicate correlated to 
-            # the other duplicates for the same case ID. Three of the duplicates correlated well with their 
-            # respective case IDs. C3L-02617-N-duplicate2 did not correlate well with the other C3L-02617 duplicates, 
-            # so we dropped it and averaged the other two. I also created a scatterplot to compare each duplicate to 
-            # the first occurence of its case ID. The linear scatterplots indicated similarity between the aliquots. 
-            # We averaged the duplicates that correlated well together and were the same tissue type.        
-            # A file containing the correlations can be downloaded at: 
-            # https://byu.box.com/shared/static/jzsq69bd079oq0zbicw4w616hyicd5ev.xlsx
-            drop_cols = ['128C', 'QC2', 'QC3', 'QC4', '129N', 'LungTumor1', 'Pooled-sample14',
-                       'LungTumor2', 'QC6', 'LungTumor3', 'Pooled-sample17', 'QC7',
-                       'Pooled-sample19', 'QC9', 'RefInt_pool01', 'RefInt_pool02',
-                       'RefInt_pool03', 'RefInt_pool04', 'RefInt_pool05', 'RefInt_pool06',
-                       'RefInt_pool07', 'RefInt_pool08', 'RefInt_pool09', 'RefInt_pool10',
-                       'RefInt_pool11', 'RefInt_pool12', 'RefInt_pool13', 'RefInt_pool14',
-                       'RefInt_pool15', 'RefInt_pool16', 'RefInt_pool17', 'RefInt_pool18',
-                       'RefInt_pool19', 'RefInt_pool20']
-            phos = df
-            phos = phos.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols        
-            phos = phos.drop(['C3L-02617-N-duplicate2'], axis = 'index') # drop duplicate that did not correlate well
-            # average IDs that correlated well to their respective duplicates
-            phos = average_replicates(phos, ['C3L-02617-T','C3L-02617-N','C3L-00994-N'], normal_identifier = '-N') 
-            phos.index = phos.index.str.replace('-T$','', regex = True)
-            phos.index = phos.index.str.replace('-N$','.N', regex = True)
-            phos.index = phos.index.str.replace('-C$','.C', regex = True) # 6 cored normal samples in Hnscc
-            df = phos
-            
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data. 
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type 
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation 
+            # to check how well the values from each duplicate correlated to its tumor flagship sample. 
+            # The first occurrence in the file had a higher correlation with the flagship sample 
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.  
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Drop quality control and ref intensity cols
+            drop_cols = ['RefInt_pool01', 'RefInt_pool02', 'RefInt_pool03', 'RefInt_pool04',
+                       'RefInt_pool05', 'RefInt_pool06', 'RefInt_pool07', 'RefInt_pool08',
+                       'RefInt_pool09', 'RefInt_pool10', 'RefInt_pool11', 'RefInt_pool12',
+                       'RefInt_pool13', 'RefInt_pool14', 'RefInt_pool15', 'RefInt_pool16',
+                       'RefInt_pool17']
+            df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
+            
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')         
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship       
+
             # save df in self._data
             self.save_df(df_type, df)
 
-
     def load_proteomics(self):
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep = "\t") 
             df['Database_ID'] = df.Index.apply(lambda x: x.split('|')[0]) # get protein identifier 
             df['Name'] = df.Index.apply(lambda x: x.split('|')[6]) # get protein name 
             df = df.set_index(['Name', 'Database_ID']) # set multiindex
             df = df.drop(columns = ['Index', 'MaxPepProb', 'NumberPSM', 'Gene']) # drop unnecessary  columns
             df = df.transpose()
             ref_intensities = df.loc["ReferenceIntensity"] # get reference intensities to use to calculate ratios 
-            df = df.subtract(ref_intensities, axis="columns") # subtract reference intensities from all the values 
+            df = df.subtract(ref_intensities, axis="columns") # subtract reference intensities from all the values
             df = df.iloc[1:,:] # drop ReferenceIntensity row 
             df.index.name = 'Patient_ID'
             
-            # There were 4 labels with "-duplicate" appended in proteomics and phosphoproteomics files.
-            # I ran a pearson correlation to check how well the values from each duplicate correlated to 
-            # the other duplicates for the same case ID. Three of the duplicates correlated well with their 
-            # respective case IDs. C3L-02617-N-duplicate2 did not correlate well with the other C3L-02617 duplicates, 
-            # so we dropped it and averaged the other two. I also created a scatterplot to compare each duplicate to 
-            # the first occurence of its case ID. The linear scatterplots indicated similarity between the aliquots. 
-            # We averaged the duplicates that correlated well together and were the same tissue type.        
-            # A file containing the correlations can be downloaded at: 
-            # https://byu.box.com/shared/static/jzsq69bd079oq0zbicw4w616hyicd5ev.xlsx
-            drop_cols = ['128C', 'QC2', 'QC3', 'QC4', '129N', 'LungTumor1', 'Pooled-sample14',
-                       'LungTumor2', 'QC6', 'LungTumor3', 'Pooled-sample17', 'QC7',
-                       'Pooled-sample19', 'QC9', 'RefInt_pool01', 'RefInt_pool02',
-                       'RefInt_pool03', 'RefInt_pool04', 'RefInt_pool05', 'RefInt_pool06',
-                       'RefInt_pool07', 'RefInt_pool08', 'RefInt_pool09', 'RefInt_pool10',
-                       'RefInt_pool11', 'RefInt_pool12', 'RefInt_pool13', 'RefInt_pool14',
-                       'RefInt_pool15', 'RefInt_pool16', 'RefInt_pool17', 'RefInt_pool18',
-                       'RefInt_pool19', 'RefInt_pool20']
-            prot = df
-            prot = prot.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols        
-            prot = prot.drop(['C3L-02617-N-duplicate2'], axis = 'index') # drop duplicate that did not correlate well  
-            # These IDs had a high correlation with their respective duplicates, so we average them
-            # duplicates: 'C3L-02617-T-duplicate', 'C3L-00994-N-duplicate', 'C3L-02617-N-duplicate'
-            prot = average_replicates(prot, ['C3L-02617-T','C3L-02617-N','C3L-00994-N'], normal_identifier = '-N') 
-            prot.index = prot.index.str.replace('-T$','', regex = True)
-            prot.index = prot.index.str.replace('-N$','.N', regex = True)
-            prot.index = prot.index.str.replace('-C$','.C', regex = True) # 6 cored normal samples in Hnscc
-            df = prot
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data. 
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type 
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation 
+            # to check how well the values from each duplicate correlated to its tumor flagship sample. 
+            # The first occurrence in the file had a higher correlation with the flagship sample 
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.  
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Drop quality control and ref intensity cols
+            drop_cols = ['RefInt_pool01', 'RefInt_pool02', 'RefInt_pool03', 'RefInt_pool04',
+                       'RefInt_pool05', 'RefInt_pool06', 'RefInt_pool07', 'RefInt_pool08',
+                       'RefInt_pool09', 'RefInt_pool10', 'RefInt_pool11', 'RefInt_pool12',
+                       'RefInt_pool13', 'RefInt_pool14', 'RefInt_pool15', 'RefInt_pool16',
+                       'RefInt_pool17']
+            df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
+            df = df.reset_index()
+            
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            
+            df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquots with patient IDs
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals 
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
             
             # save df in self._data
             self.save_df(df_type, df)
+        
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
 
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID','Site1',"Site2","Int1","Int2", "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with acetyl site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
+
+            # save df in self._data
+            self.save_df(df_type, df)
         
 #############################################
-# TODO: Readmes
+
+    # TODO the readmes
 #             elif file_name == "README_v3.boxnote":
 #                 self._readme_files["readme_proteomics"] = get_boxnote_text(file_path)
                 
 #             elif file_name == "README.boxnote":
 #                 self._readme_files["readme_phosphoproteomics"] = get_boxnote_text(file_path)
-            
-            '''
-            if file_name == "S039_BCprospective_observed_0920.tsv.gz":
-                df = pd.read_csv(file_path, sep="\t")
-                df = df.transpose()
-                df.index.name = 'Patient_ID'
-                df.columns.name = 'Name'
-                df = average_replicates(df)
-                df = df.sort_values(by=["Patient_ID"])
-                self._data["proteomics"] = df  
-                
-            if file_name == "S039_BCprospective_imputed_0920.tsv.gz":
-                df = pd.read_csv(file_path, sep="\t")
-                df = df.transpose()
-                df.index.name = 'Patient_ID'
-                df.columns.name = 'Name'
-                df = average_replicates(df)
-                df = df.sort_values(by=["Patient_ID"])
-                self._data["proteomics_imputed"] = df
-            '''
-
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichlscc.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichlscc.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,80 +5,62 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-from asyncio import CancelledError
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+import cptac.tools.dataframe_tools as df_tools
+from cptac import CPTAC_BASE_DIR
 
 class UmichLscc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "mapping" : "aliquot_to_patient_ID.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-                #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
-                #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",
+            "mapping" : "aliquot_to_patient_ID.tsv.gz",
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            "acetylproteomics" : "abundance_multi-site_MD.tsv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],
+            #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
+            #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
         }
         
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
+            'acetylproteomics' : self.load_acetylproteomics,
         }
         
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="lscc", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-
+        super().__init__(cancer_type="lscc", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_mapping(self):
         df_type = 'mapping'
 
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
             # aliquot_to_patient_ID.tsv contains only unique aliquots (no duplicates), 
             # so there is no need to slice out cancer specific aliquots
-            # This file can be found on Box under CPTAC/cptac/pancan/helper_files
             df = pd.read_csv(file_path, sep = "\t", index_col = 'aliquot_ID', usecols = ['aliquot_ID', 'patient_ID'])
             map_dict = df.to_dict()['patient_ID'] # create dictionary with aliquots as keys and patient IDs as values
             self._helper_tables["map_ids"] = map_dict
 
-
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
@@ -128,15 +110,14 @@
             mapping_dict = self._helper_tables["map_ids"]
             df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
             df = df.rename(index = mapping_dict) # replace aliquot_IDs with Patient_IDs (normal samples have .N appended)
 
             # save df in self._data
             self.save_df(df_type, df)
 
-
     def load_proteomics(self):
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
@@ -172,14 +153,61 @@
             mapping_dict = self._helper_tables["map_ids"]
             df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
             df = df.rename(index = mapping_dict) # replace aliquot_IDs with Patient_IDs (normal samples have .N appended)
             
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID','Site1',"Site2","Int1","Int2", "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            if 'C3N-01825.1' in df.index:
+                df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
+
+            # save df in self._data
+            self.save_df(df_type, df)
+
 #############################################
 
 # TODO: Add readmes
 #             elif file_name == "README_v3.boxnote":
 #                 text = get_boxnote_text(file_path)
 #                 self._readme_files["readme_proteomics"] = text
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichluad.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichluad.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,78 +5,60 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
-from asyncio import CancelledError
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+import cptac.tools.dataframe_tools as df_tools
+from cptac import CPTAC_BASE_DIR
 
 class UmichLuad(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",                    
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                "mapping" : "aliquot_to_patient_ID.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],            
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",                    
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            "acetylproteomics" : "abundance_multi-site_MD.tsv.gz",
+            "mapping" : "aliquot_to_patient_ID.tsv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],            
         }
 
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
+            'acetylproteomics' : self.load_acetylproteomics,
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="luad", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="luad", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
         df_type = 'mapping'
 
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
             # aliquot_to_patient_ID.tsv contains only unique aliquots (no duplicates), 
             # so no need to slice out cancer specific aliquots
-            # This file can be found on Box under CPTAC/cptac/pancan/helper_files
             df = pd.read_csv(file_path, sep = "\t", index_col = 'aliquot_ID', usecols = ['aliquot_ID', 'patient_ID'])
             map_dict = df.to_dict()['patient_ID'] # create dictionary with aliquot_ID as keys and patient_ID as values
             self._helper_tables["map_ids"] = map_dict
-        
-        
+
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
@@ -110,16 +92,14 @@
             # and phosphoproteomic data. I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine 
             # the tissue type for these duplicates. They were all tumor samples. Next, I ran a pearson correlation 
             # to check how well the values from each aliquot correlated to its respective tumor flagship sample. 
             # Each aliquot had a high correlation with the flagship values which indicates that they are replicates. 
             # I also created a scatterplot for each aliquot and flagship pair. The linear scatterplots indicated
             # similarity between the aliquot and flagship values. As the duplicate IDs were both tumor samples and 
             # correlated well with the flagship values, we averaged them.
-            # A file containing the correlations can be downloaded at: 
-            # https://byu.box.com/shared/static/jzsq69bd079oq0zbicw4w616hyicd5ev.xlsx
 
             # Drop quality control and ref intensity cols
             drop_cols = ['TumorOnlyIR01', 'NormalOnlyIR02', 'TumorOnlyIR03', 
                        'NormalOnlyIR04','NormalOnlyIR', 'TumorOnlyIR14',
                        'TaiwaneseIR19', 'TumorOnlyIR21', 'TaiwaneseIR22',
                        'NormalOnlyIR25', 'RefInt_pool01', 'RefInt_pool02', 'RefInt_pool03',
                        'RefInt_pool04', 'RefInt_pool05', 'RefInt_pool06', 'RefInt_pool07',
@@ -133,19 +113,18 @@
             # Get dictionary with aliquots as keys and patient IDs as values
             self.load_mapping()
             mapping_dict = self._helper_tables["map_ids"]
             df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normals have .N appended) 
             # manually map duplicates - these aliquots are in the mapping file, but they didn't map because of the appended ".1" 
             df = df.rename(index = {'CPT0146580004.1':'C3N-02379.1', 'CPT0148080004.1':'C3N-02587.1'}) 
             # these duplicates correlated well with their tumor flagship samples, so we average them
-            df = average_replicates(df, ['C3N-02379', 'C3N-02587'])
+            df = df_tools.average_replicates(df, ['C3N-02379', 'C3N-02587'])
             
             # save df in self._data
             self.save_df(df_type, df)
-            
 
     def load_proteomics(self):
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
@@ -165,16 +144,14 @@
             # and phosphoproteomic data. I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine
             # the tissue type for these duplicates. They were all tumor samples. Next, I ran a pearson correlation
             # to check how well the values from each aliquot correlated to its respective tumor flagship sample.
             # Each aliquot had a high correlation with the flagship values which indicates that they are replicates.
             # I also created a scatterplot for each aliquot and flagship pair. The linear scatterplots indicated
             # similarity between the aliquot and flagship values. As the duplicate IDs were both tumor samples and
             # correlated well with the flagship values, we averaged them.
-            # A file containing the correlations can be downloaded at:
-            # https://byu.box.com/shared/static/jzsq69bd079oq0zbicw4w616hyicd5ev.xlsx
 
             # Drop quality control and ref intensity cols
             drop_cols = ['TumorOnlyIR01', 'NormalOnlyIR02', 'TumorOnlyIR03', 
                        'NormalOnlyIR04','NormalOnlyIR', 'TumorOnlyIR14',
                        'TaiwaneseIR19', 'TumorOnlyIR21', 'TaiwaneseIR22',
                        'NormalOnlyIR25', 'RefInt_pool01', 'RefInt_pool02', 'RefInt_pool03',
                        'RefInt_pool04', 'RefInt_pool05', 'RefInt_pool06', 'RefInt_pool07',
@@ -188,15 +165,62 @@
             # Get dictionary with aliquots as keys and patient IDs as values
             self.load_mapping()
             mapping_dict = self._helper_tables["map_ids"]
             df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normals have .N appended)
             # manually map duplicates - these aliquots are in the mapping file but they didn't map because of the appended ".1"
             df = df.rename(index = {'CPT0146580004.1':'C3N-02379.1', 'CPT0148080004.1':'C3N-02587.1'})
             # these duplicates correlated well with their tumor flagship samples, so we average them
-            df = average_replicates(df, ['C3N-02379', 'C3N-02587'])
+            df = df_tools.average_replicates(df, ['C3N-02379', 'C3N-02587'])
+
+            # save df in self._data
+            self.save_df(df_type, df)
+
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID','Site1',"Site2","Int1","Int2", "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            if 'C3N-01825.1' in df.index:
+                df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
 
             # save df in self._data
             self.save_df(df_type, df)
         
 #############################################
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichov.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichov.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,87 +6,57 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+from cptac import CPTAC_BASE_DIR
 
 class UmichOv(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0", "1.1"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "mapping" : "OV_sample_TMT_annotation_UMich_GENCODE34_0315.csv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-                #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
-                #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
-            },
-            "1.1": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",                    
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv", 
-                "mapping" : "OV_sample_TMT_annotation_UMich_GENCODE34_0315.csv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",                    
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz", 
+            "mapping" : "OV_sample_TMT_annotation_UMich_GENCODE34_0315.csv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],
         }
         
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ov", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="ov", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
         df_type = 'mapping'
 
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
             # This file maps Ov aliquots to patient IDs (case ID with tissue type)
-            # It can be found on Box under CPTAC/cptac/pancan/helper_files
             ov_map = pd.read_csv(file_path, sep = ",", usecols = ['specimen', 'sample'])
             ov_map = ov_map.loc[~ ov_map['sample'].str.contains('JHU', regex = True)] # drop quality control rows
             ov_map = ov_map.set_index('specimen')
             map_dict = ov_map.to_dict()['sample'] # create dictionary with aliquots as keys and patient IDs as values
             self._helper_tables["map_ids"] = map_dict
-            
-    
+
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
@@ -110,27 +80,28 @@
             df = df.T # transpose
             df.index.name = 'Patient_ID'
             df = df.loc[df.index[~ df.index.str.contains('JHU', regex = True)]] # drop end ref intensity and quality control 
             ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios 
             df = df.subtract(ref_intensities, axis="columns")#Subtract reference intensities from all the values (get ratios)
             df = df.iloc[1:,:] # drop ReferenceIntensity row
             
-            if self.version == "1.1":
-                # Get dictionary with aliquots as keys and patient IDs as values
-                self.load_mapping()
-                mapping_dict = self._helper_tables["map_ids"]
-
-                df = df.rename(index = mapping_dict) # replace aliquot with patient IDs (normals have -N appended)         
-                df.index = df.index.str.replace('-T$','', regex = True)
-                df.index = df.index.str.replace('-N$','.N', regex = True)
+            # if self.version == "1.1":
+            # FIXME: The following code was in the if block. It should work fine without it.
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+
+            df = df.rename(index = mapping_dict) # replace aliquot with patient IDs (normals have -N appended)         
+            df.index = df.index.str.replace('-T$','', regex = True)
+            df.index = df.index.str.replace('-N$','.N', regex = True)
+            # /FIXME
             
             # save df in self._data
             self.save_df(df_type, df)
-            
-    
+
     def load_proteomics(self):
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
@@ -142,27 +113,71 @@
             df = df.transpose()                
             ref_intensities = df.loc["ReferenceIntensity"]  # get reference intensities to use to calculate ratios
             df = df.subtract(ref_intensities, axis="columns") # subtract reference intensities from all the values
             df = df.iloc[1:,:] # drop ReferenceIntensity row 
             df.index.name = 'Patient_ID'
             df = df.loc[df.index[~ df.index.str.contains('JHU', regex = True)]] # drop ref intensity and quality control
             
-            if self.version == "1.1":
-                # Get dictionary with aliquots as keys and patient IDs as values
-                self.load_mapping()
-                mapping_dict = self._helper_tables["map_ids"]
-                
-                df = df.rename(index = mapping_dict) # replace aliquot with patient IDs (normals have -N appended)       
-                df.index = df.index.str.replace('-T$','', regex = True)
-                df.index = df.index.str.replace('-N$','.N', regex = True)
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            
+            df = df.rename(index = mapping_dict) # replace aliquot with patient IDs (normals have -N appended)       
+            df.index = df.index.str.replace('-T$','', regex = True)
+            df.index = df.index.str.replace('-N$','.N', regex = True)
                         
             # save df in self._data
             self.save_df(df_type, df)
         
-        
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID', "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
+
+            # save df in self._data
+            self.save_df(df_type, df)       
+
 #############################################
 
             
     # TODO add readmes
 #             elif file_name == "README_v3.boxnote":
 #                 text = get_boxnote_text(file_path)
 #                 self._readme_files["readme_proteomics"] = text
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichpdac.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichpdac.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,76 +6,56 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+from cptac import CPTAC_BASE_DIR
 
 class UmichPdac(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                "mapping" : "aliquot_to_patient_ID.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            "mapping" : "aliquot_to_patient_ID.tsv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],
         }
         
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="pdac", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="pdac", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-        
     def load_mapping(self):
         df_type = 'mapping'
 
         if not self._helper_tables:
             file_path = self.locate_files(df_type)
             
             # aliquot_to_patient_ID.tsv contains only unique aliquots (no duplicates), 
             # so there is no need to slice out cancer specific aliquots
-            # This file can be found on Box under CPTAC/cptac/pancan/helper_files
             df = pd.read_csv(file_path, sep = "\t", index_col = 'aliquot_ID', usecols = ['aliquot_ID', 'patient_ID'])
             map_dict = df.to_dict()['patient_ID'] # create dictionary with aliquots as keys and patient IDs as values
             self._helper_tables["map_ids"] = map_dict
-            
-    
+
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
@@ -122,16 +102,15 @@
             mapping_dict = self._helper_tables["map_ids"]
 
             df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normals have .N) 
             df = df.rename(index = manually_mapped) # map 8 aliquots that were not in the mapping file
 
             # save df in self._data
             self.save_df(df_type, df)
-            
-    
+
     def load_proteomics(self):
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
@@ -160,15 +139,60 @@
 
             df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normals have .N)
             df = df.rename(index = manually_mapped) # map 8 aliquots that were not in the mapping file
 
             # save df in self._data
             self.save_df(df_type, df)
         
-        
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID', "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
+
+            # Get dictionary with aliquots as keys and patient IDs as values
+            self.load_mapping()
+            mapping_dict = self._helper_tables["map_ids"]
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
+            df = df.set_index('Patient_ID')
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
+
+            # save df in self._data
+            self.save_df(df_type, df)
+                    
 #############################################
 
 #             elif file_name == "README_v3.boxnote":
 #                 self._readme_files["readme_proteomics"] = get_boxnote_text(file_path)
                 
 #             elif file_name == "README.boxnote":
 #                 self._readme_files["readme_phosphoproteomics"] = get_boxnote_text(file_path)
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/umich/umichucec.py` & `cptac-1.5.0rc3/cptac/cancers/umich/umichhnscc.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,191 +6,222 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
-import os
-import warnings
-
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.exceptions import FailedReindexWarning, PublicationEmbargoWarning, ReindexMapError
-from cptac.utils import get_boxnote_text
-
+import cptac.tools.dataframe_tools as df_tools
+from cptac import CPTAC_BASE_DIR
 
-class UmichUcec(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+class UmichHnscc(Source):
+    def __init__(self, no_internet=False):
+        """
+        This class loads the dataset for the University of Michigan's Head and Neck Squamous Cell Carcinoma (HNSCC) study.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest datafreeze. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
 
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv",                    
-                "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv",
-                "mapping" : "aliquot_to_patient_ID.tsv",
-                # "README_v3.boxnote" is proteomics
-                # "README.boxnote" is phosphoproteomics 
-                "readme" : ["README_v3.boxnote", "README.boxnote"],
-            }
+            "proteomics" : "Report_abundance_groupby=protein_protNorm=MD_gu=2.tsv.gz",
+            "phosphoproteomics" : "Report_abundance_groupby=multi-site_protNorm=MD_gu=2.tsv.gz",
+            # "README_v3.boxnote" is proteomics
+            # "README.boxnote" is phosphoproteomics 
+            # "readme" : ["README_v3.boxnote", "README.boxnote"],
+            #"not_used": "S039_BCprospective_observed_0920.tsv.gz",
+            #"not_used": "S039_BCprospective_imputed_0920.tsv.gz"
         }
         
         self.load_functions = {
             'phosphoproteomics' : self.load_phosphoproteomics,
             'proteomics' : self.load_proteomics,
         }
-
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
+        
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ucec", source="umich", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="hnscc", source="umich", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
-    
-    def load_mapping(self):
-        df_type = 'mapping'
-
-        if not self._helper_tables:
-            file_path = self.locate_files(df_type)
-            
-            # aliquot_to_patient_ID.tsv contains only unique aliquots (no duplicates), 
-            # so there is no need to slice out cancer specific aliquots
-            # This file can be found on Box under CPTAC/cptac/pancan/helper_files
-            df = pd.read_csv(file_path, sep = "\t", index_col = 'aliquot_ID', usecols = ['aliquot_ID', 'patient_ID'])
-            map_dict = df.to_dict()['patient_ID'] # create dictionary with aliquot_ID as keys and patient_ID as values
-            self._helper_tables["map_ids"] = map_dict
-            
-    
     def load_phosphoproteomics(self):
         df_type = 'phosphoproteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
-            
+
             df = pd.read_csv(file_path, sep = "\t") 
             # Parse a few columns out of the "Index" column that we'll need for our multiindex
-            df[['Database_ID','Transcript_ID',"Gene_ID","Havana_gene","Havana_transcript","Transcript","Name","Site"]] = df.Index.str.split("\\|",expand=True)
+            df[['Database_ID','Transcript_ID',"Gene_ID","Havana_gene","Havana_transcript","Transcript","Name", "Site"]] = df.Index.str.split("\\|",expand=True)
             df[['num1','start',"end","detected_phos","localized_phos","Site"]] = df.Site.str.split("_",expand=True) 
 
-            # Some rows have at least one localized phosphorylation site, but also have other 
-            # phosphorylations that aren't localized. We'll drop those rows, if their localized sites 
-            # are duplicated in another row, to avoid creating duplicates, because we only preserve information 
-            # about the localized sites in a given row. However, if the localized sites aren't duplicated in 
-            # another row, we'll keep the row.
-            unlocalized_to_drop = df.index[~df["detected_phos"].eq(df["localized_phos"]) & df.duplicated(["Name", "Site", "Peptide", "Database_ID"], keep=False)]# dectected_phos of the split "Index" column is number of phosphorylations detected, and localized_phos is number of phosphorylations localized, so if the two values aren't equal, the row has at least one unlocalized site
+            # Some rows have at least one localized phosphorylation site, but also have other
+            # phosphorylations that aren't localized. We'll drop those rows, if their localized 
+            # sites are duplicated in another row, to avoid creating duplicates, because we only 
+            # preserve information about the localized sites in a given row. However, if the localized 
+            # sites aren't duplicated in another row, we'll keep the row.
+            unlocalized_to_drop = df.index[~df["detected_phos"].eq(df["localized_phos"]) & \
+                                           df.duplicated(["Name", "Site", "Peptide", "Database_ID"], keep=False)]
+            # dectected_phos of the split "Index" column is number of phosphorylations detected, and 
+            # localized_phos is number of phosphorylations localized, so if the two values aren't equal, the 
+            # row has at least one unlocalized site
             df = df.drop(index=unlocalized_to_drop)
             df = df[df['Site'].notna()] # only keep columns with phospho site 
-            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # create a multiindex, in this order.
             #drop columns not needed in df 
-            df.drop(["Gene", "Index", "num1", "start", "end", "detected_phos", "localized_phos", "Havana_gene", 
+            df.drop(['Gene', "Index", "num1", "start", "end", "detected_phos", "localized_phos", "Havana_gene", 
                      "Havana_transcript", "MaxPepProb", "Gene_ID", "Transcript_ID", "Transcript"], axis=1, inplace=True)
-            df = df.T # transpose 
+            df = df.T #transpose df 
             ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios 
             df = df.subtract(ref_intensities, axis="columns") # Subtract ref intensities from all the values, to get ratios
             df = df.iloc[1:,:] # drop ReferenceIntensity row
             
-            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data. 
-            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type 
-            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation 
-            # to check how well the values from each duplicate correlated to its tumor flagship sample. 
-            # The first occurrence in the file had a higher correlation with the flagship sample 
-            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.  
-            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
-            # A file containing the correlations can be downloaded at: 
-            # https://byu.box.com/shared/static/jzsq69bd079oq0zbicw4w616hyicd5ev.xlsx
-
-            # Drop quality control and ref intensity cols
-            drop_cols = ['RefInt_pool01', 'RefInt_pool02', 'RefInt_pool03', 'RefInt_pool04',
-                       'RefInt_pool05', 'RefInt_pool06', 'RefInt_pool07', 'RefInt_pool08',
-                       'RefInt_pool09', 'RefInt_pool10', 'RefInt_pool11', 'RefInt_pool12',
-                       'RefInt_pool13', 'RefInt_pool14', 'RefInt_pool15', 'RefInt_pool16',
-                       'RefInt_pool17']
-            df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
+            # There were 4 labels with "-duplicate" appended in proteomics and phosphoproteomics files.
+            # I ran a pearson correlation to check how well the values from each duplicate correlated to 
+            # the other duplicates for the same case ID. Three of the duplicates correlated well with their 
+            # respective case IDs. C3L-02617-N-duplicate2 did not correlate well with the other C3L-02617 duplicates, 
+            # so we dropped it and averaged the other two. I also created a scatterplot to compare each duplicate to 
+            # the first occurence of its case ID. The linear scatterplots indicated similarity between the aliquots. 
+            # We averaged the duplicates that correlated well together and were the same tissue type.
+            drop_cols = ['128C', 'QC2', 'QC3', 'QC4', '129N', 'LungTumor1', 'Pooled-sample14',
+                       'LungTumor2', 'QC6', 'LungTumor3', 'Pooled-sample17', 'QC7',
+                       'Pooled-sample19', 'QC9', 'RefInt_pool01', 'RefInt_pool02',
+                       'RefInt_pool03', 'RefInt_pool04', 'RefInt_pool05', 'RefInt_pool06',
+                       'RefInt_pool07', 'RefInt_pool08', 'RefInt_pool09', 'RefInt_pool10',
+                       'RefInt_pool11', 'RefInt_pool12', 'RefInt_pool13', 'RefInt_pool14',
+                       'RefInt_pool15', 'RefInt_pool16', 'RefInt_pool17', 'RefInt_pool18',
+                       'RefInt_pool19', 'RefInt_pool20']
+            phos = df
+            phos = phos.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols        
+            phos = phos.drop(['C3L-02617-N-duplicate2'], axis = 'index') # drop duplicate that did not correlate well
+            # average IDs that correlated well to their respective duplicates
+            phos = df_tools.average_replicates(phos, ['C3L-02617-T','C3L-02617-N','C3L-00994-N'], normal_identifier = '-N') 
+            phos.index = phos.index.str.replace('-T$','', regex = True)
+            phos.index = phos.index.str.replace('-N$','.N', regex = True)
+            phos.index = phos.index.str.replace('-C$','.C', regex = True) # 6 cored normal samples in Hnscc
+            df = phos
             
-            # Get dictionary with aliquots as keys and patient IDs as values
-            self.load_mapping()
-            mapping_dict = self._helper_tables["map_ids"]
-            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
-            # Add '.N' to enriched normal samples ('NX')
-            df.index.name = 'Patient_ID'
-            df = df.reset_index()
-            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
-            df = df.set_index('Patient_ID')         
-            df = rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
-            df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship       
-
             # save df in self._data
             self.save_df(df_type, df)
-            
-    
+
     def load_proteomics(self):
         df_type = 'proteomics'
 
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
             
             df = pd.read_csv(file_path, sep = "\t") 
             df['Database_ID'] = df.Index.apply(lambda x: x.split('|')[0]) # get protein identifier 
             df['Name'] = df.Index.apply(lambda x: x.split('|')[6]) # get protein name 
             df = df.set_index(['Name', 'Database_ID']) # set multiindex
             df = df.drop(columns = ['Index', 'MaxPepProb', 'NumberPSM', 'Gene']) # drop unnecessary  columns
             df = df.transpose()
             ref_intensities = df.loc["ReferenceIntensity"] # get reference intensities to use to calculate ratios 
-            df = df.subtract(ref_intensities, axis="columns") # subtract reference intensities from all the values
+            df = df.subtract(ref_intensities, axis="columns") # subtract reference intensities from all the values 
             df = df.iloc[1:,:] # drop ReferenceIntensity row 
             df.index.name = 'Patient_ID'
             
-            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data. 
-            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type 
-            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation 
-            # to check how well the values from each duplicate correlated to its tumor flagship sample. 
-            # The first occurrence in the file had a higher correlation with the flagship sample 
-            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.  
-            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
-            # A file containing the correlations can be downloaded at: 
-            # https://byu.box.com/shared/static/jzsq69bd079oq0zbicw4w616hyicd5ev.xlsx
-
-            # Drop quality control and ref intensity cols
-            drop_cols = ['RefInt_pool01', 'RefInt_pool02', 'RefInt_pool03', 'RefInt_pool04',
-                       'RefInt_pool05', 'RefInt_pool06', 'RefInt_pool07', 'RefInt_pool08',
-                       'RefInt_pool09', 'RefInt_pool10', 'RefInt_pool11', 'RefInt_pool12',
-                       'RefInt_pool13', 'RefInt_pool14', 'RefInt_pool15', 'RefInt_pool16',
-                       'RefInt_pool17']
-            df = df.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols
-            df = df.reset_index()
+            # There were 4 labels with "-duplicate" appended in proteomics and phosphoproteomics files.
+            # I ran a pearson correlation to check how well the values from each duplicate correlated to 
+            # the other duplicates for the same case ID. Three of the duplicates correlated well with their 
+            # respective case IDs. C3L-02617-N-duplicate2 did not correlate well with the other C3L-02617 duplicates, 
+            # so we dropped it and averaged the other two. I also created a scatterplot to compare each duplicate to 
+            # the first occurence of its case ID. The linear scatterplots indicated similarity between the aliquots. 
+            # We averaged the duplicates that correlated well together and were the same tissue type.
+            drop_cols = ['128C', 'QC2', 'QC3', 'QC4', '129N', 'LungTumor1', 'Pooled-sample14',
+                       'LungTumor2', 'QC6', 'LungTumor3', 'Pooled-sample17', 'QC7',
+                       'Pooled-sample19', 'QC9', 'RefInt_pool01', 'RefInt_pool02',
+                       'RefInt_pool03', 'RefInt_pool04', 'RefInt_pool05', 'RefInt_pool06',
+                       'RefInt_pool07', 'RefInt_pool08', 'RefInt_pool09', 'RefInt_pool10',
+                       'RefInt_pool11', 'RefInt_pool12', 'RefInt_pool13', 'RefInt_pool14',
+                       'RefInt_pool15', 'RefInt_pool16', 'RefInt_pool17', 'RefInt_pool18',
+                       'RefInt_pool19', 'RefInt_pool20']
+            prot = df
+            prot = prot.drop(drop_cols, axis = 'index') # drop quality control and ref intensity cols        
+            prot = prot.drop(['C3L-02617-N-duplicate2'], axis = 'index') # drop duplicate that did not correlate well  
+            # These IDs had a high correlation with their respective duplicates, so we average them
+            # duplicates: 'C3L-02617-T-duplicate', 'C3L-00994-N-duplicate', 'C3L-02617-N-duplicate'
+            prot = df_tools.average_replicates(prot, ['C3L-02617-T','C3L-02617-N','C3L-00994-N'], normal_identifier = '-N') 
+            prot.index = prot.index.str.replace('-T$','', regex = True)
+            prot.index = prot.index.str.replace('-N$','.N', regex = True)
+            prot.index = prot.index.str.replace('-C$','.C', regex = True) # 6 cored normal samples in Hnscc
+            df = prot
             
+            # save df in self._data
+            self.save_df(df_type, df)
+
+    def load_acetylproteomics(self):
+        df_type = 'acetylproteomics'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            df = pd.read_csv(file_path, sep = "\t")
+            # Parse a few columns out of the "Index" column that we'll need for our multiindex
+            df[['Database_ID', "Site"]] = df.Index.str.split("_",expand=True)
+            df = df[df['Site'].notna()] # only keep columns with phospho site
+
+            # Load the gene names and merge them with the current dataframe based on 'Database_ID'
+            df_gene_names = pd.read_csv(f"{CPTAC_BASE_DIR}/data/cptac_genes.csv")
+            df_gene_names = df_gene_names.rename(columns={'Gene_Name': 'Name'}) # Renaming 'Gene_Name' to 'Name'
+            df = pd.merge(df, df_gene_names, on='Database_ID', how='left')
+
+            # Move 'Name' into the multiindex
+            df = df.set_index(['Name', 'Site', 'Peptide', 'Database_ID']) # This will create a multiindex from these columns
+            df = df.T # transpose
+            ref_intensities = df.loc["ReferenceIntensity"]# Get reference intensities to use to calculate ratios
+            df = df.iloc[1:,:] # drop ReferenceIntensity row
+
+            # There was 1 duplicate ID (C3N-01825) in the proteomic and phosphoproteomic data.
+            # I used the Payne lab mapping file "aliquot_to_patient_ID.tsv" to determine the tissue type
+            # for these duplicates, and they were both tumor samples. Next, I ran a pearson correlation
+            # to check how well the values from each duplicate correlated to its tumor flagship sample.
+            # The first occurrence in the file had a higher correlation with the flagship sample
+            # than the second occurrence. I also created scatterplots comparing each duplicate to its flagship sample.
+            # We dropped the second occurrence of the duplicate because it didn't correlate very well to its flagship sample.
             # Get dictionary with aliquots as keys and patient IDs as values
+            
             self.load_mapping()
             mapping_dict = self._helper_tables["map_ids"]
-            
-            df['Patient_ID'] = df['Patient_ID'].replace(mapping_dict) # replace aliquots with patient IDs
-            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals 
+            df = df.rename(index = mapping_dict) # replace aliquots with patient IDs (normal samples have .N appended)
+            # Add '.N' to enriched normal samples ('NX')
+            df.index.name = 'Patient_ID'
+            df = df.reset_index()
+            df['Patient_ID'] = df['Patient_ID'].apply(lambda x: x+'.N' if 'NX' in x else x) # 'NX' are enriched normals
             df = df.set_index('Patient_ID')
-            df = rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
+            df = df_tools.rename_duplicate_labels(df, 'index') # add ".1" to the second ocurrence of the ID with a duplicate
             df = df.drop('C3N-01825.1', axis = 'index') # drop the duplicate that didn't correlate well with flagship
-            
+
             # save df in self._data
             self.save_df(df_type, df)
-        
+
         
 #############################################
-
-    # TODO the readmes
+# TODO: Readmes
 #             elif file_name == "README_v3.boxnote":
 #                 self._readme_files["readme_proteomics"] = get_boxnote_text(file_path)
                 
 #             elif file_name == "README.boxnote":
 #                 self._readme_files["readme_phosphoproteomics"] = get_boxnote_text(file_path)
+            
+            '''
+            if file_name == "S039_BCprospective_observed_0920.tsv.gz":
+                df = pd.read_csv(file_path, sep="\t")
+                df = df.transpose()
+                df.index.name = 'Patient_ID'
+                df.columns.name = 'Name'
+                df = average_replicates(df)
+                df = df.sort_values(by=["Patient_ID"])
+                self._data["proteomics"] = df  
+                
+            if file_name == "S039_BCprospective_imputed_0920.tsv.gz":
+                df = pd.read_csv(file_path, sep="\t")
+                df = df.transpose()
+                df.index.name = 'Patient_ID'
+                df.columns.name = 'Name'
+                df = average_replicates(df)
+                df = df.sort_values(by=["Patient_ID"])
+                self._data["proteomics_imputed"] = df
+            '''
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/washu/washubrca.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washucoad.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,151 +6,143 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import os
-from gtfparse import read_gtf
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.utils import get_boxnote_text
 from cptac.cancers.mssm.mssm import Mssm
 
-
-class WashuBrca(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+class WashuCoad(Source):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
-
+        
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "cibersort"         : "CIBERSORT.Output_Abs_BR.txt",
-                "CNV"               : "BR.gene_level.from_seg.filtered.tsv",
-                "mapping"           : "gencode.v22.annotation.gtf.gz",
-                "readme"            : ["README_miRNA", "README_CIBERSORT", "README_xCell", "README_somatic_mutation_WXS", "README_gene_expression", "README.boxnote", "README_ESTIMATE_WashU"],
-                "somatic_mutation"  : "BR_prospective.dnp.annotated.exonic.addrecovercases.maf.gz",
-                "transcriptomics"   : "BR_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz",
-                "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
-                "xcell"             : "BR_xCell.txt",
-                #"not_used"         : #"BR_total_miRNA_combined.tsv",  no file on box yet
-            }
+            "cibersort"         : "CIBERSORT.Output_Abs_CO.txt.gz",
+            "CNV"               : "CO.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            # "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
+            "somatic_mutation"  : "CO_prospective.dnp.annotated.exonic.addrecovercases.maf.gz",
+            "transcriptomics"   : "CO_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz",
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "CO_xCell.txt.gz",
+            #"not_used"         : #"CO_precursor_miRNA_combined.tsv.gz", # waiting for data
+            #"not_used"         : #"CO_mature_miRNA_combined.tsv.gz",                
+            #"not_used"         : #"CO_total_miRNA_combined.tsv.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
         #self._readme_files = {}
-        
+
         self.load_functions = {
             'transcriptomics'   : self.load_transcriptomics,
             'somatic_mutation'  : self.load_somatic_mutation,
             'xcell'             : self.load_xcell,
             'cibersort'         : self.load_cibersort,
             'CNV'               : self.load_CNV,
             'tumor_purity'      : self.load_tumor_purity,
             #'readme'            : self.load_readme,
+            "hla_typing": self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="brca", source="washu", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="coad", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_transcriptomics(self):
         df_type = 'transcriptomics'
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
-            # process the file and add it to self._data
             df = pd.read_csv(file_path, sep="\t")
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index(["Name", "Database_ID"])
             df = df.sort_index()
             df = df.T
             df.index.name = "Patient_ID"
             #remove label for tumor samples. All samples are tumors 
             df.index = df.index.str.replace(r"-T", "", regex=True) 
             # save df in self._data
             self.save_df(df_type, df)
-
+    
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep='\t')    
+            df = pd.read_csv(file_path, sep='\t')    
             df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
             df = df.rename(columns={
                         "Hugo_Symbol":"Gene",
                         "Gene":"Gene_Database_ID",
                         "Variant_Classification":"Mutation",
                         "HGVSp_Short":"Location"})
 
             df = df.set_index("Patient_ID")
             df = df[ ['Gene'] + ["Mutation"] + ["Location"] + [ col for col in df.columns if col not in ["Gene","Mutation","Location"] ] ]
-            df.index = df.index.str.replace(r"_T", "", regex=True)     
+            df.index = df.index.str.replace(r"_T", "", regex=True)   
+
             # save df in self._data
             self.save_df(df_type, df)
-
+    
     def load_xcell(self):
         df_type = 'xcell'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df = df.transpose()
             df.columns.name = 'Name'
             df.index.name = 'Patient_ID'
             df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
             df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
             self.save_df(df_type, df)
-
+    
     def load_cibersort(self):
         df_type = 'cibersort'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-            
+
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df.index.name = 'Patient_ID'
             df.columns.name = 'Name'
             df.index = df.index.str.replace(r'-T$', '', regex=True) 
             df.index = df.index.str.replace(r'-A$', '.N', regex=True)
             # save df in self._data
             self.save_df(df_type, df)
 
     def load_mapping(self):
         df_type = 'mapping'
         if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
             df = read_gtf(file_path)
+            df = df.as_df()
             df = df[["gene_name","gene_id"]]
             df = df.drop_duplicates()
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index("Name")
             self._helper_tables["CNV_gene_ids"] = df
 
     def load_CNV(self):
         df_type = 'CNV'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-
+            
             df = pd.read_csv(file_path, sep="\t")
             df = df.rename(columns={"Gene": "Name"})
             df = df.set_index("Name")
             cnv = df
 
             self.load_mapping()
             gene_ids = self._helper_tables["CNV_gene_ids"]
@@ -166,30 +158,51 @@
         df_type = 'tumor_purity'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
             df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
             df = df.set_index('Sample_ID') 
-            df.index.name = 'Patient_ID' 
+            df.index.name = 'Patient_ID'
 
-            # Use mssm clinical to slice out cancer specific patient_IDs in tumor_purity file
-            mssmclin = Mssm(filter_type='brca', version=self.version, no_internet=self.no_internet)
-            clinical_df = mssmclin.get_df('clinical')
+            # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
+            mssmclin = Mssm(filter_type='coad', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')             
             patient_ids = clinical_df.index.to_list()
-            df = df.loc[df.index.isin(patient_ids)]
-
+            df = df.loc[df.index.isin(patient_ids)]   
+                         
             # save df in self._data
             self.save_df(df_type, df)
-    
-    # TODO FIX
+
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
     # def load_readme(self):
     #     df_type = 'readme'
     #     if not self._readme_files: # if self._readme_files is empty
-    #         file_path_list = self.perform_initial_checks(df_type)
+    #         file_path_list = self.locate_files(df_type)
     #         # loop over list of file paths
     #         for file_path in file_path_list:
     #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
     #             file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
 
     #             if file_name == "README_miRNA":
     #                 with open(file_path, 'r') as reader:
@@ -206,14 +219,14 @@
     #             elif file_name == "README_somatic_mutation_WXS":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_somatic_mutation"] = reader.read()
                         
     #             elif file_name == "README_gene_expression":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_transcriptomics"] = reader.read()
-                
+                    
     #             elif file_name == "README.boxnote":
     #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
-                    
+
     #             elif file_name == "README_ESTIMATE_WashU":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/washu/washuccrcc.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washugbm.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,113 +6,80 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import os
-from gtfparse import read_gtf
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.utils import get_boxnote_text
+import cptac.tools.dataframe_tools as df_tools
 from cptac.cancers.mssm.mssm import Mssm
 
-
-class WashuCcrcc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+class WashuGbm(Source):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
-
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "cibersort"         : "CIBERSORT.Output_Abs_ccRCC.txt",
-                "CNV"               : "ccRCC.gene_level.from_seg.filtered.tsv",
-                "mapping"           : "gencode.v22.annotation.gtf.gz",
-                "miRNA"             : ["ccRCC_precursor_miRNA_combined.tsv", "ccRCC_mature_miRNA_combined.tsv", "ccRCC_total_miRNA_combined.tsv"],
-                "readme"            : ["README_miRNA", "README_CIBERSORT", "README_xCell", "README_somatic_mutation_WXS", "README_gene_expression", "README.boxnote", "README_ESTIMATE_WashU"],
-                "somatic_mutation"  : "ccRCC_discovery.dnp.annotated.exonic.maf.gz",
-                "transcriptomics"   : ["ccRCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz", "ccRCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
-                "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
-                "xcell"             : "ccRCC_xCell.txt",
-            }
+            "cibersort"         : "CIBERSORT.Output_Abs_GBM.txt.gz",
+            "CNV"               : "GBM.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            "miRNA"             : ["GBM_mature_miRNA_combined.tsv.gz", "GBM_precursor_miRNA_combined.tsv.gz", "GBM_total_miRNA_combined.tsv.gz"],
+            # "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"], 
+            "somatic_mutation"  : "GBM_discovery.dnp.annotated.exonic.maf.gz",
+            "transcriptomics"   : "GBM_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz",
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "GBM_xCell.txt.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
-        # self._readme_files = {}
+        #self._readme_files = {}
 
         self.load_functions = {
             'transcriptomics'   : self.load_transcriptomics,
             'somatic_mutation'  : self.load_somatic_mutation,
             'miRNA'             : self.load_miRNA,
             'xcell'             : self.load_xcell,
             'cibersort'         : self.load_cibersort,
             'CNV'               : self.load_CNV,
             'tumor_purity'      : self.load_tumor_purity,
             #'readme'            : self.load_readme,
+            "hla_typing": self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="ccrcc", source="washu", version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="gbm", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_transcriptomics(self):
         df_type = 'transcriptomics'
         if df_type not in self._data:
-            file_path_list = self.locate_files(df_type)
-            # loop over list of file paths
-            for file_path in file_path_list:
-                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
-
-                if file_name == "ccRCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
-                    df = pd.read_csv(file_path, sep="\t")
-                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
-                    df = df.set_index(["Name", "Database_ID"])
-                    df = df.sort_index()
-                    df = df.T
-                    df.index.name = "Patient_ID"
-                    df.index = df.index.str.replace(r"-T", "", regex=True) #remove label for tumor samples
-                    self._helper_tables["transcriptomics_tumor"] = df
-                    
-                if file_name == "ccRCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
-                    df = pd.read_csv(file_path, sep="\t")
-                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
-                    df = df.set_index(["Name", "Database_ID"])
-                    df = df.sort_index()
-                    df = df.T
-                    df.index.name = "Patient_ID"
-                    df.index = df.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
-                    self._helper_tables["transcriptomics_normal"] = df
-
-            # Combine the two transcriptomics dataframes
-            rna_tumor = self._helper_tables.get("transcriptomics_tumor")
-            rna_normal = self._helper_tables.get("transcriptomics_normal") # Normal entries are already marked with 'N' on the end of the ID
-            rna_combined = pd.concat([rna_tumor, rna_normal])
+            file_path = self.locate_files(df_type)
 
+            df = pd.read_csv(file_path, sep="\t")
+            df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+            df = df.set_index(["Name", "Database_ID"])
+            df = df.sort_index()
+            df = df.T
+            df.index.name = "Patient_ID"
+            #remove label for tumor samples. All samples are tumors 
+            df.index = df.index.str.replace(r"-T", "", regex=True) 
             # save df in self._data
-            self.save_df(df_type, rna_combined)
+            self.save_df(df_type, df)
 
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-
+    
             df = pd.read_csv(file_path, sep='\t')    
             df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
             df = df.rename(columns={
                         "Hugo_Symbol":"Gene",
                         "Gene":"Gene_Database_ID",
                         "Variant_Classification":"Mutation",
                         "HGVSp_Short":"Location"})
@@ -123,22 +90,23 @@
             # save df in self._data
             self.save_df(df_type, df)
 
     def load_miRNA(self):
         self.load_precursor_miRNA()
         self.load_mature_miRNA()
         self.load_total_mRNA()
-
+    
     def load_precursor_miRNA(self):
         df_type = 'precursor_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
+            df = df_tools.average_replicates(df, common = '\.\d$') # average duplicate for C3N-02788
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
@@ -185,15 +153,15 @@
             # save df in self._data
             self.save_df(df_type, all_df)
 
     def load_xcell(self):
         df_type = 'xcell'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-        
+
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df = df.transpose()
             df.columns.name = 'Name'
             df.index.name = 'Patient_ID'
             df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
             df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
@@ -214,19 +182,20 @@
 
     def load_mapping(self):
         df_type = 'mapping'
         if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
             df = read_gtf(file_path)
+            df = df.as_df()
             df = df[["gene_name","gene_id"]]
             df = df.drop_duplicates()
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index("Name")
-            self._helper_tables["CNV_gene_ids"] = df 
+            self._helper_tables["CNV_gene_ids"] = df
 
     def load_CNV(self):
         df_type = 'CNV'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep="\t")
@@ -244,29 +213,51 @@
             # save df in self._data
             self.save_df(df_type, df)
 
     def load_tumor_purity(self):
         df_type = 'tumor_purity'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-        
+
             df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
             df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
             df = df.set_index('Sample_ID') 
             df.index.name = 'Patient_ID'
 
             # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
-            mssmclin = Mssm(filter_type='ccrcc', version=self.version, no_internet=self.no_internet) #_get_version - pancandataset
-            clinical_df = mssmclin.get_df('clinical')              
-            patient_ids = clinical_df.index.to_list()
-            df = df.loc[df.index.isin(patient_ids)]     
-                       
+            mssmclin = Mssm(filter_type='gbm', no_internet=self.no_internet)
+            self._clinical_df = mssmclin.get_df('clinical')
+            patient_ids = self._clinical_df.index.to_list()
+            df = df.loc[df.index.isin(patient_ids)]
+
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
     # def load_readme(self):
     #     df_type = 'readme'
     #     if not self._readme_files:
     #         file_path_list = self.locate_files(df_type)
     #         # loop over list of file paths
     #         for file_path in file_path_list:
     #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/washu/washucoad.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washubrca.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,154 +6,140 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import os
-from gtfparse import read_gtf
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.utils import get_boxnote_text
 from cptac.cancers.mssm.mssm import Mssm
 
-
-class WashuCoad(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+class WashuBrca(Source):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
-        
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
+        # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
         self.data_files = {
-            "1.0": {
-                "cibersort"         : "CIBERSORT.Output_Abs_CO.txt",
-                "CNV"               : "CO.gene_level.from_seg.filtered.tsv",
-                "mapping"           : "gencode.v22.annotation.gtf.gz",
-                "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
-                "somatic_mutation"  : "CO_prospective.dnp.annotated.exonic.addrecovercases.maf.gz",
-                "transcriptomics"   : "CO_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz",
-                "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
-                "xcell"             : "CO_xCell.txt",
-                #"not_used"         : #"CO_precursor_miRNA_combined.tsv", # waiting for data
-                #"not_used"         : #"CO_mature_miRNA_combined.tsv",                
-                #"not_used"         : #"CO_total_miRNA_combined.tsv",
-            }
+            "cibersort"         : "CIBERSORT.Output_Abs_BR.txt.gz",
+            "CNV"               : "BR.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            # "readme"            : ["README_miRNA", "README_CIBERSORT", "README_xCell", "README_somatic_mutation_WXS", "README_gene_expression", "README.boxnote", "README_ESTIMATE_WashU"],
+            "somatic_mutation"  : "BR_prospective.dnp.annotated.exonic.addrecovercases.maf.gz",
+            "transcriptomics"   : "BR_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz",
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "BR_xCell.txt.gz",
+            #"not_used"         : #"BR_total_miRNA_combined.tsv",  no file on box yet
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
         #self._readme_files = {}
-
+        
         self.load_functions = {
             'transcriptomics'   : self.load_transcriptomics,
             'somatic_mutation'  : self.load_somatic_mutation,
             'xcell'             : self.load_xcell,
             'cibersort'         : self.load_cibersort,
             'CNV'               : self.load_CNV,
             'tumor_purity'      : self.load_tumor_purity,
             #'readme'            : self.load_readme,
+            "hla_typing": self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="coad", source='washu', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="brca", source="washu", data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_transcriptomics(self):
         df_type = 'transcriptomics'
         if df_type not in self._data:
             # perform initial checks and get file path (defined in source.py, the parent class)
             file_path = self.locate_files(df_type)
 
+            # process the file and add it to self._data
             df = pd.read_csv(file_path, sep="\t")
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index(["Name", "Database_ID"])
             df = df.sort_index()
             df = df.T
             df.index.name = "Patient_ID"
             #remove label for tumor samples. All samples are tumors 
             df.index = df.index.str.replace(r"-T", "", regex=True) 
             # save df in self._data
             self.save_df(df_type, df)
-    
+
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep='\t')    
-            df = pd.read_csv(file_path, sep='\t')    
             df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
             df = df.rename(columns={
                         "Hugo_Symbol":"Gene",
                         "Gene":"Gene_Database_ID",
                         "Variant_Classification":"Mutation",
                         "HGVSp_Short":"Location"})
 
             df = df.set_index("Patient_ID")
             df = df[ ['Gene'] + ["Mutation"] + ["Location"] + [ col for col in df.columns if col not in ["Gene","Mutation","Location"] ] ]
-            df.index = df.index.str.replace(r"_T", "", regex=True)   
-
+            df.index = df.index.str.replace(r"_T", "", regex=True)     
             # save df in self._data
             self.save_df(df_type, df)
-    
+
     def load_xcell(self):
         df_type = 'xcell'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df = df.transpose()
             df.columns.name = 'Name'
             df.index.name = 'Patient_ID'
             df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
             df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
             self.save_df(df_type, df)
-    
+
     def load_cibersort(self):
         df_type = 'cibersort'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-
+            
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df.index.name = 'Patient_ID'
             df.columns.name = 'Name'
             df.index = df.index.str.replace(r'-T$', '', regex=True) 
             df.index = df.index.str.replace(r'-A$', '.N', regex=True)
             # save df in self._data
             self.save_df(df_type, df)
 
     def load_mapping(self):
         df_type = 'mapping'
         if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
             df = read_gtf(file_path)
+            df = df.as_df()
             df = df[["gene_name","gene_id"]]
             df = df.drop_duplicates()
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index("Name")
             self._helper_tables["CNV_gene_ids"] = df
 
     def load_CNV(self):
         df_type = 'CNV'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-            
+
             df = pd.read_csv(file_path, sep="\t")
             df = df.rename(columns={"Gene": "Name"})
             df = df.set_index("Name")
             cnv = df
 
             self.load_mapping()
             gene_ids = self._helper_tables["CNV_gene_ids"]
@@ -169,29 +155,52 @@
         df_type = 'tumor_purity'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
             df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
             df = df.set_index('Sample_ID') 
-            df.index.name = 'Patient_ID'
+            df.index.name = 'Patient_ID' 
 
-            # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
-            mssmclin = Mssm(filter_type='coad', version=self.version, no_internet=self.no_internet) #_get_version - pancandataset
-            clinical_df = mssmclin.get_df('clinical')             
+            # Use mssm clinical to slice out cancer specific patient_IDs in tumor_purity file
+            mssmclin = Mssm(filter_type='brca', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')
             patient_ids = clinical_df.index.to_list()
-            df = df.loc[df.index.isin(patient_ids)]   
-                         
+            df = df.loc[df.index.isin(patient_ids)]
+
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
+    # TODO FIX
     # def load_readme(self):
     #     df_type = 'readme'
     #     if not self._readme_files: # if self._readme_files is empty
-    #         file_path_list = self.locate_files(df_type)
+    #         file_path_list = self.perform_initial_checks(df_type)
     #         # loop over list of file paths
     #         for file_path in file_path_list:
     #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
     #             file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
 
     #             if file_name == "README_miRNA":
     #                 with open(file_path, 'r') as reader:
@@ -208,14 +217,14 @@
     #             elif file_name == "README_somatic_mutation_WXS":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_somatic_mutation"] = reader.read()
                         
     #             elif file_name == "README_gene_expression":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_transcriptomics"] = reader.read()
-                    
+                
     #             elif file_name == "README.boxnote":
     #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
-
+                    
     #             elif file_name == "README_ESTIMATE_WashU":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/washu/washugbm.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washulscc.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,90 +7,109 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
 import os
-from gtfparse import read_gtf
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.utils import get_boxnote_text
 from cptac.cancers.mssm.mssm import Mssm
 
-
-class WashuGbm(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
+class WashuLscc(Source):
+    def __init__(self, no_internet=False):
+        """Load all of the washulscc dataframes as values in the self._data dict variable, with names as keys, and format them properly.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
+        
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "cibersort"         : "CIBERSORT.Output_Abs_GBM.txt",
-                "CNV"               : "GBM.gene_level.from_seg.filtered.tsv",
-                "mapping"           : "gencode.v22.annotation.gtf.gz",
-                "miRNA"             : ["GBM_mature_miRNA_combined.tsv", "GBM_precursor_miRNA_combined.tsv", "GBM_total_miRNA_combined.tsv"],
-                "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"], 
-                "somatic_mutation"  : "GBM_discovery.dnp.annotated.exonic.maf.gz",
-                "transcriptomics"   : "GBM_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz",
-                "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
-                "xcell"             : "GBM_xCell.txt",
-            }
+            "cibersort" : "CIBERSORT.Output_Abs_LSCC.txt.gz",
+            "CNV" : "LSCC.gene_level.from_seg.filtered.tsv.gz",
+            "mapping" : "gencode.v22.annotation.gtf.gz",
+            "miRNA" : ["LSCC_mature_miRNA_combined.tsv.gz","LSCC_precursor_miRNA_combined.tsv.gz","LSCC_total_miRNA_combined.tsv.gz"],
+            # "readme" : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
+            "somatic_mutation" : "LSCC_discovery.dnp.annotated.exonic.maf.gz",
+            "transcriptomics" : ["LSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz","LSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
+            "tumor_purity" : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell" : "LSCC_xCell.txt.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
         #self._readme_files = {}
 
         self.load_functions = {
             'transcriptomics'   : self.load_transcriptomics,
             'somatic_mutation'  : self.load_somatic_mutation,
             'miRNA'             : self.load_miRNA,
             'xcell'             : self.load_xcell,
             'cibersort'         : self.load_cibersort,
             'CNV'               : self.load_CNV,
             'tumor_purity'      : self.load_tumor_purity,
             #'readme'            : self.load_readme,
+            "hla_typing": self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="gbm", source='washu', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-
+        super().__init__(cancer_type="lscc", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+    
     def load_transcriptomics(self):
         df_type = 'transcriptomics'
         if df_type not in self._data:
-            file_path = self.locate_files(df_type)
+            file_path_list = self.locate_files(df_type)
+            # loop over list of file paths
+            for file_path in file_path_list:
+                path_elements = file_path.split(os.sep) # Get a list of the levels of the path
+                file_name = os.path.basename(file_path)
+
+                if file_name == "LSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df = pd.read_csv(file_path, sep="\t")
+                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+                    df = df.set_index(["Name", "Database_ID"])
+                    df = df.sort_index()
+                    df = df.T
+                    df.index.name = "Patient_ID"
+                    df.index = df.index.str.replace(r"-T", "", regex=True) #remove label for tumor samples
+                    self._helper_tables["transcriptomics_tumor"] = df
+                    
+                if file_name == "LSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df = pd.read_csv(file_path, sep="\t")
+                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
+                    df = df.set_index(["Name", "Database_ID"])
+                    df = df.sort_index()
+                    df = df.T
+                    df.index.name = "Patient_ID"
+                    df.index = df.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
+                    self._helper_tables["transcriptomics_normal"] = df
+
+            # Combine the two transcriptomics dataframes
+            rna_tumor = self._helper_tables.get("transcriptomics_tumor")
+            rna_normal = self._helper_tables.get("transcriptomics_normal") # Normal entries are already marked with 'N' on the end of the ID
+            if rna_tumor is None or rna_normal is None:
+                print("rna_tumor or rna_normal is None")
+                return
+            if not isinstance(rna_tumor, pd.DataFrame) or not isinstance(rna_normal, pd.DataFrame):
+                print("rna_tumor or rna_normal is not a DataFrame")
+                return
+       
+            rna_combined = pd.concat([rna_tumor, rna_normal])
 
-            df = pd.read_csv(file_path, sep="\t")
-            df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
-            df = df.set_index(["Name", "Database_ID"])
-            df = df.sort_index()
-            df = df.T
-            df.index.name = "Patient_ID"
-            #remove label for tumor samples. All samples are tumors 
-            df.index = df.index.str.replace(r"-T", "", regex=True) 
             # save df in self._data
-            self.save_df(df_type, df)
-
+            self.save_df(df_type, rna_combined)
+            
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-    
+
+            # Rename the columns we want to keep to the appropriate names
             df = pd.read_csv(file_path, sep='\t')    
             df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
             df = df.rename(columns={
                         "Hugo_Symbol":"Gene",
                         "Gene":"Gene_Database_ID",
                         "Variant_Classification":"Mutation",
                         "HGVSp_Short":"Location"})
@@ -101,23 +120,22 @@
             # save df in self._data
             self.save_df(df_type, df)
 
     def load_miRNA(self):
         self.load_precursor_miRNA()
         self.load_mature_miRNA()
         self.load_total_mRNA()
-    
+
     def load_precursor_miRNA(self):
         df_type = 'precursor_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
-            df = average_replicates(df, common = '\.\d$') # average duplicate for C3N-02788
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
@@ -126,15 +144,15 @@
             # save df in self._data
             self.save_df(df_type, all_df)
 
     def load_mature_miRNA(self):
         df_type = 'mature_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-            
+     
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias', 'Derives_from'])
             df = df.transpose()
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
@@ -173,15 +191,15 @@
             df = df.transpose()
             df.columns.name = 'Name'
             df.index.name = 'Patient_ID'
             df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
             df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
             self.save_df(df_type, df)
-
+    
     def load_cibersort(self):
         df_type = 'cibersort'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df.index.name = 'Patient_ID'
@@ -193,14 +211,15 @@
 
     def load_mapping(self):
         df_type = 'mapping'
         if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
             df = read_gtf(file_path)
+            df = df.as_df()
             df = df[["gene_name","gene_id"]]
             df = df.drop_duplicates()
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index("Name")
             self._helper_tables["CNV_gene_ids"] = df
 
     def load_CNV(self):
@@ -218,62 +237,84 @@
             df = cnv.join(gene_ids,how = "left") #merge in gene_ids 
             df = df.reset_index()
             df = df.set_index(["Name", "Database_ID"]) #create multi-index
             df = df.T
             df.index.name = 'Patient_ID'
             # save df in self._data
             self.save_df(df_type, df)
-
+    
     def load_tumor_purity(self):
         df_type = 'tumor_purity'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
             df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
             df = df.set_index('Sample_ID') 
             df.index.name = 'Patient_ID'
 
             # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
-            mssmclin = Mssm(filter_type='gbm', version=self.version, no_internet=self.no_internet) #_get_version - pancandataset
-            self._clinical_df = mssmclin.get_df('clinical')
-            patient_ids = self._clinical_df.index.to_list()
+            mssmclin = Mssm(filter_type='lscc', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')       
+            patient_ids = clinical_df.index.to_list()
             df = df.loc[df.index.isin(patient_ids)]
 
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
     # def load_readme(self):
     #     df_type = 'readme'
     #     if not self._readme_files:
     #         file_path_list = self.locate_files(df_type)
     #         # loop over list of file paths
     #         for file_path in file_path_list:
     #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
     #             file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
 
-    #             if file_name == "README_miRNA":
-    #                 with open(file_path, 'r') as reader:
-    #                     self._readme_files["readme_miRNA"] = reader.read()
-                        
-    #             elif file_name == "README_CIBERSORT":
-    #                 with open(file_path, 'r') as reader:
-    #                     self._readme_files["readme_cibersort"] = reader.read()
-                        
-    #             elif file_name == "README_xCell":
-    #                 with open(file_path, 'r') as reader:
-    #                     self._readme_files["readme_xcell"] = reader.read()
-                
-    #             elif file_name == "README_somatic_mutation_WXS" in file_path:
-    #                 with open(file_path, 'r') as reader:
-    #                     self._readme_files["readme_somatic_mutation"] = reader.read()
-                        
-    #             elif file_name == "README_gene_expression":
-    #                 with open(file_path, 'r') as reader:
-    #                     self._readme_files["readme_transcriptomics"] = reader.read()
+    #         if file_name == "README_miRNA":
+    #             with open(file_path, 'r') as reader:
+    #                 self._readme_files["readme_miRNA"] = reader.read()
+                    
+    #         elif file_name == "README_CIBERSORT":
+    #             with open(file_path, 'r') as reader:
+    #                 self._readme_files["readme_cibersort"] = reader.read()
+                    
+    #         elif file_name == "README_xCell":
+    #             with open(file_path, 'r') as reader:
+    #                 self._readme_files["readme_xcell"] = reader.read()
+            
+    #         elif file_name == "README_somatic_mutation_WXS":
+    #             with open(file_path, 'r') as reader:
+    #                 self._readme_files["readme_somatic_mutation"] = reader.read()
+                    
+    #         elif file_name == "README_gene_expression":
+    #             with open(file_path, 'r') as reader:
+    #                 self._readme_files["readme_transcriptomics"] = reader.read()
+               
+    #         elif file_name == "README.boxnote":
+    #             self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
                 
-    #             elif file_name == "README.boxnote":
-    #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
-
-    #             elif file_name == "README_ESTIMATE_WashU":
-    #                 with open(file_path, 'r') as reader:
-    #                     self._readme_files["readme_tumor_purity"] = reader.read()
+    #         elif file_name == "README_ESTIMATE_WashU":
+    #             with open(file_path, 'r') as reader:
+    #                 self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/washu/washuhnscc.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washupdac.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,108 +7,106 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
 import os
-from gtfparse import read_gtf
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.utils import get_boxnote_text
+import cptac.tools.dataframe_tools as df_tools
 from cptac.cancers.mssm.mssm import Mssm
 
-
-class WashuHnscc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
+class WashuPdac(Source):
+    def __init__(self, no_internet=False):
         """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
         
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "cibersort"         : "CIBERSORT.Output_Abs_HNSCC.txt",
-                "CNV"               : "HNSCC.gene_level.from_seg.filtered.tsv",
-                "mapping"           : "gencode.v22.annotation.gtf.gz",
-                "miRNA"             : ["HNSCC_mature_miRNA_combined.tsv","HNSCC_precursor_miRNA_combined.tsv","HNSCC_total_miRNA_combined.tsv"],
-                "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
-                "somatic_mutation"  : "HNSCC_discovery.dnp.annotated.exonic.maf.gz",
-                "transcriptomics"   : ["HNSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz","HNSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
-                "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
-                "xcell"             : "HNSCC_xCell.txt",
-            }
+            "cibersort"         : "CIBERSORT.Output_Abs_PDA.txt.gz",
+            "CNV"               : "PDA.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            "miRNA"             : ["PDA_mature_miRNA_combined.tsv.gz","PDA_precursor_miRNA_combined.tsv.gz","PDA_total_miRNA_combined.tsv.gz"],
+            # "readme"            : ["README_miRNA","README_CIBERSORT", "README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
+            "somatic_mutation"  : "PDA_discovery.dnp.annotated.exonic.maf.gz",
+            "transcriptomics"   : ["PDA_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz","PDA_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "PDA_xCell.txt.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
         #self._readme_files = {}
 
         self.load_functions = {
             'transcriptomics'   : self.load_transcriptomics,
             'somatic_mutation'  : self.load_somatic_mutation,
             'miRNA'             : self.load_miRNA,
             'xcell'             : self.load_xcell,
             'cibersort'         : self.load_cibersort,
             'CNV'               : self.load_CNV,
             'tumor_purity'      : self.load_tumor_purity,
             #'readme'            : self.load_readme,
+            'hla_typing'          : self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="hnscc", source='washu', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="pdac", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_transcriptomics(self):
         df_type = 'transcriptomics'
         if df_type not in self._data:
             file_path_list = self.locate_files(df_type)
             # loop over list of file paths
             for file_path in file_path_list:
                 path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
-
-                if file_name == "HNSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                file_name = os.path.basename(file_path)
+                    
+                if file_name == "PDA_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
                     df = pd.read_csv(file_path, sep='\t')
                     #change names to universal package names
                     df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
                     df = df.set_index(["Name", "Database_ID"])
                     df = df.sort_index()
                     df = df.T #transpose 
                     df.index.name = "Patient_ID"
                     df.index = df.index.str.replace(r"-T", "", regex=True) #remove label for tumor samples
                     self._helper_tables["transcriptomics_tumor"] = df
 
-                if file_name == "HNSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                if file_name == "PDA_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
                     df_norm = pd.read_csv(file_path, sep='\t')
                     #change names to universal package names
                     df_norm = df_norm.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})  
                     df_norm = df_norm.set_index(["Name", "Database_ID"])
                     df_norm = df_norm.sort_index()
                     df_norm = df_norm.T #transpose
                     df_norm.index.name = "Patient_ID"
                     df_norm.index = df_norm.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
                     self._helper_tables["transcriptomics_normal"] = df_norm
 
-            # combine and create transcriptomic dataframe            
+            # Combine the two transcriptomics dataframes
             rna_tumor = self._helper_tables.get("transcriptomics_tumor")
             rna_normal = self._helper_tables.get("transcriptomics_normal") # Normal entries are already marked with 'N' on the end of the ID
+            if rna_tumor is None or rna_normal is None:
+                print("rna_tumor or rna_normal is None")
+                return
+            if not isinstance(rna_tumor, pd.DataFrame) or not isinstance(rna_normal, pd.DataFrame):
+                print("rna_tumor or rna_normal is not a DataFrame")
+                return
+       
             rna_combined = pd.concat([rna_tumor, rna_normal])
+
             # save df in self._data
             self.save_df(df_type, rna_combined)
-    
+
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep='\t')    
             # Rename the columns we want to keep to the appropriate names
@@ -134,15 +132,15 @@
     def load_precursor_miRNA(self):
         df_type = 'precursor_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
-            df = average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
+            df = df_tools.average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
@@ -151,38 +149,38 @@
             # save df in self._data
             self.save_df(df_type, all_df)
 
     def load_mature_miRNA(self):
         df_type = 'mature_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-
+            
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias', 'Derives_from'])
             df = df.transpose()
-            df = average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
+            df = df_tools.average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
             tumor = tumor.sort_values(by=["Patient_ID"])
             all_df = pd.concat([tumor, normal])
             # save df in self._data
             self.save_df(df_type, all_df)
-
+    
     def load_total_mRNA(self):
         df_type = 'total_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-             
+            
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
-            df = average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
+            df = df_tools.average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
@@ -191,15 +189,15 @@
             # save df in self._data
             self.save_df(df_type, all_df)
 
     def load_xcell(self):
         df_type = 'xcell'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-
+        
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df = df.transpose()
             df.columns.name = 'Name'
             df.index.name = 'Patient_ID'
             df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
             df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
@@ -220,14 +218,15 @@
 
     def load_mapping(self):
         df_type = 'mapping'
         if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
             df = read_gtf(file_path)
+            df = df.as_df()
             df = df[["gene_name","gene_id"]]
             df = df.drop_duplicates()
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index("Name")
             self._helper_tables["CNV_gene_ids"] = df
 
     def load_CNV(self):
@@ -257,22 +256,45 @@
         
             df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
             df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
             df = df.set_index('Sample_ID') 
             df.index.name = 'Patient_ID'
 
             # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
-            mssmclin = Mssm(filter_type='hnscc', version=self.version, no_internet=self.no_internet) #_get_version - pancandataset
-            clinical_df = mssmclin.get_df('clinical')                
+            mssmclin = Mssm(filter_type='pdac', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')              
             patient_ids = clinical_df.index.to_list()
             df = df.loc[df.index.isin(patient_ids)]
 
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
+
     # def load_readme(self):
     #     df_type = 'readme'
     #     if not self._readme_files:
     #         file_path_list = self.locate_files(df_type)
     #         # loop over list of file paths
     #         for file_path in file_path_list:
     #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/washu/washulscc.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washuucec.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,296 +5,312 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+# Import necessary libraries
 import pandas as pd
 import os
-from gtfparse import read_gtf
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.utils import get_boxnote_text
+import cptac.tools.dataframe_tools as df_tools
 from cptac.cancers.mssm.mssm import Mssm
 
-
-class WashuLscc(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Load all of the washulscc dataframes as values in the self._data dict variable, with names as keys, and format them properly.
+class WashuUcec(Source):
+    def __init__(self, no_internet=False):
+        """Load all of the WashuUcec dataframes as values in the self._data dict variable, with names as keys, and format them properly.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
-        
-        # Set some needed variables, and pass them to the parent Dataset class __init__ function
-
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
 
+        # Define the file names and load functions to be used
         self.data_files = {
-            "1.0": {                
-                "cibersort" : "CIBERSORT.Output_Abs_LSCC.txt",
-                "CNV" : "LSCC.gene_level.from_seg.filtered.tsv",
-                "mapping" : "gencode.v22.annotation.gtf.gz",
-                "miRNA" : ["LSCC_mature_miRNA_combined.tsv","LSCC_precursor_miRNA_combined.tsv","LSCC_total_miRNA_combined.tsv"],
-                "readme" : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
-                "somatic_mutation" : "LSCC_discovery.dnp.annotated.exonic.maf.gz",
-                "transcriptomics" : ["LSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz","LSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
-                "tumor_purity" : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
-                "xcell" : "LSCC_xCell.txt",
-            }
+            "cibersort"         : "CIBERSORT.Output_Abs_EC.txt.gz",
+            "CNV"               : "UCEC.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            "miRNA"             : ["EC_precursor_miRNA_combined.tsv.gz","EC_mature_miRNA_combined.tsv.gz","EC_total_miRNA_combined.tsv.gz"],
+            # "readme"          : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
+            "somatic_mutation"  : "EC_discovery.dnp.annotated.exonic.maf.gz",
+            "transcriptomics"   : ["EC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz","EC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "EC_xCell.txt.gz",
+            "hla_typing"        : "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
         #self._readme_files = {}
 
         self.load_functions = {
             'transcriptomics'   : self.load_transcriptomics,
             'somatic_mutation'  : self.load_somatic_mutation,
             'miRNA'             : self.load_miRNA,
             'xcell'             : self.load_xcell,
             'cibersort'         : self.load_cibersort,
             'CNV'               : self.load_CNV,
             'tumor_purity'      : self.load_tumor_purity,
-            #'readme'            : self.load_readme,
+            #'readme'           : self.load_readme,
+            "hla_typing"        : self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="lscc", source='washu', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
-    
+        super().__init__(cancer_type="ucec", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+
+    # Follows are loading methods for each dataframe
+    # Load Transcriptomics dataframe
     def load_transcriptomics(self):
         df_type = 'transcriptomics'
         if df_type not in self._data:
             file_path_list = self.locate_files(df_type)
             # loop over list of file paths
             for file_path in file_path_list:
                 path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+                file_name = os.path.basename(file_path)
 
-                if file_name == "LSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                if file_name == "EC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
                     df = pd.read_csv(file_path, sep="\t")
                     df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
                     df = df.set_index(["Name", "Database_ID"])
                     df = df.sort_index()
                     df = df.T
                     df.index.name = "Patient_ID"
                     df.index = df.index.str.replace(r"-T", "", regex=True) #remove label for tumor samples
                     self._helper_tables["transcriptomics_tumor"] = df
-                    
-                if file_name == "LSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                
+                if file_name == "EC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
                     df = pd.read_csv(file_path, sep="\t")
                     df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
                     df = df.set_index(["Name", "Database_ID"])
                     df = df.sort_index()
                     df = df.T
                     df.index.name = "Patient_ID"
                     df.index = df.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
                     self._helper_tables["transcriptomics_normal"] = df
 
-            # combine and create transcriptomic dataframe            
+            # Combine the two transcriptomics dataframes
             rna_tumor = self._helper_tables.get("transcriptomics_tumor")
             rna_normal = self._helper_tables.get("transcriptomics_normal") # Normal entries are already marked with 'N' on the end of the ID
+            if rna_tumor is None or rna_normal is None:
+                print("rna_tumor or rna_normal is None")
+                return
+            if not isinstance(rna_tumor, pd.DataFrame) or not isinstance(rna_normal, pd.DataFrame):
+                print("rna_tumor or rna_normal is not a DataFrame")
+                return
+       
             rna_combined = pd.concat([rna_tumor, rna_normal])
+
             # save df in self._data
             self.save_df(df_type, rna_combined)
 
+    # Load Somatic Mutation dataframe
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
-            # Rename the columns we want to keep to the appropriate names
-            df = pd.read_csv(file_path, sep='\t')    
+            df = pd.read_csv(file_path, sep='\t', dtype={"PUBMED": "O"})    
             df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
             df = df.rename(columns={
                         "Hugo_Symbol":"Gene",
                         "Gene":"Gene_Database_ID",
                         "Variant_Classification":"Mutation",
                         "HGVSp_Short":"Location"})
 
             df = df.set_index("Patient_ID")
             df = df[ ['Gene'] + ["Mutation"] + ["Location"] + [ col for col in df.columns if col not in ["Gene","Mutation","Location"] ] ]
             df.index = df.index.str.replace(r"_T", "", regex=True)     
             # save df in self._data
             self.save_df(df_type, df)
 
+    # Load miRNA dataframe
     def load_miRNA(self):
         self.load_precursor_miRNA()
         self.load_mature_miRNA()
         self.load_total_mRNA()
 
     def load_precursor_miRNA(self):
         df_type = 'precursor_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
+            df = df_tools.average_replicates(df, common = '\.\d$') # average replicates for C3N-00326
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
-            # Sort
-            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
-            normal = normal.sort_values(by=["Patient_ID"])
-            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
-            tumor = tumor.sort_values(by=["Patient_ID"])
-            all_df = pd.concat([tumor, normal])
             # save df in self._data
-            self.save_df(df_type, all_df)
+            self.save_df(df_type, df)
 
     def load_mature_miRNA(self):
         df_type = 'mature_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-     
+
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias', 'Derives_from'])
             df = df.transpose()
+            df = df_tools.average_replicates(df, common = '\.\d$') # average replicates for C3N-00326
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
-            # Sort
-            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
-            normal = normal.sort_values(by=["Patient_ID"])
-            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
-            tumor = tumor.sort_values(by=["Patient_ID"])
-            all_df = pd.concat([tumor, normal])
             # save df in self._data
-            self.save_df(df_type, all_df)
+            self.save_df(df_type, df)
 
     def load_total_mRNA(self):
         df_type = 'total_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-            
+
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
+            df = df_tools.average_replicates(df, common = '\.\d$') # average replicates for C3N-00326
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
-            # Sort
-            normal = df.loc[df.index.str.contains('\.N$', regex =True)]
-            normal = normal.sort_values(by=["Patient_ID"])
-            tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
-            tumor = tumor.sort_values(by=["Patient_ID"])
-            all_df = pd.concat([tumor, normal])
             # save df in self._data
-            self.save_df(df_type, all_df)
+            self.save_df(df_type, df)
 
+    # Load xCell dataframe
     def load_xcell(self):
         df_type = 'xcell'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df = df.transpose()
             df.columns.name = 'Name'
             df.index.name = 'Patient_ID'
             df.index = df.index.str.replace(r'-T$', '', regex=True) # remove label for tumor samples
             df.index = df.index.str.replace(r'-A$', '.N', regex=True) # change label for normal samples
             # save df in self._data
             self.save_df(df_type, df)
-    
+
+    # Load CIBERSORT dataframe
     def load_cibersort(self):
         df_type = 'cibersort'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep = '\t', index_col = 0) 
             df.index.name = 'Patient_ID'
             df.columns.name = 'Name'
             df.index = df.index.str.replace(r'-T$', '', regex=True) 
             df.index = df.index.str.replace(r'-A$', '.N', regex=True)
             # save df in self._data
             self.save_df(df_type, df)
 
+    # Load Mapping dataframe
     def load_mapping(self):
         df_type = 'mapping'
         if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
             df = read_gtf(file_path)
+            df = df.as_df()
             df = df[["gene_name","gene_id"]]
             df = df.drop_duplicates()
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index("Name")
             self._helper_tables["CNV_gene_ids"] = df
 
+    # Load CNV dataframe
     def load_CNV(self):
         df_type = 'CNV'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep="\t")
             df = df.rename(columns={"Gene": "Name"})
             df = df.set_index("Name")
-            cnv = df
+            cnv= df
 
             self.load_mapping()
             gene_ids = self._helper_tables["CNV_gene_ids"]
             df = cnv.join(gene_ids,how = "left") #merge in gene_ids 
             df = df.reset_index()
             df = df.set_index(["Name", "Database_ID"]) #create multi-index
             df = df.T
             df.index.name = 'Patient_ID'
             # save df in self._data
             self.save_df(df_type, df)
-    
+
+    # Load Tumor Purity dataframe
     def load_tumor_purity(self):
         df_type = 'tumor_purity'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-
+ 
             df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
             df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
             df = df.set_index('Sample_ID') 
             df.index.name = 'Patient_ID'
 
             # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
-            mssmclin = Mssm(filter_type='lscc', version=self.version, no_internet=self.no_internet) #_get_version - pancandataset
-            clinical_df = mssmclin.get_df('clinical')       
+            mssmclin = Mssm(filter_type='ucec', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')               
             patient_ids = clinical_df.index.to_list()
             df = df.loc[df.index.isin(patient_ids)]
 
             # save df in self._data
             self.save_df(df_type, df)
 
+    # Load HLA Typing dataframe
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
+
     # def load_readme(self):
     #     df_type = 'readme'
     #     if not self._readme_files:
     #         file_path_list = self.locate_files(df_type)
     #         # loop over list of file paths
     #         for file_path in file_path_list:
     #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
     #             file_name = path_elements[-1]# The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
 
-    #         if file_name == "README_miRNA":
-    #             with open(file_path, 'r') as reader:
-    #                 self._readme_files["readme_miRNA"] = reader.read()
-                    
-    #         elif file_name == "README_CIBERSORT":
-    #             with open(file_path, 'r') as reader:
-    #                 self._readme_files["readme_cibersort"] = reader.read()
-                    
-    #         elif file_name == "README_xCell":
-    #             with open(file_path, 'r') as reader:
-    #                 self._readme_files["readme_xcell"] = reader.read()
-            
-    #         elif file_name == "README_somatic_mutation_WXS":
-    #             with open(file_path, 'r') as reader:
-    #                 self._readme_files["readme_somatic_mutation"] = reader.read()
-                    
-    #         elif file_name == "README_gene_expression":
-    #             with open(file_path, 'r') as reader:
-    #                 self._readme_files["readme_transcriptomics"] = reader.read()
-               
-    #         elif file_name == "README.boxnote":
-    #             self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
+    #             if file_name == "README_miRNA":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_miRNA"] = reader.read()
+                        
+    #             elif file_name == "README_CIBERSORT":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_cibersort"] = reader.read()
+                        
+    #             elif file_name == "README_xCell":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_xcell"] = reader.read()
+                
+    #             elif file_name == "README_somatic_mutation_WXS":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_somatic_mutation"] = reader.read()
+                        
+    #             elif file_name == "README_gene_expression":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_transcriptomics"] = reader.read()
+                
+    #             elif file_name == "README.boxnote":
+    #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
                 
-    #         elif file_name == "README_ESTIMATE_WashU":
-    #             with open(file_path, 'r') as reader:
-    #                 self._readme_files["readme_tumor_purity"] = reader.read()
+    #             elif file_name == "README_ESTIMATE_WashU":
+    #                 with open(file_path, 'r') as reader:
+    #                     self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/cancers/washu/washuluad.py` & `cptac-1.5.0rc3/cptac/cancers/washu/washuhnscc.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,113 +7,114 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
 import os
-from gtfparse import read_gtf
+from pyranges import read_gtf
 
 from cptac.cancers.source import Source
-from cptac.tools.dataframe_tools import *
-from cptac.utils import get_boxnote_text
+import cptac.tools.dataframe_tools as df_tools
 from cptac.cancers.mssm.mssm import Mssm
 
-
-class WashuLuad(Source):
-
-    def __init__(self, version="latest", no_internet=False):
-        """Load all of the washuluad dataframes as values in the self._data dict variable, with names as keys, and format them properly.
+class WashuHnscc(Source):
+    def __init__(self, no_internet=False):
+        """Define which dataframes as are available in the self.load_functions dictionary variable, with names as keys.
 
         Parameters:
-        version (str, optional): The version number to load, or the string "latest" to just load the latest building. Default is "latest".
         no_internet (bool, optional): Whether to skip the index update step because it requires an internet connection. This will be skipped automatically if there is no internet at all, but you may want to manually skip it if you have a spotty internet connection. Default is False.
         """
-
+        
         # Set some needed variables, and pass them to the parent Dataset class __init__ function
 
-        # This keeps a record of all versions that the code is equipped to handle. That way, if there's a new data release but they didn't update their package, it won't try to parse the new data version it isn't equipped to handle.
-        self.valid_versions = ["1.0"]
-
         self.data_files = {
-            "1.0": {
-                "cibersort"         : "CIBERSORT.Output_Abs_LUAD.txt",
-                "CNV"               : "LUAD.gene_level.from_seg.filtered.tsv",
-                "mapping"           : "gencode.v22.annotation.gtf.gz",
-                "miRNA"             : ["LUAD_mature_miRNA_combined.tsv","LUAD_precursor_miRNA_combined.tsv","LUAD_total_miRNA_combined.tsv"],
-                "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
-                "somatic_mutation"  : "LUAD_discovery.dnp.annotated.exonic.maf.gz",
-                "transcriptomics"   : ["LUAD_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz", "LUAD_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
-                "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
-                "xcell"             : "LUAD_xCell.txt",
-            }
+            "cibersort"         : "CIBERSORT.Output_Abs_HNSCC.txt.gz",
+            "CNV"               : "HNSCC.gene_level.from_seg.filtered.tsv.gz",
+            "mapping"           : "gencode.v22.annotation.gtf.gz",
+            "miRNA"             : ["HNSCC_mature_miRNA_combined.tsv.gz","HNSCC_precursor_miRNA_combined.tsv.gz","HNSCC_total_miRNA_combined.tsv.gz"],
+            # "readme"            : ["README_miRNA","README_CIBERSORT","README_xCell","README_somatic_mutation_WXS","README_gene_expression","README.boxnote","README_ESTIMATE_WashU"],
+            "somatic_mutation"  : "HNSCC_discovery.dnp.annotated.exonic.maf.gz",
+            "transcriptomics"   : ["HNSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz","HNSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz"],
+            "tumor_purity"      : "CPTAC_pancan_RNA_tumor_purity_ESTIMATE_WashU.tsv.gz",
+            "xcell"             : "HNSCC_xCell.txt.gz",
+            "hla_typing": "hla.sample.ct.10152021.sort.tsv.gz"
         }
 
         #self._readme_files = {}
 
         self.load_functions = {
             'transcriptomics'   : self.load_transcriptomics,
             'somatic_mutation'  : self.load_somatic_mutation,
             'miRNA'             : self.load_miRNA,
             'xcell'             : self.load_xcell,
             'cibersort'         : self.load_cibersort,
             'CNV'               : self.load_CNV,
             'tumor_purity'      : self.load_tumor_purity,
             #'readme'            : self.load_readme,
+            "hla_typing": self.load_hla_typing
         }
 
-        if version == "latest":
-            version = sorted(self.valid_versions)[-1]
-
         # Call the parent class __init__ function
-        super().__init__(cancer_type="luad", source='washu', version=version, valid_versions=self.valid_versions, data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
+        super().__init__(cancer_type="hnscc", source='washu', data_files=self.data_files, load_functions=self.load_functions, no_internet=no_internet)
 
     def load_transcriptomics(self):
         df_type = 'transcriptomics'
         if df_type not in self._data:
             file_path_list = self.locate_files(df_type)
             # loop over list of file paths
             for file_path in file_path_list:
                 path_elements = file_path.split(os.sep) # Get a list of the levels of the path
-                file_name = path_elements[-1] # The last element will be the name of the file. We'll use this to identify files for parsing in the if/elif statements below
+                file_name = os.path.basename(file_path)
 
-                if file_name == "LUAD_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
-                    df = pd.read_csv(file_path, sep="\t")
+                if file_name == "HNSCC_tumor_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df = pd.read_csv(file_path, sep='\t')
+                    #change names to universal package names
                     df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
                     df = df.set_index(["Name", "Database_ID"])
                     df = df.sort_index()
-                    df = df.T
+                    df = df.T #transpose 
                     df.index.name = "Patient_ID"
                     df.index = df.index.str.replace(r"-T", "", regex=True) #remove label for tumor samples
                     self._helper_tables["transcriptomics_tumor"] = df
-                    
-                if file_name == "LUAD_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
-                    df = pd.read_csv(file_path, sep="\t")
-                    df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
-                    df = df.set_index(["Name", "Database_ID"])
-                    df = df.sort_index()
-                    df = df.T
-                    df.index.name = "Patient_ID"
-                    df.index = df.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
-                    self._helper_tables["transcriptomics_normal"] = df
-            
+
+                if file_name == "HNSCC_NAT_RNA-Seq_Expr_WashU_FPKM.tsv.gz":
+                    df_norm = pd.read_csv(file_path, sep='\t')
+                    #change names to universal package names
+                    df_norm = df_norm.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})  
+                    df_norm = df_norm.set_index(["Name", "Database_ID"])
+                    df_norm = df_norm.sort_index()
+                    df_norm = df_norm.T #transpose
+                    df_norm.index.name = "Patient_ID"
+                    df_norm.index = df_norm.index.str.replace(r"-A", ".N", regex=True) #remove label for tumor samples
+                    self._helper_tables["transcriptomics_normal"] = df_norm
+
             # Combine the two transcriptomics dataframes
             rna_tumor = self._helper_tables.get("transcriptomics_tumor")
             rna_normal = self._helper_tables.get("transcriptomics_normal") # Normal entries are already marked with 'N' on the end of the ID
+            if rna_tumor is None or rna_normal is None:
+                print("rna_tumor or rna_normal is None")
+                return
+            if not isinstance(rna_tumor, pd.DataFrame) or not isinstance(rna_normal, pd.DataFrame):
+                print("rna_tumor or rna_normal is not a DataFrame")
+                return
+       
             rna_combined = pd.concat([rna_tumor, rna_normal])
+
             # save df in self._data
             self.save_df(df_type, rna_combined)
     
     def load_somatic_mutation(self):
         df_type = 'somatic_mutation'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
-            df = pd.read_csv(file_path, sep='\t', dtype={"PUBMED": "O"})    
+            df = pd.read_csv(file_path, sep='\t')    
             # Rename the columns we want to keep to the appropriate names
+            df = pd.read_csv(file_path, sep='\t')    
             df['Patient_ID'] = df.loc[:, 'Tumor_Sample_Barcode']
             df = df.rename(columns={
                         "Hugo_Symbol":"Gene",
                         "Gene":"Gene_Database_ID",
                         "Variant_Classification":"Mutation",
                         "HGVSp_Short":"Location"})
 
@@ -131,14 +132,15 @@
     def load_precursor_miRNA(self):
         df_type = 'precursor_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
+            df = df_tools.average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
@@ -147,17 +149,18 @@
             # save df in self._data
             self.save_df(df_type, all_df)
 
     def load_mature_miRNA(self):
         df_type = 'mature_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-            
+
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias', 'Derives_from'])
             df = df.transpose()
+            df = df_tools.average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
@@ -166,17 +169,18 @@
             # save df in self._data
             self.save_df(df_type, all_df)
 
     def load_total_mRNA(self):
         df_type = 'total_miRNA'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-            
+             
             df = pd.read_csv(file_path, delimiter = '\t', index_col = ['Name', 'ID','Alias'])
             df = df.transpose()
+            df = df_tools.average_replicates(df, common = '\.\d$') # average duplicates for C3L-02617 and C3N-02727
             df.index = df.index.str.replace('\.T$','', regex = True)
             df.index = df.index.str.replace('\.A$','.N', regex = True)
             df.index.name = 'Patient_ID'                
             # Sort
             normal = df.loc[df.index.str.contains('\.N$', regex =True)]
             normal = normal.sort_values(by=["Patient_ID"])
             tumor = df.loc[~ df.index.str.contains('\.N$', regex =True)]
@@ -214,19 +218,20 @@
 
     def load_mapping(self):
         df_type = 'mapping'
         if "CNV_gene_ids" not in self._helper_tables:
             file_path = self.locate_files(df_type)
 
             df = read_gtf(file_path)
+            df = df.as_df()
             df = df[["gene_name","gene_id"]]
             df = df.drop_duplicates()
             df = df.rename(columns={"gene_name": "Name","gene_id": "Database_ID"})
             df = df.set_index("Name")
-            self._helper_tables["CNV_gene_ids"] = df 
+            self._helper_tables["CNV_gene_ids"] = df
 
     def load_CNV(self):
         df_type = 'CNV'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
 
             df = pd.read_csv(file_path, sep="\t")
@@ -244,29 +249,51 @@
             # save df in self._data
             self.save_df(df_type, df)
 
     def load_tumor_purity(self):
         df_type = 'tumor_purity'
         if df_type not in self._data:
             file_path = self.locate_files(df_type)
-
+        
             df = pd.read_csv(file_path, sep = "\t", na_values = 'NA')
             df.Sample_ID = df.Sample_ID.str.replace(r'-T', '', regex=True) # only tumor samples in file
             df = df.set_index('Sample_ID') 
             df.index.name = 'Patient_ID'
 
             # get clinical df (used to slice out cancer specific patient_IDs in tumor_purity file)
-            mssmclin = Mssm(filter_type='luad', version=self.version, no_internet=self.no_internet) #_get_version - pancandataset
-            clinical_df = mssmclin.get_df('clinical')               
+            mssmclin = Mssm(filter_type='hnscc', no_internet=self.no_internet)
+            clinical_df = mssmclin.get_df('clinical')                
             patient_ids = clinical_df.index.to_list()
             df = df.loc[df.index.isin(patient_ids)]
 
             # save df in self._data
             self.save_df(df_type, df)
 
+    def load_hla_typing(self):
+        df_type = 'hla_typing'
+
+        if df_type not in self._data:
+            # perform initial checks and get file path (defined in source.py, the parent class)
+            file_path = self.locate_files(df_type)
+
+            # which cancer_type goes with which cancer in the mssm table
+            tumor_codes = {'brca':'BR', 'ccrcc':'CCRCC',
+                           'ucec':'UCEC', 'gbm':'GBM', 'hnscc':'HNSCC',
+                           'lscc':'LSCC', 'luad':'LUAD', 'pdac':'PDA',
+                           'hcc':'HCC', 'coad':'CO', 'ov':'OV'}
+
+            df = pd.read_csv(file_path, sep='\t')
+            df = df.loc[df['Cancer'] == tumor_codes[self.cancer_type]]
+            df = df.set_index("Sample")
+            df.index.name = 'Patient_ID'
+            df = df.sort_values(by=["Patient_ID"])
+
+            self.save_df(df_type, df)
+
+        return self._data[df_type]
     # def load_readme(self):
     #     df_type = 'readme'
     #     if not self._readme_files:
     #         file_path_list = self.locate_files(df_type)
     #         # loop over list of file paths
     #         for file_path in file_path_list:
     #             path_elements = file_path.split(os.sep) # Get a list of the levels of the path
@@ -290,11 +317,11 @@
                         
     #             elif file_name == "README_gene_expression":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_transcriptomics"] = reader.read()
                 
     #             elif file_name == "README.boxnote":
     #                 self._readme_files["readme_cnv"] = get_boxnote_text(file_path)
-
+                
     #             elif file_name == "README_ESTIMATE_WashU":
     #                 with open(file_path, 'r') as reader:
     #                     self._readme_files["readme_tumor_purity"] = reader.read()
```

### Comparing `cptac-1.5.0rc1/cptac/exceptions.py` & `cptac-1.5.0rc3/cptac/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,38 +22,22 @@
     """There was a problem with an HTTP response."""
     pass
 
 class InvalidParameterError(CptacError):
     """Invalid parameter."""
     pass
 
-class AmbiguousLatestError(InvalidParameterError):
-    """They pass "latest" for a version parameter, but index latest does not match latest version locally installed."""
-    pass
-
 class FileError(CptacError):
     """Base class for data-related errors."""
     pass
 
 class DatasetNotInstalledError(FileError):
     """They requested a dataset they haven't installed."""
     pass
 
-class DataVersionNotInstalledError(FileError):
-    """They requested a version they haven't installed of a dataset."""
-    pass
-
-class InvalidDataVersionError(CptacError):
-    """They requested an invalid version of a dataset for a given source."""
-    pass
-
-class PackageCannotHandleDataVersionError(CptacError):
-    """They tried to load a new version of the data, but they have an old version of the package that doesn't have the code for the new data, so they need to update the package."""
-    pass
-
 class MissingFileError(FileError):
     """A data file was missing."""
     pass
 
 class DownloadFailedError(FileError):
     """A file download failed."""
     pass
@@ -122,34 +106,26 @@
     """Mutation data was automatically filled during a dataframe join."""
     pass
 
 class ParameterWarning(CptacWarning):
     """We should warn them about a parameter for some reason."""
     pass
 
-class OldDataVersionWarning(CptacWarning):
-    """They're using an old data version."""
-    pass
-
-class OldPackageVersionWarning(CptacWarning):
-    """They're using an old version of the package."""
-    pass
-
 class PublicationEmbargoWarning(CptacWarning):
     """There is a publication embargo on the dataset."""
     pass
 
-class DownloadingNewLatestWarning(CptacWarning):
-    """Downloading a new latest data version. If they want to use an old version, they'll have to manually specify it."""
-    pass
-
 class FileNotUpdatedWarning(CptacWarning):
     """A file they wanted to update wasn't updated."""
     pass
 
+class FailedChecksumWarning(CptacWarning):
+    """A datafile failed a checksum test."""
+    pass
+
 class DatasetAlreadyInstalledWarning(CptacWarning):
     """The dataset was already installed, and they didn't want to redownload it."""
     pass
 
 class StatsWarning(CptacWarning):
     """Statistics-related warnings."""
     pass
@@ -161,8 +137,8 @@
 class PvalWarning(StatsWarning):
     """Some warning related to p values."""
     pass
 
 # Developer-directed exceptions
 class CptacDevError(Exception):
     """For exceptions that are probably the developer's fault."""
-    pass
+    pass
```

### Comparing `cptac-1.5.0rc1/cptac/tools/dataframe_tools.py` & `cptac-1.5.0rc3/cptac/tools/dataframe_tools.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,157 +6,78 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import pandas as pd
-import numpy as np
 import warnings
 from cptac.exceptions import CptacDevError, ReindexMapError, FailedReindexWarning
 from contextlib import contextmanager
 import sys, os
-import mygene
 
 
 @contextmanager
 def suppress_stdout():
     """Temporarily stops output from being printed. Use before a function when you don't want its output to
-    be printed. 
-    Example: with suppress_stdout(): 
+    be printed.
+    Example: with suppress_stdout():
                  function()
     """
     with open(os.devnull, "w") as devnull:
         old_stdout = sys.stdout
         sys.stdout = devnull
-        try:  
+        try:
             yield
         finally:
             sys.stdout = old_stdout
-            
-
-def map_database_to_gene_pdc(df, database_name = 'refseq', sep = ':'): 
-    """Add gene name to dataframe based on database IDs. This function is based on the format of PDC files. 
-    Only phosphoproteomics and acetylproteomics need the gene name added. 
-
-    Parameters:
-    df (dict): The dataframe that needs gene names.
-    database_name (str): dataframe name to use with mygene 'scopes' parameter.
-    sep (str): separator to split string with database ID. 
-
-    Returns:
-    df: The dataframe with gene name, database ID and site as a multiindex (sorted by gene name).
-    """
-    
-    if isinstance(df.index, pd.core.indexes.multi.MultiIndex):
-        was_multiindex = True
-        df = df.reset_index() # make index not a multiindex
-    else:
-        was_multiindex = False
-        
-    df = df.T.reset_index()
-    df[['Database_ID',"Site"]] = df.iloc[:, 0].str.split(sep, expand=True) # first column is reset index  
-    df.Site = df.Site.str.upper() # capitalize all amino acids sites (for consistency)
-    
-    id_list = df.Database_ID.to_list()
-    with suppress_stdout():
-        mg = mygene.MyGeneInfo()
-        db_results = mg.querymany(id_list, scopes=database_name, fields='symbol', species='human') # map ID to gene
-    db_to_gene = {results['query']: results['symbol'] for results in db_results \
-                           if 'notfound' not in results.keys()} # get mapping dictionary of ID and gene name
-    df['Name'] = df['Database_ID'].replace(db_to_gene) # add gene name 
-    df = df.set_index(['Name','Site','Database_ID']) # set multiindex
-    df = df.sort_index(level='Name', axis = 'index') # sort based on gene name
-    df = df.drop('index', axis = 1)
-    df = df.T
-    
-    if was_multiindex == True:
-        df = df.set_index([df.columns[-1], df.columns[-2]])
-        df.index.names = ['case_submitter_id','aliquot_submitter_id']
-        
-    return df
-
-
-def sort_rows_and_columns(df):
-    """This should be called on each dataframe before loading so that the order of data in all dataframes is consistent across cptac
-    The user can expect data to look the same as long as this is called on each datatype when it is parsed
-    
-    Sorts dataframe prioritized by:
-        1) Sample status (tumor samples first, followed by normal samples)
-        2) Index (patient C0001 before C0002)
-        3) Columns alhabetically based on the first level of the multiindex
-
-    Parameters:
-    df (pandas.DataFrame): The dataframe to be sorted.
-
-    Returns:
-    pandas.DataFrame: The dataframe, but sorted.
-    The index is also given the standard name ('Patient_ID').
-    """
-    
-    df = df.sort_index(axis = 'columns', level = 0) # sort columns based on first level
-    if isinstance(df.index, pd.core.indexes.multi.MultiIndex):
-        df.index.rename(['Patient_ID', 'Aliquot'], level = [0,1], inplace = True)
-        new_df = df.sort_values('Patient_ID')
-        return new_df
-    else:
-        df.index.name = "Patient_ID" # set the name of the index
-        # Sort normal samples
-        normal = df.loc[df.index.str.contains('\.[NC]$', regex = True, na = False)]#'.N' for normal, '.C' for cored normals (in HNSCC)
-        normal = normal.sort_index() # index should be Patient_ID
-        # Sort tumor samples
-        tumor = df.loc[~ df.index.str.contains('\.[NC]$', regex = True, na = False)]
-        tumor = tumor.sort_index()
-        # append normal to tumor
-        all_df = pd.concat([tumor,normal], axis=0, join='outer')
-        return all_df
 
 
 def rename_duplicate_labels(df, label_type='columns'):
-    """Returns a df with unique labels for columns or indices 
+    """Returns a df with unique labels for columns or indices
     Parameters:
     df (pandas.DataFrame): The df containing duplicate labels.
-    label_type (str): use 'columns' to make unique column labels and 'index' to make unique indices. 
-    
+    label_type (str): use 'columns' to make unique column labels and 'index' to make unique indices.
+
     Returns:
     pandas.DataFrame: df with with unique labels. ".i" is appended to every duplicate, increasing incrementally.
     """
     if label_type == 'columns':
         labs = pd.Series(df.columns[:])
 
-        for dup in labs[labs.duplicated()].unique(): 
+        for dup in labs[labs.duplicated()].unique():
             labs[labs[labs == dup].index.values.tolist()] = [dup + '.' + str(i) if i != 0 else dup for i in range(sum(labs == dup))]
 
-        # rename the columns with the labs list.
+        # rename the columns with the labs list
         df.columns=labs
-        
+
     elif label_type == 'index':
         labs = pd.Series(df.index[:])
 
-        for dup in labs[labs.duplicated()].unique(): 
+        for dup in labs[labs.duplicated()].unique():
             labs[labs[labs == dup].index.values.tolist()] = [dup + '.' + str(i) if i != 0 else dup for i in range(sum(labs == dup))]
 
-        # rename the columns with the labs list.
+        # rename the columns with the labs list
         df.index=labs
     return df
 
 def average_replicates(df, id_list = [], normal_identifier = '.N', common = '\.', to_drop = '\.\d$'):
     """Returns a df with one row for each patient_ID (all replicates for a patient are averaged)
     Parameters:
     df (pandas.DataFrame): The df containing replicates (duplicate entries for the same tissue_type).
-    id_list: list of IDs with replicates (use the ID format that is common between replicates so the 
-            list can be used to slice out all replicates for that ID). Make sure the IDs 
+    id_list: list of IDs with replicates (use the ID format that is common between replicates so the
+            list can be used to slice out all replicates for that ID). Make sure the IDs
             in the list include the symbol that distinguishes normal samples ('.N' or '-N').
     common: regex string that is common between replicates (identifies duplicate entries)
     to_drop: regex string to drop to find each patient_ID that has replicates (used to slice out all replicates)
-    
+
     Returns:
     pandas.DataFrame: df with with replicate rows averaged and one row for each patient_ID.
     """
-    # If no list of replicate IDs is given, make list from common regex 
+    # If no list of replicate IDs is given, make list from common regex
     if len(id_list) == 0:
         replicate_df = df[df.index.str.contains(common)]
         patient_ids = pd.Series(replicate_df.index) # create series of replicate IDs to prep removing appended ".i"
         ids = patient_ids.replace(to_drop, '', regex=True)
         id_list = list(set(ids)) #id_list contains only patient_IDs of replicates (without #s)
 
     new_df = df.copy()
@@ -169,54 +90,20 @@
             if normal_identifier == '.N':
                 norm_regex = '\.N' # prep for regex use
             else:
                 norm_regex = normal_identifier
             id_df = df[df.index.str.contains(patient_ID, regex = True) & \
                        ~ df.index.str.contains(norm_regex, regex = True)] # don't include normals
         #print(id_df.index.to_list())
-        vals = list(id_df.mean(axis=0)) 
+        vals = list(id_df.mean(axis=0))
         new_df = new_df.drop(id_df.index.to_list(), axis = 'index') # drop unaveraged rows
         new_df.loc[patient_ID] = vals # add averaged row
 
     return new_df
 
-def unionize_indices(dataset, exclude=[]):
-    """Return a union of all indices in a dataset, without duplicates.
-
-    Parameters:
-    dataset (dict of str: pandas.DataFrame): The data dictionary containing the dataset.
-    exclude (str or list of str, optional): A list of dataframes to exclude when unionizing indices.
-
-    Returns:
-    pandas.Index: Union of all indices in the dataset, without duplicates.
-    """
-    if isinstance(exclude, str): # If it's a single dataframe name, make it a list so we can treat everything the same
-        exclude = [exclude]
-    indices = [df.index for name, df in dataset.items() if name not in exclude]
-    master_index = pd.Index([])
-    for index in indices:
-        master_index = master_index.union(index)
-        master_index = master_index.drop_duplicates()
-   
-    return master_index
-
-def generate_sample_status_col(df, normal_test):
-    """Create a sample status column, called Sample_Tumor_Normal, for a dataframe.
-
-    Parameters:
-    df (pandas.DataFrame): The dataframe to create a Sample_Status column for, indexed with Patient_IDs.
-    normal_test (function): A function that takes a given Patient_ID and returns a bool indicating whether it corresponds to a normal sample.
-
-    Returns:
-    pandas Series: A sample status column for the dataframe.
-    """
-    sample_status_array = np.where(df.index.map(normal_test), "Normal", "Tumor")
-    sample_status_col = pd.Series(data=sample_status_array, index=df.index.copy())
-    return sample_status_col
-
 def get_reindex_map(series):
     """Generate a reindexing map from a series where the index is the new indices, and the values are the old indices.
 
     Parameters:
     series (pandas Series): The series to generate the reindex map from.
 
     Returns:
@@ -304,103 +191,99 @@
         del data_dict[name]
 
     return data_dict
 
 def reformat_normal_patient_ids(data_dict, existing_identifier=None, existing_identifier_location=None):
     """Reformat the patient IDs for normal samples to be marked by an appended ".N"
 
+    This function takes a dictionary of dataframes (all indexed by Patient IDs) and 
+    appends ".N" to normal patient IDs. It also optionally removes any existing identifier 
+    from the IDs before appending the new identifier.
+
     Parameters:
     data_dict (dict): The data dictionary for a dataset. All the tables must be indexed by Patient IDs.
-    existing_identifier (str, optional): A normal sample identifier that already exists on the normal samples' patient IDs, which we will remove before adding the new identifier. Default of None will cause nothing to be removed.
-    existing_identifier_location (str, optional): Either "start" or "end": Indicates whether the existing identifier is at the beginning or end of the normal samples' patient IDs, so we know which end to remove it from. Optional if nothing is passed to the existing_identifier parameter.
+    existing_identifier (str, optional): A normal sample identifier that already exists on the normal samples' patient IDs, 
+                                         which we will remove before adding the new identifier. Default is None.
+    existing_identifier_location (str, optional): Either "start" or "end": Indicates whether the existing identifier is at 
+                                                  the beginning or end of the normal samples' patient IDs, so we know which end 
+                                                  to remove it from. Default is None.
 
     Returns:
-    dict: The data dictionary for the dataset, with normal samples' patient IDs reformatted in the specified dataframes.
+    dict: The data dictionary for the dataset, with normal samples' patient IDs reformatted.
+
+    Raises:
+    CptacDevError: If only one of existing_identifier and existing_identifier_location is None.
     """
 
-    # Check parameters
-    if (existing_identifier is None and existing_identifier_location is not None) or (existing_identifier is not None and existing_identifier_location is None):
+    # Check if only one of the optional parameters is None
+    if (existing_identifier is None) != (existing_identifier_location is None):
         raise CptacDevError("Parameters existing_identifier and existing_identifier_location must either both be None, or both not be None.")
 
-    sample_statuses_old_index = data_dict["clinical"]["Sample_Tumor_Normal"] # We'll need this every time, and we need it with the un-reformatted index
-
-    for name in data_dict.keys(): # Loop over the keys so we can edit the values without any issues
+    # Extract the tumor/normal status column for reference
+    sample_statuses_old_index = data_dict["clinical"]["Sample_Tumor_Normal"]
 
-        df = data_dict[name]
+    for name, df in data_dict.items():
 
-        # Add in the tumor/normal statuses for these samples, if they aren't already in the table
-        added_sample_statuses = False # So we can keep track of whether to drop the column when we're done
+        # Add Sample_Tumor_Normal column if not present
         if "Sample_Tumor_Normal" not in df.columns:
             df = join_col_to_dataframe(df, sample_statuses_old_index)
             added_sample_statuses = True
+        else:
+            added_sample_statuses = False
 
-        df.index.name = "Patient_ID" # So we can easily access it when we've made it into a column
-        df = df.reset_index() # This makes the Patient_ID index a column, so we can edit it.
+        # Convert Patient_ID from index to column for editing
+        df.reset_index(level=0, inplace=True)
 
-        if (existing_identifier is not None) and (existing_identifier_location is not None): # There's an existing normal sample identifier to remove
+        # If there is an existing identifier, remove it
+        if existing_identifier is not None:
             existing_length = len(existing_identifier)
+            identifier_location_slice = slice(0, existing_length) if existing_identifier_location == "start" else slice(-existing_length, None)
 
-            if existing_identifier_location == "start":
-                df["Patient_ID"] = df["Patient_ID"].where(
-                    cond=(~((df["Sample_Tumor_Normal"] == "Normal") & (df["Patient_ID"].str[0:existing_length] == existing_identifier))),
-                    other=df["Patient_ID"].str[existing_length:]
-                )
-
-            elif existing_identifier_location == "end":
-                df["Patient_ID"] = df["Patient_ID"].where(
-                    cond=(~((df["Sample_Tumor_Normal"] == "Normal") & (df["Patient_ID"].str[-existing_length:] == existing_identifier))),
-                    other=df["Patient_ID"].str[:-existing_length] # Note that we use the negative of the existing length, since we're working with the end of the string
-                )
-
-            else:
-                raise CptacDevError("existing_identifier_location parameter must be either 'start' or 'end'")
-
-        # Append ".N" to the patient IDs of normal samples
-        df["Patient_ID"] = df["Patient_ID"].where(
-            cond=(~(df["Sample_Tumor_Normal"] == "Normal")),
-            other=df["Patient_ID"] + ".N"
-        )
+            # Only modify IDs where the status is 'Normal' and the existing identifier is present
+            condition = (~((df["Sample_Tumor_Normal"] == "Normal") & (df["Patient_ID"].str[identifier_location_slice] == existing_identifier)))
+            df.loc[~condition, "Patient_ID"] = df.loc[~condition, "Patient_ID"].str[identifier_location_slice]
+        
+        # Append ".N" to all normal sample IDs
+        df.loc[df["Sample_Tumor_Normal"] == "Normal", "Patient_ID"] += ".N"
 
-        # Set the index to the reformatted Patient IDs
-        df = df.set_index("Patient_ID")
+        # Restore Patient_ID as index
+        df.set_index("Patient_ID", inplace=True)
 
         # If we added the Sample_Tumor_Normal column, drop it
         if added_sample_statuses:
-            if isinstance(df.columns, pd.MultiIndex):
-                df = df.drop(columns="Sample_Tumor_Normal", level=0) # level=0 prevents a PerformanceWarning
-            else:
-                df = df.drop(columns="Sample_Tumor_Normal")
+            df.drop(columns="Sample_Tumor_Normal", errors="ignore", inplace=True)
 
-        # Put the dataframe with reformatted patient IDs back into the data dictionary
+        # Save the reformatted dataframe
         data_dict[name] = df
 
     return data_dict
 
+
 def join_col_to_dataframe(df, col):
     """Join a sample status column into a dataframe, automatically accounting for whether the dataframe has a column multiindex or not.
 
     Parameters:
     df (pandas.DataFrame): The dataframe to join the column into
     col (pandas Series): The column to join into the dataframe, with a matching index.
 
     Returns:
     pandas.DataFrame: The dataframe with the column joined in.
     """
     col_df = col.to_frame().copy(deep=True)
-    
+
     # Make sure the columns axes all have the same name
     df.columns.name = "Name"
     col_df.columns.name = "Name"
 
     # If df has a column multiindex, edit the col_df column index to match, so we can join them
     if col_df.columns.names != df.columns.names:
-        col_df.columns = add_index_levels(to=col_df.columns, source=df.columns) 
-    
+        col_df.columns = add_index_levels(to=col_df.columns, source=df.columns)
+
     if col_df.columns.names != df.columns.names: # Just to make sure
-        raise CptacDevError(f"col_df's column axes had levels not found in the dataframe's columns.")
+        raise CptacDevError("col_df's column axes had levels not found in the dataframe's columns.")
 
     df = df.join(col_df, how="left") # We do a left join because we only want rows that exist in our dataframe
 
     return df
 
 def standardize_axes_names(df):
     """For all dataframes in the given dictionary, sets the name of the index axes to "Patient_ID", because that's what they all are by that point, and sets the name of the column axes to "Name".
@@ -410,62 +293,14 @@
 
     Returns:
     dict: The dataframe dictionary, with the dataframe axes' names standardized. Keys are str of dataframe names, values are pandas.DataFrame
     """
     df.index.name = "Patient_ID"
     df.columns.name = "Name"
 
-def sort_all_rows(data_dict):
-    """For all dataframes in the given dictionary, sort them first by sample status, with tumor samples first, and then by the index.
-
-    Parameters:
-    data_dict (dict): The dataframe dictionary of the dataset.
-
-    Returns:
-    dict: The dataframe dictionary, with the dataframes sorted by their indices. Keys are str of dataframe names, values are pandas.DataFrame
-    """
-    # Get the Sample_Tumor_Normal column as a single-column dataframe
-    sample_status_col = data_dict["clinical"]["Sample_Tumor_Normal"].copy(deep=True) # We'll need this every time
-
-    for name in data_dict.keys(): # Loop over the keys so we can alter the values without any issues
-        df = data_dict[name]
-        df = sort_df_by_sample_status(df, sample_status_col)
-        data_dict[name] = df
-
-    return data_dict
-
-def sort_df_by_sample_status(df, sample_status_col):
-    """Sort a dataframe first by sample status, with tumor first, and then by Patient_ID.
-
-    df (pandas.DataFrame): The dataframe to sort.
-    sample_status_col (pandas Series): The Sample_Tumor_Normal column for the dataset.
-
-    Returns:
-    pandas.DataFrame: The dataframe, sorted.
-    """
-    # Add in the tumor/normal statuses for these samples, if they aren't already in the table
-    added_sample_statuses = False # So we can keep track of whether to drop the column when we're done
-
-    if "Sample_Tumor_Normal" not in df.columns:
-        df = join_col_to_dataframe(df, sample_status_col)
-        added_sample_statuses = True
-
-    # Sort first by the Sample_Tumor_Normal column, and then by the index
-    df.index.name = "Patient_ID" # To make sure we can reference it in the next line
-    df = df.sort_values(by=["Sample_Tumor_Normal", "Patient_ID"], ascending=[False, True]) # Sorts first by sample status, and in descending order, so "Tumor" samples are first
-
-    # If we added the Sample_Tumor_Normal column, drop it
-    if added_sample_statuses:
-        if isinstance(df.columns, pd.MultiIndex):
-            df = df.drop(columns="Sample_Tumor_Normal", level=0) # level=0 prevents a PerformanceWarning
-        else:
-            df = df.drop(columns="Sample_Tumor_Normal")
-
-    return df
-
 def add_index_levels(to, source, fill=""):
     """Add levels to the "to" index so it has all levels in the "source" index. The possible levels are, in this order: "Name", "Site", "Peptide", "Database_ID"
 
     Parameters:
     to (pandas.Index or pandas.MultiIndex): The index to add levels to.
     source (pandas.Index or pandas.MultiIndex): The index to match the levels of.
     fill (optional): Value to fill empty levels with. Default is an empty string, which allows us to select a column with just the first level. This is useful for boolean filters.
```

### Comparing `cptac-1.5.0rc1/cptac/utils/__init__.py` & `cptac-1.5.0rc3/cptac/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cptac-1.5.0rc1/cptac/utils/data/BioPlex_293T_Network_10K_Dec_2019.tsv.gz` & `cptac-1.5.0rc3/cptac/utils/data/BioPlex_293T_Network_10K_Dec_2019.tsv.gz`

 * *Files identical despite different names*

### Comparing `cptac-1.5.0rc1/cptac/utils/data/WikiPathwaysDataframe.tsv.gz` & `cptac-1.5.0rc3/cptac/utils/data/WikiPathwaysDataframe.tsv.gz`

 * *Files identical despite different names*

### Comparing `cptac-1.5.0rc1/cptac/utils/other_utils.py` & `cptac-1.5.0rc3/cptac/utils/other_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,64 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import json
 import os
 import pandas as pd
-import numpy as np
 import requests
 import webbrowser
 import warnings
 
 from cptac.exceptions import DropFromSingleIndexError, InvalidParameterError, MissingFileError, DuplicateColumnHeaderWarning, FileNotUpdatedWarning, FlattenSingleIndexWarning
 
+def df_to_tree(df):
+    df = df.\
+    assign(Datatypes=df["Datatypes"].str.split("\ *,\ *", expand=False, regex=True)).\
+    explode("Datatypes").\
+    reset_index(drop=True)
+    # Print our dataframe as a pretty tree structure
+    info = {}
+    for row in df.set_index(["Cancers", "Sources", "Datatypes"]).index.values:
+        if row[0] not in info.keys():
+            info[row[0]] = {}
+        if row[1] not in info[row[0]].keys():
+            info[row[0]][row[1]] = []
+        info[row[0]][row[1]].append(row[2])
+
+    df_tree = _tree(info)
+    return df_tree
+
+def _tree(nest, prepend=""):
+    """Recursively build a formatted string to represent a dictionary"""
+    tree_str = ""
+    if isinstance(nest, dict):
+        for i, (k, v) in enumerate(nest.items()):
+            if i == len(nest.keys()) - 1:
+                branch = "└"
+                newprepend = prepend + "    "
+            else:
+                branch = "├"
+                newprepend = prepend + "│   "
+            tree_str += f"{prepend}{branch}── {k}\n"
+            tree_str += _tree(nest=v, prepend=newprepend)
+    elif isinstance(nest, list):
+        for i, v in enumerate(nest):
+            if i == len(nest) - 1:
+                branch = "└"
+            else:
+                branch = "├"
+            tree_str += f"{prepend}{branch}── {v}\n"
+    else:
+        raise ValueError(f"Unexpected type '{type(nest)}'")
+
+    return tree_str
+
+
+
 def get_corum_protein_lists(update=True):
     """Reads file from CORUM and returns a dictionary where the keys are protein complex names, and the values are lists of proteins that are members of those complexes. Data is downloaded from the CORUM website (https://mips.helmholtz-muenchen.de/corum/#). We also provide get_hgnc_protein_lists to get similar data from HGNC. The CORUM data has more specific subgroups than the HGNC data, but the HGNC data is more comprehensive than the CORUM data--it contains proteins that aren't included in the CORUM data.
     Parameters:
     update (bool, optional): Whether to download the latest version of the file from CORUM. Default True. Otherwise, uses a previously downloaded copy (if one exists).
 
     Returns:
     dict: Keys are complex names; values are lists of proteins in each complex.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cptac-1.5.0rc1/cptac/utils/pathway_utils.py` & `cptac-1.5.0rc3/cptac/utils/pathway_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,172 +8,194 @@
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
 import os
 import pandas as pd
 import numpy as np
-import sys
-import urllib3
 import json
 import requests
 import webbrowser
 import warnings
 
 from cptac.exceptions import HttpResponseError, InvalidParameterError, ParameterWarning
 
 def get_interacting_proteins_string(protein, num_results=25):
-    """
-    @Param protein:
-        The name of the protein that you want to generate a list of interacting proteins for.
-
-    @Param num_results (default=25):
-        The number of interacting proteins that you want to get.
+    '''
+    Retrieves a list of proteins known to interact with the specified protein from the STRING database.
 
-    @Return:
-        A pandas.Series of proteins known by the String api to be interacting partners with the specified protein.
-        This list will always also contain the protein you were looking for interactors for.
-
-    This method takes as a parameter the name of a protein. It then accesses the STRING database, through
-    a call to their public API, and generates a list of proteins known to be interacting partners with the specified
-    protein. Optional second parameter is num_results (which by default is 25), which specifies in the API call how many
-    interacting partners to retrieve from the database. The list of interacting proteins is returned to the caller
-    as a pandas.Series.
-    """
+    Parameters
+    ----------
+    protein: str
+        The name of the protein to generate a list of interacting proteins for.
+    num_results: int, optional
+        The number of interacting proteins to retrieve. Defaults to 25.
+
+    Returns
+    -------
+    pandas.Series
+        A series of proteins known by the STRING API to interact with the specified protein. 
+        This series always also contains the queried protein.
+
+    Raises
+    ------
+    requests.exceptions.HTTPError
+        If the STRING API request fails.
+    '''
 
     # Send query to the STRING API
     query_url = "https://string-db.org/api/json/network"
-
     params = {
         "identifiers": protein,
-        "species": "9606", # Homo sapiens
+        "species": "9606",  # Homo sapiens
         "limit": num_results,
     }
 
-    query_resp = requests.get(query_url, params=params)
-
+    response = requests.get(query_url, params=params)
+    
     # Check that the response came back good
-    if query_resp.status_code != requests.codes.ok:
-        raise HttpResponseError(f"Submitting your query to the STRING API returned an HTTP status {query_resp.status_code}. The content returned from the request may be helpful:\n{query_resp.content.decode('utf-8')}")    
+    response.raise_for_status()
 
     # Put the response data in a dataframe
-    resp_df = pd.DataFrame(query_resp.json())
+    response_df = pd.DataFrame(response.json())
+
+    # Get the unique values of interacting proteins
+    interactors_A = response_df["preferredName_A"].unique()
+    interactors_B = response_df["preferredName_B"].unique()
 
-    # Get the unique values of columns we want, as a list
-    interactors = resp_df["preferredName_A"].\
-        append(resp_df["preferredName_B"]).\
-        unique()
+    # Combine and sort interactors
+    all_interactors = np.sort(np.append(interactors_A, interactors_B))
 
     # Make sure the protein they searched is in the output list
-    if protein not in interactors:
-        interactors = np.insert(interactors, 0, protein)
+    if protein not in all_interactors:
+        all_interactors = np.insert(all_interactors, 0, protein)
 
-    # Sort and convert to series
-    interactors = np.sort(interactors)
-    interactors = pd.Series(interactors)
+    # Convert to series
+    interactors_series = pd.Series(all_interactors)
 
-    return interactors
+    return interactors_series
 
-def get_interacting_proteins_biogrid(protein):
-    """Queries the BioGRID API to get interacting proteins for a given protein, based on curated literature references.
 
-    Parameters:
-    protein: The name of the protein that you want to generate a list of interacting proteins for.
+def get_interacting_proteins_biogrid(protein):
+    """
+    Queries the BioGRID API to get interacting proteins for a given protein.
 
-    Returns:
-    pandas.DataFrame: The interacting proteins, ranked by the number of literature references supporting them.
+    Parameters
+    ----------
+    protein : str
+        The name of the protein to generate a list of interacting proteins for.
+
+    Returns
+    -------
+    pandas.DataFrame
+        A dataframe of interacting proteins, ranked by the number of literature references supporting them.
+
+    Raises
+    ------
+    requests.exceptions.HTTPError
+        If the BioGRID API request fails.
+    ValueError
+        If no interactors are found for the specified protein.
     """
 
     # Post query to the BioGRID API
     query_url = "https://webservice.thebiogrid.org/interactions/"
-    
     params = {
         "searchNames": "true",
         "geneList": protein,
         "includeInteractors": "true",
         "includeInteractorInteractions": "false",
         "interSpeciesExcluded": "true",
         "format": "json",
         "taxId": "9606",
         "start": "0",
         "accesskey": "0ff59dcf3511928e78aad499688381c9"
     }
 
-    query_resp = requests.get(query_url, params=params)
-
+    response = requests.get(query_url, params=params)
+    
     # Check that the response came back good
-    if query_resp.status_code != requests.codes.ok:
-        raise HttpResponseError(f"Submitting your query to the STRING API returned an HTTP status {query_resp.status_code}. The content returned from the request may be helpful:\n{query_resp.content.decode('utf-8')}")    
+    response.raise_for_status()
 
-    elif len(query_resp.json()) == 0:
-        raise InvalidParameterError(f"No interactors found for '{protein}'. Are you sure you entered the identifier correctly?")
+    # Raise error if no interactors found
+    if len(response.json()) == 0:
+        raise ValueError(f"No interactors found for '{protein}'. Are you sure you entered the identifier correctly?")
 
     # Put the response data in a dataframe
-    resp_df = pd.DataFrame(query_resp.json()).transpose()
+    response_df = pd.DataFrame(response.json()).transpose()
 
-    # Get a list of all the interactors, and rank them by how many references each has
-    interactors = resp_df["OFFICIAL_SYMBOL_A"].\
-    where(resp_df["OFFICIAL_SYMBOL_A"] != protein, other=resp_df["OFFICIAL_SYMBOL_B"]).\
-    value_counts().\
-    to_frame("num_references")
+    # Create a series to store interactors and their counts
+    interactor_counts = pd.Series(dtype=int)
 
+    # Check each interactor, if it is not the protein, add to the count
+    for interactor in response_df[["OFFICIAL_SYMBOL_A", "OFFICIAL_SYMBOL_B"]].values:
+        interactor_counts[interactor[interactor != protein]] = interactor_counts.get(interactor[interactor != protein], 0) + 1
+
+    # Convert the series to a dataframe and set column name
+    interactors = interactor_counts.to_frame("num_references")
+
+    # Set index name
     interactors.index.name = "protein"
 
     return interactors
 
 def get_interacting_proteins_bioplex(protein, secondary_interactions=False):
     """
-    @Param protein:
-        The name of the protein that you want to generate a list of interacting proteins for.
-
-    @Return:
-        A list of proteins which are interacting partners with the specified protein, according to the bioplex data table.
-        Returns None if specified protein isn't found, or no interacting partners are found.
-
-    This method takes as a parameter the name of a protein. It then accesses the bioplex data table and returns a list of any protein found to be an interacting partner to the given protein.
-
-    The Bioplex data table is the "BioPlex 3.0 Interactions (293T Cells)" file for the HEK293T cell line, downloaded from <https://bioplex.hms.harvard.edu/interactions.php>. The direct download link is <https://bioplex.hms.harvard.edu/data/BioPlex_293T_Network_10K_Dec_2019.tsv>. IMPORTANT: After downloading the file, you need to compress it using gzip.
-    """
+    Retrieves a list of interacting proteins for a given protein from the BioPlex data table.
 
-    path_here = os.path.abspath(os.path.dirname(__file__))
-    file_name = os.path.join("data", "BioPlex_293T_Network_10K_Dec_2019.tsv.gz")
-    file_path = os.path.join(path_here, file_name)
+    Parameters
+    ----------
+    protein : str
+        The name of the protein to generate a list of interacting proteins for.
+    secondary_interactions : bool, optional
+        A flag to include secondary interactions. Default is False.
+
+    Returns
+    -------
+    list or None
+        A list of proteins which are interacting partners with the specified protein, 
+        according to the BioPlex data table. Returns None if specified protein isn't 
+        found, or no interacting partners are found.
+
+    Raises
+    ------
+    FileNotFoundError
+        If the BioPlex data file is not found.
+    """
+
+    file_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data", "BioPlex_293T_Network_10K_Dec_2019.tsv.gz")
+
+    # Raise error if file not found
+    if not os.path.isfile(file_path):
+        raise FileNotFoundError(f"BioPlex data file not found at {file_path}")
+
+    # Load the BioPlex data
+    bioplex_interactions = pd.read_csv(file_path, sep='\t')
+    bioplex_interactions.sort_values(by=["pInt", "pNI"], ascending=[False, True], inplace=True)
+
+    # Retrieve interacting proteins
+    interactors = set(bioplex_interactions.loc[bioplex_interactions['SymbolA'] == protein, 'SymbolB'])
+    interactors.update(bioplex_interactions.loc[bioplex_interactions['SymbolB'] == protein, 'SymbolA'])
 
-    # Read in the file, then sort to prioritize the interactions with the
-    # highest pInt (probability of interacting) and lowest pNI (probability of
-    # no interaction). Then, reset the index so that index number will
-    # correspond to rank under this sorting scheme.
-    bioplex_interactions = pd.read_csv(file_path, sep='\t').\
-        sort_values(by=["pInt", "pNI"], ascending=[False, True]).\
-        reset_index()
-
-    # Get all interactions with the protein of interest
-    A_df = bioplex_interactions.loc[bioplex_interactions['SymbolA'] == protein]
-    B_df = bioplex_interactions.loc[bioplex_interactions['SymbolB'] == protein]
+    # Check for secondary interactions
+    if secondary_interactions:
+        secondary_interactors = set()
+        for interactor in interactors:
+            secondary = get_interacting_proteins_bioplex(interactor, False)
+            if secondary is not None:
+                secondary_interactors.update(secondary)
 
-    A_interactions = list(A_df['SymbolB'])
-    B_interactions = list(B_df['SymbolA'])
+        interactors.update(secondary_interactors)
 
-    all_interactions = list(set(A_interactions + B_interactions))
+    # Check if there are any interactors
+    if not interactors:
+        return None
 
-    if secondary_interactions:
-        secondary_interactions_list = []
-        for interaction in all_interactions:
-            secondary = get_interacting_proteins_bioplex(interaction, False)
-            for si in secondary:
-                secondary_interactions_list.append(si)
-
-        for asi in secondary_interactions_list:
-            if asi not in all_interactions:
-                all_interactions.append(asi)
+    return list(interactors)
 
-    if len(all_interactions) > 0:
-        return all_interactions
-    else:
-        return None
     
 def get_interacting_proteins_wikipathways(protein):
     """
     @param protein:
     	String. The name of the protein
     @Return:
     	A list of proteins known by the most recent WikiPathways download to be interacting parters with the specified protein.
@@ -188,25 +210,25 @@
     file_name = "WikiPathwaysDataframe.tsv.gz"
     file_path = os.path.join(path_here, data_dir_name, file_name)
     proteinName = protein
 
     df = pd.read_csv(file_path, sep="\t", index_col=0)
 
     if (proteinName in df.index):
-    	row = df.loc[proteinName]
-    	filtered_df = df.loc[:, row.values.tolist()]
+        row = df.loc[proteinName]
+        filtered_df = df.loc[:, row.values.tolist()]
 
-    	def has_true(values):
-    		for val in values:
-    			if val == True:
-    				return True
-    		return False
+        def has_true(values):
+            for val in values:
+                if val == True:
+                    return True
+            return False
 
-    	filtered_df_final = filtered_df.loc[filtered_df.apply(lambda row: has_true(row.values.tolist()), axis=1), :]
-    	return filtered_df_final.index.tolist()
+        filtered_df_final = filtered_df.loc[filtered_df.apply(lambda row: has_true(row.values.tolist()), axis=1), :]
+        return filtered_df_final.index.tolist()
 
     return list()  # The protein was not found.
 
 def list_pathways_wikipathways():
     """
     @ Return:
     	A list of all the WikiPathways pathways
@@ -218,170 +240,184 @@
     file_name = "WikiPathwaysDataframe.tsv.gz"
     file_path = os.path.join(path_here, data_dir_name, file_name)
 
     df = pd.read_csv(file_path, sep="\t", index_col=0)
     return list(df.columns)
 
 def get_pathways_with_proteins(proteins, database, reactome_resource="UniProt", quiet=False):
-    """Query either the Reactome REST API or the WikiPathways downloaded dataframe to find pathways containing a particular gene or protein.
-
-    Parameters:
-    proteins (str or list of str): The protein(s) to look for matches to.
-    database (str): The database to use; either 'reactome' or 'wikipathways'.
-    reactome_resource (str, optional): If using Reactome, this is the resource the identifier(s) come from. Default is UniProt. Other options include HGNC, Ensembl, and GO. For more options, consult <https://reactome.org/content/schema/objects/ReferenceDatabase>. This parameter is meaningless if using WikiPathways.
-    quiet (bool, optional): Whether to suppress warnings issued when identifiers are not found. Default False.
+    """
+    Retrieves pathways containing a particular gene or protein from Reactome or WikiPathways.
 
-    Returns:
-    pandas.DataFrame: A table of pathways containing the given genes or proteins, with pathway names and, if using Reactome, their Reactome identifiers (which are needed for the pathway_overlay function).
+    Parameters
+    ----------
+    proteins : str or list of str
+        The protein(s) to look for matches to.
+    database : str
+        The database to use; either 'reactome' or 'wikipathways'.
+    reactome_resource : str, optional
+        If using Reactome, this is the resource the identifier(s) come from.
+        Default is UniProt. Other options include HGNC, Ensembl, and GO.
+    quiet : bool, optional
+        Whether to suppress warnings issued when identifiers are not found. Default False.
+
+    Returns
+    -------
+    pandas.DataFrame
+        A table of pathways containing the given genes or proteins, with pathway names and
+        their Reactome identifiers (if using Reactome).
+
+    Raises
+    ------
+    ValueError
+        If the database parameter is not 'reactome' or 'wikipathways'.
     """
 
-    # Process string input
     if isinstance(proteins, str):
         proteins = [proteins]
 
     if database.lower() == "reactome":
+        all_pathway_df = get_pathways_from_reactome(proteins, reactome_resource, quiet)
 
-        # Set headers and params
-        headers = {"accept": "application/json"}
-        params = {"species": "Homo sapiens"}
-
-        # Loop over proteins and get the interacting pathways
-        all_pathway_df = pd.DataFrame()
-        for id in proteins:
-            url = f"https://reactome.org/ContentService/data/mapping/{reactome_resource}/{id}/pathways"
-            resp = requests.get(url, headers=headers, params=params)
+    elif database.lower() == "wikipathways":
+        all_pathway_df = get_pathways_from_wikipathways(proteins, quiet)
+
+    else:
+        raise ValueError("Invalid database. Please choose 'reactome' or 'wikipathways'.")
+
+    return all_pathway_df.reset_index(drop=True)
 
-            # Check that the response came back good
+
+def get_pathways_from_reactome(proteins, reactome_resource, quiet):
+    headers = {"accept": "application/json"}
+    params = {"species": "Homo sapiens"}
+    all_pathway_df = pd.DataFrame()
+
+    for id in proteins:
+        url = f"https://reactome.org/ContentService/data/mapping/{reactome_resource}/{id}/pathways"
+        resp = requests.get(url, headers=headers, params=params)
+
+        # Error handling
+        if resp.status_code != requests.codes.ok:
             if resp.status_code == 404:
                 try:
                     msg = resp.json()["messages"]
                 except (json.JSONDecodeError, KeyError):
                     raise HttpResponseError(f"Your query returned an HTTP status {resp.status_code}. The content returned from the request may be helpful:\n{resp.content.decode('utf-8')}") from None
                 else:
                     if not quiet:
                         warnings.warn(f"The query for '{id}' returned HTTP 404 (not found). You may have mistyped the gene/protein ID or the reactome_resource name. The server gave the following message: {msg}", ParameterWarning, stacklevel=2)
                     continue
-            elif resp.status_code != requests.codes.ok:
+            else:
                 raise HttpResponseError(f"Your query returned an HTTP status {resp.status_code}. The content returned from the request may be helpful:\n{resp.content.decode('utf-8')}")
 
-            # Parse out pathway IDs and names
-            pathway_dict = resp.json()
-            names = []
-            pathway_ids = []
-            for pathway in pathway_dict:
-                names.append(pathway["displayName"])
-                pathway_ids.append(pathway["stId"])
-
-            pathway_df = pd.DataFrame({"id": id, "pathway": names, "pathway_id": pathway_ids})
-            pathway_df = pathway_df.sort_values(by="pathway_id")
-            all_pathway_df = all_pathway_df.append(pathway_df)
+        pathway_dict = resp.json()
+        pathways = [{"id": id, "pathway": pathway["displayName"], "pathway_id": pathway["stId"]} for pathway in pathway_dict]
 
-    elif database.lower() == "wikipathways":
+        all_pathway_df = all_pathway_df.append(pathways)
 
-        path_here = os.path.abspath(os.path.dirname(__file__))
-        data_dir_name = "data"
-        file_name = "WikiPathwaysDataframe.tsv.gz"
-        file_path = os.path.join(path_here, data_dir_name, file_name)
-        df = pd.read_csv(file_path, sep="\t", index_col=0)
-        all_pathway_df = pd.DataFrame()
-
-        for protein in proteins:
-
-            if protein in df.index:
-                # Column headers are pathways; select pathways where the row for the protein has a
-                # True for that pathway's column, indicating membership
-                pathways = df.columns[df.loc[protein, :]].values
+    return all_pathway_df.sort_values(by="pathway_id")
 
-                prot_df = pd.DataFrame({"id": protein, "pathway": pathways})
-                all_pathway_df = all_pathway_df.append(prot_df)
 
-            else:
-                if not quiet:
-                    warnings.warn(f"The protein '{protein}' was not found in the WikiPathways data.", ParameterWarning, stacklevel=2)
-    else:
-        raise InvalidParameterError(f"Database '{database}' not recognized. Valid options: 'reactome', 'wikipathways'")
+def get_pathways_from_wikipathways(proteins, quiet):
+    file_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data", "WikiPathwaysDataframe.tsv.gz")
+    df = pd.read_csv(file_path, sep="\t", index_col=0)
+    all_pathway_df = pd.DataFrame()
+
+    for protein in proteins:
+        if protein in df.index:
+            pathways = df.columns[df.loc[protein, :]].values
+            prot_df = [{"id": protein, "pathway": pathway} for pathway in pathways]
+            all_pathway_df = all_pathway_df.append(prot_df)
+        elif not quiet:
+            warnings.warn(f"The protein '{protein}' was not found in the WikiPathways data.", ParameterWarning, stacklevel=2)
 
-    all_pathway_df = all_pathway_df.reset_index(drop=True)
     return all_pathway_df
 
 def get_proteins_in_pathways(pathways, database, quiet=False):
-    """Query either the Reactome REST API or the downloaded WikiPathways dataframe to get a list of proteins contained in a particular pathway.
-
-    Parameters:
-    pathways (str or list of str): The pathway(s) to get the contained proteins for. If using Reactome, these must be pathway IDs (e.g. "R-HSA-140877").
-    database (str): The database to use; either 'reactome' or 'wikipathways'.
-    quiet (bool, optional): Whether to suppress warnings issued when identifiers are not found. Default False.
+    """
+    Retrieves a list of proteins contained in a particular pathway from Reactome or WikiPathways.
 
-    Returns:
-    pandas.DataFrame: The proteins contained in the pathways.
+    Parameters
+    ----------
+    pathways : str or list of str
+        The pathway(s) to get the contained proteins for.
+        If using Reactome, these must be pathway IDs (e.g. "R-HSA-140877").
+    database : str
+        The database to use; either 'reactome' or 'wikipathways'.
+    quiet : bool, optional
+        Whether to suppress warnings issued when identifiers are not found. Default False.
+
+    Returns
+    -------
+    pandas.DataFrame
+        The proteins contained in the pathways.
+
+    Raises
+    ------
+    ValueError
+        If the database parameter is not 'reactome' or 'wikipathways'.
     """
 
-    # Process string input
     if isinstance(pathways, str):
         pathways = [pathways]
 
     if database.lower() == "reactome":
-        # Set headers and url
-        headers = {"accept": "application/json"}
+        all_protein_df = get_proteins_from_reactome(pathways, quiet)
 
-        # Loop over ids and get the interacting pathways
-        all_protein_df = pd.DataFrame()
-        for pathway_id in pathways:
-
-            # Send the request
-            url = f"https://reactome.org/ContentService/data/participants/{pathway_id}"
-            resp = requests.get(url, headers=headers)
-
-            if resp.status_code == 404 or (resp.status_code == requests.codes.ok and (len(resp.content.decode("utf-8")) == 0 or len(resp.json()) == 0)):
-                if not quiet:
-                    warnings.warn(f"The query for '{pathway_id}' found no results. You may have mistyped the pathway ID.", ParameterWarning, stacklevel=2)
-                continue
-            elif resp.status_code != requests.codes.ok:
-                raise HttpResponseError(f"Your query returned an HTTP status {resp.status_code}. The content returned from the request may be helpful:\n{resp.content.decode('utf-8')}")
+    elif database.lower() == "wikipathways":
+        all_protein_df = get_proteins_from_wikipathways(pathways, quiet)
 
-            # Parse all the proteins/genes out of the response
-            members_df = pd.json_normalize(resp.json(), record_path=["refEntities"])
-            prot_df = members_df[members_df["displayName"].str.startswith("UniProt:")]
-            
-            prot_names = prot_df["displayName"].str.rsplit(" ", n=1, expand=True)[1].\
-                drop_duplicates(keep="first").\
-                sort_values().\
-                reset_index(drop=True)
-            
-            pathway_df = pd.DataFrame({"pathway": pathway_id, "member": prot_names})
-            all_protein_df = all_protein_df.append(pathway_df)
+    else:
+        raise ValueError("Invalid database. Please choose 'reactome' or 'wikipathways'.")
 
-        all_protein_df = all_protein_df.drop_duplicates(keep="first")
+    return all_protein_df.reset_index(drop=True)
 
-    elif database.lower() == "wikipathways":
 
-        path_here = os.path.abspath(os.path.dirname(__file__))
-        data_dir_name = "data"
-        file_name = "WikiPathwaysDataframe.tsv.gz"
-        file_path = os.path.join(path_here, data_dir_name, file_name)
-        df = pd.read_csv(file_path, sep="\t", index_col=0)
-        all_protein_df = pd.DataFrame()
-
-        for pathway in pathways:
-
-            if pathway in df.columns:
-                prot_names = df.index[df[pathway]].values
-                pathway_df = pd.DataFrame({"pathway": pathway, "member": prot_names})
-                all_protein_df = all_protein_df.append(pathway_df)
-                
-            else:
-                if not quiet:
-                    warnings.warn(f"The pathway '{pathway}' was not found in the WikiPathways data.", ParameterWarning, stacklevel=2)
+def get_proteins_from_reactome(pathways, quiet):
+    headers = {"accept": "application/json"}
+    all_protein_df = pd.DataFrame()
 
-    else:
-        raise InvalidParameterError(f"Database '{database}' not recognized. Valid options: 'reactome', 'wikipathways'")
+    for pathway_id in pathways:
+        url = f"https://reactome.org/ContentService/data/participants/{pathway_id}"
+        resp = requests.get(url, headers=headers)
+
+        # Error handling
+        if resp.status_code != requests.codes.ok or (len(resp.content.decode("utf-8")) == 0 or len(resp.json()) == 0):
+            if not quiet:
+                warnings.warn(f"The query for '{pathway_id}' found no results. You may have mistyped the pathway ID.", ParameterWarning, stacklevel=2)
+            continue
+
+        members_df = pd.json_normalize(resp.json(), record_path=["refEntities"])
+        prot_df = members_df[members_df["displayName"].str.startswith("UniProt:")]
+
+        prot_names = prot_df["displayName"].str.rsplit(" ", n=1, expand=True)[1]
+        proteins = [{"pathway": pathway_id, "member": name} for name in prot_names.unique()]
+
+        all_protein_df = all_protein_df.append(proteins)
+
+    return all_protein_df.drop_duplicates()
+
+
+def get_proteins_from_wikipathways(pathways, quiet):
+    file_path = os.path.join(os.path.abspath(os.path.dirname(__file__)), "data", "WikiPathwaysDataframe.tsv.gz")
+    df = pd.read_csv(file_path, sep="\t", index_col=0)
+    all_protein_df = pd.DataFrame()
+
+    for pathway in pathways:
+        if pathway in df.columns:
+            prot_names = df.index[df[pathway]].values
+            proteins = [{"pathway": pathway, "member": name} for name in prot_names]
+
+            all_protein_df = all_protein_df.append(proteins)
+        elif not quiet:
+            warnings.warn(f"The pathway '{pathway}' was not found in the WikiPathways data.", ParameterWarning, stacklevel=2)
 
-    all_protein_df = all_protein_df.reset_index(drop=True)
     return all_protein_df
 
+
 def reactome_pathway_overlay(pathway, df=None, analysis_token=None, open_browser=True, export_path=None, image_format="png", display_col_idx=0, diagram_colors="Modern", overlay_colors="Standard", quality=7):
     """Visualize numerical data (e.g. protein expression) on a Reactome pathway diagram, with each node's color corresponding to the expression value provided for that molecule.
 
     Parameters:
     pathway (str): The Reactome ID for the pathway you want to overlay the data on, e.g. "R-HSA-73929".
     df (pandas.DataFrame or pandas.Series, optional): If you haven't previously analyzed your data with Reactome, give this parameter the data you want to overlay. Each row corresponds to a particular gene/protein/etc, and each column is expression or other data for a sample or aggregate. Index must be unique identifiers. Multiple data columns allowed. All dtypes must be numeric. Default None assumes you are instead passing a token for previously analyzed data to the "analysis_token" parameter.
     analysis_token (str, optional): If the data you want to visualize has been recently analyzed in Reactome already, pass the token for that analysis to this parameter to overlay it on the specified pathway. This will allow this function to reaccess the archived results, thus avoiding wasting time by repeating the work of submitting and analyzing the data. Default of None assumes you are instead passing data to the "df" parameter.
```

### Comparing `cptac-1.5.0rc1/cptac/utils/stats_utils.py` & `cptac-1.5.0rc3/cptac/utils/stats_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,16 @@
     for column in comparison_columns:
         if len(partition1[column].dropna(axis=0)) <= mincount:
             continue
         elif len(partition2[column].dropna(axis=0)) <= mincount:
             continue
         else:
 
-            group1 = partition1[column].dropna(axis=0)
-            group2 = partition2[column].dropna(axis=0)
+            group1 = partition1[column].dropna(axis=0).astype(float)
+            group2 = partition2[column].dropna(axis=0).astype(float)
 
             if (np.std(group1) == 0 or np.std(group2) == 0) and not quiet:
                 warnings.warn(f"At least one group for column {column} had a standard deviation of zero.", StDevWarning)
 
             stat, pval = scipy.stats.ttest_ind(
                 a=group1,
                 b=group2,
```

### Comparing `cptac-1.5.0rc1/cptac.egg-info/PKG-INFO` & `cptac-1.5.0rc3/cptac.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 Metadata-Version: 2.1
 Name: cptac
-Version: 1.5.0rc1
+Version: 1.5.0rc3
 Summary: Python packaging for CPTAC data
 Home-page: http://github.com/PayneLab/cptac
 Author: Dr. Samuel Payne
 Author-email: sam_payne@byu.edu
 License: Apache 2.0
 Project-URL: Documentation, https://paynelab.github.io/cptac/
-Description: # Easy access to CPTAC data
-        This software provides easy access to cancer data from the National Cancer Institute's CPTAC program, which characterizes and studies the proteogenomic landscape of tumors. We implement the software as a Python package called `cptac`, but you can seamlessly use it in an R environment with the help of the `reticulate` package (demonstrated in [Tutorial 6](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)). Our package is installed in one step with `pip`:
-        ```
-        pip install cptac
-        ```
-        See the [Installation section below](https://paynelab.github.io/cptac/#installation) if you have further questions.
-        
-        The package gives you the data as `pandas` `DataFrame` objects in Python. If you are using R, `reticulate` converts the tables to `data.frame` objects. By providing the tables natively in your programming environment, we eliminate the need for parsing and formatting, allowing you to quickly feed the data into whatever analysis code you have written. Follow our walkthrough tutorials and use cases for examples of how to use the software.
-        
-        Additionally, the software automatically handles data downloading, storage, and updates. You need only to tell it which datasets you want downloaded, and it will automatically get the data without requiring you to write any HTTP requests or database queries.
-        
-        ## Installation
-        This package is intended to run on Python 3.6 or greater. If you plan on interfacing with it from R via `reticulate`, you must still have Python installed on your computer, and download the package into that Python environment.
-        
-        ### Installing Python
-        If you do not already have Python installed on your computer, we suggest using either the [standard Python distribution](https://www.python.org/downloads/) or the [Anaconda distribution](https://www.anaconda.com/distribution/). Follow the installation instructions at the respective links. The Anaconda distribution allows you to set up multiple distinct Python environments and comes with many useful Python packages pre-installed. For more information, see the Ananconda documentation.
-        
-        ### Installing the cptac package
-        We distribute the package [through the Python Package Index (PyPI)](https://pypi.org/project/cptac/), so regardless of which Python distribution you are using, you install the package using the `pip` program:
-        ```
-        pip install cptac
-        ```
-        If you are using the Anaconda distribution of Python, this will install `cptac` to the currently active environment as long as `pip` is available in that environment, which it would be by default. If `pip` is not installed in your environment, you can install it with `conda install -c anaconda pip`. Then, you can use `pip` to install the `cptac` package. We plan on making `cptac` directly available through `conda` in the near future.
-        
-        The package depends on several other Python libraries including `numpy`, `pandas`, `requests`, and others. Normally, `pip` will automatically handle these dependencies when it installs `cptac` and you don't have to worry about any of it. However, if you have a special use case or are interested in exactly which versions of which packages are needed, you can consult the `install_requires` list in the [setup.py file](https://github.com/PayneLab/cptac/blob/master/setup.py).
-        
-        ## Documentation
-        Our goal is that our documentation will make this software and data accessible both to people without a computer science background, and people without a biology background. We provide two types of documentation to accomplish this: tutorials and use cases. The tutorials give a basic introduction to the software as well as conventions for storing and accessing the data. The use cases are short examples focused on a biological question and show practical uses of the software and data for biological discovery. Each use case works with a different combination of data types and explores meaningful cancer research hypotheses. 
-        
-        You can access the tutorials and use cases as static webpages using the links below. They were originally written in Python as interactive Jupyter notebooks, so if you want to run them interactively with Jupyter you can download the notebooks from the [notebooks folder](https://github.com/PayneLab/cptac/tree/master/notebooks) on the GitHub repository. If you are unfamiliar with Jupyter, follow the installation and usage instructions given [here](https://jupyter.org/install) on the Jupyter website. You will then be able to run our tutorials as interactive, exploratory data analyses. If you want to run them interactively without installing anything, please visit our Binder site which hosts the notebooks [here](https://mybinder.org/v2/gh/PayneLab/cptac/master?filepath=%2Fnotebooks).
-        
-        ### Tutorials
-        - [Tutorial 1: CPTAC data introduction](https://paynelab.github.io/cptac/tutorial01_data_intro.html)
-        - [Tutorial 2: Using pandas to work with cptac dataframes](https://paynelab.github.io/cptac/tutorial02_pandas.html)
-        - [Tutorial 3: Joining dataframes with cptac](https://paynelab.github.io/cptac/tutorial03_joining_dataframes.html)
-        - [Tutorial 4: Understanding multi-indexes](https://paynelab.github.io/cptac/tutorial04_multiindex.html)
-        - [Tutorial 5: How to keep up to date with new package and data releases](https://paynelab.github.io/cptac/tutorial05_updates.html)
-        - [Tutorial 6: Easy integration with R](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)
-        
-        ### Use cases
-        - [Use Case 1: Comparing transcriptomics and proteomics](https://paynelab.github.io/cptac/usecase01_omics.html)
-        - [Use Case 2: Correlation between clinical attributes](https://paynelab.github.io/cptac/usecase02_clinical_attributes.html)
-        - [Use Case 3: Associating clinical variables with omics data](https://paynelab.github.io/cptac/usecase03_clinical_and_acetylation.html)
-        - [Use Case 4: How Do Mutations Affect Protein Abundance?](https://paynelab.github.io/cptac/usecase04_mutations_and_omics.html)
-        - [Use Case 5: Gene Set Enrichment Analysis](https://paynelab.github.io/cptac/usecase05_enrichment_analysis.html)
-        - [Use Case 6: Comparing Derived Molecular Data with Proteomics](https://paynelab.github.io/cptac/usecase06_derived_molecular.html)
-        - [Use Case 7: Trans Genetics Effects](https://paynelab.github.io/cptac/usecase07_trans_genetic_effect.html)
-        - [Use Case 8: Outliers](https://paynelab.github.io/cptac/usecase08_outliers.html)
-        - [Use Case 9: Clinical Outcomes](https://paynelab.github.io/cptac/usecase09_clinical_outcomes.html)
-        - [Use Case 10: Pathway diagram overlay](https://paynelab.github.io/cptac/usecase10_pathway_overlay.html)
-        
-        ## Developer documentation
-        Documentation for anyone wanting to understand the internal workings of the package is available on the GitHub repository in the [devdocs folder](https://github.com/PayneLab/cptac/tree/master/devdocs).
-        
-        ## License
-        See the [LICENSE.md](https://github.com/PayneLab/cptac/blob/master/LICENSE.md) document on the GitHub repository. Please note the difference between the license as it applies to code versus data.
-        
-        ## Contact
-        This package is maintained by [the Payne lab](https://payne.byu.edu) at Brigham Young University.
-        
 Keywords: bioinformatics cancer proteomics genomics open science open data
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# CPTAC v.1.5 Release Candidate is now available
+Please report any bugs or possible improvements. Enjoy!
+
+# Easy access to CPTAC data
+This software provides easy access to cancer data from the National Cancer Institute's CPTAC program, which characterizes and studies the proteogenomic landscape of tumors. We implement the software as a Python package called `cptac`, but you can seamlessly use it in an R environment with the help of the `reticulate` package (demonstrated in [Tutorial 6](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)). Our package is installed in one step with `pip`:
+```
+pip install cptac
+```
+See the [Installation section below](https://paynelab.github.io/cptac/#installation) if you have further questions.
+
+The package gives you the data as `pandas` `DataFrame` objects in Python. If you are using R, `reticulate` converts the tables to `data.frame` objects. By providing the tables natively in your programming environment, we eliminate the need for parsing and formatting, allowing you to quickly feed the data into whatever analysis code you have written. Follow our walkthrough tutorials and use cases for examples of how to use the software.
+
+Additionally, the software automatically handles data downloading, storage, and updates. You need only to tell it which datasets you want downloaded, and it will automatically get the data without requiring you to write any HTTP requests or database queries.
+
+## Installation
+This package is intended to run on Python 3.6 or greater. If you plan on interfacing with it from R via `reticulate`, you must still have Python installed on your computer, and download the package into that Python environment.
+
+### Installing Python
+If you do not already have Python installed on your computer, we suggest using either the [standard Python distribution](https://www.python.org/downloads/) or the [Anaconda distribution](https://www.anaconda.com/distribution/). Follow the installation instructions at the respective links. The Anaconda distribution allows you to set up multiple distinct Python environments and comes with many useful Python packages pre-installed. For more information, see the Ananconda documentation.
+
+### Installing the cptac package
+We distribute the package [through the Python Package Index (PyPI)](https://pypi.org/project/cptac/), so regardless of which Python distribution you are using, you install the package using the `pip` program:
+```
+pip install cptac
+```
+If you are using the Anaconda distribution of Python, this will install `cptac` to the currently active environment as long as `pip` is available in that environment, which it would be by default. If `pip` is not installed in your environment, you can install it with `conda install -c anaconda pip`. Then, you can use `pip` to install the `cptac` package. We plan on making `cptac` directly available through `conda` in the near future.
+
+The package depends on several other Python libraries including `numpy`, `pandas`, `requests`, and others. Normally, `pip` will automatically handle these dependencies when it installs `cptac` and you don't have to worry about any of it. However, if you have a special use case or are interested in exactly which versions of which packages are needed, you can consult the `install_requires` list in the [setup.py file](https://github.com/PayneLab/cptac/blob/master/setup.py).
+
+## Documentation
+Our goal is that our documentation will make this software and data accessible both to people without a computer science background, and people without a biology background. We provide two types of documentation to accomplish this: tutorials and use cases. The tutorials give a basic introduction to the software as well as conventions for storing and accessing the data. The use cases are short examples focused on a biological question and show practical uses of the software and data for biological discovery. Each use case works with a different combination of data types and explores meaningful cancer research hypotheses. 
+
+You can access the tutorials and use cases as static webpages using the links below. They were originally written in Python as interactive Jupyter notebooks, so if you want to run them interactively with Jupyter you can download the notebooks from the [notebooks folder](https://github.com/PayneLab/cptac/tree/master/notebooks) on the GitHub repository. If you are unfamiliar with Jupyter, follow the installation and usage instructions given [here](https://jupyter.org/install) on the Jupyter website. You will then be able to run our tutorials as interactive, exploratory data analyses. If you want to run them interactively without installing anything, please visit our Binder site which hosts the notebooks [here](https://mybinder.org/v2/gh/PayneLab/cptac/master?filepath=%2Fnotebooks).
+
+### Tutorials
+- [Tutorial 1: CPTAC data introduction](https://paynelab.github.io/cptac/tutorial01_data_intro.html)
+- [Tutorial 2: Using pandas to work with cptac dataframes](https://paynelab.github.io/cptac/tutorial02_pandas.html)
+- [Tutorial 3: Joining dataframes with cptac](https://paynelab.github.io/cptac/tutorial03_joining_dataframes.html)
+- [Tutorial 4: Understanding multi-indexes](https://paynelab.github.io/cptac/tutorial04_multiindex.html)
+- [Tutorial 5: How to keep up to date with new package and data releases](https://paynelab.github.io/cptac/tutorial05_updates.html)
+- [Tutorial 6: Easy integration with R](https://paynelab.github.io/cptac/tutorial06_cptac_in_R.html)
+
+### Use cases
+- [Use Case 1: Comparing transcriptomics and proteomics](https://paynelab.github.io/cptac/usecase01_omics.html)
+- [Use Case 2: Correlation between clinical attributes](https://paynelab.github.io/cptac/usecase02_clinical_attributes.html)
+- [Use Case 3: Associating clinical variables with omics data](https://paynelab.github.io/cptac/usecase03_clinical_and_acetylation.html)
+- [Use Case 4: How Do Mutations Affect Protein Abundance?](https://paynelab.github.io/cptac/usecase04_mutations_and_omics.html)
+- [Use Case 5: Gene Set Enrichment Analysis](https://paynelab.github.io/cptac/usecase05_enrichment_analysis.html)
+- [Use Case 6: Comparing Derived Molecular Data with Proteomics](https://paynelab.github.io/cptac/usecase06_derived_molecular.html)
+- [Use Case 7: Trans Genetics Effects](https://paynelab.github.io/cptac/usecase07_trans_genetic_effect.html)
+- [Use Case 8: Outliers](https://paynelab.github.io/cptac/usecase08_outliers.html)
+- [Use Case 9: Clinical Outcomes](https://paynelab.github.io/cptac/usecase09_clinical_outcomes.html)
+- [Use Case 10: Pathway diagram overlay](https://paynelab.github.io/cptac/usecase10_pathway_overlay.html)
+
+## Developer documentation
+Documentation for anyone wanting to understand the internal workings of the package is available on the GitHub repository in the [devdocs folder](https://github.com/PayneLab/cptac/tree/master/devdocs).
+
+## License
+See the [LICENSE.md](https://github.com/PayneLab/cptac/blob/master/LICENSE.md) document on the GitHub repository. Please note the difference between the license as it applies to code versus data.
+
+## Contact
+This package is maintained by [the Payne lab](https://payne.byu.edu) at Brigham Young University.
```

### Comparing `cptac-1.5.0rc1/setup.py` & `cptac-1.5.0rc3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,34 +28,29 @@
 	packages=find_packages(
         where='.',
         include=['cptac*'],  # ["*"] by default
         exclude=[],  # empty by default
     ),
 	install_requires=[
 		'numpy>=1.16.3',
-		'pandas>=1.2.0',
+		'pandas>=2.0.0',
 		'requests>=2.21.0',
-		'beautifulsoup4>=4.7.1',
-		'scipy>=1.2.1',
-		'urllib3>=1.24.2',
+		'scipy>=1.10.0',
 		'openpyxl>=2.6.0',
-		'packaging>=19.2',
-		'xlrd>=2.0.1',
 		'statsmodels>=0.10.0',
-		'flask>=1.1.0',
-		'gtfparse>=1.2.1',
-		'mygene>=3.2.2'
+		'pyranges>=0.0.111',
+        'tqdm>=4.65.0',
 	],
 	classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: Apache Software License',
 	],
 	keywords='bioinformatics cancer proteomics genomics open science open data',
-	python_requires='>=3.6.*',
+	python_requires='>=3.6',
 	zip_safe=False,
 	include_package_data=True,
 	project_urls={
 	   'Documentation': 'https://paynelab.github.io/cptac/'
 	},
-	)
+)
```

