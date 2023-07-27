# Comparing `tmp/envisionriskraas-1.1.3.tar.gz` & `tmp/envisionriskraas-1.1.4.tar.gz`

## Comparing `envisionriskraas-1.1.3.tar` & `envisionriskraas-1.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86253 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/README.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 envisionriskraas-1.1.4/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0    86306 2020-02-02 00:00:00.000000 envisionriskraas-1.1.4/src/EnvisionRiskRaaS/core.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.4/README.md
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 envisionriskraas-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 envisionriskraas-1.1.4/PKG-INFO
```

### Comparing `envisionriskraas-1.1.3/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.1.4/src/EnvisionRiskRaaS/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #* the communication with the cloud server, and transform the JSON output
 #* from the API into Python data structures.
 
 import requests
 import json
 import os
 import datetime
+import maskpass
 import pandas as pd
 from typing import Dict
 from queue import Empty
 
 #******************************************************************************
 #### General API Functions - GET/POST                                      ####
 #******************************************************************************
@@ -191,16 +192,16 @@
     Returns:
         dict: A dictionary with status code and a corresponding message.
     
     Provide credentials - email and password. In case you have not yet received
     your personal credentials, contact EnvisionRisk at support@envisionrisk.com 
     """
     
-    os.environ["USR_ID"] = input("Please provide email: ")       
-    os.environ["USR_PWD"] = input("Please provide password: ")
+    os.environ["USR_ID"] = maskpass.askpass(prompt="Please provide email: ")       
+    os.environ["USR_PWD"] = maskpass.askpass(prompt="Please provide password: ")
 
     return envrsk_auth_log_in(os.getenv("USR_ID"), os.getenv("USR_PWD"))
     
 def envrsk_auth_log_out():
     """ 
     Function to log out from the API.
```

### Comparing `envisionriskraas-1.1.3/LICENSE.txt` & `envisionriskraas-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.3/README.md` & `envisionriskraas-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.3/pyproject.toml` & `envisionriskraas-1.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.1.3"
+version = "1.1.4"
 authors = [{name="EnvisionRisk", email="support@envisionrisk.com" },{name="Coptolon",email="mark@brezina.dk"},]
 keywords = ["Risk-as-a-service","Market risk","Quantitative finance"]
 description = "EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation."
 readme = "README.md"
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [ 
 "requests>= 2.31.0; python_version<'3.9'",  
 "pandas>= 2.0.2; python_version<'3.9'", 
 "typing >= 3.10.0.0; python_version<'3.9'", 
-"queuelib >= 1.5.0; python_version<'3.9'" ]
+"queuelib >= 1.5.0; python_version<'3.9'", ]
 
 [project.urls]
 "API webpage" = "https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management"
 "Homepage" = "https://www.envisionrisk.com/"
```

### Comparing `envisionriskraas-1.1.3/PKG-INFO` & `envisionriskraas-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.1.3
+Version: 1.1.4
 Summary: EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management
 Project-URL: Homepage, https://www.envisionrisk.com/
 Author-email: EnvisionRisk <support@envisionrisk.com>, Coptolon <mark@brezina.dk>
 License-File: LICENSE.txt
 Keywords: Market risk,Quantitative finance,Risk-as-a-service
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Requires-Dist: pandas>=2.0.2; python_version < '3.9'
 Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
 Requires-Dist: requests>=2.31.0; python_version < '3.9'
 Requires-Dist: typing>=3.10.0.0; python_version < '3.9'
 Description-Content-Type: text/markdown
 
 <h1>EnvisionRiskRaaS</h1>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.3 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.4 Summary:
 EnvisionRisk improves market risk management by providing predictive analytics
 for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-
 documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-
 risk-management Project-URL: Homepage, https://www.envisionrisk.com/ Author-
 email: EnvisionRisk
 envisionrisk.com>, Coptolon
 brezina.dk> License-File: LICENSE.txt Keywords: Market risk,Quantitative
 finance,Risk-as-a-service Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Requires-Python: >=3.11 Requires-Dist: pandas>=2.0.2;
+:: Python :: 3 Requires-Python: >=3.9 Requires-Dist: pandas>=2.0.2;
 python_version < '3.9' Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
 Requires-Dist: requests>=2.31.0; python_version < '3.9' Requires-Dist:
 typing>=3.10.0.0; python_version < '3.9' Description-Content-Type: text/
 markdown
 ****** EnvisionRiskRaaS ******
 ===============================================================================
 Delve into the world of EnvisionRiskâs Python package, your portal to our
```

