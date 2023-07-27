# Comparing `tmp/salure_helpers_profit-2.1.0.tar.gz` & `tmp/salure_helpers_profit-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_profit-2.1.0.tar", last modified: Fri Jul 21 15:32:35 2023, max compression
+gzip compressed data, was "dist/salure_helpers_profit-2.1.1.tar", last modified: Thu Jul 27 13:32:33 2023, max compression
```

## Comparing `salure_helpers_profit-2.1.0.tar` & `salure_helpers_profit-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_data_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get.py
--rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get_async.py
--rw-rw-rw-   0 root         (0) root         (0)   142534 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/salure_helpers/profit/profit_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      262 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/salure_helpers_profit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:32:35.000000 salure_helpers_profit-2.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-21 15:32:22.000000 salure_helpers_profit-2.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_data_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)    14489 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get.py
+-rw-rw-rw-   0 root         (0) root         (0)    17456 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get_async.py
+-rw-rw-rw-   0 root         (0) root         (0)   142536 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/salure_helpers/profit/profit_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-27 13:32:32.000000 salure_helpers_profit-2.1.1/salure_helpers_profit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-27 13:32:33.000000 salure_helpers_profit-2.1.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-27 13:32:18.000000 salure_helpers_profit-2.1.1/setup.py
```

### Comparing `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_data_cleaner.py` & `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_data_cleaner.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get.py` & `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_get_async.py` & `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_get_async.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_profit-2.1.0/salure_helpers/profit/profit_update.py` & `salure_helpers_profit-2.1.1/salure_helpers/profit/profit_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1495,15 +1495,15 @@
                 }
             }
         }
 
         # Add overload fields to the base of the employee data
         fields_to_update_employee = {}
         fields_to_update_employee.update({"DaMa": data['date_of_marriage']}) if 'date_of_marriage' in data else fields_to_update_employee
-        fields_to_update_employee.update({"DaDe": data['date_of_death']}) if 'employee_id' in data else fields_to_update_employee
+        fields_to_update_employee.update({"DaDe": data['date_of_death']}) if 'date_of_death' in data else fields_to_update_employee
         fields_to_update_employee.update({"PsPv": data['send_payslip']}) if 'send_payslip' in data else fields_to_update_employee
         fields_to_update_employee.update({"YsPv": data['send_annual_statement']}) if 'send_annual_statement' in data else fields_to_update_employee
         body['AfasEmployee']['Element'].update({"@EmId": data['employee_id'] if "employee_id" in data else {}})
         # add overload employee fields to  the body
         if overload_fields is not None and 'employee' in overload_fields.keys():
             fields_to_update_employee.update(overload_fields['employee'])
         body['AfasEmployee']['Element']['Fields'].update(fields_to_update_employee)
```

### Comparing `salure_helpers_profit-2.1.0/setup.py` & `salure_helpers_profit-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_profit',
-    version='2.1.0',
+    version='2.1.1',
     description='Profit wrapper from Salure',
     long_description='Profit wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.profit"],
     license='Salure License',
     install_requires=[
```

