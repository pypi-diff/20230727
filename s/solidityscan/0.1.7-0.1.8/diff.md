# Comparing `tmp/solidityscan-0.1.7.tar.gz` & `tmp/solidityscan-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidityscan-0.1.7.tar", last modified: Tue Jun 13 10:03:33 2023, max compression
+gzip compressed data, was "solidityscan-0.1.8.tar", last modified: Thu Jul 27 05:51:36 2023, max compression
```

## Comparing `solidityscan-0.1.7.tar` & `solidityscan-0.1.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-13 10:03:33.851954 solidityscan-0.1.7/
--rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-13 10:03:33.851807 solidityscan-0.1.7/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)       55 2023-05-15 17:56:15.000000 solidityscan-0.1.7/README.md
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-06-13 10:03:33.851991 solidityscan-0.1.7/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)     1290 2023-06-13 10:03:29.000000 solidityscan-0.1.7/setup.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-13 10:03:33.850683 solidityscan-0.1.7/solidityscan.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-13 10:03:33.000000 solidityscan-0.1.7/solidityscan.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      444 2023-06-13 10:03:33.000000 solidityscan-0.1.7/solidityscan.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-06-13 10:03:33.000000 solidityscan-0.1.7/solidityscan.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       74 2023-06-13 10:03:33.000000 solidityscan-0.1.7/solidityscan.egg-info/entry_points.txt
--rw-r--r--   0 manosriram   (501) staff       (20)      387 2023-06-13 10:03:33.000000 solidityscan-0.1.7/solidityscan.egg-info/requires.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       19 2023-06-13 10:03:33.000000 solidityscan-0.1.7/solidityscan.egg-info/top_level.txt
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-13 10:03:33.851632 solidityscan-0.1.7/solidityscan_agent/
--rw-r--r--   0 manosriram   (501) staff       (20)     4376 2023-06-13 10:02:52.000000 solidityscan-0.1.7/solidityscan_agent/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1833 2023-06-12 12:35:16.000000 solidityscan-0.1.7/solidityscan_agent/config.py
--rw-r--r--   0 manosriram   (501) staff       (20)      304 2023-06-13 09:50:21.000000 solidityscan-0.1.7/solidityscan_agent/constants.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1606 2023-06-12 12:25:13.000000 solidityscan-0.1.7/solidityscan_agent/exceptions.py
--rw-r--r--   0 manosriram   (501) staff       (20)      916 2023-06-12 12:35:24.000000 solidityscan-0.1.7/solidityscan_agent/lang.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1464 2023-06-13 10:02:41.000000 solidityscan-0.1.7/solidityscan_agent/report.py
--rw-r--r--   0 manosriram   (501) staff       (20)     2884 2023-06-13 10:03:10.000000 solidityscan-0.1.7/solidityscan_agent/scan.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-07-27 05:51:36.066984 solidityscan-0.1.8/
+-rw-r--r--   0 manosriram   (501) staff       (20)      271 2023-07-27 05:51:36.066846 solidityscan-0.1.8/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)       55 2023-05-15 17:56:15.000000 solidityscan-0.1.8/README.md
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-07-27 05:51:36.067021 solidityscan-0.1.8/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)     1289 2023-07-27 05:51:29.000000 solidityscan-0.1.8/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-07-27 05:51:36.065920 solidityscan-0.1.8/solidityscan.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)      271 2023-07-27 05:51:36.000000 solidityscan-0.1.8/solidityscan.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      444 2023-07-27 05:51:36.000000 solidityscan-0.1.8/solidityscan.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-07-27 05:51:36.000000 solidityscan-0.1.8/solidityscan.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       74 2023-07-27 05:51:36.000000 solidityscan-0.1.8/solidityscan.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)      387 2023-07-27 05:51:36.000000 solidityscan-0.1.8/solidityscan.egg-info/requires.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       19 2023-07-27 05:51:36.000000 solidityscan-0.1.8/solidityscan.egg-info/top_level.txt
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-07-27 05:51:36.066695 solidityscan-0.1.8/solidityscan_agent/
+-rw-r--r--   0 manosriram   (501) staff       (20)     4084 2023-07-27 05:47:54.000000 solidityscan-0.1.8/solidityscan_agent/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1833 2023-07-27 05:47:54.000000 solidityscan-0.1.8/solidityscan_agent/config.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      211 2023-07-27 05:47:54.000000 solidityscan-0.1.8/solidityscan_agent/constants.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1606 2023-07-27 05:47:54.000000 solidityscan-0.1.8/solidityscan_agent/exceptions.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      916 2023-07-27 05:47:54.000000 solidityscan-0.1.8/solidityscan_agent/lang.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1217 2023-07-27 05:47:54.000000 solidityscan-0.1.8/solidityscan_agent/report.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     2872 2023-07-27 05:47:54.000000 solidityscan-0.1.8/solidityscan_agent/scan.py
```

### Comparing `solidityscan-0.1.7/setup.py` & `solidityscan-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import os
 
 def readme():
     with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
         return f.read()
 
 setup(name="solidityscan",
-      version="0.1.7",
+      version="0.1.8",
       description="Get your smart contracts audited by a smarter tool",
       long_description=readme(),
       long_description_content_type='text/markdown',
       url="https://solidityscan.com",
       entry_points={
         'console_scripts': [
             'solidityscan=solidityscan_agent.__init__:solidityscan',
         ],
       },
-      python_requires=">=3.10",
+      python_requires=">=3.6",
       packages=find_packages(),
       install_requires=[
         "anyio==3.6.2",
         "beautifulsoup4==4.12.2",
         "certifi==2023.5.7",
         "chardet==5.1.0",
         "charset-normalizer==2.1.1",
```

### Comparing `solidityscan-0.1.7/solidityscan_agent/__init__.py` & `solidityscan-0.1.8/solidityscan_agent/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,26 +77,24 @@
         if not contract_platform:
             raise click.UsageError("-contract-platform flag is required")
         
         s.block_scan(contract_address, contract_chain, contract_platform, rescan, token)
 
 @solidityscan.command()
 @click.option("--report-type", "-r", required=True, type=click.Choice(["generate"]), prompt=False, help="report command")
-@click.option("-scan-type", required=True, type=click.Choice(["project", "block"]), help="type of scan")
 @click.option("-project-id", required=False, help="project id to generate report for")
 @click.option("-scan-id", required=False, help="scan associated with the project")
-@click.option("--token", "-t", required=False, help="api token generated from solidityscan")
-def report(report_type, scan_type, project_id, scan_id, token=None):
-    """generates report for a project or block"""
+def report(report_type, project_id, scan_id):
+    """perform report related actions"""
 
+    r = Report()
 
     if report_type == "generate":
         if not project_id:
             raise click.UsageError("-project-id flag is required")
         if not scan_id:
             raise click.UsageError("-scan-id flag is required")
 
-        r = Report(project_id=project_id, scan_id=scan_id, scan_type=scan_type).generate_report(token=token)
-        return r
+        r.generate_report(project_id, scan_id)
 
 if __name__ == "__main__":
     solidityscan()
```

### Comparing `solidityscan-0.1.7/solidityscan_agent/config.py` & `solidityscan-0.1.8/solidityscan_agent/config.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.7/solidityscan_agent/exceptions.py` & `solidityscan-0.1.8/solidityscan_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.7/solidityscan_agent/lang.py` & `solidityscan-0.1.8/solidityscan_agent/lang.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.7/solidityscan_agent/scan.py` & `solidityscan-0.1.8/solidityscan_agent/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+from solidityscan_agent.config import Config
 
 import requests
 import click
 
 from solidityscan_agent.exceptions import ScanFailed, HostNotReachable
-from solidityscan_agent.constants import HOST_API
-from solidityscan_agent.config import Config
+from solidityscan_agent.constants import HOST
 
 class Scan:
 
     @property
     def project_scan_host_url(self):
-        return f"{HOST_API}/api-project-scan/"
+        return f"{HOST}/api-project-scan/"
 
     @property
     def block_scan_host_url(self):
-        return f"{HOST_API}/api-start-scan-block/"
+        return f"{HOST}/api-start-scan-block/"
 
     def make_headers(self, token):
         return {
             "Authorization": f"Bearer {token}"
         }
 
     """
```

