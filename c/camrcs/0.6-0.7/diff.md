# Comparing `tmp/camrcs-0.6.tar.gz` & `tmp/camrcs-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camrcs-0.6.tar", last modified: Tue Jul 25 10:23:24 2023, max compression
+gzip compressed data, was "camrcs-0.7.tar", last modified: Thu Jul 27 13:08:46 2023, max compression
```

## Comparing `camrcs-0.6.tar` & `camrcs-0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-25 10:23:24.716755 camrcs-0.6/
--rw-rw-r--   0 niek      (1000) niek      (1000)     1528 2023-07-25 10:23:24.716755 camrcs-0.6/PKG-INFO
--rw-rw-r--   0 niek      (1000) niek      (1000)      895 2023-07-25 07:38:12.000000 camrcs-0.6/README.md
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-25 10:23:24.716755 camrcs-0.6/camrcs.egg-info/
--rw-rw-r--   0 niek      (1000) niek      (1000)     1528 2023-07-25 10:23:24.000000 camrcs-0.6/camrcs.egg-info/PKG-INFO
--rw-rw-r--   0 niek      (1000) niek      (1000)      362 2023-07-25 10:23:24.000000 camrcs-0.6/camrcs.egg-info/SOURCES.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)        1 2023-07-25 10:23:24.000000 camrcs-0.6/camrcs.egg-info/dependency_links.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-25 10:23:24.000000 camrcs-0.6/camrcs.egg-info/entry_points.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)       19 2023-07-25 10:23:24.000000 camrcs-0.6/camrcs.egg-info/requires.txt
--rw-rw-r--   0 niek      (1000) niek      (1000)        7 2023-07-25 10:23:24.000000 camrcs-0.6/camrcs.egg-info/top_level.txt
--rw-r--r--   0 niek      (1000) niek      (1000)     8907 2023-07-24 12:16:53.000000 camrcs-0.6/camrcs.py
-drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-25 10:23:24.716755 camrcs-0.6/docs/
--rw-rw-r--   0 niek      (1000) niek      (1000)      634 2023-07-20 06:51:26.000000 camrcs-0.6/docs/Makefile
--rw-rw-r--   0 niek      (1000) niek      (1000)     1195 2023-07-24 12:10:28.000000 camrcs-0.6/docs/about.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)     1821 2023-07-24 12:22:55.000000 camrcs-0.6/docs/archiving.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)     1933 2023-07-24 14:37:09.000000 camrcs-0.6/docs/conf.py
--rw-rw-r--   0 niek      (1000) niek      (1000)      239 2023-07-20 10:11:08.000000 camrcs-0.6/docs/data_pre.csv
--rw-rw-r--   0 niek      (1000) niek      (1000)      585 2023-07-24 12:20:45.000000 camrcs-0.6/docs/index.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)     1055 2023-07-20 11:35:47.000000 camrcs-0.6/docs/installation.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)      795 2023-07-20 06:51:26.000000 camrcs-0.6/docs/make.bat
--rw-rw-r--   0 niek      (1000) niek      (1000)      270 2023-07-24 10:57:51.000000 camrcs-0.6/docs/requirements.rst
--rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-25 10:23:24.716755 camrcs-0.6/setup.cfg
--rw-r--r--   0 niek      (1000) niek      (1000)     1200 2023-07-25 10:20:18.000000 camrcs-0.6/setup.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-27 13:08:46.612685 camrcs-0.7/
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1524 2023-07-27 13:08:46.608685 camrcs-0.7/PKG-INFO
+-rw-rw-r--   0 niek      (1000) niek      (1000)      895 2023-07-25 07:38:12.000000 camrcs-0.7/README.md
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-27 13:08:46.608685 camrcs-0.7/camrcs.egg-info/
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1524 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/PKG-INFO
+-rw-rw-r--   0 niek      (1000) niek      (1000)      362 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/SOURCES.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)        1 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/dependency_links.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/entry_points.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)       19 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/requires.txt
+-rw-rw-r--   0 niek      (1000) niek      (1000)        7 2023-07-27 13:08:46.000000 camrcs-0.7/camrcs.egg-info/top_level.txt
+-rw-r--r--   0 niek      (1000) niek      (1000)     9764 2023-07-27 13:01:35.000000 camrcs-0.7/camrcs.py
+drwxrwxr-x   0 niek      (1000) niek      (1000)        0 2023-07-27 13:08:46.608685 camrcs-0.7/docs/
+-rw-rw-r--   0 niek      (1000) niek      (1000)      634 2023-07-20 06:51:26.000000 camrcs-0.7/docs/Makefile
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1195 2023-07-24 12:10:28.000000 camrcs-0.7/docs/about.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)     2696 2023-07-26 10:04:11.000000 camrcs-0.7/docs/archiving.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1930 2023-07-26 09:59:43.000000 camrcs-0.7/docs/conf.py
+-rw-rw-r--   0 niek      (1000) niek      (1000)      296 2023-07-26 10:03:30.000000 camrcs-0.7/docs/data_pre.csv
+-rw-rw-r--   0 niek      (1000) niek      (1000)      585 2023-07-26 09:56:52.000000 camrcs-0.7/docs/index.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)     1051 2023-07-26 10:07:35.000000 camrcs-0.7/docs/installation.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)      795 2023-07-20 06:51:26.000000 camrcs-0.7/docs/make.bat
+-rw-rw-r--   0 niek      (1000) niek      (1000)      272 2023-07-26 10:02:35.000000 camrcs-0.7/docs/requirements.rst
+-rw-rw-r--   0 niek      (1000) niek      (1000)       38 2023-07-27 13:08:46.612685 camrcs-0.7/setup.cfg
+-rw-r--r--   0 niek      (1000) niek      (1000)     1196 2023-07-27 13:03:59.000000 camrcs-0.7/setup.py
```

### Comparing `camrcs-0.6/PKG-INFO` & `camrcs-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: camrcs
-Version: 0.6
+Version: 0.7
 Summary: A package for management of Cambridge Research Cold Storage backups
 Author: Niek Wit
 Author-email: nw416@cam.ac.uk
 License: MIT
-Project-URL: Documentation, https://github.com/niekwit/camrcs
+Project-URL: Documentation, https://camrcs.readthedocs.io
 Project-URL: Source, https://github.com/niekwit/camrcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `camrcs-0.6/README.md` & `camrcs-0.7/README.md`

 * *Files identical despite different names*

### Comparing `camrcs-0.6/camrcs.egg-info/PKG-INFO` & `camrcs-0.7/camrcs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: camrcs
-Version: 0.6
+Version: 0.7
 Summary: A package for management of Cambridge Research Cold Storage backups
 Author: Niek Wit
 Author-email: nw416@cam.ac.uk
 License: MIT
-Project-URL: Documentation, https://github.com/niekwit/camrcs
+Project-URL: Documentation, https://camrcs.readthedocs.io
 Project-URL: Source, https://github.com/niekwit/camrcs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Archiving :: Backup
```

### Comparing `camrcs-0.6/camrcs.py` & `camrcs-0.7/camrcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import pandas as pd
 import numpy as np
 import subprocess
 import hashlib
 from pathlib import Path
 from datetime import datetime
 import time
+import timeit
 
+VERSION = 0.7
 
 #get current working dir
 cdir = os.getcwd()
  
 
 ####Python functions####
 
@@ -35,15 +37,15 @@
     '''Runs shell commands with exception handling
     '''
     
     try:
         
         command = subprocess.run(command,
                                  shell=True,
-                                 executable='/bin/bash', #process substitution only works in bash
+                                 executable='/bin/bash', #process substitution does not work in all shells
                                  check=True)
         
         click.echo("Done...")
         
         return True
                             
     except subprocess.CalledProcessError as error:
@@ -53,46 +55,71 @@
         sys.exit()
 
 
 def update_csv(csv):
     '''Updates data.csv
     '''
     
-    #overwrite csv with md5 hashe/date
+    #overwrite csv with md5 hash/date
     click.echo("Updating data.csv...")
     csv.to_csv("data.csv")  
 
 
+def total_run_time(start):
+    '''Print total run time
+    '''
+    
+    stop = timeit.default_timer()
+    total_time = stop - start
+    
+    #format time
+    ty_res = time.gmtime(total_time)
+    res = time.strftime("%H:%M:%S",ty_res)
+    
+    click.echo(f"Total run time: {res}")
+
+
 ####command line parser####
 @click.group()
+
 def cli():
     '''Management of data backups to/from Cambridge University Research Cold Storage (RCS)
     '''
 
 
+
 #define subparser for uploading data to RCS        
 @click.command(name="up")
+
 @click.option("-k","--keep", 
               is_flag=True,
               help="Keep split archive files of target dir")
-@click.option("-n","--new", 
+
+@click.option("-c","--csv", 
               is_flag=True,
               help="Create empty data.csv file in current directory")
 
 
-def up(new,keep):
+def up(csv,keep):
     '''Upload data to RCS
     '''
-            
-    if new:
+    
+    #start total run timer
+    start = timeit.default_timer()
+    
+    #create empty data.csv if requested        
+    if csv:
         
-        header = "id,crsid,project_dir,date_up,date_down,temp_path,target_dir,remote_dest_dir,chunk_size,exclude_dir,md5sum_up,md5sum_down,download_dir"
+        click.secho("Creating new data.csv", fg="green")
+        
+        header = "id,crsid,project_dir,date_up,date_down,temp_path,target_dir,remote_dest_dir,chunk_size,exclude_dir,md5sum_up,md5sum_down,download_dir,version"
 
         #write to file
         with open(os.path.join(cdir,"data.csv"), "w") as text_file:
+            
             print(header, file=text_file)
             
         return
         
     #open data.csv
     csv = pd.read_csv(os.path.join(cdir,"data.csv"))
     csv = csv.set_index("id")
@@ -101,14 +128,15 @@
     csv_up = csv[csv["date_up"].isnull()]
 
     #total number of archives to upload
     total = len(csv_up)
     
     #exit if all directories have been uploaded already to RCS
     if total == 0:
+        
         sys.exit("Nothing to upload to RCS!")
     
     #upload data
     for index,row in csv_up.iterrows():
         
         #get info
         crsid = row["crsid"]
@@ -128,35 +156,35 @@
             
             exclude = f"--exclude={exclude}"
 
         #check if target directory exists
         if not path.exists(target_dir):
             
             click.secho(f"ERROR: target_dir ({target_dir}) does not exist!", fg="red")
+            
             continue #go to next dir if any
         
         #tar file name
         archive = os.path.join(temp_path,f"{os.path.basename(target_dir)}.tar.gz")
         
         click.secho(f"Creating archive for {target_dir} at RCS...", fg="green")
         
         
         #check if archive has been split before
         if not os.path.exists(f"{archive}.split.done"):
             
-            #check if unsplit archive exists
-            #if not os.path.exists(archive):
-            
             #create archive
             click.echo(f"Creating split {archive} ...")
+            
             target_base = os.path.dirname(target_dir)
             target_name = os.path.basename(target_dir)
+            
             md5sum_file = os.path.join(temp_path,f"md5sum_{os.path.basename(target_dir)}.txt")
-            #Path(md5sum_file).touch()
-            tar = f'tar -vcz -C {target_base} {exclude} {target_name} | pigz | tee >(md5sum > "{md5sum_file}") | split -b {chunk_size} - {archive}.part-'
+            
+            tar = f'tar -vc -C {target_base} {exclude} {target_name} | pigz | tee >(md5sum > "{md5sum_file}") | split -b {chunk_size} - {archive}.part-'
             
             time.sleep(5)
             
             #get md5sum from text file
             if run(tar):
                 
                 Path(os.path.join(f"{archive}.split.done")).touch()
@@ -168,58 +196,68 @@
                 os.remove(md5sum_file)
                     
         else:
             
             click.echo(f"{archive} has been created and split before...")
             
         #wait for user input (otherwise rsync can timeout if user does not promptly enter password)
+        click.echo("Transferring split archive files to RCS...")
+        
         input("Press Enter to continue...") 
         
-        click.echo("Transferring split archive files to RCS...")
-              
         rsync = f"rsync -v -h --progress $(ls {archive}.part-*) {crsid}@rcs.uis.cam.ac.uk:{project_dir}/{remote_dest_dir}" 
                
         if run(rsync):
             
+            #update csv
             csv.at[index,"md5sum_up"] = md5sum_up
             csv.at[index,"date_up"] = str(datetime.now().astimezone())
+            csv.at[index,"version"] = VERSION
                       
+        
     #update csv with md5sum hash/date
     update_csv(csv)
                 
     #remove archive and split archive files
     if not keep:
     
         click.echo("Removing all archive files...")
         remove = f"rm -r {archive}*"
     
     else:
     
-        click.echo("Removing all split archive files...")
-        remove = f"rm -r {archive}.part-*"
+        click.echo("Keeping all split archive files...")
     
     if run(remove):
+        
         click.echo("Finished!")
 
-
-    
+    #display total run time
+    total_run_time(start)
     
 
+
 #define subparser for retrieving data from RCS
 @click.command(name="down")
+
 @click.option("-k","--keep", 
               is_flag=True,
               help="Keep split archive files of target dir")
+
 @click.option("-t","--target", 
               type=int,
               help="Target archive (id) to retrieve from RCS")
 
+
 def down(keep,target):
     '''Retrieve data from RCS
     '''
+    #start run timer
+    start = timeit.default_timer()
+    
     #open data.csv
     csv = pd.read_csv(os.path.join(cdir,"data.csv"))
     csv = csv.set_index("id")
     
     #select row with relevant information
     row = csv.loc[target]
     
@@ -232,15 +270,15 @@
     md5sum_up = row["md5sum_up"]
     
     click.secho(f"Retrieving archive {os.path.join(project_dir,remote_dest_dir)} from RCS...", fg="green")
     
     #perform some checks
     if type(download_dir) != str:
         
-        click.secho("ERROR: download_dir is not a valid path (left empty?)...", fg="red")
+        click.secho("ERROR: download_dir is not a valid path (no value in data.csv?)...", fg="red")
         sys.exit()
         
     #create rsync command
     archive = f"{os.path.basename(target_dir)}.tar.gz.part-*"
     archive = f"{os.path.join(project_dir,remote_dest_dir,archive)}"
     rsync = f"rsync -v -h {crsid}@rcs.uis.cam.ac.uk:{archive} {download_dir}"
     
@@ -254,15 +292,17 @@
     archive = os.path.join(download_dir,os.path.basename(target_dir)) + ".tar.gz"
     parts = f"{archive}.part-*"
     cat = f"cat $(ls {parts}) > {archive}"
     
     if run(cat):
         
         click.echo(f"Calculating md5sum for retrieved archive...")
+        
         csv.at[target,"md5sum_down"] = md5(archive)
+        
         click.echo("Done...")
     
     
     click.echo("Removing archive parts...")
     remove = f"rm {parts}"
     
     if run(remove):
@@ -274,40 +314,57 @@
         
         click.echo("Retrieved archive correct...")
                     
     else:
         
         click.secho(f"Retrieved archive incorrect...\nRun camrcs again!", fg="red")
         
-        return
+        sys.exit()
     
     click.echo("Unpacking retrieved archive...")
-    
+        
     #unzipping/unpacking in seperate commands
     #https://superuser.com/questions/841865/extracting-a-tar-gz-file-returns-this-does-not-look-like-a-tar-archive
     unzip_archive = os.path.basename(archive.replace(".gz",""))
     
     if keep:
         
-        untar = f"pigz -d -k {archive} ; cd {download_dir}; tar -xvf {unzip_archive}; rm {unzip_archive}"
+        untar = f"pigz -dk {archive} ; cd {download_dir}; tar -xvf {unzip_archive}; rm {unzip_archive}"
+    
     else:
+        
         os.makedirs(download_dir, exist_ok=True)
         untar = f"pigz -d {archive} ; cd {download_dir}; tar -xvf {unzip_archive}; rm {unzip_archive}"
         
     if run(untar): 
         
         #update csv with md5 hash/date
         update_csv(csv)
         
         click.echo("Finished!")
     
+    #display total run time
+    total_run_time(start)
+    
     
+
+@click.command(name="version")
+
+def version():
+    '''Print version and quit
+    '''
+
+    click.secho(f"camrcs v{VERSION}", fg="green")
+
+
+
 #add subparsers
 cli.add_command(up)
 cli.add_command(down)
+cli.add_command(version)
```

### Comparing `camrcs-0.6/docs/Makefile` & `camrcs-0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `camrcs-0.6/docs/about.rst` & `camrcs-0.7/docs/about.rst`

 * *Files identical despite different names*

### Comparing `camrcs-0.6/docs/conf.py` & `camrcs-0.7/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
-# import os
-# import sys
-# sys.path.insert(0, os.path.abspath('.'))
+import os
+import sys
+sys.path.insert(0, os.path.abspath('../.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'camrcs'
 copyright = '2023, Niek Wit'
 author = 'Niek Wit'
 
 # The full version, including alpha/beta/rc tags
-release = '0.6'
+release = '0.7'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `camrcs-0.6/docs/index.rst` & `camrcs-0.7/docs/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 
 Welcome to camrcs's documentation!
 ====================================
 
-**camrcs** is a Python package that can upload or retrieve data to/from `Cambridge University's Research Cold Storage (RCS) <https://www.hpc.cam.ac.uk/research-cold-store>`_.
+``camrcs`` is a Python package that can upload or retrieve data to/from `Cambridge University's Research Cold Storage (RCS) <https://www.hpc.cam.ac.uk/research-cold-store>`_.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    requirements
    installation
```

### Comparing `camrcs-0.6/docs/installation.rst` & `camrcs-0.7/docs/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =======================
 Installation
 =======================
 
-*camrcs*
+camrcs
 =======================
 
 Via github
 -----------
 
 .. code-block:: console
    
@@ -26,15 +26,15 @@
    
    $ pip install camrcs
 
 
 This will install the most recent stable version of `camrcs`.
 
 
-*pigz*
+pigz
 =======================
 
 ``camrcs`` uses ``pigz`` for data compression
 
 Debian-based GNU/Linux
 -----------------------
```

### Comparing `camrcs-0.6/docs/make.bat` & `camrcs-0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `camrcs-0.6/setup.py` & `camrcs-0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='camrcs',
-    version='0.6',
+    version='0.7',
     py_modules=['camrcs'], 
     description='A package for management of Cambridge Research Cold Storage backups',
     long_description=long_description,
     long_description_content_type='text/markdown',
     project_urls={
-        'Documentation': 'https://github.com/niekwit/camrcs',
+        'Documentation': 'https://camrcs.readthedocs.io',
         'Source': 'https://github.com/niekwit/camrcs',
     },
     author='Niek Wit',
     author_email='nw416@cam.ac.uk',
     license='MIT',
     packages=find_packages(),
     install_requires=['pandas','Click','numpy',
```

