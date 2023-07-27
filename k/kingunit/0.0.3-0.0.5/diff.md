# Comparing `tmp/kingunit-0.0.3.tar.gz` & `tmp/kingunit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-4p_9szvl/kingunit-0.0.3.tar", last modified: Fri Jul 21 01:19:51 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit/dist/.tmp-j_3w1qs1/kingunit-0.0.5.tar", last modified: Thu Jul 27 06:32:11 2023, max compression
```

## Comparing `kingunit-0.0.3.tar` & `kingunit-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 01:19:51.479140 kingunit-0.0.3/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-21 01:19:51.478881 kingunit-0.0.3/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.3/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 01:19:51.474920 kingunit-0.0.3/kingunit/
--rw-r--r--   0 jiayu      (501) staff       (20)       45 2023-07-21 00:51:02.000000 kingunit-0.0.3/kingunit/__init__.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 01:19:51.476890 kingunit-0.0.3/kingunit/cmd/
--rw-r--r--   0 jiayu      (501) staff       (20)       18 2023-07-19 01:25:45.000000 kingunit-0.0.3/kingunit/cmd/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.3/kingunit/cmd/cmd.py
--rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.3/kingunit/cmd/main.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 01:19:51.477439 kingunit-0.0.3/kingunit/config/
--rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.3/kingunit/config/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.3/kingunit/config/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     3240 2023-07-21 00:48:38.000000 kingunit-0.0.3/kingunit/generator.py
--rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.3/kingunit/init.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 01:19:51.478401 kingunit-0.0.3/kingunit/utils/
--rw-r--r--   0 jiayu      (501) staff       (20)       42 2023-07-18 06:09:17.000000 kingunit-0.0.3/kingunit/utils/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.3/kingunit/utils/loader.py
--rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.3/kingunit/utils/mail.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-21 01:19:51.476124 kingunit-0.0.3/kingunit.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-21 01:19:51.000000 kingunit-0.0.3/kingunit.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      438 2023-07-21 01:19:51.000000 kingunit-0.0.3/kingunit.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-21 01:19:51.000000 kingunit-0.0.3/kingunit.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-21 01:19:51.000000 kingunit-0.0.3/kingunit.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-21 01:19:51.000000 kingunit-0.0.3/kingunit.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-21 01:19:45.000000 kingunit-0.0.3/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-21 01:19:51.479244 kingunit-0.0.3/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.453187 kingunit-0.0.5/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:32:11.452977 kingunit-0.0.5/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      557 2023-07-21 01:16:19.000000 kingunit-0.0.5/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.449633 kingunit-0.0.5/kingunit/
+-rw-r--r--   0 jiayu      (501) staff       (20)       45 2023-07-21 00:51:02.000000 kingunit-0.0.5/kingunit/__init__.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.451229 kingunit-0.0.5/kingunit/cmd/
+-rw-r--r--   0 jiayu      (501) staff       (20)       18 2023-07-19 01:25:45.000000 kingunit-0.0.5/kingunit/cmd/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     1417 2023-07-21 00:48:38.000000 kingunit-0.0.5/kingunit/cmd/cmd.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      107 2023-07-21 00:49:06.000000 kingunit-0.0.5/kingunit/cmd/main.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.451834 kingunit-0.0.5/kingunit/config/
+-rw-r--r--   0 jiayu      (501) staff       (20)       24 2023-07-19 07:26:28.000000 kingunit-0.0.5/kingunit/config/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      330 2023-07-21 00:48:38.000000 kingunit-0.0.5/kingunit/config/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     4367 2023-07-27 06:18:46.000000 kingunit-0.0.5/kingunit/generator.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      699 2023-07-21 01:17:04.000000 kingunit-0.0.5/kingunit/init.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.452719 kingunit-0.0.5/kingunit/utils/
+-rw-r--r--   0 jiayu      (501) staff       (20)       66 2023-07-27 06:19:49.000000 kingunit-0.0.5/kingunit/utils/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      181 2023-07-18 05:54:49.000000 kingunit-0.0.5/kingunit/utils/loader.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     2447 2023-07-21 00:48:38.000000 kingunit-0.0.5/kingunit/utils/mail.py
+-rw-r--r--   0 jiayu      (501) staff       (20)      171 2023-07-27 06:19:42.000000 kingunit-0.0.5/kingunit/utils/validator.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-27 06:32:11.450548 kingunit-0.0.5/kingunit.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)      811 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      466 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       57 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-27 06:32:11.000000 kingunit-0.0.5/kingunit.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      493 2023-07-27 06:30:49.000000 kingunit-0.0.5/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-27 06:32:11.453257 kingunit-0.0.5/setup.cfg
```

### Comparing `kingunit-0.0.3/PKG-INFO` & `kingunit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.3
+Version: 0.0.5
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

### Comparing `kingunit-0.0.3/README.md` & `kingunit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.3/kingunit/cmd/cmd.py` & `kingunit-0.0.5/kingunit/cmd/cmd.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.3/kingunit/generator.py` & `kingunit-0.0.5/kingunit/generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,46 @@
             file.write(f"    inspector('{api_file['baseUrl']}', {str(case)})\n")
 
     # 使用black格式化代码
     # 检查是否安装了black
     if os.system("black --version") == 0:
         os.system(f"black {config['output_path']}/{api_file['name']}/{config['test_cases_file']}")
 
+def Gen_Cases_With_Json(api_file: str):
+    """
+    生成测试用例
+    """
+
+    # 校验json格式
+    if not utils.CheckJson(api_file):
+        raise Exception("Invalid json.")
+    
+
+    # 创建测试文件夹，检查是否存在
+    if not os.path.exists(f"{config['output_path']}"):
+        os.mkdir(f"{config['output_path']}")
+    if not os.path.exists(f"{config['output_path']}/{api_file['name']}"):
+        os.mkdir(f"{config['output_path']}/{api_file['name']}")
+
+    # 生成测试文件
+    with open(
+        f"{config['output_path']}/{api_file['name']}/{config['test_cases_file']}", "w"
+    ) as file:
+        file.write("from kingunit_inspector.inspector import *\n")
+        for case in api_file["apis"]:
+            file.write("\n")
+            file.write("\n")
+            file.write(f"def test_{case['name']}():\n")
+            file.write(f"    inspector('{api_file['baseUrl']}', {str(case)})\n")
+
+    # 使用black格式化代码
+    # 检查是否安装了black
+    if os.system("black --version") == 0:
+        os.system(f"black {config['output_path']}/{api_file['name']}/{config['test_cases_file']}")
+
 
 def Gen_Report(case_name: str, use_allure: bool = False):
     """
     生成测试报告
     """
 
     # 检查pytest是否安装
```

### Comparing `kingunit-0.0.3/kingunit/init.py` & `kingunit-0.0.5/kingunit/init.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.3/kingunit/utils/mail.py` & `kingunit-0.0.5/kingunit/utils/mail.py`

 * *Files identical despite different names*

### Comparing `kingunit-0.0.3/kingunit.egg-info/PKG-INFO` & `kingunit-0.0.5/kingunit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit
-Version: 0.0.3
+Version: 0.0.5
 Summary: KingUnit
 Author-email: 东南dnf <zjy2414@outlook.com>
 Project-URL: Home, https://github.com/zjy2414
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # KingUnit
```

