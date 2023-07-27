# Comparing `tmp/LibcSearcher3-1.3.0.tar.gz` & `tmp/LibcSearcher3-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/LibcSearcher3-1.3.0.tar", last modified: Fri Mar 18 01:20:03 2022, max compression
+gzip compressed data, was "dist/LibcSearcher3-1.4.0.tar", last modified: Thu Jul 27 02:54:01 2023, max compression
```

## Comparing `LibcSearcher3-1.3.0.tar` & `LibcSearcher3-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 01:20:03.000000 LibcSearcher3-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 01:20:03.000000 LibcSearcher3-1.3.0/LibcSearcher3/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/LibcSearcher3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/LibcSearcher3/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 01:20:03.000000 LibcSearcher3-1.3.0/LibcSearcher3/db/
--rw-r--r--   0 runner    (1001) docker     (121)  3167836 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/LibcSearcher3/db/libc.tar.bz2
--rwxr-xr-x   0 runner    (1001) docker     (121)     4309 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/LibcSearcher3/main.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/LibcSearcher3/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 01:20:03.000000 LibcSearcher3-1.3.0/LibcSearcher3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-03-18 01:20:02.000000 LibcSearcher3-1.3.0/LibcSearcher3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-03-18 01:20:03.000000 LibcSearcher3-1.3.0/LibcSearcher3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 01:20:02.000000 LibcSearcher3-1.3.0/LibcSearcher3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-18 01:20:02.000000 LibcSearcher3-1.3.0/LibcSearcher3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-18 01:20:02.000000 LibcSearcher3-1.3.0/LibcSearcher3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4472 2022-03-18 01:20:03.000000 LibcSearcher3-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3363 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-18 01:20:03.000000 LibcSearcher3-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-03-18 01:19:48.000000 LibcSearcher3-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:54:01.000000 LibcSearcher3-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:54:01.000000 LibcSearcher3-1.4.0/LibcSearcher3/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/LibcSearcher3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/LibcSearcher3/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:54:01.000000 LibcSearcher3-1.4.0/LibcSearcher3/db/
+-rw-r--r--   0 runner    (1001) docker     (123)  3167836 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/LibcSearcher3/db/libc.tar.bz2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4372 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/LibcSearcher3/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/LibcSearcher3/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/LibcSearcher3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 02:54:01.000000 LibcSearcher3-1.4.0/LibcSearcher3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-27 02:54:00.000000 LibcSearcher3-1.4.0/LibcSearcher3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-27 02:54:01.000000 LibcSearcher3-1.4.0/LibcSearcher3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 02:54:00.000000 LibcSearcher3-1.4.0/LibcSearcher3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-27 02:54:00.000000 LibcSearcher3-1.4.0/LibcSearcher3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 02:54:00.000000 LibcSearcher3-1.4.0/LibcSearcher3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-27 02:54:01.000000 LibcSearcher3-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 02:54:01.000000 LibcSearcher3-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-27 02:53:48.000000 LibcSearcher3-1.4.0/setup.py
```

### Comparing `LibcSearcher3-1.3.0/LibcSearcher3/cmd.py` & `LibcSearcher3-1.4.0/LibcSearcher3/cmd.py`

 * *Files identical despite different names*

### Comparing `LibcSearcher3-1.3.0/LibcSearcher3/db/libc.tar.bz2` & `LibcSearcher3-1.4.0/LibcSearcher3/db/libc.tar.bz2`

 * *Files identical despite different names*

### Comparing `LibcSearcher3-1.3.0/LibcSearcher3/main.py` & `LibcSearcher3-1.4.0/LibcSearcher3/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,23 +32,25 @@
         for name, address in self.condition.items():
             addr_last12 = address & 0xfff
             res.append(re.compile("^%s .*%x" % (name, addr_last12)))
 
         db = self.libc_database_path
         # only read "*.symbols" file to find
         files = [x for x in os.listdir(db) if x.endswith('.symbols')]
-        
+
         result = []
         for ff in files:
             with open(db+ff, 'rb') as f:
                 data = f.read().decode(errors='ignore').split("\n")
+                matched = len(res)
                 for x in res:
                     if any(map(lambda line: x.match(line), data)):
-                        result.append(ff)
-                        break
+                        matched -= 1
+                if matched == 0:
+                    result.append(ff)
 
         if len(result) == 0:
             print("No matched libc, please add more libc or try others")
             return
 
         if len(result) > 1:
             print("Multi Results:")
```

### Comparing `LibcSearcher3-1.3.0/LibcSearcher3/utils.py` & `LibcSearcher3-1.4.0/LibcSearcher3/utils.py`

 * *Files identical despite different names*

### Comparing `LibcSearcher3-1.3.0/LibcSearcher3.egg-info/PKG-INFO` & `LibcSearcher3-1.4.0/LibcSearcher3.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibcSearcher3
-Version: 1.3.0
+Version: 1.4.0
 Summary: libc offset database searcher
 Home-page: https://github.com/Ro0tk1t/LibcSearcher3.git
 Author: Ro0tk1t
 Author-email: R00tk1t@qq.com
 License: UNKNOWN
 Description: [![PKGS](https://github.com/Ro0tk1t/LibcSearcher3/workflows/Upload%20Python%20Package/badge.svg)](https://github.com/Ro0tk1t/LibcSearcher3/actions)
         [![PyPI package](https://badge.fury.io/py/LibcSearcher3.svg)](https://pypi.org/project/LibcSearcher3/)
@@ -46,22 +46,24 @@
         ```
         
         ## 使用
         
         ### 实例化
         
         ```python
-        from LibcSearcher import *
+        from LibcSearcher3 import *
         
         #第二个参数，为已泄露的实际地址,或最后12位(比如：d90)，int类型
         obj = LibcSearcher("fgets", 0x7ff39014bd90)
         
-        obj.dump("system")        #system 偏移
-        obj.dump("str_bin_sh")    #/bin/sh 偏移
-        obj.dump("__libc_start_main_ret")    
+        obj = LibcSearcher("fgets", 0x7ff39014bd90) # 使用一个已知符号地址作为初始约束，初始化 LibcSearcher
+        obj.add_condition("atoi", 218528) # 添加一个约束条件
+        
+        print("[+]/bin/sh offset: ", hex(obj.dump("str_bin_sh"))) # 根据已有约束条件，查询某个符号在 Libc 中的地址
+        print("[+]system  offset: ", hex(obj.dump("system")))
         ```
         
         ### 命令行
         
         ```bash
         $ libcsearch --help
         usage: libcsearch [-h] [-i] [-f FUNC] [-d ADDR] [-t TO_LEAK]
```

### Comparing `LibcSearcher3-1.3.0/PKG-INFO` & `LibcSearcher3-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibcSearcher3
-Version: 1.3.0
+Version: 1.4.0
 Summary: libc offset database searcher
 Home-page: https://github.com/Ro0tk1t/LibcSearcher3.git
 Author: Ro0tk1t
 Author-email: R00tk1t@qq.com
 License: UNKNOWN
 Description: [![PKGS](https://github.com/Ro0tk1t/LibcSearcher3/workflows/Upload%20Python%20Package/badge.svg)](https://github.com/Ro0tk1t/LibcSearcher3/actions)
         [![PyPI package](https://badge.fury.io/py/LibcSearcher3.svg)](https://pypi.org/project/LibcSearcher3/)
@@ -46,22 +46,24 @@
         ```
         
         ## 使用
         
         ### 实例化
         
         ```python
-        from LibcSearcher import *
+        from LibcSearcher3 import *
         
         #第二个参数，为已泄露的实际地址,或最后12位(比如：d90)，int类型
         obj = LibcSearcher("fgets", 0x7ff39014bd90)
         
-        obj.dump("system")        #system 偏移
-        obj.dump("str_bin_sh")    #/bin/sh 偏移
-        obj.dump("__libc_start_main_ret")    
+        obj = LibcSearcher("fgets", 0x7ff39014bd90) # 使用一个已知符号地址作为初始约束，初始化 LibcSearcher
+        obj.add_condition("atoi", 218528) # 添加一个约束条件
+        
+        print("[+]/bin/sh offset: ", hex(obj.dump("str_bin_sh"))) # 根据已有约束条件，查询某个符号在 Libc 中的地址
+        print("[+]system  offset: ", hex(obj.dump("system")))
         ```
         
         ### 命令行
         
         ```bash
         $ libcsearch --help
         usage: libcsearch [-h] [-i] [-f FUNC] [-d ADDR] [-t TO_LEAK]
```

### Comparing `LibcSearcher3-1.3.0/README.md` & `LibcSearcher3-1.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,22 +38,24 @@
 ```
 
 ## 使用
 
 ### 实例化
 
 ```python
-from LibcSearcher import *
+from LibcSearcher3 import *
 
 #第二个参数，为已泄露的实际地址,或最后12位(比如：d90)，int类型
 obj = LibcSearcher("fgets", 0x7ff39014bd90)
 
-obj.dump("system")        #system 偏移
-obj.dump("str_bin_sh")    #/bin/sh 偏移
-obj.dump("__libc_start_main_ret")    
+obj = LibcSearcher("fgets", 0x7ff39014bd90) # 使用一个已知符号地址作为初始约束，初始化 LibcSearcher
+obj.add_condition("atoi", 218528) # 添加一个约束条件
+
+print("[+]/bin/sh offset: ", hex(obj.dump("str_bin_sh"))) # 根据已有约束条件，查询某个符号在 Libc 中的地址
+print("[+]system  offset: ", hex(obj.dump("system")))
 ```
 
 ### 命令行
 
 ```bash
 $ libcsearch --help
 usage: libcsearch [-h] [-i] [-f FUNC] [-d ADDR] [-t TO_LEAK]
```

### Comparing `LibcSearcher3-1.3.0/setup.py` & `LibcSearcher3-1.4.0/setup.py`

 * *Files identical despite different names*

