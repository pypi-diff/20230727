# Comparing `tmp/sniffles-2.0.7.tar.gz` & `tmp/sniffles-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniffles-2.0.7.tar", last modified: Mon Jul 25 09:22:43 2022, max compression
+gzip compressed data, was "sniffles-2.2.tar", last modified: Thu Jul 27 18:10:34 2023, max compression
```

## Comparing `sniffles-2.0.7.tar` & `sniffles-2.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 moritz     (501) staff       (20)        0 2022-07-25 09:22:43.480075 sniffles-2.0.7/
--rw-r--r--   0 moritz     (501) staff       (20)     1070 2022-07-25 09:22:20.000000 sniffles-2.0.7/LICENSE
--rw-r--r--   0 moritz     (501) staff       (20)     4168 2022-07-25 09:22:43.480290 sniffles-2.0.7/PKG-INFO
--rw-r--r--   0 moritz     (501) staff       (20)     3618 2022-05-11 19:01:51.000000 sniffles-2.0.7/README.md
--rw-r--r--   0 moritz     (501) staff       (20)      104 2022-07-25 09:22:31.000000 sniffles-2.0.7/pyproject.toml
--rw-r--r--   0 moritz     (501) staff       (20)      744 2022-07-25 09:22:43.481680 sniffles-2.0.7/setup.cfg
-drwxr-xr-x   0 moritz     (501) staff       (20)        0 2022-07-25 09:22:43.466880 sniffles-2.0.7/src/
-drwxr-xr-x   0 moritz     (501) staff       (20)        0 2022-07-25 09:22:43.476574 sniffles-2.0.7/src/sniffles/
--rw-r--r--   0 moritz     (501) staff       (20)      190 2021-08-15 20:58:29.000000 sniffles-2.0.7/src/sniffles/__init__.py
--rw-r--r--   0 moritz     (501) staff       (20)    13814 2022-03-20 20:27:06.000000 sniffles-2.0.7/src/sniffles/cluster.py
--rw-r--r--   0 moritz     (501) staff       (20)    20481 2022-07-25 09:17:49.000000 sniffles-2.0.7/src/sniffles/config.py
--rw-r--r--   0 moritz     (501) staff       (20)    15125 2022-02-06 10:50:24.000000 sniffles-2.0.7/src/sniffles/consensus.py
--rwxr-xr-x   0 moritz     (501) staff       (20)    20574 2022-04-05 17:54:18.000000 sniffles-2.0.7/src/sniffles/leadprov.py
--rw-r--r--   0 moritz     (501) staff       (20)    13928 2022-04-05 18:12:57.000000 sniffles-2.0.7/src/sniffles/parallel.py
--rw-r--r--   0 moritz     (501) staff       (20)    13774 2022-03-20 20:30:29.000000 sniffles-2.0.7/src/sniffles/postprocessing.py
--rw-r--r--   0 moritz     (501) staff       (20)     4240 2022-02-06 10:50:00.000000 sniffles-2.0.7/src/sniffles/snf.py
--rwxr-xr-x   0 moritz     (501) staff       (20)    27114 2022-07-25 09:14:38.000000 sniffles-2.0.7/src/sniffles/sniffles
--rwxr-xr-x   0 moritz     (501) staff       (20)    18929 2022-07-25 09:16:55.000000 sniffles-2.0.7/src/sniffles/sv.py
--rw-r--r--   0 moritz     (501) staff       (20)     3283 2022-03-20 16:33:40.000000 sniffles-2.0.7/src/sniffles/util.py
--rwxr-xr-x   0 moritz     (501) staff       (20)    15330 2022-03-22 14:10:45.000000 sniffles-2.0.7/src/sniffles/vcf.py
-drwxr-xr-x   0 moritz     (501) staff       (20)        0 2022-07-25 09:22:43.479483 sniffles-2.0.7/src/sniffles.egg-info/
--rw-r--r--   0 moritz     (501) staff       (20)     4168 2022-07-25 09:22:43.000000 sniffles-2.0.7/src/sniffles.egg-info/PKG-INFO
--rw-r--r--   0 moritz     (501) staff       (20)      502 2022-07-25 09:22:43.000000 sniffles-2.0.7/src/sniffles.egg-info/SOURCES.txt
--rw-r--r--   0 moritz     (501) staff       (20)        1 2022-07-25 09:22:43.000000 sniffles-2.0.7/src/sniffles.egg-info/dependency_links.txt
--rw-r--r--   0 moritz     (501) staff       (20)       14 2022-07-25 09:22:43.000000 sniffles-2.0.7/src/sniffles.egg-info/requires.txt
--rw-r--r--   0 moritz     (501) staff       (20)        9 2022-07-25 09:22:43.000000 sniffles-2.0.7/src/sniffles.egg-info/top_level.txt
+drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     1070 2023-03-26 18:37:33.000000 sniffles-2.2/LICENSE
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     4486 2023-07-27 18:10:34.749090 sniffles-2.2/PKG-INFO
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     3905 2023-07-27 17:54:14.000000 sniffles-2.2/README.md
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      104 2023-03-26 18:37:33.000000 sniffles-2.2/pyproject.toml
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      775 2023-07-27 18:10:34.753089 sniffles-2.2/setup.cfg
+drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/src/
+drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/src/sniffles/
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      190 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/__init__.py
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    14161 2023-07-06 18:59:06.000000 sniffles-2.2/src/sniffles/cluster.py
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    23091 2023-07-06 16:32:31.000000 sniffles-2.2/src/sniffles/config.py
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    15172 2023-07-06 16:58:35.000000 sniffles-2.2/src/sniffles/consensus.py
+-rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    24947 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/leadprov.py
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    15210 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/parallel.py
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)    17006 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/postprocessing.py
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     5108 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/snf.py
+-rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    26976 2023-07-06 17:01:28.000000 sniffles-2.2/src/sniffles/sniffles
+-rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    19538 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/sv.py
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     3283 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/util.py
+-rwxr-xr-x   0 lpaz      (1000) lpaz      (1000)    15909 2023-03-26 18:37:33.000000 sniffles-2.2/src/sniffles/vcf.py
+drwxrwxr-x   0 lpaz      (1000) lpaz      (1000)        0 2023-07-27 18:10:34.749090 sniffles-2.2/src/sniffles.egg-info/
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)     4486 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/PKG-INFO
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)      502 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)        1 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)       14 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/requires.txt
+-rw-rw-r--   0 lpaz      (1000) lpaz      (1000)        9 2023-07-27 18:10:34.000000 sniffles-2.2/src/sniffles.egg-info/top_level.txt
```

### Comparing `sniffles-2.0.7/LICENSE` & `sniffles-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sniffles-2.0.7/PKG-INFO` & `sniffles-2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.0.7
+Version: 2.2
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
-Author: Moritz Smolka
-Author-email: moritz.g.smolka@gmail.com
+Author: Moritz Smolka, Luis Paulin
+Author-email: moritz.g.smolka@gmail.com, lfpaulin@gmail.com
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sniffles2
 A fast structural variant caller for long-read sequencing, Sniffles2 accurately detect SVs on germline, somatic and population-level for PacBio and Oxford Nanopore read data.
 
 ## Quick Start: Germline SV calling using Sniffles2
@@ -32,30 +32,30 @@
 
 or
 
 `conda install sniffles=2.0 `
 
 If you previously installed Sniffles1 using conda and want to upgrade to Sniffles2, you can use:
 
-`conda update sniffles=2.0`
+`conda update sniffles=2.2`
 
 ## Requirements
-* Python >= 3.7
+* Python >= 3.8
 * pysam
 
 #### Tested on:
 * python==3.9.5
 * pysam==0.16.0.1
 
 ## Citation
 Please cite our paper at:
 
 https://www.nature.com/articles/s41592-018-0001-7
 
-A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1 
+A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1
 
 ## Use-Cases / Modes
 
 ### A. General (all Modes)
 * To output deletion (DEL SV) sequences, the reference genome (.fasta) must be specified using e.g. `--reference reference.fasta`.
 * Sniffles2 supports optionally specifying tandem repeat region annotations (.bed), which can improve calling in these regions `--tandem-repeats annotations.bed`. Sniffles2 compatible tandem repeat annotations for human references can be found in the [annotations/ folder](https://github.com/fritzsedlazeck/Sniffles/tree/master/annotations).
 * Sniffles2 is fully parallelized and uses 4 threads by default. This value can be adapted using e.g. `--threads 4` as option. Memory requirements will increase with the number of threads used.
@@ -66,23 +66,27 @@
 
 1. Call SV candidates and create an associated .snf file for each sample: `sniffles --input sample1.bam --snf sample1.snf`
 2. Combined calling using multiple .snf files into a single .vcf: `sniffles --input sample1.snf sample2.snf ... sampleN.snf --vcf multisample.vcf`
 
 Alternatively, for step 2. you can supply a .tsv file, containing a list of .snf files, and custom sample ids in an optional second column (one sample per line), .e.g.:
 2. Combined calling using a .tsv as sample list: `sniffles --input snf_files_list.tsv --vcf multisample.vcf`
 
-### C. Non-Germline SV Calling (Somatic)
-To call non-germline SVs (i.e. somatic/mosaic) SVs, the *--non-germline* option should be added, i.e.:
+### C. Mosaic SV Calling (Non-germline or somatic SVs)
+To call mosaic SVs, the *--mosaic* option should be added, i.e.:
 
-`sniffles --input mapped_input.bam --vcf output.vcf --non-germline`
+`sniffles --input mapped_input.bam --vcf output.vcf --mosaic`
 
 ### D. Genotyping a known set of SVs (Force Calling)
 Example command, to determine the genotype of each SV in *input_known_svs.vcf* for *sample.bam* and write the re-genotyped SVs to *output_genotypes.vcf*:
 
 `sniffles --input sample.bam --genotype-vcf input_known_svs.vcf --vcf output_genotypes.vcf`
 
 ## Quick Tips
 
 ### Input / Output
 * .bam or .cram files containing long read alignments (i.e. from minimap2 or ngmlr) are supported as input
 * .vcf.gz (bgzipped+tabix indexed) output is supported
 * Simultaneous output of both .vcf and .snf file (for multi-sample calling) is supported
+
+## Companion apps
+* We have developed a plotting tools for Sniffles2: [https://github.com/farhangus/sniffle2_plot](https://github.com/farhangus/sniffle2_plot)
+* We also provide VCF and scripts used for the manuscript [https://github.com/smolkmo/Sniffles2-Supplement](https://github.com/smolkmo/Sniffles2-Supplement)
```

### Comparing `sniffles-2.0.7/README.md` & `sniffles-2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 
 or
 
 `conda install sniffles=2.0 `
 
 If you previously installed Sniffles1 using conda and want to upgrade to Sniffles2, you can use:
 
-`conda update sniffles=2.0`
+`conda update sniffles=2.2`
 
 ## Requirements
-* Python >= 3.7
+* Python >= 3.8
 * pysam
 
 #### Tested on:
 * python==3.9.5
 * pysam==0.16.0.1
 
 ## Citation
 Please cite our paper at:
 
 https://www.nature.com/articles/s41592-018-0001-7
 
-A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1 
+A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1
 
 ## Use-Cases / Modes
 
 ### A. General (all Modes)
 * To output deletion (DEL SV) sequences, the reference genome (.fasta) must be specified using e.g. `--reference reference.fasta`.
 * Sniffles2 supports optionally specifying tandem repeat region annotations (.bed), which can improve calling in these regions `--tandem-repeats annotations.bed`. Sniffles2 compatible tandem repeat annotations for human references can be found in the [annotations/ folder](https://github.com/fritzsedlazeck/Sniffles/tree/master/annotations).
 * Sniffles2 is fully parallelized and uses 4 threads by default. This value can be adapted using e.g. `--threads 4` as option. Memory requirements will increase with the number of threads used.
@@ -51,23 +51,27 @@
 
 1. Call SV candidates and create an associated .snf file for each sample: `sniffles --input sample1.bam --snf sample1.snf`
 2. Combined calling using multiple .snf files into a single .vcf: `sniffles --input sample1.snf sample2.snf ... sampleN.snf --vcf multisample.vcf`
 
 Alternatively, for step 2. you can supply a .tsv file, containing a list of .snf files, and custom sample ids in an optional second column (one sample per line), .e.g.:
 2. Combined calling using a .tsv as sample list: `sniffles --input snf_files_list.tsv --vcf multisample.vcf`
 
-### C. Non-Germline SV Calling (Somatic)
-To call non-germline SVs (i.e. somatic/mosaic) SVs, the *--non-germline* option should be added, i.e.:
+### C. Mosaic SV Calling (Non-germline or somatic SVs)
+To call mosaic SVs, the *--mosaic* option should be added, i.e.:
 
-`sniffles --input mapped_input.bam --vcf output.vcf --non-germline`
+`sniffles --input mapped_input.bam --vcf output.vcf --mosaic`
 
 ### D. Genotyping a known set of SVs (Force Calling)
 Example command, to determine the genotype of each SV in *input_known_svs.vcf* for *sample.bam* and write the re-genotyped SVs to *output_genotypes.vcf*:
 
 `sniffles --input sample.bam --genotype-vcf input_known_svs.vcf --vcf output_genotypes.vcf`
 
 ## Quick Tips
 
 ### Input / Output
 * .bam or .cram files containing long read alignments (i.e. from minimap2 or ngmlr) are supported as input
 * .vcf.gz (bgzipped+tabix indexed) output is supported
 * Simultaneous output of both .vcf and .snf file (for multi-sample calling) is supported
+
+## Companion apps
+* We have developed a plotting tools for Sniffles2: [https://github.com/farhangus/sniffle2_plot](https://github.com/farhangus/sniffle2_plot)
+* We also provide VCF and scripts used for the manuscript [https://github.com/smolkmo/Sniffles2-Supplement](https://github.com/smolkmo/Sniffles2-Supplement)
```

### Comparing `sniffles-2.0.7/setup.cfg` & `sniffles-2.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = sniffles
-version = 2.0.7
-author = Moritz Smolka
-author_email = moritz.g.smolka@gmail.com
+version = 2.2
+author = Moritz Smolka, Luis Paulin
+author_email = moritz.g.smolka@gmail.com, lfpaulin@gmail.com
 description = A fast structural variation caller for long-read sequencing data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritzsedlazeck/Sniffles
 project_urls = 
 	Bug Tracker = https://github.com/fritzsedlazeck/Sniffles/issues
 classifiers = 
@@ -14,17 +14,17 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
-	pysam>=0.16.0
+	pysam>=0.20.0
 scripts = 
 	src/sniffles/sniffles
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `sniffles-2.0.7/src/sniffles/cluster.py` & `sniffles-2.2/src/sniffles/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
         n=min(len(self.leads),max_n)
         if n==0:
             self.mean_svlen=0
             self.stdev_start=0
             return
 
+        # REVIEW: might need fix based on issue #407
         step=int(len(self.leads)/n)
         if n>1:
             self.mean_svlen=sum(self.leads[i].svlen for i in range(0,len(self.leads),step))/float(n)
             self.stdev_start=statistics.stdev(self.leads[i].ref_start for i in range(0,len(self.leads),step))
         else:
             self.mean_svlen=self.leads[0].svlen
             self.stdev_start=0
@@ -243,14 +244,20 @@
                 curr_cluster.leads_long+=next_cluster.leads_long
             curr_cluster.end=next_cluster.end
             curr_cluster.repeat=curr_cluster.repeat or next_cluster.repeat
             curr_cluster.compute_metrics()
             i=max(0,i-2)
         i+=1
 
+    if config.dev_trace_read:
+        for c in clusters:
+            for ld in c.leads:
+                if ld.read_qname==config.dev_trace_read:
+                    print(f"[DEV_TRACE_READ [2/4] [cluster.resolve] Read lead {ld} is in cluster {c.id}, containing a total of {len(c.leads)} leads")
+
     if config.dev_dump_clusters:
         filename=f"{config.input}.clusters.{svtype}.{leadtab_provider.contig}.{leadtab_provider.start}.{leadtab_provider.end}.bed"
         print(f"Dumping clusters to {filename}")
         with open(filename,"w") as h:
             for c in clusters:
                 info=f"ID={c.id}, #LEADS={len(c.leads)}; "
                 for ld in c.leads:
@@ -261,15 +268,15 @@
         if len(cluster.leads)==0:
             continue
 
         if svtype == "BND":
             if config.dev_no_resplit:
                 yield cluster
             else:
-                for new_cluster in resplit_bnd(cluster,merge_threshold=config.bnd_cluster_resplit):
+                for new_cluster in resplit_bnd(cluster,merge_threshold=config.cluster_merge_bnd):
                     yield new_cluster
         else:
             if svtype=="INS" or svtype=="DEL":
                 if cluster.repeat:
                     merge_inner_threshold=-1
                 else:
                     merge_inner_threshold=config.cluster_merge_pos
```

### Comparing `sniffles-2.0.7/src/sniffles/config.py` & `sniffles-2.2/src/sniffles/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 import sys
 import datetime
 import argparse
 
 from sniffles import util
 
 VERSION="Sniffles2"
-BUILD="2.0.7"
+BUILD="2.2"
 SNF_VERSION="S2_rc4"
 
 class ArgFormatter(argparse.ArgumentDefaultsHelpFormatter, argparse.RawDescriptionHelpFormatter):
     pass
 
 def tobool(v):
     if v==True or v==False:
         return v
-    elif v.lower()=="true" or v=="1":
+    elif v.strip().lower()=="true" or v.strip()=="1":
         return True
-    elif v.lower()=="false" or v=="0":
+    elif v.strip().lower()=="false" or v.strip()=="0":
         return False
     else:
         raise argparse.ArgumentTypeError("Boolean value (True | False) required for argument")
 
 def from_cmdline():
     header=f"Sniffles2: A fast structural variant (SV) caller for long-read sequencing data\n Version {BUILD}\n Contact: moritz.g.smolka@gmail.com"
     example=""" Usage example A - Call SVs for a single sample:
@@ -42,72 +42,73 @@
 
     ... OR, producing only a SNF file with SV candidates for later multi-sample calling:
       sniffles --input sample1.bam --snf sample1.snf
 
     ... OR, simultaneously producing a single-sample VCF and SNF file for later multi-sample calling:
       sniffles --input sample1.bam --vcf sample1.vcf.gz --snf sample1.snf
 
-    ... OR, with additional options to specify tandem repeat annotations (for improved call accuracy), reference (for DEL sequences) and non-germline mode for detecting rare SVs:
-      sniffles --input sample1.bam --vcf sample1.vcf.gz --tandem-repeats tandem_repeats.bed --reference genome.fa --non-germline
+    ... OR, with additional options to specify tandem repeat annotations (for improved call accuracy), reference (for DEL sequences) and mosaic mode for detecting rare SVs:
+      sniffles --input sample1.bam --vcf sample1.vcf.gz --tandem-repeats tandem_repeats.bed --reference genome.fa --mosaic
 
  Usage example B - Multi-sample calling:
     Step 1. Create .snf for each sample: sniffles --input sample1.bam --snf sample1.snf
     Step 2. Combined calling: sniffles --input sample1.snf sample2.snf ... sampleN.snf --vcf multisample.vcf
 
     ... OR, using a .tsv file containing a list of .snf files, and custom sample ids in an optional second column (one sample per line):
     Step 2. Combined calling: sniffles --input snf_files_list.tsv --vcf multisample.vcf
 
  Usage example C - Determine genotypes for a set of known SVs (force calling):
     sniffles --input sample.bam --genotype-vcf input_known_svs.vcf --vcf output_genotypes.vcf
     """
-    usage="sniffles --input SORTED_INPUT.bam [--vcf OUTPUT.vcf] [--snf MERGEABLE_OUTPUT.snf] [--threads 4] [--non-germline]\n\n" + header + "\n\n" + example + "\n\n Use --help for full parameter/usage information\n \n"
+    usage="sniffles --input SORTED_INPUT.bam [--vcf OUTPUT.vcf] [--snf MERGEABLE_OUTPUT.snf] [--threads 4] [--mosaic]\n\n" + header + "\n\n" + example + "\n\n Use --help for full parameter/usage information\n \n"
     parser = argparse.ArgumentParser(description="", epilog=example, formatter_class=lambda prog: ArgFormatter(prog,max_help_position=100,width=150), usage=usage)
     parser.add_argument("--version", action="version", version=f"Sniffles2, Version {BUILD}")
 
     main_args = parser.add_argument_group("Common parameters")
     main_args.add_argument("-i","--input", metavar="IN", type=str, help="For single-sample calling: A coordinate-sorted and indexed .bam/.cram (BAM/CRAM format) file containing aligned reads. - OR - For multi-sample calling: Multiple .snf files (generated before by running Sniffles2 for individual samples with --snf)", required=True, nargs="+")
     main_args.add_argument("-v","--vcf", metavar="OUT.vcf", type=str, help="VCF output filename to write the called and refined SVs to. If the given filename ends with .gz, the VCF file will be automatically bgzipped and a .tbi index built for it.", required=False)
     main_args.add_argument("--snf", metavar="OUT.snf", type=str, help="Sniffles2 file (.snf) output filename to store candidates for later multi-sample calling", required=False)
     main_args.add_argument("--reference", metavar="reference.fasta", type=str, help="(Optional) Reference sequence the reads were aligned against. To enable output of deletion SV sequences, this parameter must be set.", default=None)
     main_args.add_argument("--tandem-repeats", metavar="IN.bed", type=str, help="(Optional) Input .bed file containing tandem repeat annotations for the reference genome.", default=None)
-    main_args.add_argument("--non-germline", help="Call non-germline SVs (rare, somatic or mosaic SVs)", default=False, action="store_true")
     main_args.add_argument("--phase", help="Determine phase for SV calls (requires the input alignments to be phased)", default=False, action="store_true")
     main_args.add_argument("-t","--threads", metavar="N", type=int, help="Number of parallel threads to use (speed-up for multi-core CPUs)", default=4)
 
     filter_args = parser.add_argument_group("SV Filtering parameters")
     filter_args.add_argument("--minsupport", metavar="auto", type=str, help="Minimum number of supporting reads for a SV to be reported (default: automatically choose based on coverage)", default="auto")
-    filter_args.add_argument("--minsupport-auto-mult", metavar="0.1/0.025", type=float, help="Coverage based minimum support multiplier for germline/non-germline modes (only for auto minsupport) ", default=None)
-    filter_args.add_argument("--minsvlen", metavar="N", type=int, help="Minimum SV length (in bp)", default=35)
+    filter_args.add_argument("--minsupport-auto-mult", metavar="0.1/0.025", type=float, help="Coverage based minimum support multiplier for germline mode (only for auto minsupport) ", default=None)
+    filter_args.add_argument("--minsvlen", metavar="N", type=int, help="Minimum SV length (in bp)", default=50)
     filter_args.add_argument("--minsvlen-screen-ratio", metavar="N", type=float, help="Minimum length for SV candidates (as fraction of --minsvlen)", default=0.9)
-    filter_args.add_argument("--mapq", metavar="N", type=int, help="Alignments with mapping quality lower than this value will be ignored", default=25)
+    filter_args.add_argument("--mapq", metavar="N", type=int, help="Alignments with mapping quality lower than this value will be ignored", default=20)
     filter_args.add_argument("--no-qc", "--qc-output-all", help="Output all SV candidates, disregarding quality control steps.", default=False, action="store_true")
     filter_args.add_argument("--qc-stdev", help="Apply filtering based on SV start position and length standard deviation", metavar="True", type=tobool, default=True)
     filter_args.add_argument("--qc-stdev-abs-max", help="Maximum standard deviation for SV length and size (in bp)", metavar="N", type=int, default=500)
     filter_args.add_argument("--qc-strand", help="Apply filtering based on strand support of SV calls", metavar="False", type=tobool, default=False)
     filter_args.add_argument("--qc-coverage", help="Minimum surrounding region coverage of SV calls", metavar="N", type=int, default=1)
     filter_args.add_argument("--long-ins-length", help="Insertion SVs longer than this value are considered as hard to detect based on the aligner and read length and subjected to more sensitive filtering.", metavar="2500", type=int, default=2500)
-    filter_args.add_argument("--long-del-length", help="Deletion SVs longer than this value are subjected to central coverage drop-based filtering (Not applicable for --non-germline)", metavar="50000", type=int, default=50000)
-    filter_args.add_argument("--long-del-coverage", help="Long deletions with central coverage (in relation to upstream/downstream coverage) higher than this value will be filtered (Not applicable for --non-germline)", metavar="0.66", type=float, default=0.66)
-    filter_args.add_argument("--long-dup-length", help="Duplication SVs longer than this value are subjected to central coverage increase-based filtering (Not applicable for --non-germline)", metavar="50000", type=int, default=50000)
-    filter_args.add_argument("--long-dup-coverage", help="Long duplications with central coverage (in relation to upstream/downstream coverage) lower than this value will be filtered (Not applicable for --non-germline)", metavar="1.33", type=float, default=1.33)
+    filter_args.add_argument("--long-del-length", help="Deletion SVs longer than this value are subjected to central coverage drop-based filtering (Not applicable for --mosaic)", metavar="50000", type=int, default=50000)
+    filter_args.add_argument("--long-del-coverage", help="Long deletions with central coverage (in relation to upstream/downstream coverage) higher than this value will be filtered (Not applicable for --mosaic)", metavar="0.66", type=float, default=0.66)
+    filter_args.add_argument("--long-dup-length", help="Duplication SVs longer than this value are subjected to central coverage increase-based filtering (Not applicable for --mosaic)", metavar="50000", type=int, default=50000)
+    filter_args.add_argument("--qc-bnd-filter-strand", help="Filter breakends that do not have support for both strands", type=tobool, default=True)
+    filter_args.add_argument("--bnd-min-split-length", help="Minimum length of read splits to be considered for breakends", type=int, default=1000)
+    filter_args.add_argument("--long-dup-coverage", help="Long duplications with central coverage (in relation to upstream/downstream coverage) lower than this value will be filtered (Not applicable for --mosaic)", metavar="1.33", type=float, default=1.33)
     filter_args.add_argument("--max-splits-kb", metavar="N", type=float, help="Additional number of splits per kilobase read sequence allowed before reads are ignored", default=0.1)
     filter_args.add_argument("--max-splits-base", metavar="N", type=int, help="Base number of splits allowed before reads are ignored (in addition to --max-splits-kb)", default=3)
     filter_args.add_argument("--min-alignment-length", metavar="N", type=int, help="Reads with alignments shorter than this length (in bp) will be ignored", default=1000)
     filter_args.add_argument("--phase-conflict-threshold", metavar="F", type=float, help="Maximum fraction of conflicting reads permitted for SV phase information to be labelled as PASS (only for --phase)", default=0.1)
     filter_args.add_argument("--detect-large-ins", help="Infer insertions that are longer than most reads and therefore are spanned by few alignments only.", metavar="True", type=tobool, default=True)
     #filter_args.add_argument("--large-ins-threshold", metavar="N", type=int, help="Minimum clipping at read ends to be considered a potential large insertion (only with --detect-large-ins)", default=5000)
 
     cluster_args = parser.add_argument_group("SV Clustering parameters")
     cluster_args.add_argument("--cluster-binsize", metavar="N", type=int, help="Initial screening bin size in bp", default=100)
     cluster_args.add_argument("--cluster-r", metavar="R", type=float, help="Multiplier for SV start position standard deviation criterion in cluster merging", default=2.5)
     cluster_args.add_argument("--cluster-repeat-h", metavar="H", type=float, help="Multiplier for mean SV length criterion for tandem repeat cluster merging", default=1.5)
     cluster_args.add_argument("--cluster-repeat-h-max", metavar="N", type=float, help="Max. merging distance based on SV length criterion for tandem repeat cluster merging", default=1000)
     cluster_args.add_argument("--cluster-merge-pos", metavar="N", type=int, help="Max. merging distance for insertions and deletions on the same read and cluster in non-repeat regions", default=150)
     cluster_args.add_argument("--cluster-merge-len", metavar="F", type=float, help="Max. size difference for merging SVs as fraction of SV length", default=0.33)
-    cluster_args.add_argument("--cluster-merge-bnd", metavar="N", type=int, help="Max. merging distance for breakend SV candidates.", default=1500)
+    cluster_args.add_argument("--cluster-merge-bnd", metavar="N", type=int, help="Max. merging distance for breakend SV candidates.", default=1000)
 
     genotype_args = parser.add_argument_group("SV Genotyping parameters")
     genotype_args.add_argument("--genotype-ploidy", metavar="N", type=int, help="Sample ploidy (currently fixed at value 2)", default=2)
     genotype_args.add_argument("--genotype-error", metavar="N", type=float, help="Estimated false positve rate for leads (relating to total coverage)", default=0.05)
     genotype_args.add_argument("--sample-id", type=str, help="Custom ID for this sample, used for later multi-sample calling (stored in .snf)", default=None)
     genotype_args.add_argument("--genotype-vcf", metavar="IN.vcf", type=str, help="Determine the genotypes for all SVs in the given input .vcf file (forced calling). Re-genotyped .vcf will be written to the output file specified with --vcf.", default=None)
 
@@ -115,29 +116,44 @@
     multi_args.add_argument("--combine-high-confidence", metavar="F", type=float, help="Minimum fraction of samples in which a SV needs to have individually passed QC for it to be reported in combined output (a value of zero will report all SVs that pass QC in at least one of the input samples)", default=0.0)
     multi_args.add_argument("--combine-low-confidence", metavar="F", type=float, help="Minimum fraction of samples in which a SV needs to be present (failed QC) for it to be reported in combined output", default=0.2)
     multi_args.add_argument("--combine-low-confidence-abs", metavar="N", type=int, help="Minimum absolute number of samples in which a SV needs to be present (failed QC) for it to be reported in combined output", default=2)
     multi_args.add_argument("--combine-null-min-coverage", metavar="N", type=int, help="Minimum coverage for a sample genotype to be reported as 0/0 (sample genotypes with coverage below this threshold at the SV location will be output as ./.)", default=5)
     multi_args.add_argument("--combine-match", metavar="N", type=int, help="Multiplier for maximum deviation of multiple SV's start/end position for them to be combined across samples. Given by max_dev=M*sqrt(min(SV_length_a,SV_length_b)), where M is this parameter.", default=250)
     multi_args.add_argument("--combine-match-max", metavar="N", type=int, help="Upper limit for the maximum deviation computed for --combine-match, in bp.", default=1000)
     multi_args.add_argument("--combine-separate-intra", help="Disable combination of SVs within the same sample", default=False, action="store_true")
-    multi_args.add_argument("--combine-output-filtered", help="Include low-confidence / putative non-germline SVs in multi-calling", default=False, action="store_true")
+    multi_args.add_argument("--combine-output-filtered", help="Include low-confidence / mosaic SVs in multi-calling", default=False, action="store_true")
+    multi_args.add_argument("--combine-pair-relabel", help="Override low-quality genotypes when combining 2 samples (may be used for e.g. tumor-normal comparisons)", default=False, action="store_true")
+    multi_args.add_argument("--combine-pair-relabel-threshold", help="Genotype quality below which a genotype call will be relabeled", default=20, type=int)
+    multi_args.add_argument("--combine-close-handles", help="Close .SNF file handles after each use. May lower performance, but may be required when maximum number of file handles supported by OS is reached when merging many samples.", default=False, action="store_true")
     #multi_args.add_argument("--combine-exhaustive", help="(DEV) Disable performance optimization in multi-calling", default=False, action="store_true")
     #multi_args.add_argument("--combine-relabel-rare", help="(DEV)", default=False, action="store_true")
     #multi_args.add_argument("--combine-with-missing", help="(DEV)", default=False, action="store_true")
 
     postprocess_args = parser.add_argument_group("SV Postprocessing, QC and output parameters")
     postprocess_args.add_argument("--output-rnames", help="Output names of all supporting reads for each SV in the RNAMEs info field", default=False, action="store_true")
     postprocess_args.add_argument("--no-consensus", help="Disable consensus sequence generation for insertion SV calls (may improve performance)", default=False, action="store_true")
     postprocess_args.add_argument("--no-sort", help="Do not sort output VCF by genomic coordinates (may slightly improve performance)", default=False, action="store_true")
     postprocess_args.add_argument("--no-progress", help="Disable progress display", default=False, action="store_true")
     postprocess_args.add_argument("--quiet", help="Disable all logging, except errors", default=False, action="store_true")
     postprocess_args.add_argument("--max-del-seq-len", metavar="N", type=int, help="Maximum deletion sequence length to be output. Deletion SVs longer than this value will be written to the output as symbolic SVs.", default=50000)
     postprocess_args.add_argument("--symbolic", help="Output all SVs as symbolic, including insertions and deletions, instead of reporting nucleotide sequences.", default=False, action="store_true")
     postprocess_args.add_argument("--allow-overwrite", help="Allow overwriting output files if already existing", default=False, action="store_true")
 
+    mosaic_args = parser.add_argument_group("Mosaic calling mode parameters")
+    mosaic_args.add_argument("--mosaic", help="Set Sniffles run mode to detect rare, somatic and mosaic SVs", default=False, action="store_true")
+    mosaic_args.add_argument("--mosaic-af-max", help="Maximum allele frequency for which SVs are considered mosaic", metavar="F", default=0.3, type=float)
+    mosaic_args.add_argument("--mosaic-af-min", help="Minimum allele frequency for mosaic SVs to be output", metavar="F", default=0.05, type=float)
+    mosaic_args.add_argument("--mosaic-qc-invdup-min-length", help="Minimum SV length for mosaic inversion and duplication SVs", metavar="N", default=500, type=int)
+    mosaic_args.add_argument("--mosaic-qc-nm", default=True, action="store_true", help=argparse.SUPPRESS)
+    mosaic_args.add_argument("--mosaic-qc-nm-mult", metavar="F", type=float, default=1.66, help=argparse.SUPPRESS)
+    mosaic_args.add_argument("--mosaic-qc-coverage-max-change-frac", help="Maximum relative coverage change across SV breakpoints", metavar="F", type=float, default=0.1)
+    mosaic_args.add_argument("--mosaic-qc-strand", help="Apply filtering based on strand support of SV calls", metavar="True", type=tobool, default=True)
+    mosaic_args.add_argument("--mosaic-include-germline", help="Report germline SVs as well in mosaic mode", default=False, action="store_true")
+
+
     developer_args = parser.add_argument_group("Developer parameters")
     developer_args.add_argument("--dev-cache", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-cache-dir", metavar="PATH", type=str, default=None, help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-debug-svtyping", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-keep-lowqual-splits", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-call-region", metavar="REGION", type=str, default=None, help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-dump-clusters", default=False, action="store_true", help=argparse.SUPPRESS)
@@ -149,20 +165,25 @@
     developer_args.add_argument("--dev-dump-coverage", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-no-resplit", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-no-resplit-repeat", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--dev-skip-snf-validation", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--low-memory", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--repeat", default=False, action="store_true", help=argparse.SUPPRESS)
     developer_args.add_argument("--qc-nm", default=False, action="store_true", help=argparse.SUPPRESS)
-    developer_args.add_argument("--qc-nm-max", metavar="F", type=float, default=0.2, help=argparse.SUPPRESS)
+    developer_args.add_argument("--qc-nm-mult", metavar="F", type=float, default=1.66, help=argparse.SUPPRESS)
+    developer_args.add_argument("--qc-coverage-max-change-frac", help="Maximum relative coverage change across SV breakpoints", metavar="F", type=float, default=-1)
     developer_args.add_argument("--coverage-updown-bins", metavar="N", type=int, default=5, help=argparse.SUPPRESS)
     developer_args.add_argument("--coverage-shift-bins", metavar="N", type=int, default=3, help=argparse.SUPPRESS)
     developer_args.add_argument("--coverage-shift-bins-min-aln-length", metavar="N", type=int, default=1000, help=argparse.SUPPRESS)
     developer_args.add_argument("--cluster-binsize-combine-mult", metavar="N", type=int, default=5, help=argparse.SUPPRESS)
     developer_args.add_argument("--cluster-resplit-binsize", metavar="N", type=int, default=20, help=argparse.SUPPRESS)
+    developer_args.add_argument("--dev-trace-read", default=False, metavar="read_id", type=str, help=argparse.SUPPRESS)
+    developer_args.add_argument("--dev-split-max-query-distance-mult", metavar="N", type=int, default=5, help=argparse.SUPPRESS)
+
+
     #developer_args.add_argument("--qc-strand", help="(DEV)", default=False, action="store_true")
 
     config=parser.parse_args()
 
     if config.quiet:
         sys.stdout=open(os.devnull,"w")
 
@@ -194,21 +215,15 @@
         config.minsupport=int(config.minsupport)
 
     #--minsupport auto defaults
     config.minsupport_auto_base=1.5
     config.minsupport_auto_regional_coverage_weight=0.75
 
     if config.minsupport_auto_mult==None:
-        if config.non_germline:
-            config.minsupport_auto_mult=0.025
-        else:
-            config.minsupport_auto_mult=0.1
-
-    if config.non_germline:
-        config.qc_nm=True
+        config.minsupport_auto_mult=0.1
 
     config.coverage_binsize=config.cluster_binsize
     config.coverage_binsize_combine=config.cluster_binsize*config.cluster_binsize_combine_mult
 
 
     #INS Consensus parameters
     #config.consensus_max_reads=20
@@ -221,27 +236,25 @@
 
     #Large INS
     config.long_ins_rescale_base=1.66
     config.long_ins_rescale_mult=0.33
 
     #BND
     config.bnd_cluster_length=1000
-    config.bnd_cluster_resplit=0
 
     #Genotyping
     config.genotype_format="GT:GQ:DR:DV"
     config.genotype_none=(".",".",0,0,0,None)
     config.genotype_null=(0,0,0,0,0,None)
     config.genotype_min_z_score=5
     if config.genotype_ploidy!=2:
         util.fatal_error("Currently only --genotype-ploidy 2 is supported")
 
     #SNF
     config.snf_block_size=10**5
-    config.snf_combine_keep_open=True #Keep file handles open during .snf combining (might be an issue if the number of .snf files to merge is very large)
 
     #Combine
     config.combine_exhaustive=False
     config.combine_relabel_rare=False
     config.combine_overlap_abs=2500
     config.combine_min_size=100
 
@@ -251,8 +264,19 @@
     config.id_prefix="Sniffles2."
     config.phase_identifiers=["1","2"]
 
     config.dev_profile=False
 
     config.workdir=os.getcwd()
 
+    #Mosaic
+    if config.mosaic_include_germline:
+        config.mosaic=True
+
+    config.qc_nm_measure=config.qc_nm
+    if config.mosaic:
+        #config.qc_coverage_max_change_frac=config.mosaic_qc_coverage_max_change_frac
+        config.qc_nm_measure=config.qc_nm_measure or config.mosaic_qc_nm
+        #config.qc_nm_mult=config.mosaic_qc_nm_mult
+        #config.qc_strand=config.mosaic_qc_strand
+
     return config
```

### Comparing `sniffles-2.0.7/src/sniffles/consensus.py` & `sniffles-2.2/src/sniffles/consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,14 +350,15 @@
                     h+=1
                 if ident/float(len(buffer)) > minident and ident>minident_abs:
                     conseq_new.append("".join(buffer))
                 else:
                     conseq_new.append("-"*len(buffer))
         conseq="".join(conseq_new)
 
+        # FIXME: can lead to ZeroDivisionError
         if span/float(len(best_lead.seq)) > minspan:
             alignments.append(conseq)
 
     maxal=1
     for i in range(len(best_lead.seq)):
         maxal=max(maxal,len([best_lead.seq[i]]+[a[i] for a in alignments if not a[i] in "^_"]))
     maxal=float(maxal)
```

### Comparing `sniffles-2.0.7/src/sniffles/leadprov.py` & `sniffles-2.2/src/sniffles/leadprov.py`

 * *Files 19% similar despite different names*

```diff
@@ -158,14 +158,15 @@
     strand="-" if read.is_reverse else "+"
     CINS=pysam.CINS
     CDEL=pysam.CDEL
     CSOFT_CLIP=pysam.CSOFT_CLIP
 
     pos_read=0
     pos_ref=read.reference_start
+
     for op,oplength in read.cigartuples:
         add_read,add_ref,event=OPLIST[op]
         if event and oplength >= minsvlen:
             if op==CINS:
                 yield Lead(read_id,
                            qname,
                            contig,
@@ -208,14 +209,42 @@
                            "INLINE",
                            "INS",
                            None,
                            seq=None)
         pos_read+=add_read*oplength
         pos_ref+=add_ref*oplength
 
+def get_cigar_indels(read_id,read,contig,config,use_clips,read_nm):
+    minsvlen=config.minsvlen_screen
+    longinslen=config.long_ins_length/2.0
+    seq_cache_maxlen=config.dev_seq_cache_maxlen
+    qname=read.query_name
+    mapq=read.mapping_quality
+    strand="-" if read.is_reverse else "+"
+    CINS=pysam.CINS
+    CDEL=pysam.CDEL
+    CSOFT_CLIP=pysam.CSOFT_CLIP
+
+    INS_SUM=0
+    DEL_SUM=0
+
+    pos_read=0
+    pos_ref=read.reference_start
+    for op,oplength in read.cigartuples:
+        add_read,add_ref,event=OPLIST[op]
+        if event:
+            if op==CINS:
+                INS_SUM+=oplength
+            elif op==CDEL:
+                DEL_SUM+=oplength
+        pos_read+=add_read*oplength
+        pos_ref+=add_ref*oplength
+
+    return INS_SUM,DEL_SUM
+
 def read_itersplits_bnd(read_id,read,contig,config,read_nm):
     assert(read.is_supplementary)
     #SA:refname,pos,strand,CIGAR,MAPQ,NM
     all_leads=[]
     supps=[part.split(",") for part in read.get_tag("SA").split(";") if len(part)>0]
 
     if len(supps) > config.max_splits_base + config.max_splits_kb*(read.query_length/1000.0):
@@ -272,15 +301,15 @@
                               refname,
                               pos_zero,
                               pos_zero + refspan,
                               split_qry_start,
                               split_qry_start+readspan,
                               strand,
                               mapq,
-                              nm/float(readspan+1),
+                              read_nm,
                               "SPLIT_SUP",
                               "?"))
 
     sv.classify_splits(read,all_leads,config,contig)
 
     for lead in all_leads:
         for svtype, svstart, arg in lead.svtypes_starts_lens:
@@ -303,18 +332,22 @@
                 #print(lead.contig,svstart,bnd.bnd_info)
                 yield bnd
 
 def read_itersplits(read_id,read,contig,config,read_nm):
     #SA:refname,pos,strand,CIGAR,MAPQ,NM
     all_leads=[]
     supps=[part.split(",") for part in read.get_tag("SA").split(";") if len(part)>0]
+    trace_read=config.dev_trace_read!=False and config.dev_trace_read==read.query_name
 
     if len(supps) > config.max_splits_base + config.max_splits_kb*(read.query_length/1000.0):
         return
 
+    if trace_read:
+        print(f"[DEV_TRACE_READ] [0c/4] [LeadProvider.read_itersplits] [{read.query_name}] passed max_splits check")
+
     #QC on: 18Aug21, HG002.ont.chr22; O.K.
     #cigarl=CIGAR_tolist(read.cigarstring)
     #if read.is_reverse:
     #    cigarl.reverse()
 
     #if read.is_reverse:
     #    assert(read.query_length-read.query_alignment_end == CIGAR_listreadstart(cigarl))
@@ -372,28 +405,48 @@
                               refname,
                               pos_zero,
                               pos_zero + refspan,
                               split_qry_start,
                               split_qry_start+readspan,
                               strand,
                               mapq,
-                              nm/float(readspan+1),
+                              read_nm,
                               "SPLIT_SUP",
                               "?"))
 
         #QC on: 08Sep21; O.K.
         #cigarl=CIGAR_tolist(cigar)
         #assert(CIGAR_listrefspan(cigarl)==refspan)
         #assert(CIGAR_listreadspan(cigarl)==readspan)
         #assert(CIGAR_listreadstart_fwd(cigarl)==readstart_fwd)
         #assert(CIGAR_listreadstart_rev(cigarl)==readstart_rev)
         #End QC
 
+    if trace_read:
+        print(f"[DEV_TRACE_READ] [0c/4] [LeadProvider.read_itersplits] [{read.query_name}] all_leads: {all_leads}")
+
     sv.classify_splits(read,all_leads,config,contig)
 
+    if trace_read:
+        print(f"[DEV_TRACE_READ] [0c/4] [LeadProvider.read_itersplits] [{read.query_name}] classify_splits(all_leads): {all_leads}")
+
+
+    """
+    if config.dev_trace_read != False:
+        print(read.query_name)
+        if read.query_name == config.dev_trace_read:
+            for lead_i, lead in enumerate(all_leads):
+                for svtype, svstart, arg in lead.svtypes_starts_lens:
+                    min_mapq=min(lead.mapq,all_leads[max(0,lead_i-1)].mapq)
+                    keep=True
+                    if not config.dev_keep_lowqual_splits and min_mapq < config.mapq:
+                        keep=False
+                    print(f"[DEV_TRACE_READ] [REPORT_LEAD_SPLIT] Splits identified from read {read.read_id}")
+    """
+
     for lead_i, lead in enumerate(all_leads):
         for svtype, svstart, arg in lead.svtypes_starts_lens:
             min_mapq=min(lead.mapq,all_leads[max(0,lead_i-1)].mapq)
             if not config.dev_keep_lowqual_splits and min_mapq < config.mapq:
                 continue
 
             if svtype=="BND":
@@ -484,15 +537,14 @@
 
         externals=[]
         ld_binsize=self.config.cluster_binsize
 
         for ld in self.iter_region(bam,contig,start,end):
             ld_contig,ld_ref_start=ld.contig,ld.ref_start
 
-            #TODO: Handle leads overlapping region ends (start/end)
             if contig==ld_contig and ld_ref_start >= start and ld_ref_start < end:
                 pos_leadtab=int(ld_ref_start/ld_binsize)*ld_binsize
                 self.record_lead(ld,pos_leadtab)
             else:
                 externals.append(ld)
 
         if self.config.dev_cache:
@@ -503,21 +555,28 @@
     def iter_region(self,bam,contig,start=None,end=None):
         leads_all=[]
         binsize=self.config.cluster_binsize
         coverage_binsize=self.config.coverage_binsize
         coverage_shift_bins=self.config.coverage_shift_bins
         coverage_shift_min_aln_len=self.config.coverage_shift_bins_min_aln_length
         long_ins_threshold=self.config.long_ins_length*0.5
-        qc_nm=self.config.qc_nm
+        qc_nm=self.config.qc_nm_measure
         phase=self.config.phase
         advanced_tags=qc_nm or phase
         mapq_min=self.config.mapq
         alen_min=self.config.min_alignment_length
+        nm_sum=0
+        nm_count=0
+        trace_read=self.config.dev_trace_read
 
         for read in bam.fetch(contig,start,end,until_eof=False):
+            if trace_read!=False:
+                if trace_read==read.query_name:
+                    print(f"[DEV_TRACE_READ] [0b/4] [LeadProvider.iter_region] [{contig}:{start}-{end}] [{read.query_name}] has been fetched and is entering pre-filtering")
+
             #if self.read_count % 1000000 == 0:
             #    gc.collect()
             if read.reference_start < start or read.reference_start >= end:
                 continue
 
             self.read_id+=1
             self.read_count+=1
@@ -530,30 +589,56 @@
             use_clips=self.config.detect_large_ins and not read.is_supplementary and not has_sa
 
             nm=-1
             curr_read_id=self.read_id
             if advanced_tags:
                 if qc_nm:
                     if read.has_tag("NM"):
-                        nm=read.get_tag("NM")/float(read.query_alignment_length+1)
+                        nm_raw=read.get_tag("NM")
+                        nm_ratio=read.get_tag("NM")/float(read.query_alignment_length+1)
+                        ins_sum,del_sum=get_cigar_indels(curr_read_id,read,contig,self.config,use_clips,read_nm=nm)
+                        nm_adj=(nm_raw-(ins_sum+del_sum))
+                        nm_adj_ratio=nm_adj/float(read.query_alignment_length+1)
+                        nm=nm_adj_ratio
+                        nm_sum+=nm
+                        nm_count+=1
 
                 if phase:
                     curr_read_id=(self.read_id,str(read.get_tag("HP")) if read.has_tag("HP") else "NULL",str(read.get_tag("PS")) if read.has_tag("PS") else "NULL")
 
+            if trace_read!=False:
+                if trace_read==read.query_name:
+                    print(f"[DEV_TRACE_READ] [0b/4] [LeadProvider.iter_region] [{contig}:{start}-{end}] [{read.query_name}] passed pre-filtering (whole-read), begin to extract leads")
+
             #Extract small indels
             for lead in read_iterindels(curr_read_id,read,contig,self.config,use_clips,read_nm=nm):
+                if trace_read!=False:
+                    if trace_read==read.query_name:
+                        print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_iterindels] [{contig}:{start}-{end}] [{read.query_name}] new lead: {lead}")
                 yield lead
 
             #Extract read splits
             if has_sa:
                 if read.is_supplementary:
+                    if trace_read!=False:
+                        if trace_read==read.query_name:
+                            print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits_bnd] [{contig}:{start}-{end}] [{read.query_name}] is entering read_itersplits_bnd")
                     for lead in read_itersplits_bnd(curr_read_id,read,contig,self.config,read_nm=nm):
+                        if trace_read!=False:
+                            if trace_read==read.query_name:
+                                print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits_bnd] [{contig}:{start}-{end}] [{read.query_name}] new lead: {lead}")
                         yield lead
                 else:
+                    if trace_read!=False:
+                        if trace_read==read.query_name:
+                            print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits] [{contig}:{start}-{end}] [{read.query_name}] is entering read_itersplits")
                     for lead in read_itersplits(curr_read_id,read,contig,self.config,read_nm=nm):
+                        if trace_read!=False:
+                            if trace_read==read.query_name:
+                                print(f"[DEV_TRACE_READ] [1/4] [leadprov.read_itersplits] [{contig}:{start}-{end}] [{read.query_name}] new lead: {lead}")
                         yield lead
 
             #Record in coverage table
             read_end=read.reference_start+read.reference_length
             assert(read_end==read.reference_end)
             #assert(read_end>=read.reference_start)
             if read.is_reverse:
@@ -566,14 +651,18 @@
             if covr_end_bin > covr_start_bin:
                 self.covrtab_min_bin=min(self.covrtab_min_bin,covr_start_bin)
                 target_tab[covr_start_bin]=target_tab[covr_start_bin]+1 if covr_start_bin in target_tab else 1
 
                 if read_end <= self.end:
                     target_tab[covr_end_bin]=target_tab[covr_end_bin]-1 if covr_end_bin in target_tab else -1
 
+        self.config.average_regional_nm=nm_sum/float(max(1,nm_count))
+        self.config.qc_nm_threshold=self.config.average_regional_nm
+        #print(f"Contig {contig} avg. regional NM={self.config.average_regional_nm}, threshold={self.config.qc_nm_threshold}")
+
 
     def dev_leadtab_filename(self,contig,start,end):
         scriptloc=os.path.dirname(os.path.realpath(sys.argv[0]))
         if self.config.dev_cache_dir==None:
             cache_dir=f"{scriptloc}/cache"
         else:
             cache_dir=self.config.dev_cache_dir
```

### Comparing `sniffles-2.0.7/src/sniffles/parallel.py` & `sniffles-2.2/src/sniffles/parallel.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,24 @@
         return externals,self.lead_provider.read_count
 
     def call_candidates(self,keep_qc_fails,config):
         candidates=[]
         for svtype in sv.TYPES:
             for svcluster in cluster.resolve(svtype,self.lead_provider,config,self.tandem_repeats):
                 for svcall in sv.call_from(svcluster,config,keep_qc_fails,self):
+                    if config.dev_trace_read!=False:
+                        cluster_has_read=False
+                        for ld in svcluster.leads:
+                            if ld.read_qname==config.dev_trace_read:
+                                cluster_has_read=True
+                        if cluster_has_read:
+                            import copy
+                            svcall_copy=copy.deepcopy(svcall)
+                            svcall_copy.postprocess=None
+                            print(f"[DEV_TRACE_READ] [3/4] [Task.call_candidates] Read {config.dev_trace_read} -> Cluster {svcluster.id} -> preliminary SVCall {svcall_copy}")
                     candidates.append(svcall)
 
         self.coverage_average_fwd,self.coverage_average_rev=postprocessing.coverage(candidates,self.lead_provider,config)
         self.coverage_average_total=self.coverage_average_fwd+self.coverage_average_rev
         return candidates
 
     def finalize_candidates(self,candidates,keep_qc_fails,config):
@@ -62,29 +72,41 @@
             svcall.qc=svcall.qc and postprocessing.qc_sv_support(svcall,self.coverage_average_total,config)
             if not keep_qc_fails and not svcall.qc:
                 continue
 
             postprocessing.annotate_sv(svcall,config)
 
             svcall.qc=svcall.qc and postprocessing.qc_sv_post_annotate(svcall,config)
+
+            if config.dev_trace_read!=False:
+                cluster_has_read=False
+                for ld in svcall.postprocess.cluster.leads:
+                    if ld.read_qname==config.dev_trace_read:
+                        cluster_has_read=True
+                if cluster_has_read:
+                    import copy
+                    svcall_copy=copy.deepcopy(svcall)
+                    svcall_copy.postprocess=None
+                    print(f"[DEV_TRACE_READ] [4/4] [Task.finalize_candidates] Read {config.dev_trace_read} -> Cluster {svcall.postprocess.cluster.id} -> finalized SVCall, QC={svcall_copy.qc}: {svcall_copy}")
+
             if not keep_qc_fails and not svcall.qc:
                 continue
 
             svcall.finalize() #Remove internal information (not written to output) before sending to mainthread for VCF writing
             passed.append(svcall)
         return passed
 
     def combine(self,config):
         samples_headers_snf={}
         for snf_info in config.snf_input_info:
             snf_in=snf.SNFile(config,open(snf_info["filename"],"rb"),filename=snf_info["filename"])
             snf_in.read_header()
             samples_headers_snf[snf_info["internal_id"]]=(snf_info["filename"],snf_in.header,snf_in)
 
-            if not config.snf_combine_keep_open:
+            if config.combine_close_handles:
                 snf_in.close()
 
         svcalls=[]
 
         #block_groups_keep_threshold=5000
         #TODO: Parameterize
         bin_min_size=config.combine_min_size
```

### Comparing `sniffles-2.0.7/src/sniffles/postprocessing.py` & `sniffles-2.2/src/sniffles/postprocessing.py`

 * *Files 20% similar despite different names*

```diff
@@ -116,14 +116,16 @@
         coverage_rev_total+=coverage_rev
 
     average_coverage_fwd=coverage_fwd_total/float(n) if n>0 else 0
     average_coverage_rev=coverage_rev_total/float(n) if n>0 else 0
     return average_coverage_fwd,average_coverage_rev
 
 def qc_sv_support(svcall,coverage_global,config):
+    if config.mosaic:
+        return True
     if config.minsupport == "auto":
         if not qc_support_auto(svcall,coverage_global,config):
             svcall.filter="SUPPORT_MIN"
             return False
     else:
         if not qc_support_const(svcall,config):
             svcall.filter="SUPPORT_MIN"
@@ -161,14 +163,18 @@
     #return True
 
 def qc_support_const(svcall,config):
     #svcall.set_info("MINSUPPORT",config.minsupport)
     return svcall.support >= config.minsupport
 
 def qc_sv(svcall,config):
+    af=svcall.get_info("AF")
+    af=af if af!=None else 0
+    sv_is_mosaic = af <= config.mosaic_af_max
+
     if config.qc_stdev:
         stdev_pos=svcall.get_info("STDEV_POS")
         if stdev_pos > config.qc_stdev_abs_max:
             svcall.filter="STDEV_POS"
             return False
         if svcall.svtype!="BND" and stdev_pos / abs(svcall.svlen) > 2.0:
             svcall.filter="STDEV_POS"
@@ -183,38 +189,119 @@
                 svcall.filter="STDEV_LEN"
                 return False
 
     if abs(svcall.svlen) < config.minsvlen:
         svcall.filter="SVLEN_MIN"
         return False
 
+    if svcall.svtype=="BND":
+        if config.qc_bnd_filter_strand and len(set(l.strand for l in svcall.postprocess.cluster.leads))<2:
+            svcall.filter="STRAND"
+            return False
+    elif ((config.mosaic and sv_is_mosaic) and config.mosaic_qc_strand) or (not (config.mosaic and sv_is_mosaic) and config.qc_strand):
+        is_long_ins=(svcall.svtype=="INS" and svcall.svlen >= config.long_ins_length)
+        if not is_long_ins and len(set(l.strand for l in svcall.postprocess.cluster.leads))<2:
+            svcall.filter="STRAND"
+            return False
+
+    if config.mosaic and sv_is_mosaic:
+        if svcall.svtype=="INV" or svcall.svtype=="DUP" and svcall.svlen < config.mosaic_qc_invdup_min_length:
+            svcall.filter="SVLEN_MIN"
+            return False
+
     #if (svcall.coverage_upstream != None and svcall.coverage_upstream < config.qc_coverage) or (svcall.coverage_downstream != None and svcall.coverage_downstream < config.qc_coverage):
     if svcall.svtype != "DEL" and svcall.svtype != "INS" and (svcall.coverage_center != None and svcall.coverage_center < config.qc_coverage):
         svcall.filter="COV_MIN"
         return False
 
-    if svcall.svtype == "DEL" and config.long_del_length != -1 and abs(svcall.svlen) >= config.long_del_length and not config.non_germline:
+    if svcall.svtype == "DEL" and config.long_del_length != -1 and abs(svcall.svlen) >= config.long_del_length and not config.mosaic:
         if svcall.coverage_center != None and svcall.coverage_upstream != None and svcall.coverage_downstream != None and svcall.coverage_center > (svcall.coverage_upstream+svcall.coverage_downstream)/2.0 * config.long_del_coverage:
             svcall.filter="COV_CHANGE"
             return False
     elif svcall.svtype=="INS" and ( (svcall.coverage_upstream != None and svcall.coverage_upstream < config.qc_coverage) or (svcall.coverage_downstream != None and svcall.coverage_downstream < config.qc_coverage)):
         svcall.filter="COV_CHANGE"
         return False
-    elif svcall.svtype == "DUP" and config.long_dup_length != -1 and abs(svcall.svlen) >= config.long_dup_length and not config.non_germline:
+    elif svcall.svtype == "DUP" and config.long_dup_length != -1 and abs(svcall.svlen) >= config.long_dup_length and not config.mosaic:
         if svcall.coverage_center != None and svcall.coverage_upstream != None and svcall.coverage_downstream != None and svcall.coverage_center < (svcall.coverage_upstream+svcall.coverage_downstream)/2.0 * config.long_dup_coverage:
             svcall.filter="COV_CHANGE"
             return False
 
+    qc_coverage_max_change_frac=config.qc_coverage_max_change_frac
+    if config.mosaic and sv_is_mosaic:
+        qc_coverage_max_change_frac=config.mosaic_qc_coverage_max_change_frac
+    if qc_coverage_max_change_frac != -1.0:
+        if svcall.coverage_upstream!=None and svcall.coverage_upstream!=0:
+            u=float(svcall.coverage_upstream)
+        else:
+            u=1.0
+
+        if svcall.coverage_start!=None and svcall.coverage_start!=0:
+            s=float(svcall.coverage_start)
+        else:
+            s=1.0
+
+        if svcall.coverage_center!=None and svcall.coverage_center!=0:
+            c=float(svcall.coverage_center)
+        else:
+            c=1.0
+
+        if svcall.coverage_end!=None and svcall.coverage_end!=0:
+            e=float(svcall.coverage_end)
+        else:
+            e=1.0
+
+        if svcall.coverage_downstream!=None and svcall.coverage_downstream!=0:
+            d=float(svcall.coverage_downstream)
+        else:
+            d=1.0
+
+        if abs(u-s)/max(u,s) > qc_coverage_max_change_frac:
+            svcall.filter="COV_CHANGE_FRAC"
+            return False
+
+        if abs(s-c)/max(s,c) > qc_coverage_max_change_frac:
+            svcall.filter="COV_CHANGE_FRAC"
+            return False
+
+        if abs(c-e)/max(c,e) > qc_coverage_max_change_frac:
+            svcall.filter="COV_CHANGE_FRAC"
+            return False
+
+        if abs(e-d)/max(e,d) > qc_coverage_max_change_frac:
+            svcall.filter="COV_CHANGE_FRAC"
+            return False
+
     return True
 
 def qc_sv_post_annotate(svcall,config):
+    af=svcall.get_info("AF")
+    af=af if af!=None else 0
+    sv_is_mosaic = af <= config.mosaic_af_max
+
     if (len(svcall.genotypes)==0 or (svcall.genotypes[0][0]!="." and svcall.genotypes[0][0]+svcall.genotypes[0][1]<2)) and (svcall.coverage_center != None and svcall.coverage_center < config.qc_coverage):
         svcall.filter="COV_MIN"
         return False
 
+    qc_nm=config.qc_nm
+    qc_nm_threshold=config.qc_nm_threshold*config.qc_nm_mult
+    if config.mosaic and sv_is_mosaic:
+        qc_nm=config.mosaic_qc_nm
+        qc_nm_threshold=config.qc_nm_threshold*config.qc_nm_mult
+    if qc_nm and svcall.nm > qc_nm_threshold and (len(svcall.genotypes)==0 or svcall.genotypes[0][1]==0):
+        svcall.filter="ALN_NM"
+        return False
+
+    if config.mosaic:
+        if sv_is_mosaic and ( af < config.mosaic_af_min or af > config.mosaic_af_max ):
+            svcall.filter="MOSAIC_AF"
+            return False
+        elif not sv_is_mosaic and not config.mosaic_include_germline:
+            svcall.filter="MOSAIC_AF"
+            return False
+
     return True
 
 def binomial_coef(n,k):
     return math.factorial(n)/(math.factorial(k)*math.factorial(n-k))
 
 def binomial_probability(k,n,p):
     try:
@@ -296,16 +383,16 @@
 
     gt1,q1=normalized_likelihoods[0]
     gt2,q2=normalized_likelihoods[1]
     qz=[q for gt,q in normalized_likelihoods if gt==(0,0)][0]
     genotype_z_score = min(60,int((-10) * likelihood_ratio(qz,q1)))
     genotype_quality = min(60,int((-10) * likelihood_ratio(q2,q1)))
 
-    is_long_ins=(svcall.svtype=="INS" and svcall.svlen >= config.long_ins_length)
-    if genotype_z_score < config.genotype_min_z_score and not config.non_germline and not is_long_ins:
+    is_long_ins=(svcall.svtype=="INS" and svcall.svlen >= config.long_ins_length and config.detect_large_ins)
+    if genotype_z_score < config.genotype_min_z_score and not config.mosaic and not is_long_ins:
         if svcall.filter=="PASS":
             svcall.filter="GT"
 
     if is_long_ins and gt1==(0,0):
         a,b=".","."
     else:
         a,b=gt1
```

### Comparing `sniffles-2.0.7/src/sniffles/snf.py` & `sniffles-2.2/src/sniffles/snf.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,22 @@
         self.config=config
         self.handle=handle
         self.filename=filename
         self.blocks={}
         self.index={}
         self.total_length=0
 
+    def is_open(self):
+        return self.handle!=False
+
+    def open(self):
+        if self.handle!=False:
+            self.close()
+        self.handle=open(self.filename,"rb")
+
     def store(self,svcand):
         block_index=int(svcand.pos/self.config.snf_block_size)*self.config.snf_block_size
         if not block_index in self.blocks:
             self.blocks[block_index]={svtype: [] for svtype in sv.TYPES}
             self.blocks[block_index]["_COVERAGE"]={}
         if not self.config.output_rnames:
             svcand.rnames=None
@@ -73,53 +81,73 @@
     def serialize_block(self,block_id):
         return pickle.dumps(self.blocks[block_id])
 
     def unserialize_block(self,data):
         return pickle.loads(data)
 
     def write_and_index(self):
+        if not self.is_open():
+            self.open()
         offset=0
         for block_id in sorted(self.blocks):
             data=gzip.compress(self.serialize_block(block_id))
             self.handle.write(data)
             data_len=len(data)
             self.index[block_id]=(offset,data_len)
             offset+=data_len
             self.total_length+=data_len
+        if self.config.combine_close_handles:
+            self.close()
 
     def read_header(self):
+        if not self.is_open():
+            self.open()
         try:
             header_text=self.handle.readline()
             self.header_length=len(header_text)
             self.header=json.loads(header_text.strip())
         except Exception as e:
             print(f"Error when reading SNF header from '{self.filename}': {e}. The file may not be a valid .snf file or could have been corrupted.")
             raise e
         self.index=self.header["index"]
+        if self.config.combine_close_handles:
+            self.close()
 
     def read_blocks(self,contig,block_index):
+        if not self.is_open():
+            self.open()
         block_index=str(block_index)
         if not contig in self.index:
+            if self.config.combine_close_handles:
+                self.close()
             return None
 
         if not block_index in self.index[contig]:
+            if self.config.combine_close_handles:
+                self.close()
             return None
 
         blocks=[]
         for block_data_start,block_data_length in self.index[contig][block_index]:
             try:
                 self.handle.seek(self.header_length+block_data_start)
                 data=gzip.decompress(self.handle.read(block_data_length))
                 blocks.append(self.unserialize_block(data))
             except Exception as e:
                 print(f"Error when reading block '{contig}.{block_index}' from '{self.filename}': {e}. The file may not be a valid .snf file or could have been corrupted.")
+                if self.config.combine_close_handles:
+                    self.close()
                 raise e
+        if self.config.combine_close_handles:
+            self.close()
         return blocks
 
     def get_index(self):
         return self.index
 
     def get_total_length(self):
         return self.total_length
 
     def close(self):
-        self.handle.close()
+        if self.handle!=False:
+            self.handle.close()
+            self.handle=False
```

### Comparing `sniffles-2.0.7/src/sniffles/sniffles` & `sniffles-2.2/src/sniffles/sniffles`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     exit(1)
 
 import multiprocessing
 import collections
 import math
 import time
 import os
-from pathlib import Path
 import json
 
 import pysam
 
 from dataclasses import dataclass
 
 from sniffles import config
@@ -78,15 +77,15 @@
 
     elif "snf" in input_ext or "tsv" in input_ext:
         config.mode="combine"
     else:
         util.fatal_error_main(f"Failed to determine run mode from input. Please specify either: A single .bam file - OR - one or more .snf files - OR - a single .tsv file containing a list of .snf files and optional sample ids as input. (supplied were: {list(set(input_ext))})")
 
     if config.mode != "call_sample" and config.snf != None:
-        util.fatal_error_main(f"--snf cannot be used with run mode {mode}")
+        util.fatal_error_main(f"--snf cannot be used with run mode {config.mode}")
 
     if config.vcf == None and config.snf == None:
         util.fatal_error_main("Please specify at least one of: --vcf or --snf for output (both may be used at the same time)")
 
     if config.mode=="call_sample":
         if config.sample_id==None:
             #config.sample_id,_=os.path.splitext(os.path.basename(config.input))
@@ -181,16 +180,14 @@
             vcf_output_info_str=""
         else:
             vcf_output_info_str=f"({', '.join(vcf_output_info)})"
 
         if os.path.exists(config.vcf) and not config.allow_overwrite:
             util.fatal_error_main(f"Output file '{config.vcf}' already exists! Use --allow-overwrite to ignore this check and overwrite.")
         else:
-            if not Path(config.vcf).parent.exists():
-                Path(config.vcf).parent.mkdir(parents=True)
             if config.vcf_output_bgz:
                 if not config.sort:
                     util.fatal_error_main(".gz (bgzip) output is only supported with sorting enabled")
                 vcf_handle=pysam.BGZFile(config.vcf,"w")
             else:
                 vcf_handle=open(config.vcf,"w")
 
@@ -329,15 +326,15 @@
             if sample_id==None:
                 if snf_in.header["config"]["sample_id"] != None:
                     sample_id=snf_in.header["config"]["sample_id"]
                 else:
                     sample_id,_=os.path.splitext(os.path.basename(input_filename))
             config.snf_input_info.append({"internal_id":snf_internal_id, "sample_id": sample_id, "filename": input_filename})
             snf_internal_id+=1
-            snf_in.handle.close()
+            snf_in.close()
 
         if not config.combine_consensus:
             for info in config.snf_input_info:
                 config.sample_ids_vcf.append((info["internal_id"],info["sample_id"]))
 
         #TODO: Assure header consistency across multiple .snfs
```

### Comparing `sniffles-2.0.7/src/sniffles/sv.py` & `sniffles-2.2/src/sniffles/sv.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,23 +122,17 @@
     svstart,svend=calculate_bounds(svtype,ref_start,svlen)
     qual=int(util.mean(v.mapq for v in leads))
 
     support_fwd=sum(lead.strand == "+" for lead in leads)
     support_rev=len(leads) - support_fwd
 
     filter="PASS"
-    if config.qc_strand and (support_fwd==0 or support_rev==0):
-        filter="STRAND"
-        qc=False
 
-    if config.qc_nm:
+    if config.qc_nm_measure:
         nm_mean=util.mean(v.nm for v in leads)
-        if nm_mean > config.qc_nm_max:
-            filter="NM"
-            qc=False
     else:
         nm_mean=-1
 
     if not keep_qc_fails and not qc:
         return
 
     svpi=SVCallPostprocessingInfo(cluster=cluster)
@@ -295,14 +289,28 @@
         most_common_gt=[gt for gt in genotypes_consensus if genotypes_consensus[gt]["count"]==most_common_count]
         cons_a,cons_b=max(most_common_gt)
         consensus_info=genotypes_consensus[(cons_a,cons_b)]
         genotypes={0:(cons_a,cons_b,int(sum(consensus_info["qual"])/consensus_info["count"]),sum(consensus_info["dr"]),sum(consensus_info["dv"]))}
         if cons_a!=1 and cons_b!=1:
             return None
 
+    if config.combine_pair_relabel:
+        max_gt=(0,0)
+        for sample_id in genotypes:
+            a,b,qual,dr,dv,ps,new_id=genotypes[sample_id]
+            if qual > config.combine_pair_relabel_threshold and a!=".":
+                max_gt=max(max_gt,(a,b))
+
+        if max_gt!=(0,0):
+            for sample_id in genotypes:
+                a,b,qual,dr,dv,ps,new_id=genotypes[sample_id]
+                if qual < config.combine_pair_relabel_threshold and a!=".":
+                    max_a,max_b=max_gt
+                    genotypes[sample_id]=(max_a,max_b,qual,dr,dv,ps,new_id)
+
     svcall_pos=int(util.median(cand.pos for cand in svgroup.candidates))
     svcall_svlen=int(util.median(cand.svlen for cand in svgroup.candidates))
     svcall_alt=first_cand.alt
     svcall_alt_mindist=abs(len(svcall_alt)-svcall_svlen)
     if first_cand.svtype=="INS":
         svcall_end=svcall_pos
         for cand in svgroup.candidates:
@@ -347,15 +355,16 @@
 
     task.sv_id+=1
 
     return svcall
 
 def classify_splits(read,leads,config,main_contig):
     minsvlen_screen=config.minsvlen_screen
-    maxsvlen_other=minsvlen_screen*5
+    maxsvlen_other=minsvlen_screen*config.dev_split_max_query_distance_mult
+    min_split_len_bnd=config.bnd_min_split_length
 
     leads.sort(key=lambda ld: ld.qry_start)
     last=leads[0]
     last.svtypes_starts_lens=[]
 
     if last.qry_start >= config.long_ins_length*0.5:
         last.svtypes_starts_lens.append(("INS",last.ref_start,None))
@@ -465,15 +474,15 @@
             #BND
             #
             if curr.contig == main_contig:
                 a,b=curr,last
             else:
                 a,b=last,curr
 
-            if a.contig == main_contig:
+            if a.contig == main_contig and abs(last.qry_end-last.qry_start) >= min_split_len_bnd and abs(curr.qry_end-curr.qry_start) >= min_split_len_bnd:
                 is_first=a.qry_start < b.qry_start
                 if is_first:
                     if a.strand=="+":
                         svstart=a.ref_end
                     else:
                         svstart=a.ref_start
                 else:
```

### Comparing `sniffles-2.0.7/src/sniffles/util.py` & `sniffles-2.2/src/sniffles/util.py`

 * *Files identical despite different names*

### Comparing `sniffles-2.0.7/src/sniffles/vcf.py` & `sniffles-2.2/src/sniffles/vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 class VCF:
     def __init__(self,config,handle):
         self.config=config
         self.handle=handle
         self.call_count=0
         self.info_order=["SVTYPE","SVLEN","END","SUPPORT","RNAMES","COVERAGE","STRAND"]
-        if config.qc_nm:
+        if config.qc_nm_measure:
             self.info_order.append("NM")
 
         self.default_genotype=config.genotype_none
 
         if config.mode=="combine":
             self.genotype_format=config.genotype_format+":ID"
             self.default_genotype+=tuple(["NULL"])
@@ -92,19 +92,22 @@
         self.write_header_line('FILTER=<ID=PASS,Description="All filters passed">')
         self.write_header_line('FILTER=<ID=GT,Description="Genotype filter">')
         self.write_header_line('FILTER=<ID=SUPPORT_MIN,Description="Minimum read support filter">')
         self.write_header_line('FILTER=<ID=STDEV_POS,Description="SV Breakpoint standard deviation filter">')
         self.write_header_line('FILTER=<ID=STDEV_LEN,Description="SV length standard deviation filter">')
         self.write_header_line('FILTER=<ID=COV_MIN,Description="Minimum coverage filter">')
         self.write_header_line('FILTER=<ID=COV_CHANGE,Description="Coverage change filter">')
+        self.write_header_line('FILTER=<ID=COV_CHANGE_FRAC,Description="Coverage fractional change filter">')
+        self.write_header_line('FILTER=<ID=MOSAIC_AF,Description="Mosaic maximum allele frequency filter">')
+        self.write_header_line('FILTER=<ID=ALN_NM,Description="Length adjusted mismatch filter">')
         self.write_header_line('FILTER=<ID=STRAND,Description="Strand support filter">')
         self.write_header_line('FILTER=<ID=SVLEN_MIN,Description="SV length filter">')
-        self.write_header_line('FILTER=<ID=NM,Description="Alignment noise level filter">')
         self.write_header_line('INFO=<ID=PRECISE,Number=0,Type=Flag,Description="Structural variation with precise breakpoints">')
         self.write_header_line('INFO=<ID=IMPRECISE,Number=0,Type=Flag,Description="Structural variation with imprecise breakpoints">')
+        self.write_header_line('INFO=<ID=MOSAIC,Number=0,Type=Flag,Description="Structural variation classified as putative mosaic">')
         self.write_header_line('INFO=<ID=SVLEN,Number=1,Type=Integer,Description="Length of structural variation">')
         self.write_header_line('INFO=<ID=SVTYPE,Number=1,Type=String,Description="Type of structural variation">')
         self.write_header_line('INFO=<ID=CHR2,Number=1,Type=String,Description="Mate chromsome for BND SVs">')
         self.write_header_line('INFO=<ID=SUPPORT,Number=1,Type=Integer,Description="Number of reads supporting the structural variation">')
         self.write_header_line('INFO=<ID=SUPPORT_INLINE,Number=1,Type=Integer,Description="Number of reads supporting an INS/DEL SV (non-split events only)">')
         self.write_header_line('INFO=<ID=SUPPORT_LONG,Number=1,Type=Integer,Description="Number of soft-clipped reads putatively supporting the long insertion SV">')
         self.write_header_line('INFO=<ID=END,Number=1,Type=Integer,Description="End position of structural variation">')
@@ -174,14 +177,19 @@
                "NM": call.nm}
 
         if call.svtype=="BND":
             infos["SVLEN"]=None
             infos["END"]=None
 
         infos_ordered=["PRECISE" if call.precise else "IMPRECISE"]
+        af=call.get_info("AF")
+        af=af if af!=None else 0
+        sv_is_mosaic = af <= self.config.mosaic_af_max
+        if sv_is_mosaic and self.config.mosaic:
+            infos_ordered.append("MOSAIC")
         infos_ordered.extend(format_info(k,infos[k]) for k in self.info_order if infos[k]!=None)
         info_str=";".join(infos_ordered)
 
         #Output call specific additional information
         for k in sorted(call.info):
             if call.info[k]==None:
                 continue
```

### Comparing `sniffles-2.0.7/src/sniffles.egg-info/PKG-INFO` & `sniffles-2.2/src/sniffles.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sniffles
-Version: 2.0.7
+Version: 2.2
 Summary: A fast structural variation caller for long-read sequencing data
 Home-page: https://github.com/fritzsedlazeck/Sniffles
-Author: Moritz Smolka
-Author-email: moritz.g.smolka@gmail.com
+Author: Moritz Smolka, Luis Paulin
+Author-email: moritz.g.smolka@gmail.com, lfpaulin@gmail.com
 Project-URL: Bug Tracker, https://github.com/fritzsedlazeck/Sniffles/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sniffles2
 A fast structural variant caller for long-read sequencing, Sniffles2 accurately detect SVs on germline, somatic and population-level for PacBio and Oxford Nanopore read data.
 
 ## Quick Start: Germline SV calling using Sniffles2
@@ -32,30 +32,30 @@
 
 or
 
 `conda install sniffles=2.0 `
 
 If you previously installed Sniffles1 using conda and want to upgrade to Sniffles2, you can use:
 
-`conda update sniffles=2.0`
+`conda update sniffles=2.2`
 
 ## Requirements
-* Python >= 3.7
+* Python >= 3.8
 * pysam
 
 #### Tested on:
 * python==3.9.5
 * pysam==0.16.0.1
 
 ## Citation
 Please cite our paper at:
 
 https://www.nature.com/articles/s41592-018-0001-7
 
-A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1 
+A new preprint for the new methods and improvements introduced with Sniffles2 is here: https://www.biorxiv.org/content/10.1101/2022.04.04.487055v1
 
 ## Use-Cases / Modes
 
 ### A. General (all Modes)
 * To output deletion (DEL SV) sequences, the reference genome (.fasta) must be specified using e.g. `--reference reference.fasta`.
 * Sniffles2 supports optionally specifying tandem repeat region annotations (.bed), which can improve calling in these regions `--tandem-repeats annotations.bed`. Sniffles2 compatible tandem repeat annotations for human references can be found in the [annotations/ folder](https://github.com/fritzsedlazeck/Sniffles/tree/master/annotations).
 * Sniffles2 is fully parallelized and uses 4 threads by default. This value can be adapted using e.g. `--threads 4` as option. Memory requirements will increase with the number of threads used.
@@ -66,23 +66,27 @@
 
 1. Call SV candidates and create an associated .snf file for each sample: `sniffles --input sample1.bam --snf sample1.snf`
 2. Combined calling using multiple .snf files into a single .vcf: `sniffles --input sample1.snf sample2.snf ... sampleN.snf --vcf multisample.vcf`
 
 Alternatively, for step 2. you can supply a .tsv file, containing a list of .snf files, and custom sample ids in an optional second column (one sample per line), .e.g.:
 2. Combined calling using a .tsv as sample list: `sniffles --input snf_files_list.tsv --vcf multisample.vcf`
 
-### C. Non-Germline SV Calling (Somatic)
-To call non-germline SVs (i.e. somatic/mosaic) SVs, the *--non-germline* option should be added, i.e.:
+### C. Mosaic SV Calling (Non-germline or somatic SVs)
+To call mosaic SVs, the *--mosaic* option should be added, i.e.:
 
-`sniffles --input mapped_input.bam --vcf output.vcf --non-germline`
+`sniffles --input mapped_input.bam --vcf output.vcf --mosaic`
 
 ### D. Genotyping a known set of SVs (Force Calling)
 Example command, to determine the genotype of each SV in *input_known_svs.vcf* for *sample.bam* and write the re-genotyped SVs to *output_genotypes.vcf*:
 
 `sniffles --input sample.bam --genotype-vcf input_known_svs.vcf --vcf output_genotypes.vcf`
 
 ## Quick Tips
 
 ### Input / Output
 * .bam or .cram files containing long read alignments (i.e. from minimap2 or ngmlr) are supported as input
 * .vcf.gz (bgzipped+tabix indexed) output is supported
 * Simultaneous output of both .vcf and .snf file (for multi-sample calling) is supported
+
+## Companion apps
+* We have developed a plotting tools for Sniffles2: [https://github.com/farhangus/sniffle2_plot](https://github.com/farhangus/sniffle2_plot)
+* We also provide VCF and scripts used for the manuscript [https://github.com/smolkmo/Sniffles2-Supplement](https://github.com/smolkmo/Sniffles2-Supplement)
```

