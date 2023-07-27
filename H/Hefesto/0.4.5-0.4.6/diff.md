# Comparing `tmp/Hefesto-0.4.5.tar.gz` & `tmp/Hefesto-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.4.5.tar", last modified: Fri Jun 30 05:47:51 2023, max compression
+gzip compressed data, was "Hefesto-0.4.6.tar", last modified: Thu Jul 27 09:10:40 2023, max compression
```

## Comparing `Hefesto-0.4.5.tar` & `Hefesto-0.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-30 05:47:51.953725 Hefesto-0.4.5/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-30 05:47:51.953725 Hefesto-0.4.5/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.5/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12391 2023-06-28 12:39:32.000000 Hefesto-0.4.5/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    17203 2023-06-27 12:31:17.000000 Hefesto-0.4.5/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-06-30 05:47:51.953725 Hefesto-0.4.5/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-06-30 05:47:51.000000 Hefesto-0.4.5/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.5/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-06-30 05:47:51.953725 Hefesto-0.4.5/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     2581 2023-06-19 08:51:18.000000 Hefesto-0.4.5/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.5/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-06-30 05:47:51.953725 Hefesto-0.4.5/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-06-28 11:52:18.000000 Hefesto-0.4.5/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-07-27 09:10:40.936933 Hefesto-0.4.6/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-07-27 09:10:40.936933 Hefesto-0.4.6/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.6/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    12403 2023-07-27 09:09:46.000000 Hefesto-0.4.6/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    17218 2023-07-27 08:35:48.000000 Hefesto-0.4.6/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-07-27 09:10:40.936933 Hefesto-0.4.6/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-07-27 09:10:40.000000 Hefesto-0.4.6/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.6/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-07-27 09:10:40.936933 Hefesto-0.4.6/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     2581 2023-06-19 08:51:18.000000 Hefesto-0.4.6/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       22 2023-05-29 17:45:16.000000 Hefesto-0.4.6/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-07-27 09:10:40.936933 Hefesto-0.4.6/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-07-27 09:09:56.000000 Hefesto-0.4.6/setup.py
```

### Comparing `Hefesto-0.4.5/Hefesto/main.py` & `Hefesto-0.4.6/Hefesto/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,19 +297,20 @@
         return new
         
 
 # # Test 1:
 
 # test = Hefesto(datainput = "../data/INPUT_DATA.csv")
 # transform = test.transformFiab()
-# transform.to_csv ("../data/OUTPUT_DATA.csv", index = False, header=True)
+# transform.to_csv ("../data/OUTPUT_DATA_new.csv", index = False, header=True)
+
+# # Test 2:
 
-# Test 2
 # with open("../data/CDEconfig.yaml") as file:
 #     configuration = yaml.load(file, Loader=yaml.FullLoader)
 
 # test = Hefesto(datainput = "../data/INPUT_DATA2.csv")
 # transform = test.transformShape(configuration=configuration, clean_blanks = True) #, clean_blanks=False
 # # label = test.get_label("output_type")
 # # url_from_label= test.get_uri("output_type_label","ncit")
 # # repl= test.replacement("output_type_label", "Date","DateXXX", duplicate=False)
-# transform.to_csv ("../data/OUTPUT_DATA2.csv", index = False, header=True)
+# transform.to_csv ("../data/OUTPUT_DATA2_new.csv", index = False, header=True)
```

### Comparing `Hefesto-0.4.5/Hefesto/template.py` & `Hefesto-0.4.6/Hefesto/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,15 +592,15 @@
       frequency_value = None,
       route_type = None,
       value_id = None,
       value_date = None,
       value_integer = None,
       value_string = None,
       value_float = None,
-      value_datatype = None,
+      value_datatype = "xsd:string",
       age = None,
       date = None,
       startdate = None,
       enddate = None,
       uniqid = None,
       context_startdate = None,
       context_enddate = None
@@ -624,15 +624,15 @@
       frequency_value = None,
       route_type = None,
       value_id = None,
       value_date = None,
       value_integer = None,
       value_string = None,
       value_float = None,
-      value_datatype = None,
+      value_datatype = "xsd:float",
       age = None,
       date = None,
       startdate = None,
       enddate = None,
       uniqid = None,
       context_startdate = None,
       context_enddate = None
```

### Comparing `Hefesto-0.4.5/README.md` & `Hefesto-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `Hefesto-0.4.5/setup.py` & `Hefesto-0.4.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.4.5",
+    version="0.4.6",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

