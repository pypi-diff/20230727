# Comparing `tmp/grpc4bmi-0.3.2.tar.gz` & `tmp/grpc4bmi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grpc4bmi-0.3.2.tar", last modified: Mon Oct 19 13:47:58 2020, max compression
+gzip compressed data, was "grpc4bmi-0.4.0.tar", last modified: Tue Mar 21 11:48:01 2023, max compression
```

## Comparing `grpc4bmi-0.3.2.tar` & `grpc4bmi-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,46 @@
-drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     7713 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/PKG-INFO
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1923 2020-10-19 13:32:28.000000 grpc4bmi-0.3.2/setup.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)      266 2020-07-30 07:53:20.000000 grpc4bmi-0.3.2/pyproject.toml
-drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi.egg-info/
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)      791 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi.egg-info/SOURCES.txt
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)       14 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi.egg-info/top_level.txt
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     7713 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi.egg-info/PKG-INFO
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)       61 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi.egg-info/entry_points.txt
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)      148 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi.egg-info/requires.txt
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        1 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi.egg-info/dependency_links.txt
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)       38 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/setup.cfg
-drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/test/
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     7925 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/test_subproc.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     2112 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/flatbmiheat.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     8991 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/test_legacy_server.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1718 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/conftest.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        0 2020-03-11 08:40:13.000000 grpc4bmi-0.3.2/test/__init__.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     2747 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/test_singularity.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    15767 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/test_server.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     3435 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/test_docker.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1470 2020-03-11 08:40:13.000000 grpc4bmi-0.3.2/test/test_utils.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    10523 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/fake_models.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    26239 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/test/test_client.py
-drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2020-10-19 13:47:58.000000 grpc4bmi-0.3.2/grpc4bmi/
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    15764 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_grpc_server.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        0 2020-03-11 08:40:13.000000 grpc4bmi-0.3.2/grpc4bmi/__init__.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     5405 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_r_model.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1784 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/reserve.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     4211 2020-10-19 13:32:02.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_client_singularity.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    32836 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_pb2_grpc.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1261 2020-03-24 11:18:34.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_client_subproc.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    70570 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_pb2.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1905 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/utils.py
--rwxrwxr-x   0 verhoes   (1000) verhoes   (1000)     5580 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/run_server.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    16474 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_grpc_client.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     5294 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_client_docker.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    11173 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/grpc4bmi/bmi_grpc_legacy_server.py
--rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     5691 2020-10-19 13:30:31.000000 grpc4bmi-0.3.2/README.md
+drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2023-03-21 11:48:01.275981 grpc4bmi-0.4.0/
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    11357 2020-03-11 08:40:13.000000 grpc4bmi-0.4.0/LICENSE
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     7769 2023-03-21 11:48:01.271981 grpc4bmi-0.4.0/PKG-INFO
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     6610 2023-03-21 11:47:47.000000 grpc4bmi-0.4.0/README.md
+drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2023-03-21 11:48:01.271981 grpc4bmi-0.4.0/grpc4bmi/
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        0 2020-03-11 08:40:13.000000 grpc4bmi-0.4.0/grpc4bmi/__init__.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    12081 2023-03-21 10:54:47.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_client_apptainer.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     4952 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_client_docker.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    12592 2023-03-21 10:54:47.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_client_singularity.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1261 2020-03-24 11:18:34.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_client_subproc.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    17152 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_grpc_client.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    11025 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_grpc_legacy_server.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    15764 2023-01-06 07:58:32.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_grpc_server.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     5868 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_memoized.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     8053 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_optionaldest.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    13387 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_pb2.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    63387 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_pb2_grpc.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     5834 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/bmi_r_model.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)       77 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/constants.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)      631 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/exceptions.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        0 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/py.typed
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     2691 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/reserve.py
+-rwxrwxr-x   0 verhoes   (1000) verhoes   (1000)     5580 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/grpc4bmi/run_server.py
+drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2023-03-21 11:48:01.271981 grpc4bmi-0.4.0/grpc4bmi.egg-info/
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     7769 2023-03-21 11:48:01.000000 grpc4bmi-0.4.0/grpc4bmi.egg-info/PKG-INFO
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)      969 2023-03-21 11:48:01.000000 grpc4bmi-0.4.0/grpc4bmi.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        1 2023-03-21 11:48:01.000000 grpc4bmi-0.4.0/grpc4bmi.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)       60 2023-03-21 11:48:01.000000 grpc4bmi-0.4.0/grpc4bmi.egg-info/entry_points.txt
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)      342 2023-03-21 11:48:01.000000 grpc4bmi-0.4.0/grpc4bmi.egg-info/requires.txt
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        9 2023-03-21 11:48:01.000000 grpc4bmi-0.4.0/grpc4bmi.egg-info/top_level.txt
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     2032 2023-03-21 11:47:47.000000 grpc4bmi-0.4.0/pyproject.toml
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)       38 2023-03-21 11:48:01.275981 grpc4bmi-0.4.0/setup.cfg
+drwxrwxr-x   0 verhoes   (1000) verhoes   (1000)        0 2023-03-21 11:48:01.271981 grpc4bmi-0.4.0/test/
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)        0 2020-03-11 08:40:13.000000 grpc4bmi-0.4.0/test/__init__.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     1677 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/conftest.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    10837 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/fake_models.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     4494 2023-03-21 10:54:47.000000 grpc4bmi-0.4.0/test/test_apptainer.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    27717 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_client.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     5157 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_docker.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    10680 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_legacy_server.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     4106 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_memoized.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     4395 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_optionaldest.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     2959 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_r.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    15178 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_server.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)    10184 2023-03-21 10:54:47.000000 grpc4bmi-0.4.0/test/test_singularity.py
+-rw-rw-r--   0 verhoes   (1000) verhoes   (1000)     8346 2023-03-20 14:19:00.000000 grpc4bmi-0.4.0/test/test_subproc.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grpc4bmi-0.3.2/PKG-INFO` & `grpc4bmi-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,188 @@
 Metadata-Version: 2.1
 Name: grpc4bmi
-Version: 0.3.2
+Version: 0.4.0
 Summary: Run your BMI implementation in a separate process and expose it as BMI-python with GRPC
-Home-page: https://github.com/eWaterCycle/grpc4bmi
-Author: Gijs van den Oord
-Author-email: g.vandenoord@esciencecenter.nl
-License: Apache License, Version 2.0
-Description: # grpc4bmi
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1462641.svg)](https://doi.org/10.5281/zenodo.1462641)
-        [![CI](https://github.com/eWaterCycle/grpc4bmi/workflows/CI/badge.svg)](https://github.com/eWaterCycle/grpc4bmi/actions?query=workflow%3ACI)
-        [![Documentation Status](https://readthedocs.org/projects/grpc4bmi/badge/?version=latest)](https://grpc4bmi.readthedocs.io/en/latest/?badge=latest)
-        [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=alert_status)](https://sonarcloud.io/dashboard?id=grpc4bmi)
-        [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=coverage)](https://sonarcloud.io/dashboard?id=grpc4bmi)
-        
-        ## Purpose
-        
-        This software allows you to wrap your Basic Model Interface (BMI) implementation ([https://github.com/csdms/bmi](https://github.com/csdms/bmi)) in a server process and communicate with it via the included Python client. The communication is serialized to protocol buffers by gRPC ([https://grpc.io/](https://grpc.io/)) and occurs over network ports.
-        
-        ## Installation
-        
-        Optionally, create your virtual environment and activate it, Then, run
-        
-        ```bash
-        pip install grpc4bmi
-        ```
-        
-        on the client (Python) side. If your server model is implemented in Python, do the same in the server environment (e.g. docker container). If the model is implemented in R, run instead
-        
-        ```bash
-        pip install grpc4bmi[R]
-        ```
-        
-        in the server environment. For bleeding edge version from GitHub use
-        
-        ```bash
-        pip install git+https://github.com/eWaterCycle/grpc4bmi.git#egg=grpc4bmi
-        ```
-        
-        Finally if the model is implemented in C or C++, clone this git repo and run
-        
-        ```bash
-        make
-        make install
-        ```
-        
-        in the cpp folder.
-        
-        ## Usage
-        
-        ### Model written in Python
-        
-        For inspiration look at the example in the test directory. To start a server process that allows calls to your BMI implementation, type
-        
-        ```bash
-        run-bmi-server --name <PACKAGE>.<MODULE>.<CLASS> --port <PORT> --path <PATH>
-        ```
-        
-        where ```<PACKAGE>, <MODULE>``` are the Python package and module containing your implementation, ```<CLASS>``` is your
-        bmi model class name, ```<PORT>``` is any available port on the host system, and optionally ```<PATH>``` denotes an
-        additional path that should be added to the system path to make your implementation work. The name option above is
-        optional, and if not provided the script will look at the environment variables ```BMI_PACKAGE```, ```BMI_MODULE``` and
-        ```BMI_CLASS```. Similarly, the port can be defined by the environment variable ```BMI_PORT```.
-        This software assumes that your implementation constructor has no parameters.
-        
-        ### Model written in C/C++ (beta)
-        
-        Create an executable along the lines of cpp/run-bmi-server.cc. You can copy the file and replace the function
-        
-        ```C++
-        Bmi* create_model_instance()
-        {
-            /* Return your new BMI instance pointer here... */
-        }
-        ```
-        
-        with the instantiation of your model BMI. The model needs to implement the csdms BMI for C, but you may also implement our more object-oriented C++ interface [BmiCppExtension](https://github.com/eWaterCycle/grpc4bmi/blob/master/cpp/bmi_cpp_extension.h).
-        
-        ### Model written in R
-        
-        The grpc4bmi Python package can also run BMI models written in R if the model is a subclass of [AbstractBmi](https://github.com/eWaterCycle/bmi-r/blob/master/R/abstract-bmi.R#L9)
-        See [https://github.com/eWaterCycle/bmi-r](https://github.com/eWaterCycle/bmi-r) for instruction on R and Docker.
-        
-        Run the R model a server with
-        
-        ```bash
-        run-bmi-server --lang R [--path <R file with BMI model>] --name [<PACKAGE>::]<CLASS> --port <PORT>
-        ```
-        
-        For example with [WALRUS](https://github.com/eWaterCycle/grpc4bmi-examples/tree/master/walrus) use
-        
-        ```bash
-        run-bmi-server --lang R --path ~/git/eWaterCycle/grpc4bmi-examples/walrus/walrus-bmi.r --name WalrusBmi --port 55555
-        ```
-        
-        ### The client side
-        
-        The client side has only a Python implementation. The default BMI client assumes a running server process on a given port.
-        
-        ```python
-        from grpc4bmi.bmi_grpc_client import BmiClient
-        import grpc
-        mymodel = BmiClient(grpc.insecure_channel("localhost:<PORT>"))
-        print mymodel.get_component_name()
-        mymodel.initialize(<FILEPATH>)
-        ...further BMI calls...
-        ```
-        
-        The package contains also client implementation that own the server process, either as a Python subprocess or a docker
-        image or a singularity image running the ```run-bmi-server``` script. For instance
-        
-        ```python
-        from grpc4bmi.bmi_client_subproc import BmiClientSubProcess
-        mymodel = BmiClientSubProcess(<PACKAGE>.<MODULE>.<CLASS>)
-        ```
-        
-        will automatically launch the server in a sub-process and
-        
-        ```python
-        from grpc4bmi.bmi_client_subproc import BmiClientDocker
-        mymodel = BmiClientDocker(<IMAGE>,<PORT>)
-        ```
-        
-        will launch a docker container, assuming that a gRPC BMI server will start and exposes the port ```<PORT>```.
-        
-        ```python
-        from grpc4bmi.bmi_client_singularity import BmiClientSingularity
-        mymodel = BmiClientSingularity(<IMAGE>,<PORT>)
-        ```
-        
-        will launch a singularity container, assuming that a gRPC BMI server will start and exposes the port ```<PORT>```.
-        
-        For more documentation see [https://grpc4bmi.readthedocs.io/](https://grpc4bmi.readthedocs.io/).
-        
-        ## Development: generating the gRPC code
-        
-        When developers change the proto-file, it is necessary to install gRPC tools Python packages in your Python environment:
-        
-        ```bash
-        pip install -r requirements.txt
-        pip install -e .
-        # For R integration also install the R extras with
-        pip install -e .[R]
-        ```
-        
-        and install the C++ runtime and `protoc` command as described in <https://github.com/google/protobuf/blob/master/src/README.md>.
-        After this, simply executing the `proto_gen.sh` script should do the job.
-        
-        ## Future work
-        
-        More language bindings are underway.
-        
-Platform: UNKNOWN
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/eWaterCycle/grpc4bmi
+Project-URL: Bug Tracker, https://github.com/eWaterCycle/grpc4bmi/issues
+Project-URL: Documentation, https://grpc4bmi.readthedocs.io/
+Project-URL: Source code, https://github.com/eWaterCycle/grpc4bmi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: R
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
+# grpc4bmi
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1462641.svg)](https://doi.org/10.5281/zenodo.1462641)
+[![CI](https://github.com/eWaterCycle/grpc4bmi/workflows/CI/badge.svg)](https://github.com/eWaterCycle/grpc4bmi/actions?query=workflow%3ACI)
+[![Documentation Status](https://readthedocs.org/projects/grpc4bmi/badge/?version=latest)](https://grpc4bmi.readthedocs.io/en/latest/?badge=latest)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=alert_status)](https://sonarcloud.io/dashboard?id=grpc4bmi)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=coverage)](https://sonarcloud.io/dashboard?id=grpc4bmi)
+
+## Purpose
+
+This software allows you to wrap your [Basic Model Interface (BMI)](https://github.com/csdms/bmi) implementation in a server process and communicate with it via the included Python client. The communication is serialized to protocol buffers by [GRPC](https://grpc.io/) and occurs over network ports. Can run models in isolated containers using Docker or Apptainer.
+
+## Installation
+
+Optionally, create your virtual environment and activate it, Then, run
+
+```bash
+pip install grpc4bmi
+```
+
+on the client (Python) side. If your server model is implemented in Python, do the same in the server environment (e.g. docker container). If the model is implemented in R, run instead
+
+```bash
+pip install grpc4bmi[R]
+```
+
+in the server environment. For bleeding edge version from GitHub use
+
+```bash
+pip install git+https://github.com/eWaterCycle/grpc4bmi.git#egg=grpc4bmi
+```
+
+Finally if the model is implemented in C or C++, clone this git repo and run
+
+```bash
+make
+make install
+```
+
+in the cpp folder.
+
+## Usage
+
+### Model written in Python
+
+A model should be a subclass of the `Bmi` class from the [bmipy](https://pypi.org/project/bmipy/2.0/) package.
+
+For inspiration look at the [example](test/fake_models.py) in the test directory. 
+
+To start a server process that allows calls to your BMI implementation, type
+
+```bash
+run-bmi-server --name <PACKAGE>.<MODULE>.<CLASS> --port <PORT> --path <PATH>
+```
+
+where ```<PACKAGE>, <MODULE>``` are the python package and module containing your implementation, ```<CLASS>``` is your
+bmi model class name, ```<PORT>``` is any available port on the host system, and optionally ```<PATH>``` denotes an
+additional path that should be added to the system path to make your implementation work. The name option above is
+optional, and if not provided the script will look at the environment variables ```BMI_PACKAGE```, ```BMI_MODULE``` and
+```BMI_CLASS```. Similarly, the port can be defined by the environment variable ```BMI_PORT```.
+This software assumes that your implementation constructor has no parameters.
+
+### Model written in C/C++ (beta)
+
+Create an executable along the lines of cpp/run-bmi-server.cc. You can copy the file and replace the function
+
+```C++
+Bmi* create_model_instance()
+{
+    /* Return your new BMI instance pointer here... */
+}
+```
+
+with the instantiation of your model BMI. The model needs to implement the csdms BMI for C, but you may also implement our more object-oriented C++ interface [BmiCppExtension](https://github.com/eWaterCycle/grpc4bmi/blob/master/cpp/bmi_cpp_extension.h).
+
+### Model written in R
+
+The grpc4bmi Python package can also run BMI models written in R if the model is a subclass of [AbstractBmi](https://github.com/eWaterCycle/bmi-r/blob/master/R/abstract-bmi.R#L9)
+See [https://github.com/eWaterCycle/bmi-r](https://github.com/eWaterCycle/bmi-r) for instruction on R and Docker.
+
+Run the R model a server with
+
+```bash
+run-bmi-server --lang R [--path <R file with BMI model>] --name [<PACKAGE>::]<CLASS> --port <PORT>
+```
+
+For example with [WALRUS](https://github.com/eWaterCycle/grpc4bmi-examples/tree/master/walrus) use
+
+```bash
+run-bmi-server --lang R --path ~/git/eWaterCycle/grpc4bmi-examples/walrus/walrus-bmi.r --name WalrusBmi --port 55555
+```
+
+### The client side
+
+The client side has only a Python implementation. The default BMI client assumes a running server process on a given port.
+
+```python
+from grpc4bmi.bmi_grpc_client import BmiClient
+import grpc
+mymodel = BmiClient(grpc.insecure_channel("localhost:<PORT>"))
+print mymodel.get_component_name()
+mymodel.initialize(<FILEPATH>)
+...further BMI calls...
+```
+
+The package contains also client implementation that own the server process, either as a Python subprocess or a Docker
+container or a Singularity container or a Apptainer container running the ```run-bmi-server``` script. For instance
+```python
+from grpc4bmi.bmi_client_subproc import BmiClientSubProcess
+mymodel = BmiClientSubProcess(<PACKAGE>.<MODULE>.<CLASS>)
+```
+
+will automatically launch the server in a sub-process and
+
+```python
+from grpc4bmi.bmi_client_docker import BmiClientDocker
+mymodel = BmiClientDocker(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
+```
+will launch a Docker container based on supplied Docker image
+and will mount supplied directories to share files between the container and host.
+
+```python
+from grpc4bmi.bmi_client_singularity import BmiClientSingularity
+mymodel = BmiClientSingularity(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
+```
+will launch a singularity container on based supplied Singularity image
+and will mount supplied directories to share files between the container and host.
+
+```python
+from grpc4bmi.bmi_client_apptainer import BmiClientApptainer
+mymodel = BmiClientApptainer(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
+```
+will launch a Apptainer container on based supplied Apptainer image
+and will mount supplied directories to share files between the container and host.
+
+For more documentation see [https://grpc4bmi.readthedocs.io/](https://grpc4bmi.readthedocs.io/).
+
+## Development: generating the gRPC code
+
+When developers change the proto-file, it is necessary to install gRPC tools Python packages in your Python environment:
+
+```bash
+# Create virtual env
+python3 -m venv .venv
+. venv/bin/activate
+# Make sure latest pip and wheel are install
+pip install -U pip wheel
+pip install -r dev-requirements.txt
+# For R integration also install the R extras with
+pip install -e .[R]
+# For building docs (cd docs && make html) also install the docs extras with
+pip install -e .[docs]
+```
+
+and install the C++ runtime and `protoc` command as described in <https://github.com/google/protobuf/blob/master/src/README.md>.
+After this, simply executing the `proto_gen.sh` script should do the job.
+
+## Future work
+
+More language bindings are underway.
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi.egg-info/SOURCES.txt` & `grpc4bmi-0.4.0/grpc4bmi.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,40 @@
+LICENSE
 README.md
 pyproject.toml
-setup.py
 grpc4bmi/__init__.py
+grpc4bmi/bmi_client_apptainer.py
 grpc4bmi/bmi_client_docker.py
 grpc4bmi/bmi_client_singularity.py
 grpc4bmi/bmi_client_subproc.py
 grpc4bmi/bmi_grpc_client.py
 grpc4bmi/bmi_grpc_legacy_server.py
 grpc4bmi/bmi_grpc_server.py
+grpc4bmi/bmi_memoized.py
+grpc4bmi/bmi_optionaldest.py
 grpc4bmi/bmi_pb2.py
 grpc4bmi/bmi_pb2_grpc.py
 grpc4bmi/bmi_r_model.py
+grpc4bmi/constants.py
+grpc4bmi/exceptions.py
+grpc4bmi/py.typed
 grpc4bmi/reserve.py
 grpc4bmi/run_server.py
-grpc4bmi/utils.py
 grpc4bmi.egg-info/PKG-INFO
 grpc4bmi.egg-info/SOURCES.txt
 grpc4bmi.egg-info/dependency_links.txt
 grpc4bmi.egg-info/entry_points.txt
 grpc4bmi.egg-info/requires.txt
 grpc4bmi.egg-info/top_level.txt
 test/__init__.py
 test/conftest.py
 test/fake_models.py
-test/flatbmiheat.py
+test/test_apptainer.py
 test/test_client.py
 test/test_docker.py
 test/test_legacy_server.py
+test/test_memoized.py
+test/test_optionaldest.py
+test/test_r.py
 test/test_server.py
 test/test_singularity.py
-test/test_subproc.py
-test/test_utils.py
+test/test_subproc.py
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi.egg-info/PKG-INFO` & `grpc4bmi-0.4.0/grpc4bmi.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,188 @@
 Metadata-Version: 2.1
 Name: grpc4bmi
-Version: 0.3.2
+Version: 0.4.0
 Summary: Run your BMI implementation in a separate process and expose it as BMI-python with GRPC
-Home-page: https://github.com/eWaterCycle/grpc4bmi
-Author: Gijs van den Oord
-Author-email: g.vandenoord@esciencecenter.nl
-License: Apache License, Version 2.0
-Description: # grpc4bmi
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1462641.svg)](https://doi.org/10.5281/zenodo.1462641)
-        [![CI](https://github.com/eWaterCycle/grpc4bmi/workflows/CI/badge.svg)](https://github.com/eWaterCycle/grpc4bmi/actions?query=workflow%3ACI)
-        [![Documentation Status](https://readthedocs.org/projects/grpc4bmi/badge/?version=latest)](https://grpc4bmi.readthedocs.io/en/latest/?badge=latest)
-        [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=alert_status)](https://sonarcloud.io/dashboard?id=grpc4bmi)
-        [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=coverage)](https://sonarcloud.io/dashboard?id=grpc4bmi)
-        
-        ## Purpose
-        
-        This software allows you to wrap your Basic Model Interface (BMI) implementation ([https://github.com/csdms/bmi](https://github.com/csdms/bmi)) in a server process and communicate with it via the included Python client. The communication is serialized to protocol buffers by gRPC ([https://grpc.io/](https://grpc.io/)) and occurs over network ports.
-        
-        ## Installation
-        
-        Optionally, create your virtual environment and activate it, Then, run
-        
-        ```bash
-        pip install grpc4bmi
-        ```
-        
-        on the client (Python) side. If your server model is implemented in Python, do the same in the server environment (e.g. docker container). If the model is implemented in R, run instead
-        
-        ```bash
-        pip install grpc4bmi[R]
-        ```
-        
-        in the server environment. For bleeding edge version from GitHub use
-        
-        ```bash
-        pip install git+https://github.com/eWaterCycle/grpc4bmi.git#egg=grpc4bmi
-        ```
-        
-        Finally if the model is implemented in C or C++, clone this git repo and run
-        
-        ```bash
-        make
-        make install
-        ```
-        
-        in the cpp folder.
-        
-        ## Usage
-        
-        ### Model written in Python
-        
-        For inspiration look at the example in the test directory. To start a server process that allows calls to your BMI implementation, type
-        
-        ```bash
-        run-bmi-server --name <PACKAGE>.<MODULE>.<CLASS> --port <PORT> --path <PATH>
-        ```
-        
-        where ```<PACKAGE>, <MODULE>``` are the Python package and module containing your implementation, ```<CLASS>``` is your
-        bmi model class name, ```<PORT>``` is any available port on the host system, and optionally ```<PATH>``` denotes an
-        additional path that should be added to the system path to make your implementation work. The name option above is
-        optional, and if not provided the script will look at the environment variables ```BMI_PACKAGE```, ```BMI_MODULE``` and
-        ```BMI_CLASS```. Similarly, the port can be defined by the environment variable ```BMI_PORT```.
-        This software assumes that your implementation constructor has no parameters.
-        
-        ### Model written in C/C++ (beta)
-        
-        Create an executable along the lines of cpp/run-bmi-server.cc. You can copy the file and replace the function
-        
-        ```C++
-        Bmi* create_model_instance()
-        {
-            /* Return your new BMI instance pointer here... */
-        }
-        ```
-        
-        with the instantiation of your model BMI. The model needs to implement the csdms BMI for C, but you may also implement our more object-oriented C++ interface [BmiCppExtension](https://github.com/eWaterCycle/grpc4bmi/blob/master/cpp/bmi_cpp_extension.h).
-        
-        ### Model written in R
-        
-        The grpc4bmi Python package can also run BMI models written in R if the model is a subclass of [AbstractBmi](https://github.com/eWaterCycle/bmi-r/blob/master/R/abstract-bmi.R#L9)
-        See [https://github.com/eWaterCycle/bmi-r](https://github.com/eWaterCycle/bmi-r) for instruction on R and Docker.
-        
-        Run the R model a server with
-        
-        ```bash
-        run-bmi-server --lang R [--path <R file with BMI model>] --name [<PACKAGE>::]<CLASS> --port <PORT>
-        ```
-        
-        For example with [WALRUS](https://github.com/eWaterCycle/grpc4bmi-examples/tree/master/walrus) use
-        
-        ```bash
-        run-bmi-server --lang R --path ~/git/eWaterCycle/grpc4bmi-examples/walrus/walrus-bmi.r --name WalrusBmi --port 55555
-        ```
-        
-        ### The client side
-        
-        The client side has only a Python implementation. The default BMI client assumes a running server process on a given port.
-        
-        ```python
-        from grpc4bmi.bmi_grpc_client import BmiClient
-        import grpc
-        mymodel = BmiClient(grpc.insecure_channel("localhost:<PORT>"))
-        print mymodel.get_component_name()
-        mymodel.initialize(<FILEPATH>)
-        ...further BMI calls...
-        ```
-        
-        The package contains also client implementation that own the server process, either as a Python subprocess or a docker
-        image or a singularity image running the ```run-bmi-server``` script. For instance
-        
-        ```python
-        from grpc4bmi.bmi_client_subproc import BmiClientSubProcess
-        mymodel = BmiClientSubProcess(<PACKAGE>.<MODULE>.<CLASS>)
-        ```
-        
-        will automatically launch the server in a sub-process and
-        
-        ```python
-        from grpc4bmi.bmi_client_subproc import BmiClientDocker
-        mymodel = BmiClientDocker(<IMAGE>,<PORT>)
-        ```
-        
-        will launch a docker container, assuming that a gRPC BMI server will start and exposes the port ```<PORT>```.
-        
-        ```python
-        from grpc4bmi.bmi_client_singularity import BmiClientSingularity
-        mymodel = BmiClientSingularity(<IMAGE>,<PORT>)
-        ```
-        
-        will launch a singularity container, assuming that a gRPC BMI server will start and exposes the port ```<PORT>```.
-        
-        For more documentation see [https://grpc4bmi.readthedocs.io/](https://grpc4bmi.readthedocs.io/).
-        
-        ## Development: generating the gRPC code
-        
-        When developers change the proto-file, it is necessary to install gRPC tools Python packages in your Python environment:
-        
-        ```bash
-        pip install -r requirements.txt
-        pip install -e .
-        # For R integration also install the R extras with
-        pip install -e .[R]
-        ```
-        
-        and install the C++ runtime and `protoc` command as described in <https://github.com/google/protobuf/blob/master/src/README.md>.
-        After this, simply executing the `proto_gen.sh` script should do the job.
-        
-        ## Future work
-        
-        More language bindings are underway.
-        
-Platform: UNKNOWN
+License: Apache License 2.0
+Project-URL: Homepage, https://github.com/eWaterCycle/grpc4bmi
+Project-URL: Bug Tracker, https://github.com/eWaterCycle/grpc4bmi/issues
+Project-URL: Documentation, https://grpc4bmi.readthedocs.io/
+Project-URL: Source code, https://github.com/eWaterCycle/grpc4bmi
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: R
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
+# grpc4bmi
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1462641.svg)](https://doi.org/10.5281/zenodo.1462641)
+[![CI](https://github.com/eWaterCycle/grpc4bmi/workflows/CI/badge.svg)](https://github.com/eWaterCycle/grpc4bmi/actions?query=workflow%3ACI)
+[![Documentation Status](https://readthedocs.org/projects/grpc4bmi/badge/?version=latest)](https://grpc4bmi.readthedocs.io/en/latest/?badge=latest)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=alert_status)](https://sonarcloud.io/dashboard?id=grpc4bmi)
+[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=coverage)](https://sonarcloud.io/dashboard?id=grpc4bmi)
+
+## Purpose
+
+This software allows you to wrap your [Basic Model Interface (BMI)](https://github.com/csdms/bmi) implementation in a server process and communicate with it via the included Python client. The communication is serialized to protocol buffers by [GRPC](https://grpc.io/) and occurs over network ports. Can run models in isolated containers using Docker or Apptainer.
+
+## Installation
+
+Optionally, create your virtual environment and activate it, Then, run
+
+```bash
+pip install grpc4bmi
+```
+
+on the client (Python) side. If your server model is implemented in Python, do the same in the server environment (e.g. docker container). If the model is implemented in R, run instead
+
+```bash
+pip install grpc4bmi[R]
+```
+
+in the server environment. For bleeding edge version from GitHub use
+
+```bash
+pip install git+https://github.com/eWaterCycle/grpc4bmi.git#egg=grpc4bmi
+```
+
+Finally if the model is implemented in C or C++, clone this git repo and run
+
+```bash
+make
+make install
+```
+
+in the cpp folder.
+
+## Usage
+
+### Model written in Python
+
+A model should be a subclass of the `Bmi` class from the [bmipy](https://pypi.org/project/bmipy/2.0/) package.
+
+For inspiration look at the [example](test/fake_models.py) in the test directory. 
+
+To start a server process that allows calls to your BMI implementation, type
+
+```bash
+run-bmi-server --name <PACKAGE>.<MODULE>.<CLASS> --port <PORT> --path <PATH>
+```
+
+where ```<PACKAGE>, <MODULE>``` are the python package and module containing your implementation, ```<CLASS>``` is your
+bmi model class name, ```<PORT>``` is any available port on the host system, and optionally ```<PATH>``` denotes an
+additional path that should be added to the system path to make your implementation work. The name option above is
+optional, and if not provided the script will look at the environment variables ```BMI_PACKAGE```, ```BMI_MODULE``` and
+```BMI_CLASS```. Similarly, the port can be defined by the environment variable ```BMI_PORT```.
+This software assumes that your implementation constructor has no parameters.
+
+### Model written in C/C++ (beta)
+
+Create an executable along the lines of cpp/run-bmi-server.cc. You can copy the file and replace the function
+
+```C++
+Bmi* create_model_instance()
+{
+    /* Return your new BMI instance pointer here... */
+}
+```
+
+with the instantiation of your model BMI. The model needs to implement the csdms BMI for C, but you may also implement our more object-oriented C++ interface [BmiCppExtension](https://github.com/eWaterCycle/grpc4bmi/blob/master/cpp/bmi_cpp_extension.h).
+
+### Model written in R
+
+The grpc4bmi Python package can also run BMI models written in R if the model is a subclass of [AbstractBmi](https://github.com/eWaterCycle/bmi-r/blob/master/R/abstract-bmi.R#L9)
+See [https://github.com/eWaterCycle/bmi-r](https://github.com/eWaterCycle/bmi-r) for instruction on R and Docker.
+
+Run the R model a server with
+
+```bash
+run-bmi-server --lang R [--path <R file with BMI model>] --name [<PACKAGE>::]<CLASS> --port <PORT>
+```
+
+For example with [WALRUS](https://github.com/eWaterCycle/grpc4bmi-examples/tree/master/walrus) use
+
+```bash
+run-bmi-server --lang R --path ~/git/eWaterCycle/grpc4bmi-examples/walrus/walrus-bmi.r --name WalrusBmi --port 55555
+```
+
+### The client side
+
+The client side has only a Python implementation. The default BMI client assumes a running server process on a given port.
+
+```python
+from grpc4bmi.bmi_grpc_client import BmiClient
+import grpc
+mymodel = BmiClient(grpc.insecure_channel("localhost:<PORT>"))
+print mymodel.get_component_name()
+mymodel.initialize(<FILEPATH>)
+...further BMI calls...
+```
+
+The package contains also client implementation that own the server process, either as a Python subprocess or a Docker
+container or a Singularity container or a Apptainer container running the ```run-bmi-server``` script. For instance
+```python
+from grpc4bmi.bmi_client_subproc import BmiClientSubProcess
+mymodel = BmiClientSubProcess(<PACKAGE>.<MODULE>.<CLASS>)
+```
+
+will automatically launch the server in a sub-process and
+
+```python
+from grpc4bmi.bmi_client_docker import BmiClientDocker
+mymodel = BmiClientDocker(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
+```
+will launch a Docker container based on supplied Docker image
+and will mount supplied directories to share files between the container and host.
+
+```python
+from grpc4bmi.bmi_client_singularity import BmiClientSingularity
+mymodel = BmiClientSingularity(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
+```
+will launch a singularity container on based supplied Singularity image
+and will mount supplied directories to share files between the container and host.
+
+```python
+from grpc4bmi.bmi_client_apptainer import BmiClientApptainer
+mymodel = BmiClientApptainer(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
+```
+will launch a Apptainer container on based supplied Apptainer image
+and will mount supplied directories to share files between the container and host.
+
+For more documentation see [https://grpc4bmi.readthedocs.io/](https://grpc4bmi.readthedocs.io/).
+
+## Development: generating the gRPC code
+
+When developers change the proto-file, it is necessary to install gRPC tools Python packages in your Python environment:
+
+```bash
+# Create virtual env
+python3 -m venv .venv
+. venv/bin/activate
+# Make sure latest pip and wheel are install
+pip install -U pip wheel
+pip install -r dev-requirements.txt
+# For R integration also install the R extras with
+pip install -e .[R]
+# For building docs (cd docs && make html) also install the docs extras with
+pip install -e .[docs]
+```
+
+and install the C++ runtime and `protoc` command as described in <https://github.com/google/protobuf/blob/master/src/README.md>.
+After this, simply executing the `proto_gen.sh` script should do the job.
+
+## Future work
+
+More language bindings are underway.
```

### Comparing `grpc4bmi-0.3.2/test/test_subproc.py` & `grpc4bmi-0.4.0/test/test_subproc.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import numpy
 import numpy.random
 import pytest
 import os
 
 from grpc4bmi.reserve import reserve_values_at_indices, reserve_values, reserve_grid_shape, reserve_grid_padding
 from test.fake_models import HugeModel
-from test.flatbmiheat import FlatBmiHeat
+from test.legacybmiheat import BmiHeat
 
 from grpc4bmi.bmi_client_subproc import BmiClientSubProcess
 
 """
 Unit tests for the BMI client and a server running in a child process. Every test performs cross-checking with a local 
 instance of the BMI heat toy model.
 """
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def make_bmi_classes(init=False):
     numpy.random.seed(0)
     os.environ["PYTHONPATH"] = os.path.dirname(os.path.abspath(__file__))
-    client = BmiClientSubProcess("flatbmiheat.FlatBmiHeat")
-    local = FlatBmiHeat()
+    client = BmiClientSubProcess("heat.BmiHeat")
+    local = BmiHeat()
     if init:
         client.initialize(None)
         local.initialize(None)
     return client, local
 
 
 def test_server_start():
@@ -141,14 +141,26 @@
     result = client.get_value(varname, reserve_values(client, varname))
     expected = local.get_value(varname, reserve_values(local, varname))
     assert numpy.array_equal(result, expected)
     del client
 
 
 def test_get_value_huge():
+    os.environ["PYTHONPATH"] = os.path.dirname(os.path.abspath(__file__))
+    client = BmiClientSubProcess("fake_models.HugeModel")
+    local = HugeModel()
+    varname = local.get_output_var_names()[0]
+
+    result = client.get_value(varname, reserve_values(client, varname))
+    expected = local.get_value(varname, reserve_values(local, varname))
+    assert numpy.array_equal(result, expected)
+    del client
+
+
+def test_get_value_huge():
     os.environ["PYTHONPATH"] = os.path.dirname(os.path.abspath(__file__))
     client = BmiClientSubProcess("fake_models.HugeModel")
     local = HugeModel()
     varname = local.get_output_var_names()[0]
 
     result = client.get_value(varname, reserve_values(client, varname))
     expected = local.get_value(varname, reserve_values(local, varname))
```

### Comparing `grpc4bmi-0.3.2/test/test_legacy_server.py` & `grpc4bmi-0.4.0/test/test_legacy_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 
 import numpy
 import numpy.random
 import pytest
 
 from grpc4bmi.bmi_grpc_legacy_server import BmiLegacyServer02
-from test.flatbmiheat import FlatLegacyBmiHeat
+from test.fake_models import Rect3DGridModel
+from test.legacybmiheat import LegacyBmiHeat
 
 """
 Unit tests for the BMI server class. Every test performs cross-checking with a local instance of the BMI heat toy model.
 """
 
 logging.basicConfig(level=logging.DEBUG)
 
@@ -35,16 +36,16 @@
     if obj is list:
         return obj
     if obj is None:
         return []
     return [obj]
 
 
-def make_bmi_classes(init=False):
-    server, local = BmiLegacyServer02(FlatLegacyBmiHeat()), FlatLegacyBmiHeat()
+def make_bmi_classes(init=False, bmi_class=LegacyBmiHeat):
+    server, local = BmiLegacyServer02(bmi_class()), bmi_class()
     if init:
         req = RequestStub()
         numpy.random.seed(0)
         server.initialize(req, None)
         numpy.random.seed(0)
         local.initialize(None)
     return server, local
@@ -154,14 +155,21 @@
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     setattr(request, "name", varname)
     assert server.getVarNBytes(request, None).nbytes == local.get_var_nbytes(varname)
     del server
 
+def test_get_var_itemsize():
+    server, local = make_bmi_classes(True)
+    request = RequestStub()
+    varname = local.get_output_var_names()[0]
+    setattr(request, "name", varname)
+    assert server.getVarItemSize(request, None).size == local.get_var_itemsize(varname)
+    del server
 
 def test_get_var_values():
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     setattr(request, "name", varname)
     values = local.get_value(varname)
@@ -185,26 +193,14 @@
     setattr(request, "name", varname)
     setattr(request, "indices", indices.flatten())
     setattr(request, "index_size", 1)
     values = local.get_value_at_indices(varname, indices)
     numpy.testing.assert_allclose(server.getValueAtIndices(request, None).values_double.values, values.flatten())
 
 
-def test_get_vals_indices_2d():
-    server, local = make_bmi_classes(True)
-    request = RequestStub()
-    varname = local.get_output_var_names()[0]
-    indices = numpy.array([[0, 1], [1, 0], [2, 2]])
-    setattr(request, "name", varname)
-    setattr(request, "indices", indices.flatten())
-    setattr(request, "index_size", 2)
-    values = local.get_value_at_indices(varname, indices)
-    numpy.testing.assert_allclose(server.getValueAtIndices(request, None).values_double.values, values.flatten())
-
-
 def test_set_var_values():
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     values = 0.123 * local.get_value(varname)
     setattr(request, "name", varname)
     setattr(request, "values_double", value_wrapper(values))
@@ -262,26 +258,73 @@
 
 def test_get_grid_shape():
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     grid_id = local.get_var_grid(varname)
     setattr(request, "grid_id", grid_id)
-    assert tuple(server.getGridShape(request, None).shape) == local.get_grid_shape(grid_id)
+    actual = tuple(server.getGridShape(request, None).shape)
+    expected = local.get_grid_shape(grid_id)
+    numpy.testing.assert_allclose(actual, expected)
 
 
 def test_get_grid_spacing():
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     grid_id = local.get_var_grid(varname)
     setattr(request, "grid_id", grid_id)
-    assert tuple(server.getGridSpacing(request, None).spacing) == local.get_grid_spacing(grid_id)
+    actual = tuple(server.getGridSpacing(request, None).spacing) 
+    expected = local.get_grid_spacing(grid_id)
+    numpy.testing.assert_allclose(actual, expected)
 
 
 def test_get_grid_origin():
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     grid_id = local.get_var_grid(varname)
     setattr(request, "grid_id", grid_id)
-    assert tuple(server.getGridOrigin(request, None).origin) == local.get_grid_origin(grid_id)
+    actual = tuple(server.getGridOrigin(request, None).origin) 
+    expected = local.get_grid_origin(grid_id)
+    numpy.testing.assert_allclose(actual, expected)
+
+class LegacyRect3DGridModel(Rect3DGridModel):
+    def get_grid_x(self, grid: int):
+        return numpy.array([0.1, 0.2, 0.3, 0.4])
+
+    def get_grid_y(self, grid: int):
+        return numpy.array([1.1, 1.2, 1.3])
+
+    def get_grid_z(self, grid: int):
+        return numpy.array([2.1, 2.2])
+
+class TestLegacyRect3DGrid:
+    def test_get_grid_x(self):
+        server, local = make_bmi_classes(True, LegacyRect3DGridModel)
+        request = RequestStub()
+        varname = local.get_output_var_names()[0]
+        grid_id = local.get_var_grid(varname)
+        setattr(request, "grid_id", grid_id)
+        actual = tuple(server.getGridX(request, None).coordinates) 
+        expected = local.get_grid_x(grid_id)
+        numpy.testing.assert_allclose(actual, expected)
+
+    def test_get_grid_y(self):
+        server, local = make_bmi_classes(True, LegacyRect3DGridModel)
+        request = RequestStub()
+        varname = local.get_output_var_names()[0]
+        grid_id = local.get_var_grid(varname)
+        setattr(request, "grid_id", grid_id)
+        actual = tuple(server.getGridY(request, None).coordinates) 
+        expected = local.get_grid_y(grid_id)
+        numpy.testing.assert_allclose(actual, expected)
+
+    def test_get_grid_z(self):
+        server, local = make_bmi_classes(True, LegacyRect3DGridModel)
+        request = RequestStub()
+        varname = local.get_output_var_names()[0]
+        grid_id = local.get_var_grid(varname)
+        setattr(request, "grid_id", grid_id)
+        actual = tuple(server.getGridZ(request, None).coordinates) 
+        expected = local.get_grid_z(grid_id)
+        numpy.testing.assert_allclose(actual, expected)
```

### Comparing `grpc4bmi-0.3.2/test/test_server.py` & `grpc4bmi-0.4.0/test/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from unittest.mock import Mock
 
 import numpy
 import numpy.random
 import pytest
 import grpc
 from google.rpc import error_details_pb2, status_pb2
+from heat import BmiHeat
 
 from grpc4bmi import bmi_pb2
 from grpc4bmi.bmi_grpc_server import BmiServer
 from grpc4bmi.reserve import reserve_values, reserve_grid_shape, reserve_grid_padding
 from test.fake_models import SomeException, FailingModel, Rect3DGridModel, UnstructuredGridBmiModel
-from test.flatbmiheat import FlatBmiHeat
 
 """
 Unit tests for the BMI server class. Every test performs cross-checking with a local instance of the BMI heat toy model.
 """
 
 logging.basicConfig(level=logging.DEBUG)
 
@@ -42,15 +42,15 @@
         return obj
     if obj is None:
         return []
     return [obj]
 
 
 def make_bmi_classes(init=False):
-    server, local = BmiServer(FlatBmiHeat()), FlatBmiHeat()
+    server, local = BmiServer(BmiHeat()), BmiHeat()
     if init:
         req = RequestStub()
         numpy.random.seed(0)
         server.initialize(req, None)
         numpy.random.seed(0)
         local.initialize(None)
     return server, local
@@ -215,32 +215,19 @@
 
 def test_get_value_at_indices():
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     indices = numpy.array([29, 8, 19, 81])
     setattr(request, "name", varname)
-    setattr(request, "indices", indices.flatten())
+    setattr(request, "indices", indices)
     setattr(request, "index_size", 1)
     dest = numpy.empty(4)
     values = local.get_value_at_indices(varname, dest, indices)
-    numpy.testing.assert_allclose(server.getValueAtIndices(request, None).values_double.values, values.flatten())
-
-
-def test_get_vals_indices_2d():
-    server, local = make_bmi_classes(True)
-    request = RequestStub()
-    varname = local.get_output_var_names()[0]
-    indices = numpy.array([[0, 1], [1, 0], [2, 2]])
-    setattr(request, "name", varname)
-    setattr(request, "indices", indices.flatten())
-    setattr(request, "index_size", 2)
-    dest = numpy.empty(6)
-    values = local.get_value_at_indices(varname, dest, indices)
-    numpy.testing.assert_allclose(server.getValueAtIndices(request, None).values_double.values, values.flatten())
+    numpy.testing.assert_allclose(server.getValueAtIndices(request, None).values_double.values, values)
 
 
 def test_set_var_values():
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     dest = reserve_values(local, varname)
@@ -259,15 +246,15 @@
     server, local = make_bmi_classes(True)
     request = RequestStub()
     varname = local.get_output_var_names()[0]
     indices = numpy.array([1, 11, 21])
     values = numpy.array([0.123, 4.567, 8.901])
     setattr(request, "name", varname)
     setattr(request, "values_double", value_wrapper(values))
-    setattr(request, "indices", indices.flatten())
+    setattr(request, "indices", indices)
     setattr(request, "index_size", 1)
     server.setValueAtIndices(request, None)
     delattr(request, "values_double")
     response = server.getValueAtIndices(request, None)
     values_copy = numpy.array(response.values_double.values)
     numpy.testing.assert_allclose(values, values_copy)
 
@@ -368,15 +355,15 @@
     context.abort_with_status.assert_called_once()
     status = context.abort_with_status.call_args[0][0]
     assert status.code == grpc.StatusCode.INTERNAL
     assert status.details == 'Bmi method always fails'
     metadata = status_pb2.Status.FromString(status.trailing_metadata[0][1])
     debuginfo = error_details_pb2.DebugInfo()
     metadata.details[0].Unpack(debuginfo)
-    assert debuginfo.detail == "SomeException('Bmi method always fails',)"
+    assert debuginfo.detail == "SomeException('Bmi method always fails')"
     assert len(debuginfo.stack_entries) > 0
 
 
 def test_get_grid_x():
     model = Rect3DGridModel()
     server = BmiServer(model, True)
     grid_id, request = make_grid_request(model)
```

### Comparing `grpc4bmi-0.3.2/test/fake_models.py` & `grpc4bmi-0.4.0/test/fake_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple
 
 import numpy
 import numpy as np
 from bmipy import Bmi
 
-from grpc4bmi.utils import GRPC_MAX_MESSAGE_LENGTH
+from grpc4bmi.constants import GRPC_MAX_MESSAGE_LENGTH
 
 
 class SomeException(Exception):
     pass
 
 
 class FailingModel(Bmi):
@@ -139,14 +139,17 @@
         raise self.exc
 
 
 class GridModel(FailingModel):
     def __init__(self):
         super(GridModel, self).__init__(SomeException('not used'))
 
+    def initialize(self, filename):
+        pass
+
     def get_output_var_names(self) -> Tuple[str]:
         return 'plate_surface__temperature',
 
     def get_var_grid(self, name):
         return 0
 
 
@@ -391,21 +394,29 @@
     def __init__(self):
         super().__init__()
         self.dtype = numpy.dtype('bool')
         self.value = numpy.array((True, False, True), dtype=self.dtype)
 
 
 class HugeModel(DTypeModel):
-    """Model which has value which does not fit in message body
+    """Model which has value which does not fit in single message body
 
     Can be run from command line with
 
     ..code-block:: bash
 
         run-bmi-server --path $PWD/test --name fake_models.HugeModel --port 55555 --debug
     """
     def __init__(self):
         super().__init__()
         self.dtype = numpy.dtype('float64')
         # Create value which is bigger than 4Mb
         dimension = (3 * GRPC_MAX_MESSAGE_LENGTH) // self.dtype.itemsize + 1000
         self.value = numpy.ones((dimension,), dtype=self.dtype)
+
+class WithItemSizeZeroAndVarTypeFloat32Model(Float32Model):
+    def get_var_itemsize(self, name):
+        return 0
+
+class WithItemSizeZeroAndUnknownVarType(WithItemSizeZeroAndVarTypeFloat32Model):
+    def get_var_type(self, name):
+        return 'real'
```

### Comparing `grpc4bmi-0.3.2/test/test_client.py` & `grpc4bmi-0.4.0/test/test_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import grpc
 import numpy
 import numpy.random
 import pytest
 from google.protobuf import any_pb2
 from google.rpc import error_details_pb2, status_pb2, code_pb2
 from grpc_status import rpc_status
+from heat import BmiHeat
+from typeguard import TypeCheckError
 
 from grpc4bmi.bmi_grpc_server import BmiServer
 from grpc4bmi.bmi_grpc_client import BmiClient, RemoteException, handle_error
 from grpc4bmi.reserve import reserve_values, reserve_grid_shape, reserve_grid_padding
 from test.fake_models import SomeException, FailingModel, Rect3DGridModel, UnstructuredGridBmiModel, UniRectGridModel, \
     Rect2DGridModel, Structured3DQuadrilateralsGridModel, Structured2DQuadrilateralsGridModel, Float32Model, Int32Model, \
-    BooleanModel
-from test.flatbmiheat import FlatBmiHeat
+    BooleanModel, WithItemSizeZeroAndUnknownVarType, WithItemSizeZeroAndVarTypeFloat32Model
 
 logging.basicConfig(level=logging.DEBUG)
 
 """
 Unit tests for the BMI client class. Every test performs cross-checking with a local instance of the BMI heat toy model.
 """
 
@@ -48,16 +49,16 @@
                 return orig_attr(*args, **kwargs)
 
             return add_context
         return orig_attr
 
 
 def make_bmi_classes(init=False):
-    client = BmiClient(stub=ServerWrapper(BmiServer(FlatBmiHeat())))
-    local = FlatBmiHeat()
+    client = BmiClient(stub=ServerWrapper(BmiServer(BmiHeat())))
+    local = BmiHeat()
     if init:
         numpy.random.seed(0)
         client.initialize(None)
         numpy.random.seed(0)
         local.initialize(None)
     return client, local
 
@@ -101,14 +102,23 @@
 def test_initialize():
     client, local = make_bmi_classes(True)
     assert client is not None
     client.finalize()
     del client
 
 
+def test_initialize_with_nonstring():
+    client, local = make_bmi_classes(False)
+    assert client is not None
+    with pytest.raises(TypeCheckError, match='did not match any element in the union'):
+        client.initialize(42)
+    client.finalize()
+    del client
+
+
 def test_update():
     client, local = make_bmi_classes(True)
     client.update()
     assert client is not None
     client.finalize()
     del client
 
@@ -550,39 +560,39 @@
 
     def test_get_grid_face_count(self, bmiclient):
         result = bmiclient.get_grid_face_count(0)
 
         assert result == 3
 
     def test_get_grid_edge_nodes(self, bmiclient):
-        placeholder = numpy.empty(16, dtype=numpy.int)
+        placeholder = numpy.empty(16, dtype=int)
 
         result = bmiclient.get_grid_edge_nodes(0, placeholder)
 
         expected = (0, 1, 1, 2, 2, 3, 3, 0, 1, 4, 4, 5, 5, 2, 5, 3)
         numpy.testing.assert_allclose(result, expected)
 
     def test_grid_face_nodes(self, bmiclient):
-        placeholder = numpy.empty(11, dtype=numpy.int)
+        placeholder = numpy.empty(11, dtype=int)
 
         result = bmiclient.get_grid_face_nodes(0, placeholder)
 
         expected = (0, 1, 2, 3, 1, 4, 5, 2, 2, 5, 3)
         numpy.testing.assert_allclose(result, expected)
 
     def test_grid_face_edges(self, bmiclient):
-        placeholder = numpy.empty(11, dtype=numpy.int)
+        placeholder = numpy.empty(11, dtype=int)
 
         result = bmiclient.get_grid_face_edges(0, placeholder)
 
         expected = (0, 1, 2, 3, 4, 5, 6, 1, 6, 7, 2)
         numpy.testing.assert_allclose(result, expected)
 
     def test_grid_nodes_per_face(self, bmiclient):
-        placeholder = numpy.empty(3, dtype=numpy.int)
+        placeholder = numpy.empty(3, dtype=int)
 
         result = bmiclient.get_grid_nodes_per_face(0, placeholder)
 
         expected = (4, 4, 3)
         numpy.testing.assert_allclose(result, expected)
 
     def test_grid_x(self, bmiclient):
@@ -697,24 +707,24 @@
 
     def test_get_value(self, bmiclient):
         with pytest.raises(MyRpcError):
             bmiclient.get_value(self.name, numpy.empty(3))
 
     def test_get_value_at_indices(self, bmiclient):
         with pytest.raises(MyRpcError):
-            bmiclient.get_value_at_indices(self.name, numpy.empty(1, dtype=numpy.bool), numpy.array([1]))
+            bmiclient.get_value_at_indices(self.name, numpy.empty(1, dtype=numpy.bool_), numpy.array([1]))
 
     def test_set_value(self, bmiclient):
-        value = numpy.array((False, False, False), dtype=numpy.bool)
+        value = numpy.array((False, False, False), dtype=numpy.bool_)
 
         with pytest.raises(NotImplementedError):
             bmiclient.set_value(self.name, value)
 
     def test_set_value_at_indices(self, bmiclient):
-        value = numpy.array([False], dtype=numpy.bool)
+        value = numpy.array([False], dtype=numpy.bool_)
 
         with pytest.raises(NotImplementedError):
             bmiclient.set_value_at_indices(self.name, numpy.array([1]), value)
 
 
 class MyCall(grpc.RpcError):
     def __init__(self, message, exc, stack_entries):
@@ -818,7 +828,47 @@
             assert target == b'somehost:51234'
 
     def test_same_port_twice(self):
         port = 51235
         with BmiClient.create_grpc_channel(port) as channel1, BmiClient.create_grpc_channel(port) as channel2:
             assert channel1._channel.target() == b'localhost:51235'
             assert channel2._channel.target() == b'localhost:51235'
+
+class TestModelWithItemSizeZeroAndVarTypeFloat32:
+    name = 'plate_surface__temperature'
+
+    @pytest.fixture
+    def bmimodel(self):
+        model = WithItemSizeZeroAndVarTypeFloat32Model()
+        yield model
+        del model
+
+    @pytest.fixture
+    def bmiclient(self, bmimodel):
+        client = BmiClient(stub=ServerWrapper(BmiServer(bmimodel)))
+        yield client
+        del client
+
+    def test_get_var_itemsize(self, bmiclient):
+        result = bmiclient.get_var_itemsize(self.name)
+
+        expected = 4
+        assert result == expected
+
+class TestModelWithItemSizeZeroAndUnknownVarType:
+    name = 'plate_surface__temperature'
+
+    @pytest.fixture
+    def bmimodel(self):
+        model = WithItemSizeZeroAndUnknownVarType()
+        yield model
+        del model
+
+    @pytest.fixture
+    def bmiclient(self, bmimodel):
+        client = BmiClient(stub=ServerWrapper(BmiServer(bmimodel)))
+        yield client
+        del client
+
+    def test_get_var_itemsize(self, bmiclient):
+        with pytest.raises(ValueError, match='get_var_itemsize returned 0, which is impossible'):
+            bmiclient.get_var_itemsize(self.name)
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi/bmi_grpc_server.py` & `grpc4bmi-0.4.0/grpc4bmi/bmi_grpc_server.py`

 * *Files identical despite different names*

### Comparing `grpc4bmi-0.3.2/grpc4bmi/bmi_r_model.py` & `grpc4bmi-0.4.0/grpc4bmi/bmi_r_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,21 +30,30 @@
     # base
     def initialize(self, filename):
         self.model['bmi_initialize'](filename)
 
     def update(self):
         self.model['update']()
 
+    def update_until(self, time):
+        self.model['updateUntil'](time)
+
     def finalize(self):
         self.model['bmi_finalize']()
 
     # info
     def get_component_name(self):
         return self.model['getComponentName']()[0]
 
+    def get_input_item_count(self):
+        return self.model['getInputItemCount']()
+
+    def get_output_item_count(self):
+        return self.model['getOutputItemCount']()
+
     def get_input_var_names(self):
         return self.model['getInputVarNames']()
 
     def get_output_var_names(self):
         return self.model['getOutputVarNames']()
 
     # time
@@ -171,11 +180,16 @@
         return edge_nodes
 
     def get_grid_face_nodes(self, grid, face_nodes):
         result = self.model['getGridFaceNodes'](grid)
         np.copyto(src=result, dst=face_nodes)
         return face_nodes
 
+    def get_grid_face_edges(self, grid, face_edges):
+        result = self.model['getGridFaceEdges'](grid)
+        np.copyto(src=result, dst=face_edges)
+        return face_edges
+
     def get_grid_nodes_per_face(self, grid, edge_nodes):
         result = self.model['getGridNodesPerFace'](grid)
         np.copyto(src=result, dst=edge_nodes)
         return edge_nodes
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi/reserve.py` & `grpc4bmi-0.4.0/grpc4bmi/reserve.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Helpers to reserve numpy arrays for use in some of the Bmi methods as output argument
 """
 import numpy
-
 from bmipy import Bmi
 
 
 def reserve_values(model: Bmi, name: str) -> numpy.ndarray:
     """Reserve dest for :func:`bmipy.Bmi.get_value`"""
     dtype = model.get_var_type(name)
     item_size = model.get_var_itemsize(name)
@@ -39,7 +38,23 @@
     return numpy.empty(shape, dtype=numpy.float64)
 
 
 def reserve_values_at_indices(model: Bmi, name: str, indices) -> numpy.ndarray:
     """Reserve dest for :func:`bmipy.Bmi.get_value_at_indices` """
     dtype = model.get_var_type(name)
     return numpy.empty(len(indices), dtype=dtype)
+
+def reserve_grid_edge_nodes(model: Bmi, grid_id: int) -> numpy.ndarray:
+    """Reserve edge_nodes for :func:`bmipy.Bmi.get_grid_edge_nodes`"""
+    edge_count = model.get_grid_edge_count(grid_id)
+    return numpy.empty(2 * edge_count, dtype=numpy.int64)
+
+def reserve_grid_nodes_per_face(model: Bmi, grid_id: int) -> numpy.ndarray:
+    """Reserve nodes_per_face for :func:`bmipy.Bmi.get_grid_nodes_per_face`"""
+    face_count = model.get_grid_face_count(grid_id)
+    return numpy.empty(face_count, dtype=numpy.int64)
+
+def reserve_grid_face_(model: Bmi, grid_id: int) -> numpy.ndarray:
+    """Reserve face_edges or face_node in respectivly :func:`bmipy.Bmi.get_grid_face_edges` or :func:`bmipy.Bmi.get_grid_face_nodes`"""
+    nodes_per_face = reserve_grid_nodes_per_face(model, grid_id)
+    model.get_grid_nodes_per_face(grid_id, nodes_per_face)
+    return numpy.empty(nodes_per_face.sum(), dtype=numpy.int64)
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi/bmi_client_subproc.py` & `grpc4bmi-0.4.0/grpc4bmi/bmi_client_subproc.py`

 * *Files identical despite different names*

### Comparing `grpc4bmi-0.3.2/grpc4bmi/run_server.py` & `grpc4bmi-0.4.0/grpc4bmi/run_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     parser.add_argument("--path", "-d", metavar="DIR", default=None, type=str,
                         help="Extra path name to append to the server instance process")
     lang_choices = ['python']
     if BmiR:
         lang_choices.append('R')
     parser.add_argument("--language", default="python", choices=lang_choices,
                         help="Language in which BMI implementation class is written")
-    parser.add_argument("--bmi-version", default="1.0.0", choices=["1.0.0", "0.2"],
+    parser.add_argument("--bmi-version", default="2.0.0", choices=["2.0.0", "0.2"],
                         help="Version of BMI interface implemented by model")
     parser.add_argument("--debug", action="store_true",
                         help="Run server in debug mode. "
                              "Logs errors with stacktraces and returns stacktrace in error response")
     return parser
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi/bmi_grpc_client.py` & `grpc4bmi-0.4.0/grpc4bmi/bmi_grpc_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 import math
 import os
 import socket
 from contextlib import closing
+from typing import Optional
 
 import numpy as np
 from bmipy import Bmi
 import grpc
 import numpy
+from typeguard import typechecked
 
 from grpc_status import rpc_status
 from google.rpc import error_details_pb2
 
 from . import bmi_pb2, bmi_pb2_grpc
-from .utils import GRPC_MAX_MESSAGE_LENGTH
+from .constants import GRPC_MAX_MESSAGE_LENGTH
 
 log = logging.getLogger(__name__)
 
 
 class RemoteException(grpc.RpcError):
     def __init__(self, message, tb):
         super().__init__(message)
@@ -88,15 +90,16 @@
 
     @staticmethod
     def get_unique_port(host=None):
         with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as s:
             s.bind(("" if host is None else host, 0))
             return int(s.getsockname()[1])
 
-    def initialize(self, filename):
+    @typechecked
+    def initialize(self, filename: Optional[str]):
         fname = "" if filename is None else filename
         try:
             return self.stub.initialize(bmi_pb2.InitializeRequest(config_file=fname))
         except grpc.RpcError as e:
             handle_error(e)
 
     def update(self):
@@ -188,15 +191,25 @@
         try:
             return str(self.stub.getVarType(bmi_pb2.GetVarRequest(name=name)).type)
         except grpc.RpcError as e:
             handle_error(e)
 
     def get_var_itemsize(self, name):
         try:
-            return self.stub.getVarItemSize(bmi_pb2.GetVarRequest(name=name)).size
+            item_size = self.stub.getVarItemSize(bmi_pb2.GetVarRequest(name=name)).size
+            if item_size == 0:
+                # BMI < v2.0 did not have get_var_itemsize, so old server will return 0
+                # fallback to getting item size from var type
+                var_type = self.get_var_type(name)
+                try:
+                    item_size = numpy.dtype(var_type).itemsize
+                    log.info(f'get_var_itemsize returned 0, corrected to {item_size} using get_var_type.')
+                except TypeError:
+                    raise ValueError('get_var_itemsize returned 0, which is impossible')
+            return item_size
         except grpc.RpcError as e:
             handle_error(e)
 
     def get_var_units(self, name):
         try:
             response = str(self.stub.getVarUnits(bmi_pb2.GetVarRequest(name=name)).units)
             return None if not response else response
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi/bmi_client_docker.py` & `grpc4bmi-0.4.0/grpc4bmi/bmi_client_docker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,110 @@
 import os
-import errno
 import time
+from os.path import abspath
+from typing import Iterable
 
 import docker
+from docker.models.containers import Container
+from typeguard import typechecked
 
 from grpc4bmi.bmi_grpc_client import BmiClient
-from grpc4bmi.utils import stage_config_file
-
-
-class LogsException(Exception):
-    pass
-
-
-class DeadDockerContainerException(ChildProcessError):
-    """
-    Exception for when a Docker container has died.
-
-    Args:
-        message (str): Human readable error message
-        exitcode (int): The non-zero exit code of the container
-        logs (str): Logs the container produced
-
-    """
-    def __init__(self, message, exitcode, logs, *args):
-        super().__init__(message, *args)
-        #: Exit code of container
-        self.exitcode = exitcode
-        #: Stdout and stderr of container
-        self.logs = logs
+from grpc4bmi.exceptions import DeadContainerException
 
 
 class BmiClientDocker(BmiClient):
     """
     BMI gRPC client for dockerized server processes: the initialization launches the docker container which should have the
-    run-bmi-server as its command. Also, it should expose the tcp port 55555 for communication with this client. Upon
+    run-bmi-server as its command. Also, it should expose the tcp port 50001 for communication with this client. Upon
     destruction, this class terminates the corresponding docker server.
 
     Args:
         image (str): Docker image name of grpc4bmi wrapped model
         image_port (int): Port of server inside the image
         host (str): Host on which the image port is published on a random port
-        input_dir (str): Directory for input files of model
-        output_dir (str): Directory for input files of model
-        user (str): Username or UID of Docker container
+        input_dirs (Iterable[str]): Directories for input files of model.
+
+            All of directories will be mounted read-only inside Docker container on same path as outside container.
+
+        work_dir (str): Working directory for model.
+
+            Directory is mounted inside container and changed into.
+
+        user (str): Username or UID of Docker container. Defaults to own UID.
         remove (bool): Automatically remove the container and logs when it exits.
+
+            Enable to get logs when container dies prematurely.
+
         delay (int): Seconds to wait for Docker container to startup, before connecting to it
         timeout (int): Seconds to wait for gRPC client to connect to server
         extra_volumes (Dict[str,Dict]): Extra volumes to attach to Docker container.
             The key is either the hosts path or a volume name and the value is a dictionary with the keys:
 
             - ``bind`` The path to mount the volume inside the container
             - ``mode`` Either ``rw`` to mount the volume read/write, or ``ro`` to mount it read-only.
 
             For example:
 
             .. code-block:: python
 
                 {'/data/shared/forcings/': {'bind': '/forcings', 'mode': 'ro'}}
 
-    """
+            Increase when container takes a long time to startup.
+
+        timeout (int): Seconds to wait for gRPC client to connect to server.
 
-    input_mount_point = "/data/input"
-    output_mount_point = "/data/output"
+            By default will try forever to connect to gRPC server inside container.
+            Set to low number to escape endless wait.
 
-    def __init__(self, image, image_port=55555, host=None,
-                 input_dir=None, output_dir=None,
-                 user=os.getuid(), remove=False,
-                 delay=5, timeout=None, extra_volumes=None):
+    See :py:class:`grpc4bmi.bmi_client_apptainer.BmiClientApptainer` for examples using `input_dirs` and `work_dir`.
+    """
+
+    @typechecked
+    def __init__(self, image: str, work_dir: str, image_port=50051, host=None,
+                 input_dirs: Iterable[str] = tuple(),
+                 user=os.getuid(), remove=False, delay=5,
+                 timeout=None):
+        if type(input_dirs) == str:
+            msg = f'type of argument "input_dirs" must be collections.abc.Iterable; ' \
+                  f'got {type(input_dirs)} instead'
+            raise TypeError(msg)
         port = BmiClient.get_unique_port()
         client = docker.from_env()
         volumes = {}
-        if extra_volumes is not None:
-            volumes.update(extra_volumes)
-        self.input_dir = None
-        if input_dir is not None:
-            self.input_dir = os.path.abspath(input_dir)
-            if not os.path.isdir(self.input_dir):
+        for raw_input_dir in input_dirs:
+            input_dir = abspath(raw_input_dir)
+            if not os.path.isdir(input_dir):
                 raise NotADirectoryError(input_dir)
-            volumes[self.input_dir] = {"bind": BmiClientDocker.input_mount_point, "mode": "rw"}
-        self.output_dir = None
-        if output_dir is not None:
-            self.output_dir = os.path.abspath(output_dir)
-            try:
-                # Create output dir ourselves, otherwise Docker will create it as root user, resulting in permission
-                # errors
-                os.mkdir(self.output_dir)
-            except OSError as e:
-                if e.errno != errno.EEXIST:
-                    raise
-            volumes[self.output_dir] = {"bind": BmiClientDocker.output_mount_point, "mode": "rw"}
-        self.container = client.containers.run(image,
+            volumes[input_dir] = {"bind": input_dir, "mode": "ro"}
+
+        self.work_dir = abspath(work_dir)
+        if self.work_dir in volumes:
+            raise ValueError('Found work_dir equal to one of the input directories. Please drop that input dir.')
+        if not os.path.isdir(self.work_dir):
+            raise NotADirectoryError(self.work_dir)
+        volumes[self.work_dir] = {"bind": self.work_dir, "mode": "rw"}
+        self.container: Container = client.containers.run(image,
                                                ports={str(image_port) + "/tcp": port},
                                                volumes=volumes,
+                                               working_dir=self.work_dir,
                                                user=user,
                                                remove=remove,
                                                detach=True)
         time.sleep(delay)
         if not remove:
-            # Only able to reload, read logs when container is not in auto remove mode
+            # Only able to reload, read logs on exited container when remove=False
             self.container.reload()
             if self.container.status == 'exited':
                 exitcode = self.container.attrs["State"]["ExitCode"]
-                logs = self.container.logs()
+                logs = self.logs()
                 msg = f'Failed to start Docker container with image {image}, Container log: {logs}'
-                raise DeadDockerContainerException(msg, exitcode, logs)
+                raise DeadContainerException(msg, exitcode, logs)
 
         super(BmiClientDocker, self).__init__(BmiClient.create_grpc_channel(port=port, host=host), timeout=timeout)
 
     def __del__(self):
-        if hasattr(self, "container"):
-            self.container.stop()
+        self.container.stop()
 
-    def initialize(self, filename):
-        fn = stage_config_file(filename, self.input_dir, self.input_mount_point)
-        super(BmiClientDocker, self).initialize(fn)
-
-    def get_value_ptr(self, var_name):
-        raise NotImplementedError("Cannot exchange memory references across process boundary")
-
-    def logs(self):
-        """Logs of the Docker container"""
-        try:
-            return self.container.logs()
-        except docker.errors.APIError as e:
-            raise LogsException("Unable to fetch logs, try pass remove=False to BmiClientDocker constructor, so logs are retained after container dies") from e
+    def logs(self) -> str:
+        """Returns complete combined stdout and stderr written by the Docker container.
+        """
+        return self.container.logs().decode('utf8')
```

### Comparing `grpc4bmi-0.3.2/grpc4bmi/bmi_grpc_legacy_server.py` & `grpc4bmi-0.4.0/grpc4bmi/bmi_grpc_legacy_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,17 +187,14 @@
                 self.bmi_model_.set_value(request.name, request.values_float.values)
             if request.HasField("values_double"):
                 self.bmi_model_.set_value(request.name, request.values_double.values)
             return bmi_pb2.Empty()
         except Exception as e:
             self.exception_handler(e, context)
 
-    def setValuePtr(self, request, context):
-        raise NotImplementedError("Array references cannot be transmitted through this GRPC channel")
-
     def setValueAtIndices(self, request, context):
         try:
             index_array = numpy.array(request.indices)
             if request.HasField("values_int"):
                 array = numpy.array(request.values_int.values, dtype=numpy.int32)
                 self.bmi_model_.set_value_at_indices(request.name, index_array, array)
             if request.HasField("values_float"):
```

### Comparing `grpc4bmi-0.3.2/README.md` & `grpc4bmi-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [![CI](https://github.com/eWaterCycle/grpc4bmi/workflows/CI/badge.svg)](https://github.com/eWaterCycle/grpc4bmi/actions?query=workflow%3ACI)
 [![Documentation Status](https://readthedocs.org/projects/grpc4bmi/badge/?version=latest)](https://grpc4bmi.readthedocs.io/en/latest/?badge=latest)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=alert_status)](https://sonarcloud.io/dashboard?id=grpc4bmi)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=grpc4bmi&metric=coverage)](https://sonarcloud.io/dashboard?id=grpc4bmi)
 
 ## Purpose
 
-This software allows you to wrap your Basic Model Interface (BMI) implementation ([https://github.com/csdms/bmi](https://github.com/csdms/bmi)) in a server process and communicate with it via the included Python client. The communication is serialized to protocol buffers by gRPC ([https://grpc.io/](https://grpc.io/)) and occurs over network ports.
+This software allows you to wrap your [Basic Model Interface (BMI)](https://github.com/csdms/bmi) implementation in a server process and communicate with it via the included Python client. The communication is serialized to protocol buffers by [GRPC](https://grpc.io/) and occurs over network ports. Can run models in isolated containers using Docker or Apptainer.
 
 ## Installation
 
 Optionally, create your virtual environment and activate it, Then, run
 
 ```bash
 pip install grpc4bmi
@@ -39,21 +39,25 @@
 
 in the cpp folder.
 
 ## Usage
 
 ### Model written in Python
 
-For inspiration look at the example in the test directory. To start a server process that allows calls to your BMI implementation, type
+A model should be a subclass of the `Bmi` class from the [bmipy](https://pypi.org/project/bmipy/2.0/) package.
+
+For inspiration look at the [example](test/fake_models.py) in the test directory. 
+
+To start a server process that allows calls to your BMI implementation, type
 
 ```bash
 run-bmi-server --name <PACKAGE>.<MODULE>.<CLASS> --port <PORT> --path <PATH>
 ```
 
-where ```<PACKAGE>, <MODULE>``` are the Python package and module containing your implementation, ```<CLASS>``` is your
+where ```<PACKAGE>, <MODULE>``` are the python package and module containing your implementation, ```<CLASS>``` is your
 bmi model class name, ```<PORT>``` is any available port on the host system, and optionally ```<PATH>``` denotes an
 additional path that should be added to the system path to make your implementation work. The name option above is
 optional, and if not provided the script will look at the environment variables ```BMI_PACKAGE```, ```BMI_MODULE``` and
 ```BMI_CLASS```. Similarly, the port can be defined by the environment variable ```BMI_PORT```.
 This software assumes that your implementation constructor has no parameters.
 
 ### Model written in C/C++ (beta)
@@ -95,49 +99,61 @@
 import grpc
 mymodel = BmiClient(grpc.insecure_channel("localhost:<PORT>"))
 print mymodel.get_component_name()
 mymodel.initialize(<FILEPATH>)
 ...further BMI calls...
 ```
 
-The package contains also client implementation that own the server process, either as a Python subprocess or a docker
-image or a singularity image running the ```run-bmi-server``` script. For instance
-
+The package contains also client implementation that own the server process, either as a Python subprocess or a Docker
+container or a Singularity container or a Apptainer container running the ```run-bmi-server``` script. For instance
 ```python
 from grpc4bmi.bmi_client_subproc import BmiClientSubProcess
 mymodel = BmiClientSubProcess(<PACKAGE>.<MODULE>.<CLASS>)
 ```
 
 will automatically launch the server in a sub-process and
 
 ```python
-from grpc4bmi.bmi_client_subproc import BmiClientDocker
-mymodel = BmiClientDocker(<IMAGE>,<PORT>)
+from grpc4bmi.bmi_client_docker import BmiClientDocker
+mymodel = BmiClientDocker(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
 ```
-
-will launch a docker container, assuming that a gRPC BMI server will start and exposes the port ```<PORT>```.
+will launch a Docker container based on supplied Docker image
+and will mount supplied directories to share files between the container and host.
 
 ```python
 from grpc4bmi.bmi_client_singularity import BmiClientSingularity
-mymodel = BmiClientSingularity(<IMAGE>,<PORT>)
+mymodel = BmiClientSingularity(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
 ```
+will launch a singularity container on based supplied Singularity image
+and will mount supplied directories to share files between the container and host.
 
-will launch a singularity container, assuming that a gRPC BMI server will start and exposes the port ```<PORT>```.
+```python
+from grpc4bmi.bmi_client_apptainer import BmiClientApptainer
+mymodel = BmiClientApptainer(<IMAGE>, <WORK DIR TO MOUNT>, input_dirs=[<INPUT DIRECTORIES TO MOUNT>])
+```
+will launch a Apptainer container on based supplied Apptainer image
+and will mount supplied directories to share files between the container and host.
 
 For more documentation see [https://grpc4bmi.readthedocs.io/](https://grpc4bmi.readthedocs.io/).
 
 ## Development: generating the gRPC code
 
 When developers change the proto-file, it is necessary to install gRPC tools Python packages in your Python environment:
 
 ```bash
-pip install -r requirements.txt
-pip install -e .
+# Create virtual env
+python3 -m venv .venv
+. venv/bin/activate
+# Make sure latest pip and wheel are install
+pip install -U pip wheel
+pip install -r dev-requirements.txt
 # For R integration also install the R extras with
 pip install -e .[R]
+# For building docs (cd docs && make html) also install the docs extras with
+pip install -e .[docs]
 ```
 
 and install the C++ runtime and `protoc` command as described in <https://github.com/google/protobuf/blob/master/src/README.md>.
 After this, simply executing the `proto_gen.sh` script should do the job.
 
 ## Future work
```

