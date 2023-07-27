# Comparing `tmp/envisionriskraas-1.1.2.tar.gz` & `tmp/envisionriskraas-1.1.3.tar.gz`

## Comparing `envisionriskraas-1.1.2.tar` & `envisionriskraas-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    86243 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/src/EnvisionRiskRaaS/RAAS.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/src/EnvisionRiskRaaS/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/README.md
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 envisionriskraas-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    86253 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/src/EnvisionRiskRaaS/RAAS.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/src/EnvisionRiskRaaS/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/README.md
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9965 2020-02-02 00:00:00.000000 envisionriskraas-1.1.3/PKG-INFO
```

### Comparing `envisionriskraas-1.1.2/src/EnvisionRiskRaaS/RAAS.py` & `envisionriskraas-1.1.3/src/EnvisionRiskRaaS/RAAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,14 +262,15 @@
         base_cur = "USD",
         horizon = 1,
         signif_level = 0.975,
         volatility_id = "point_in_time",
         report_depth = 0,
         simplify = True)
     """
+    
     if os.getenv("LOGGED_IN") != 'Yes':
         return {"message": "Please login before using the functionality - use 'envrsk_auth_log_in()' or 'envrsk_auth_log_in_interactively()'"}
     else:
         end_point = "portfolio-risk-regular"
         api_url = get_api_url(end_point)
 
         # Query parameters
@@ -278,15 +279,15 @@
             "base_cur": base_cur,
             "horizon": horizon,
             "signif_level": signif_level,
             "volatility_id": volatility_id,
             "report_depth": report_depth
         }
         params = {k: v for k, v in params.items() if v is not None}
-        if positions == pd.DataFrame():
+        if type(positions) == pd.DataFrame:
             positions_dict = pd.DataFrame(positions).to_dict('list')
         else:
             positions_dict = positions
 
         res_out = envrsk_post(url=api_url, access_token=get_access_token(), params=params, body=positions_dict)
 
         out = process_portfolio_return_values(res_out, simplify)
```

### Comparing `envisionriskraas-1.1.2/LICENSE.txt` & `envisionriskraas-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.2/README.md` & `envisionriskraas-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `envisionriskraas-1.1.2/pyproject.toml` & `envisionriskraas-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EnvisionRiskRaaS"
-version = "1.1.2"
+version = "1.1.3"
 authors = [{name="EnvisionRisk", email="support@envisionrisk.com" },{name="Coptolon",email="mark@brezina.dk"},]
 keywords = ["Risk-as-a-service","Market risk","Quantitative finance"]
 description = "EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [ 
-"requests>= 2.31.0; python_version<'3.11'",  
-"pandas>= 2.0.3; python_version<'3.11'", 
-"typing >= 3.10.0.0; python_version<'3.11'", 
+"requests>= 2.31.0; python_version<'3.9'",  
+"pandas>= 2.0.2; python_version<'3.9'", 
+"typing >= 3.10.0.0; python_version<'3.9'", 
 "queuelib >= 1.5.0; python_version<'3.9'" ]
 
 [project.urls]
 "API webpage" = "https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management"
 "Homepage" = "https://www.envisionrisk.com/"
```

### Comparing `envisionriskraas-1.1.2/PKG-INFO` & `envisionriskraas-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: EnvisionRiskRaaS
-Version: 1.1.2
+Version: 1.1.3
 Summary: EnvisionRisk improves market risk management by providing predictive analytics for risk quantification, aiding strategic decisions and risk mitigation.
 Project-URL: API webpage, https://envisionrisk.stoplight.io/docs/api-aleadomus-documentation/cjr0z7gv4x6en-harnessing-advanced-tools-for-strategic-market-risk-management
 Project-URL: Homepage, https://www.envisionrisk.com/
 Author-email: EnvisionRisk <support@envisionrisk.com>, Coptolon <mark@brezina.dk>
 License-File: LICENSE.txt
 Keywords: Market risk,Quantitative finance,Risk-as-a-service
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
-Requires-Dist: pandas>=2.0.3; python_version < '3.11'
+Requires-Dist: pandas>=2.0.2; python_version < '3.9'
 Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
-Requires-Dist: requests>=2.31.0; python_version < '3.11'
-Requires-Dist: typing>=3.10.0.0; python_version < '3.11'
+Requires-Dist: requests>=2.31.0; python_version < '3.9'
+Requires-Dist: typing>=3.10.0.0; python_version < '3.9'
 Description-Content-Type: text/markdown
 
 <h1>EnvisionRiskRaaS</h1>
 <hr>
 Delve into the world of EnvisionRisk’s Python package, your portal to our sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows you to tap into our cutting-edge risk management services, retrieve relevant data, perform complex calculations, and generate actionable insights, all without leaving your Python programming environment. Embrace this smarter, efficient approach to handling market risk.
 
 Are you navigating the volatile waters of financial uncertainties, seeking to make strategic decisions? Allow EnvisionRisk’s Cloud Service to be your compass, providing a precise mechanism for quantifying market risks. Replace guesswork with certainty; our platform furnishes you with standardized metrics designed to enhance cost-efficiency and fortify your financial bulwark.
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.2 Summary:
+Metadata-Version: 2.1 Name: EnvisionRiskRaaS Version: 1.1.3 Summary:
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
-:: Python :: 3 Requires-Python: >=3.11 Requires-Dist: pandas>=2.0.3;
-python_version < '3.11' Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
-Requires-Dist: requests>=2.31.0; python_version < '3.11' Requires-Dist:
-typing>=3.10.0.0; python_version < '3.11' Description-Content-Type: text/
+:: Python :: 3 Requires-Python: >=3.11 Requires-Dist: pandas>=2.0.2;
+python_version < '3.9' Requires-Dist: queuelib>=1.5.0; python_version < '3.9'
+Requires-Dist: requests>=2.31.0; python_version < '3.9' Requires-Dist:
+typing>=3.10.0.0; python_version < '3.9' Description-Content-Type: text/
 markdown
 ****** EnvisionRiskRaaS ******
 ===============================================================================
 Delve into the world of EnvisionRiskâs Python package, your portal to our
 sophisticated Market Risk-as-a-Service (RaaS). This comprehensive tool allows
 you to tap into our cutting-edge risk management services, retrieve relevant
 data, perform complex calculations, and generate actionable insights, all
```

