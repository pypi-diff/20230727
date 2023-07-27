# Comparing `tmp/nvidia-smi2-0.0.1.post3.tar.gz` & `tmp/nvidia-smi2-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-smi2-0.0.1.post3.tar", last modified: Fri Jul 14 08:54:14 2023, max compression
+gzip compressed data, was "nvidia-smi2-0.0.2.post1.tar", last modified: Thu Jul 27 04:27:31 2023, max compression
```

## Comparing `nvidia-smi2-0.0.1.post3.tar` & `nvidia-smi2-0.0.2.post1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     9117 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8992 2023-07-13 10:29:51.000000 nvidia-smi2-0.0.1.post3/README.md
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/bin/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      112 2023-07-13 10:28:58.000000 nvidia-smi2-0.0.1.post3/bin/nvidia-smi2
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/nvidia-smi2/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8442 2023-07-13 10:29:59.000000 nvidia-smi2-0.0.1.post3/nvidia-smi2/__init__.py
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      120 2023-07-13 10:28:41.000000 nvidia-smi2-0.0.1.post3/nvidia-smi2/__main__.py
-drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     9117 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/PKG-INFO
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      256 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/SOURCES.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/dependency_links.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/requires.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       12 2023-07-14 08:54:14.000000 nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/top_level.txt
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       38 2023-07-14 08:54:14.079248 nvidia-smi2-0.0.1.post3/setup.cfg
--rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      470 2023-07-14 08:53:41.000000 nvidia-smi2-0.0.1.post3/setup.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-27 04:27:31.947820 nvidia-smi2-0.0.2.post1/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     9275 2023-07-27 04:27:31.947820 nvidia-smi2-0.0.2.post1/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     9150 2023-07-27 04:24:26.000000 nvidia-smi2-0.0.2.post1/README.md
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-27 04:27:31.947820 nvidia-smi2-0.0.2.post1/bin/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      112 2023-07-13 10:28:58.000000 nvidia-smi2-0.0.2.post1/bin/nvidia-smi2
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-27 04:27:31.947820 nvidia-smi2-0.0.2.post1/nvidia-smi2/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     8811 2023-07-27 04:25:29.000000 nvidia-smi2-0.0.2.post1/nvidia-smi2/__init__.py
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      120 2023-07-13 10:28:41.000000 nvidia-smi2-0.0.2.post1/nvidia-smi2/__main__.py
+drwxrwxr-x   0 dongtrinh  (1006) dongtrinh  (1006)        0 2023-07-27 04:27:31.947820 nvidia-smi2-0.0.2.post1/nvidia_smi2.egg-info/
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)     9275 2023-07-27 04:27:31.000000 nvidia-smi2-0.0.2.post1/nvidia_smi2.egg-info/PKG-INFO
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      256 2023-07-27 04:27:31.000000 nvidia-smi2-0.0.2.post1/nvidia_smi2.egg-info/SOURCES.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)        1 2023-07-27 04:27:31.000000 nvidia-smi2-0.0.2.post1/nvidia_smi2.egg-info/dependency_links.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       10 2023-07-27 04:27:31.000000 nvidia-smi2-0.0.2.post1/nvidia_smi2.egg-info/requires.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       12 2023-07-27 04:27:31.000000 nvidia-smi2-0.0.2.post1/nvidia_smi2.egg-info/top_level.txt
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)       38 2023-07-27 04:27:31.947820 nvidia-smi2-0.0.2.post1/setup.cfg
+-rw-rw-r--   0 dongtrinh  (1006) dongtrinh  (1006)      470 2023-07-27 04:25:58.000000 nvidia-smi2-0.0.2.post1/setup.py
```

### Comparing `nvidia-smi2-0.0.1.post3/PKG-INFO` & `nvidia-smi2-0.0.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-smi2
-Version: 0.0.1.post3
+Version: 0.0.2.post1
 Author: NNDam, PD-Mera
 Description-Content-Type: text/markdown
 
 # nvidia-smi2
 
 A tool for enriching the output of nvidia-smi.
 
@@ -14,45 +14,47 @@
 
 Install
 
     pip install nvidia-smi2
     
 Run
 
-    nvidia-smi2 [-l [length]] [-u [username]]
+    nvidia-smi2 [-L [length]] [-u [username]]
       print GPU utilization with usernames and CPU stats for each GPU-utilizing process
 
-      -l|--command-length [length]     Print longer part of the commandline. If `length'
+      -L|--command-length [length]     Print longer part of the commandline. If `length'
                                        is provided, use it as the commandline length,
                                        otherwise print first 100 characters.
       -c|--color                       Colorize the output (green - free GPU, yellow -
                                        moderately used GPU, red - fully used GPU)
       -u|--user                        Name of user to summarize
+      -l|--loop                        Loop nvidia-smi2 after a period of time
 
 Or run from src
 
     pip install termcolor
     chmod a+x nvidia-htop.py
-    ./nvidia-htop.py [-l [length]] [-u [username]]
+    ./nvidia-htop.py [-L [length]] [-u [username]]
       print GPU utilization with usernames and CPU stats for each GPU-utilizing process
 
-      -l|--command-length [length]     Print longer part of the commandline. If `length'
+      -L|--command-length [length]     Print longer part of the commandline. If `length'
                                        is provided, use it as the commandline length,
                                        otherwise print first 100 characters.
       -c|--color                       Colorize the output (green - free GPU, yellow -
                                        moderately used GPU, red - fully used GPU)
       -u|--user                        Name of user to summarize
+      -l|--loop                        Loop nvidia-smi2 after a period of time
 
-Note: for backward compatibility, `nvidia-smi | ./nvidia-htop.py [-l [length]] [-u [username]]` is also supported.
+Note: for backward compatibility, `nvidia-smi | ./nvidia-htop.py [-L [length]] [-u [username]]` is also supported.
 
 Note: running inside a container (docker, singularity, ...), `nvidia-smi` can only see processes running in the container.
 
 ## Example output
 ```
-rnd@rnd:~$ nvidia-smi2 -l
+rnd@rnd:~$ nvidia-smi2 -L
 Wed Jul 12 10:41:16 2023
 +-----------------------------------------------------------------------------+
 | NVIDIA-SMI 470.57.02    Driver Version: 470.57.02    CUDA Version: 11.4     |
 |-------------------------------+----------------------+----------------------+
 | GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
 | Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
 |                               |                      |               MIG M. |
@@ -87,15 +89,15 @@
 |   anonym1          2365MiB         2.9         3.1  |
 |       rnd           135MiB         0.1         0.8  |
 |   anonym2          6917MiB       128.0         4.3  |
 +-----------------------------------------------------+
 ```
 
 ```
-rnd@rnd:~$ nvidia-smi2 -l -u root
+rnd@rnd:~$ nvidia-smi2 -L -u root
 Wed Jul 12 10:51:06 2023
 +-----------------------------------------------------------------------------+
 | NVIDIA-SMI 470.57.02    Driver Version: 470.57.02    CUDA Version: 11.4     |
 |-------------------------------+----------------------+----------------------+
 | GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
 | Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
 |                               |                      |               MIG M. |
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: nvidia-smi2 Version: 0.0.1.post3 Author: NNDam, PD-
+Metadata-Version: 2.1 Name: nvidia-smi2 Version: 0.0.2.post1 Author: NNDam, PD-
 Mera Description-Content-Type: text/markdown # nvidia-smi2 A tool for enriching
 the output of nvidia-smi. [Alt_text] ## Usage Install pip install nvidia-smi2
-Run nvidia-smi2 [-l [length]] [-u [username]] print GPU utilization with
-usernames and CPU stats for each GPU-utilizing process -l|--command-length
+Run nvidia-smi2 [-L [length]] [-u [username]] print GPU utilization with
+usernames and CPU stats for each GPU-utilizing process -L|--command-length
 [length] Print longer part of the commandline. If `length' is provided, use it
 as the commandline length, otherwise print first 100 characters. -c|--color
 Colorize the output (green - free GPU, yellow - moderately used GPU, red -
-fully used GPU) -u|--user Name of user to summarize Or run from src pip install
-termcolor chmod a+x nvidia-htop.py ./nvidia-htop.py [-l [length]] [-u
-[username]] print GPU utilization with usernames and CPU stats for each GPU-
-utilizing process -l|--command-length [length] Print longer part of the
-commandline. If `length' is provided, use it as the commandline length,
-otherwise print first 100 characters. -c|--color Colorize the output (green -
-free GPU, yellow - moderately used GPU, red - fully used GPU) -u|--user Name of
-user to summarize Note: for backward compatibility, `nvidia-smi | ./nvidia-
-htop.py [-l [length]] [-u [username]]` is also supported. Note: running inside
-a container (docker, singularity, ...), `nvidia-smi` can only see processes
-running in the container. ## Example output ``` rnd@rnd:~$ nvidia-smi2 -l Wed
-Jul 12 10:41:16 2023 +---------------------------------------------------------
---------------------+ | NVIDIA-SMI 470.57.02 Driver Version: 470.57.02 CUDA
-Version: 11.4 | |-------------------------------+----------------------+-------
----------------+ | GPU Name Persistence-M| Bus-Id Disp.A | Volatile Uncorr. ECC
-| | Fan Temp Perf Pwr:Usage/Cap| Memory-Usage | GPU-Util Compute M. | | | | MIG
-M. |
+fully used GPU) -u|--user Name of user to summarize -l|--loop Loop nvidia-smi2
+after a period of time Or run from src pip install termcolor chmod a+x nvidia-
+htop.py ./nvidia-htop.py [-L [length]] [-u [username]] print GPU utilization
+with usernames and CPU stats for each GPU-utilizing process -L|--command-length
+[length] Print longer part of the commandline. If `length' is provided, use it
+as the commandline length, otherwise print first 100 characters. -c|--color
+Colorize the output (green - free GPU, yellow - moderately used GPU, red -
+fully used GPU) -u|--user Name of user to summarize -l|--loop Loop nvidia-smi2
+after a period of time Note: for backward compatibility, `nvidia-smi | ./
+nvidia-htop.py [-L [length]] [-u [username]]` is also supported. Note: running
+inside a container (docker, singularity, ...), `nvidia-smi` can only see
+processes running in the container. ## Example output ``` rnd@rnd:~$ nvidia-
+smi2 -L Wed Jul 12 10:41:16 2023 +---------------------------------------------
+--------------------------------+ | NVIDIA-SMI 470.57.02 Driver Version:
+470.57.02 CUDA Version: 11.4 | |-------------------------------+---------------
+-------+----------------------+ | GPU Name Persistence-M| Bus-Id Disp.A |
+Volatile Uncorr. ECC | | Fan Temp Perf Pwr:Usage/Cap| Memory-Usage | GPU-Util
+Compute M. | | | | MIG M. |
 |===============================+======================+======================|
 | 0 NVIDIA GeForce ... On | 00000000:01:00.0 Off | N/A | | 55% 73C P2 88W /
 280W | 3248MiB / 11176MiB | 64% Default | | | | N/A | +------------------------
 -------+----------------------+----------------------+ | 1 NVIDIA GeForce ...
 On | 00000000:02:00.0 Off | N/A | | 59% 67C P2 91W / 280W | 9397MiB / 11178MiB
 | 7% Default | | | | N/A | +-------------------------------+-------------------
 ---+----------------------+ +--------------------------------------------------
@@ -45,15 +46,15 @@
 128 4.3 22:30:29 python train_image_classifier.py xxxx | | 1 27877 root 2017MiB
 9.4 1.4 15 days python consumer.py | +-----------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------+ | USER TOTAL GPU MEM TOTAL %CPU TOTAL
 %MEM | +-----------------------------------------------------+ | root 3210MiB
 158.6 9.8 | | gdm 4MiB 0.0 0.0 | | anonym1 2365MiB 2.9 3.1 | | rnd 135MiB 0.1
 0.8 | | anonym2 6917MiB 128.0 4.3 | +------------------------------------------
------------+ ``` ``` rnd@rnd:~$ nvidia-smi2 -l -u root Wed Jul 12 10:51:06 2023
+-----------+ ``` ``` rnd@rnd:~$ nvidia-smi2 -L -u root Wed Jul 12 10:51:06 2023
 +-----------------------------------------------------------------------------
 + | NVIDIA-SMI 470.57.02 Driver Version: 470.57.02 CUDA Version: 11.4 | |------
 -------------------------+----------------------+----------------------+ | GPU
 Name Persistence-M| Bus-Id Disp.A | Volatile Uncorr. ECC | | Fan Temp Perf Pwr:
 Usage/Cap| Memory-Usage | GPU-Util Compute M. | | | | MIG M. |
 |===============================+======================+======================|
 | 0 NVIDIA GeForce ... On | 00000000:01:00.0 Off | N/A | | 58% 69C P2 106W /
```

### Comparing `nvidia-smi2-0.0.1.post3/README.md` & `nvidia-smi2-0.0.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,45 +8,47 @@
 
 Install
 
     pip install nvidia-smi2
     
 Run
 
-    nvidia-smi2 [-l [length]] [-u [username]]
+    nvidia-smi2 [-L [length]] [-u [username]]
       print GPU utilization with usernames and CPU stats for each GPU-utilizing process
 
-      -l|--command-length [length]     Print longer part of the commandline. If `length'
+      -L|--command-length [length]     Print longer part of the commandline. If `length'
                                        is provided, use it as the commandline length,
                                        otherwise print first 100 characters.
       -c|--color                       Colorize the output (green - free GPU, yellow -
                                        moderately used GPU, red - fully used GPU)
       -u|--user                        Name of user to summarize
+      -l|--loop                        Loop nvidia-smi2 after a period of time
 
 Or run from src
 
     pip install termcolor
     chmod a+x nvidia-htop.py
-    ./nvidia-htop.py [-l [length]] [-u [username]]
+    ./nvidia-htop.py [-L [length]] [-u [username]]
       print GPU utilization with usernames and CPU stats for each GPU-utilizing process
 
-      -l|--command-length [length]     Print longer part of the commandline. If `length'
+      -L|--command-length [length]     Print longer part of the commandline. If `length'
                                        is provided, use it as the commandline length,
                                        otherwise print first 100 characters.
       -c|--color                       Colorize the output (green - free GPU, yellow -
                                        moderately used GPU, red - fully used GPU)
       -u|--user                        Name of user to summarize
+      -l|--loop                        Loop nvidia-smi2 after a period of time
 
-Note: for backward compatibility, `nvidia-smi | ./nvidia-htop.py [-l [length]] [-u [username]]` is also supported.
+Note: for backward compatibility, `nvidia-smi | ./nvidia-htop.py [-L [length]] [-u [username]]` is also supported.
 
 Note: running inside a container (docker, singularity, ...), `nvidia-smi` can only see processes running in the container.
 
 ## Example output
 ```
-rnd@rnd:~$ nvidia-smi2 -l
+rnd@rnd:~$ nvidia-smi2 -L
 Wed Jul 12 10:41:16 2023
 +-----------------------------------------------------------------------------+
 | NVIDIA-SMI 470.57.02    Driver Version: 470.57.02    CUDA Version: 11.4     |
 |-------------------------------+----------------------+----------------------+
 | GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
 | Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
 |                               |                      |               MIG M. |
@@ -81,15 +83,15 @@
 |   anonym1          2365MiB         2.9         3.1  |
 |       rnd           135MiB         0.1         0.8  |
 |   anonym2          6917MiB       128.0         4.3  |
 +-----------------------------------------------------+
 ```
 
 ```
-rnd@rnd:~$ nvidia-smi2 -l -u root
+rnd@rnd:~$ nvidia-smi2 -L -u root
 Wed Jul 12 10:51:06 2023
 +-----------------------------------------------------------------------------+
 | NVIDIA-SMI 470.57.02    Driver Version: 470.57.02    CUDA Version: 11.4     |
 |-------------------------------+----------------------+----------------------+
 | GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
 | Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
 |                               |                      |               MIG M. |
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
 # nvidia-smi2 A tool for enriching the output of nvidia-smi. [Alt_text] ##
-Usage Install pip install nvidia-smi2 Run nvidia-smi2 [-l [length]] [-u
+Usage Install pip install nvidia-smi2 Run nvidia-smi2 [-L [length]] [-u
 [username]] print GPU utilization with usernames and CPU stats for each GPU-
-utilizing process -l|--command-length [length] Print longer part of the
+utilizing process -L|--command-length [length] Print longer part of the
 commandline. If `length' is provided, use it as the commandline length,
 otherwise print first 100 characters. -c|--color Colorize the output (green -
 free GPU, yellow - moderately used GPU, red - fully used GPU) -u|--user Name of
-user to summarize Or run from src pip install termcolor chmod a+x nvidia-
-htop.py ./nvidia-htop.py [-l [length]] [-u [username]] print GPU utilization
-with usernames and CPU stats for each GPU-utilizing process -l|--command-length
-[length] Print longer part of the commandline. If `length' is provided, use it
-as the commandline length, otherwise print first 100 characters. -c|--color
-Colorize the output (green - free GPU, yellow - moderately used GPU, red -
-fully used GPU) -u|--user Name of user to summarize Note: for backward
-compatibility, `nvidia-smi | ./nvidia-htop.py [-l [length]] [-u [username]]` is
-also supported. Note: running inside a container (docker, singularity, ...),
-`nvidia-smi` can only see processes running in the container. ## Example output
-``` rnd@rnd:~$ nvidia-smi2 -l Wed Jul 12 10:41:16 2023 +-----------------------
-------------------------------------------------------+ | NVIDIA-SMI 470.57.02
-Driver Version: 470.57.02 CUDA Version: 11.4 | |-------------------------------
-+----------------------+----------------------+ | GPU Name Persistence-M| Bus-
-Id Disp.A | Volatile Uncorr. ECC | | Fan Temp Perf Pwr:Usage/Cap| Memory-Usage
-| GPU-Util Compute M. | | | | MIG M. |
+user to summarize -l|--loop Loop nvidia-smi2 after a period of time Or run from
+src pip install termcolor chmod a+x nvidia-htop.py ./nvidia-htop.py [-L
+[length]] [-u [username]] print GPU utilization with usernames and CPU stats
+for each GPU-utilizing process -L|--command-length [length] Print longer part
+of the commandline. If `length' is provided, use it as the commandline length,
+otherwise print first 100 characters. -c|--color Colorize the output (green -
+free GPU, yellow - moderately used GPU, red - fully used GPU) -u|--user Name of
+user to summarize -l|--loop Loop nvidia-smi2 after a period of time Note: for
+backward compatibility, `nvidia-smi | ./nvidia-htop.py [-L [length]] [-u
+[username]]` is also supported. Note: running inside a container (docker,
+singularity, ...), `nvidia-smi` can only see processes running in the
+container. ## Example output ``` rnd@rnd:~$ nvidia-smi2 -L Wed Jul 12 10:41:16
+2023 +-------------------------------------------------------------------------
+----+ | NVIDIA-SMI 470.57.02 Driver Version: 470.57.02 CUDA Version: 11.4 | |--
+-----------------------------+----------------------+----------------------+ |
+GPU Name Persistence-M| Bus-Id Disp.A | Volatile Uncorr. ECC | | Fan Temp Perf
+Pwr:Usage/Cap| Memory-Usage | GPU-Util Compute M. | | | | MIG M. |
 |===============================+======================+======================|
 | 0 NVIDIA GeForce ... On | 00000000:01:00.0 Off | N/A | | 55% 73C P2 88W /
 280W | 3248MiB / 11176MiB | 64% Default | | | | N/A | +------------------------
 -------+----------------------+----------------------+ | 1 NVIDIA GeForce ...
 On | 00000000:02:00.0 Off | N/A | | 59% 67C P2 91W / 280W | 9397MiB / 11178MiB
 | 7% Default | | | | N/A | +-------------------------------+-------------------
 ---+----------------------+ +--------------------------------------------------
@@ -43,15 +44,15 @@
 128 4.3 22:30:29 python train_image_classifier.py xxxx | | 1 27877 root 2017MiB
 9.4 1.4 15 days python consumer.py | +-----------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------+ | USER TOTAL GPU MEM TOTAL %CPU TOTAL
 %MEM | +-----------------------------------------------------+ | root 3210MiB
 158.6 9.8 | | gdm 4MiB 0.0 0.0 | | anonym1 2365MiB 2.9 3.1 | | rnd 135MiB 0.1
 0.8 | | anonym2 6917MiB 128.0 4.3 | +------------------------------------------
------------+ ``` ``` rnd@rnd:~$ nvidia-smi2 -l -u root Wed Jul 12 10:51:06 2023
+-----------+ ``` ``` rnd@rnd:~$ nvidia-smi2 -L -u root Wed Jul 12 10:51:06 2023
 +-----------------------------------------------------------------------------
 + | NVIDIA-SMI 470.57.02 Driver Version: 470.57.02 CUDA Version: 11.4 | |------
 -------------------------+----------------------+----------------------+ | GPU
 Name Persistence-M| Bus-Id Disp.A | Volatile Uncorr. ECC | | Fan Temp Perf Pwr:
 Usage/Cap| Memory-Usage | GPU-Util Compute M. | | | | MIG M. |
 |===============================+======================+======================|
 | 0 NVIDIA GeForce ... On | 00000000:01:00.0 Off | N/A | | 58% 69C P2 106W /
```

### Comparing `nvidia-smi2-0.0.1.post3/nvidia-smi2/__init__.py` & `nvidia-smi2-0.0.2.post1/nvidia-smi2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 import sys
 import os
 import re
 import subprocess
 import select
 import argparse
+import time
 from termcolor import colored
 
 MEMORY_FREE_RATIO = 0.05
 MEMORY_MODERATE_RATIO = 0.9
 GPU_FREE_RATIO = 0.05
 GPU_MODERATE_RATIO = 0.75
 
@@ -146,92 +147,96 @@
 
 
 def main():
     import argparse
     import sys
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('-l', '--command-length', default=20, const=100, type=int, nargs='?')
+    parser.add_argument('-L', '--command-length', default=20, const=100, type=int, nargs='?')
     parser.add_argument('-c', '--color', action='store_true')
     parser.add_argument('-u', '--user', type = str, default = '', help = 'user to analyst instead of all user')
+    parser.add_argument('-l', '--loop', default=1, type=float)
 
     args = parser.parse_args()
 
     # parse the command length argument
     command_length = args.command_length
     color = args.color
 
-    # Get nvidia-smi stdout
-    lines = get_nvidia_smi_stdout()
+    while True:
+        # Get nvidia-smi stdout
+        lines = get_nvidia_smi_stdout()
+
+        # Get line to print
+        lines_to_print, ps_start_idx, is_new_format = get_line_to_print(lines)
+
+        # Colorize
+        if color:
+            lines_to_print = colorize(lines_to_print)
+
+        # we print all but the last line which is the +---+ separator
+        for line in lines_to_print[:-1]:
+            print(line)
+
+        no_running_process = "No running processes found"
+        if no_running_process in lines[ps_start_idx] or lines[ps_start_idx].startswith("+--"):
+            print(lines[-1].strip())
+            print("| " + no_running_process + " " * (73 - len(no_running_process)) + "   |")
+            # Issue #9, running inside docker and seeing no processes
+            if lines[ps_start_idx].startswith("+--"):
+                print("| If you're running in a container, you'll only see processes running inside. |")
+            print(lines[-1])
+            sys.exit()
+
+        # Get all process detail
+        ps_detail, user_detail = get_process_user_detail(ps_start_idx, is_new_format, lines)
 
-    # Get line to print
-    lines_to_print, ps_start_idx, is_new_format = get_line_to_print(lines)
+        # Print process detail
+        max_pid_length = max(5, max([len(x) for x in ps_detail["pid"]]))
+        print_format = ("|  %3s %" + str(max_pid_length) + "s %8s   %8s %5s %5s %9s  %-" + str(command_length) + "." + str(command_length) + "s  |")
+
+        line = print_format % (
+            "GPU", "PID", "USER", "GPU MEM", "%CPU", "%MEM", "TIME", "COMMAND"
+        )
 
-    # Colorize
-    if color:
-        lines_to_print = colorize(lines_to_print)
+        print("+" + ("-" * (len(line) - 2)) + "+")
+
+        print(line)
 
-    # we print all but the last line which is the +---+ separator
-    for line in lines_to_print[:-1]:
+        for i in range(len(ps_detail["pid"])):
+            if len(args.user) > 0:
+                if ps_detail["user"][i][:7] != args.user[:7]:
+                    continue
+            print(print_format % (
+                ps_detail["gpu_num"][i],
+                ps_detail["pid"][i],
+                ps_detail["user"][i],
+                ps_detail["gpu_mem"][i],
+                ps_detail["cpu"][i],
+                ps_detail["mem"][i],
+                ps_detail["time"][i],
+                ps_detail["command"][i]
+            ))
+
+        print("+" + ("-" * (len(line) - 2)) + "+")
+
+        # Print user detail
+        sum_format = ("|  %8s   %14s %11s %11s  |")
+        line = sum_format % (
+            "USER", "TOTAL GPU MEM", "TOTAL %CPU", "TOTAL %MEM"
+        )
         print(line)
+        print("+" + ("-" * (len(line) - 2)) + "+")
+        for user in user_detail:
+            if len(args.user) > 0:
+                if user[:7] != args.user[:7]:
+                    continue
+            print(sum_format % (
+                user,
+                str(user_detail[user]["total_gpu_mem"]) + "MiB",
+                str(round(user_detail[user]["total_cpu"], 1)),
+                str(round(user_detail[user]["total_mem"], 1))
+            ))
 
-    no_running_process = "No running processes found"
-    if no_running_process in lines[ps_start_idx] or lines[ps_start_idx].startswith("+--"):
-        print(lines[-1].strip())
-        print("| " + no_running_process + " " * (73 - len(no_running_process)) + "   |")
-        # Issue #9, running inside docker and seeing no processes
-        if lines[ps_start_idx].startswith("+--"):
-            print("| If you're running in a container, you'll only see processes running inside. |")
-        print(lines[-1])
-        sys.exit()
-
-    # Get all process detail
-    ps_detail, user_detail = get_process_user_detail(ps_start_idx, is_new_format, lines)
-
-    # Print process detail
-    max_pid_length = max(5, max([len(x) for x in ps_detail["pid"]]))
-    print_format = ("|  %3s %" + str(max_pid_length) + "s %8s   %8s %5s %5s %9s  %-" + str(command_length) + "." + str(command_length) + "s  |")
-
-    line = print_format % (
-        "GPU", "PID", "USER", "GPU MEM", "%CPU", "%MEM", "TIME", "COMMAND"
-    )
-
-    print("+" + ("-" * (len(line) - 2)) + "+")
-
-    print(line)
-
-    for i in range(len(ps_detail["pid"])):
-        if len(args.user) > 0:
-            if ps_detail["user"][i][:7] != args.user[:7]:
-                continue
-        print(print_format % (
-            ps_detail["gpu_num"][i],
-            ps_detail["pid"][i],
-            ps_detail["user"][i],
-            ps_detail["gpu_mem"][i],
-            ps_detail["cpu"][i],
-            ps_detail["mem"][i],
-            ps_detail["time"][i],
-            ps_detail["command"][i]
-        ))
-
-    print("+" + ("-" * (len(line) - 2)) + "+")
-
-    # Print user detail
-    sum_format = ("|  %8s   %14s %11s %11s  |")
-    line = sum_format % (
-        "USER", "TOTAL GPU MEM", "TOTAL %CPU", "TOTAL %MEM"
-    )
-    print(line)
-    print("+" + ("-" * (len(line) - 2)) + "+")
-    for user in user_detail:
-        if len(args.user) > 0:
-            if user[:7] != args.user[:7]:
-                continue
-        print(sum_format % (
-            user,
-            str(user_detail[user]["total_gpu_mem"]) + "MiB",
-            str(round(user_detail[user]["total_cpu"], 1)),
-            str(round(user_detail[user]["total_mem"], 1))
-        ))
+        print("+" + ("-" * (len(line) - 2)) + "+")
 
-    print("+" + ("-" * (len(line) - 2)) + "+")
+        time.sleep(args.loop)
```

### Comparing `nvidia-smi2-0.0.1.post3/nvidia_smi2.egg-info/PKG-INFO` & `nvidia-smi2-0.0.2.post1/nvidia_smi2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-smi2
-Version: 0.0.1.post3
+Version: 0.0.2.post1
 Author: NNDam, PD-Mera
 Description-Content-Type: text/markdown
 
 # nvidia-smi2
 
 A tool for enriching the output of nvidia-smi.
 
@@ -14,45 +14,47 @@
 
 Install
 
     pip install nvidia-smi2
     
 Run
 
-    nvidia-smi2 [-l [length]] [-u [username]]
+    nvidia-smi2 [-L [length]] [-u [username]]
       print GPU utilization with usernames and CPU stats for each GPU-utilizing process
 
-      -l|--command-length [length]     Print longer part of the commandline. If `length'
+      -L|--command-length [length]     Print longer part of the commandline. If `length'
                                        is provided, use it as the commandline length,
                                        otherwise print first 100 characters.
       -c|--color                       Colorize the output (green - free GPU, yellow -
                                        moderately used GPU, red - fully used GPU)
       -u|--user                        Name of user to summarize
+      -l|--loop                        Loop nvidia-smi2 after a period of time
 
 Or run from src
 
     pip install termcolor
     chmod a+x nvidia-htop.py
-    ./nvidia-htop.py [-l [length]] [-u [username]]
+    ./nvidia-htop.py [-L [length]] [-u [username]]
       print GPU utilization with usernames and CPU stats for each GPU-utilizing process
 
-      -l|--command-length [length]     Print longer part of the commandline. If `length'
+      -L|--command-length [length]     Print longer part of the commandline. If `length'
                                        is provided, use it as the commandline length,
                                        otherwise print first 100 characters.
       -c|--color                       Colorize the output (green - free GPU, yellow -
                                        moderately used GPU, red - fully used GPU)
       -u|--user                        Name of user to summarize
+      -l|--loop                        Loop nvidia-smi2 after a period of time
 
-Note: for backward compatibility, `nvidia-smi | ./nvidia-htop.py [-l [length]] [-u [username]]` is also supported.
+Note: for backward compatibility, `nvidia-smi | ./nvidia-htop.py [-L [length]] [-u [username]]` is also supported.
 
 Note: running inside a container (docker, singularity, ...), `nvidia-smi` can only see processes running in the container.
 
 ## Example output
 ```
-rnd@rnd:~$ nvidia-smi2 -l
+rnd@rnd:~$ nvidia-smi2 -L
 Wed Jul 12 10:41:16 2023
 +-----------------------------------------------------------------------------+
 | NVIDIA-SMI 470.57.02    Driver Version: 470.57.02    CUDA Version: 11.4     |
 |-------------------------------+----------------------+----------------------+
 | GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
 | Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
 |                               |                      |               MIG M. |
@@ -87,15 +89,15 @@
 |   anonym1          2365MiB         2.9         3.1  |
 |       rnd           135MiB         0.1         0.8  |
 |   anonym2          6917MiB       128.0         4.3  |
 +-----------------------------------------------------+
 ```
 
 ```
-rnd@rnd:~$ nvidia-smi2 -l -u root
+rnd@rnd:~$ nvidia-smi2 -L -u root
 Wed Jul 12 10:51:06 2023
 +-----------------------------------------------------------------------------+
 | NVIDIA-SMI 470.57.02    Driver Version: 470.57.02    CUDA Version: 11.4     |
 |-------------------------------+----------------------+----------------------+
 | GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
 | Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
 |                               |                      |               MIG M. |
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 2.1 Name: nvidia-smi2 Version: 0.0.1.post3 Author: NNDam, PD-
+Metadata-Version: 2.1 Name: nvidia-smi2 Version: 0.0.2.post1 Author: NNDam, PD-
 Mera Description-Content-Type: text/markdown # nvidia-smi2 A tool for enriching
 the output of nvidia-smi. [Alt_text] ## Usage Install pip install nvidia-smi2
-Run nvidia-smi2 [-l [length]] [-u [username]] print GPU utilization with
-usernames and CPU stats for each GPU-utilizing process -l|--command-length
+Run nvidia-smi2 [-L [length]] [-u [username]] print GPU utilization with
+usernames and CPU stats for each GPU-utilizing process -L|--command-length
 [length] Print longer part of the commandline. If `length' is provided, use it
 as the commandline length, otherwise print first 100 characters. -c|--color
 Colorize the output (green - free GPU, yellow - moderately used GPU, red -
-fully used GPU) -u|--user Name of user to summarize Or run from src pip install
-termcolor chmod a+x nvidia-htop.py ./nvidia-htop.py [-l [length]] [-u
-[username]] print GPU utilization with usernames and CPU stats for each GPU-
-utilizing process -l|--command-length [length] Print longer part of the
-commandline. If `length' is provided, use it as the commandline length,
-otherwise print first 100 characters. -c|--color Colorize the output (green -
-free GPU, yellow - moderately used GPU, red - fully used GPU) -u|--user Name of
-user to summarize Note: for backward compatibility, `nvidia-smi | ./nvidia-
-htop.py [-l [length]] [-u [username]]` is also supported. Note: running inside
-a container (docker, singularity, ...), `nvidia-smi` can only see processes
-running in the container. ## Example output ``` rnd@rnd:~$ nvidia-smi2 -l Wed
-Jul 12 10:41:16 2023 +---------------------------------------------------------
---------------------+ | NVIDIA-SMI 470.57.02 Driver Version: 470.57.02 CUDA
-Version: 11.4 | |-------------------------------+----------------------+-------
----------------+ | GPU Name Persistence-M| Bus-Id Disp.A | Volatile Uncorr. ECC
-| | Fan Temp Perf Pwr:Usage/Cap| Memory-Usage | GPU-Util Compute M. | | | | MIG
-M. |
+fully used GPU) -u|--user Name of user to summarize -l|--loop Loop nvidia-smi2
+after a period of time Or run from src pip install termcolor chmod a+x nvidia-
+htop.py ./nvidia-htop.py [-L [length]] [-u [username]] print GPU utilization
+with usernames and CPU stats for each GPU-utilizing process -L|--command-length
+[length] Print longer part of the commandline. If `length' is provided, use it
+as the commandline length, otherwise print first 100 characters. -c|--color
+Colorize the output (green - free GPU, yellow - moderately used GPU, red -
+fully used GPU) -u|--user Name of user to summarize -l|--loop Loop nvidia-smi2
+after a period of time Note: for backward compatibility, `nvidia-smi | ./
+nvidia-htop.py [-L [length]] [-u [username]]` is also supported. Note: running
+inside a container (docker, singularity, ...), `nvidia-smi` can only see
+processes running in the container. ## Example output ``` rnd@rnd:~$ nvidia-
+smi2 -L Wed Jul 12 10:41:16 2023 +---------------------------------------------
+--------------------------------+ | NVIDIA-SMI 470.57.02 Driver Version:
+470.57.02 CUDA Version: 11.4 | |-------------------------------+---------------
+-------+----------------------+ | GPU Name Persistence-M| Bus-Id Disp.A |
+Volatile Uncorr. ECC | | Fan Temp Perf Pwr:Usage/Cap| Memory-Usage | GPU-Util
+Compute M. | | | | MIG M. |
 |===============================+======================+======================|
 | 0 NVIDIA GeForce ... On | 00000000:01:00.0 Off | N/A | | 55% 73C P2 88W /
 280W | 3248MiB / 11176MiB | 64% Default | | | | N/A | +------------------------
 -------+----------------------+----------------------+ | 1 NVIDIA GeForce ...
 On | 00000000:02:00.0 Off | N/A | | 59% 67C P2 91W / 280W | 9397MiB / 11178MiB
 | 7% Default | | | | N/A | +-------------------------------+-------------------
 ---+----------------------+ +--------------------------------------------------
@@ -45,15 +46,15 @@
 128 4.3 22:30:29 python train_image_classifier.py xxxx | | 1 27877 root 2017MiB
 9.4 1.4 15 days python consumer.py | +-----------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------+ | USER TOTAL GPU MEM TOTAL %CPU TOTAL
 %MEM | +-----------------------------------------------------+ | root 3210MiB
 158.6 9.8 | | gdm 4MiB 0.0 0.0 | | anonym1 2365MiB 2.9 3.1 | | rnd 135MiB 0.1
 0.8 | | anonym2 6917MiB 128.0 4.3 | +------------------------------------------
------------+ ``` ``` rnd@rnd:~$ nvidia-smi2 -l -u root Wed Jul 12 10:51:06 2023
+-----------+ ``` ``` rnd@rnd:~$ nvidia-smi2 -L -u root Wed Jul 12 10:51:06 2023
 +-----------------------------------------------------------------------------
 + | NVIDIA-SMI 470.57.02 Driver Version: 470.57.02 CUDA Version: 11.4 | |------
 -------------------------+----------------------+----------------------+ | GPU
 Name Persistence-M| Bus-Id Disp.A | Volatile Uncorr. ECC | | Fan Temp Perf Pwr:
 Usage/Cap| Memory-Usage | GPU-Util Compute M. | | | | MIG M. |
 |===============================+======================+======================|
 | 0 NVIDIA GeForce ... On | 00000000:01:00.0 Off | N/A | | 58% 69C P2 106W /
```

