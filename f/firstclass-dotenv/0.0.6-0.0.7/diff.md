# Comparing `tmp/firstclass_dotenv-0.0.6.tar.gz` & `tmp/firstclass_dotenv-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/firstclass_dotenv-0.0.6.tar", last modified: Wed Nov 18 10:26:27 2020, max compression
+gzip compressed data, was "firstclass_dotenv-0.0.7.tar", last modified: Thu Jul 27 05:29:33 2023, max compression
```

## Comparing `firstclass_dotenv-0.0.6.tar` & `firstclass_dotenv-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 hwp        (502) staff       (20)        0 2020-11-18 10:26:27.025583 firstclass_dotenv-0.0.6/
--rw-r--r--   0 hwp        (502) staff       (20)     2046 2020-11-18 10:26:27.025111 firstclass_dotenv-0.0.6/PKG-INFO
--rw-r--r--   0 hwp        (502) staff       (20)     1138 2020-11-18 10:26:00.000000 firstclass_dotenv-0.0.6/README.md
-drwxr-xr-x   0 hwp        (502) staff       (20)        0 2020-11-18 10:26:27.020324 firstclass_dotenv-0.0.6/firstclass_dotenv/
--rw-r--r--   0 hwp        (502) staff       (20)       52 2020-11-18 09:46:16.000000 firstclass_dotenv-0.0.6/firstclass_dotenv/__init__.py
--rw-r--r--   0 hwp        (502) staff       (20)      774 2020-11-18 10:24:58.000000 firstclass_dotenv-0.0.6/firstclass_dotenv/main.py
-drwxr-xr-x   0 hwp        (502) staff       (20)        0 2020-11-18 10:26:27.022892 firstclass_dotenv-0.0.6/firstclass_dotenv.egg-info/
--rw-r--r--   0 hwp        (502) staff       (20)     2046 2020-11-18 10:26:26.000000 firstclass_dotenv-0.0.6/firstclass_dotenv.egg-info/PKG-INFO
--rw-r--r--   0 hwp        (502) staff       (20)      286 2020-11-18 10:26:26.000000 firstclass_dotenv-0.0.6/firstclass_dotenv.egg-info/SOURCES.txt
--rw-r--r--   0 hwp        (502) staff       (20)        1 2020-11-18 10:26:26.000000 firstclass_dotenv-0.0.6/firstclass_dotenv.egg-info/dependency_links.txt
--rw-r--r--   0 hwp        (502) staff       (20)       24 2020-11-18 10:26:26.000000 firstclass_dotenv-0.0.6/firstclass_dotenv.egg-info/top_level.txt
--rw-r--r--   0 hwp        (502) staff       (20)       38 2020-11-18 10:26:27.025793 firstclass_dotenv-0.0.6/setup.cfg
--rw-r--r--   0 hwp        (502) staff       (20)      650 2020-11-18 10:25:21.000000 firstclass_dotenv-0.0.6/setup.py
-drwxr-xr-x   0 hwp        (502) staff       (20)        0 2020-11-18 10:26:27.023730 firstclass_dotenv-0.0.6/tests/
--rw-r--r--   0 hwp        (502) staff       (20)        0 2020-11-18 09:46:16.000000 firstclass_dotenv-0.0.6/tests/__init__.py
--rw-r--r--   0 hwp        (502) staff       (20)      846 2020-11-18 10:00:28.000000 firstclass_dotenv-0.0.6/tests/test_1stclass_dotenv.py
+drwxr-xr-x   0 hajimekurita   (501) staff       (20)        0 2023-07-27 05:29:33.366804 firstclass_dotenv-0.0.7/
+-rw-r--r--   0 hajimekurita   (501) staff       (20)     1070 2023-07-27 05:13:58.000000 firstclass_dotenv-0.0.7/LICENSE
+-rw-r--r--   0 hajimekurita   (501) staff       (20)     1540 2023-07-27 05:29:33.366629 firstclass_dotenv-0.0.7/PKG-INFO
+-rw-r--r--   0 hajimekurita   (501) staff       (20)     1137 2023-07-27 05:13:58.000000 firstclass_dotenv-0.0.7/README.md
+drwxr-xr-x   0 hajimekurita   (501) staff       (20)        0 2023-07-27 05:29:33.364925 firstclass_dotenv-0.0.7/firstclass_dotenv/
+-rw-r--r--   0 hajimekurita   (501) staff       (20)       52 2023-07-27 05:13:58.000000 firstclass_dotenv-0.0.7/firstclass_dotenv/__init__.py
+-rw-r--r--   0 hajimekurita   (501) staff       (20)      823 2023-07-27 05:15:38.000000 firstclass_dotenv-0.0.7/firstclass_dotenv/main.py
+drwxr-xr-x   0 hajimekurita   (501) staff       (20)        0 2023-07-27 05:29:33.365918 firstclass_dotenv-0.0.7/firstclass_dotenv.egg-info/
+-rw-r--r--   0 hajimekurita   (501) staff       (20)     1540 2023-07-27 05:29:33.000000 firstclass_dotenv-0.0.7/firstclass_dotenv.egg-info/PKG-INFO
+-rw-r--r--   0 hajimekurita   (501) staff       (20)      294 2023-07-27 05:29:33.000000 firstclass_dotenv-0.0.7/firstclass_dotenv.egg-info/SOURCES.txt
+-rw-r--r--   0 hajimekurita   (501) staff       (20)        1 2023-07-27 05:29:33.000000 firstclass_dotenv-0.0.7/firstclass_dotenv.egg-info/dependency_links.txt
+-rw-r--r--   0 hajimekurita   (501) staff       (20)       24 2023-07-27 05:29:33.000000 firstclass_dotenv-0.0.7/firstclass_dotenv.egg-info/top_level.txt
+-rw-r--r--   0 hajimekurita   (501) staff       (20)       38 2023-07-27 05:29:33.366865 firstclass_dotenv-0.0.7/setup.cfg
+-rw-r--r--   0 hajimekurita   (501) staff       (20)      650 2023-07-27 05:28:28.000000 firstclass_dotenv-0.0.7/setup.py
+drwxr-xr-x   0 hajimekurita   (501) staff       (20)        0 2023-07-27 05:29:33.366288 firstclass_dotenv-0.0.7/tests/
+-rw-r--r--   0 hajimekurita   (501) staff       (20)        0 2023-07-27 05:13:58.000000 firstclass_dotenv-0.0.7/tests/__init__.py
+-rw-r--r--   0 hajimekurita   (501) staff       (20)      846 2023-07-27 05:13:58.000000 firstclass_dotenv-0.0.7/tests/test_1stclass_dotenv.py
```

### Comparing `firstclass_dotenv-0.0.6/PKG-INFO` & `firstclass_dotenv-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: firstclass_dotenv
-Version: 0.0.6
+Version: 0.0.7
 Summary: Read value of .env(dotenv) into ENV values
 Home-page: https://github.com/hikarine3/firstclass_dotenv
 Author: Hajime Kurita
-License: UNKNOWN
-Description: # firstclass-dotenv
-        dotenv package for python
-        
-        # How to install
-        pip install firstclass_dotenv
-        
-        # How to use
-        
-        ```
-        import os
-        from firstclass_dotenv import Dotenv
-        
-        if __name__ == "__main__":
-          dotenv = Dotenv
-          
-          # Load .env in current directory
-          dotenv.load()
-          
-          # Load specified .env
-          dotenv.load(".env.test")
-        
-          # print specified env value
-          print(os.environ["TESTENVVALUE"])
-        ```
-        
-        # Source code
-        You can find source code at
-        https://github.com/hikarine3/firstclass_dotenv
-        <!--
-        # How to test this module (This procedure is for developer of this module)
-        
-        ## Preparation
-        sudo pip install wheel;
-        
-        sudo pip install twine;
-        
-        ## Update version
-        vi setup.py
-        
-        ## Create distribution
-        rm -f dist/*;
-        python3 setup.py sdist bdist_wheel;
-        
-        ## Register if you haven't
-        https://test.pypi.org/
-        
-        ## Upload to Test
-        python -m twine upload --repository testpypi dist/*
-        
-        ## Confirm
-        https://test.pypi.org/project/firstclass-dotenv/
-        
-        ## Confirm by intallation
-        pip install -i https://test.pypi.org/simple/ firstclass-dotenv
-        
-        ## Deploy to production
-        python -m twine upload --repository pypi dist/*
-        
-        ## Confirm on Page
-        https://pypi.org/project/firstclass-dotenv/
-        -->
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# firstclass-dotenv
+dotenv package for python
+
+# How to install
+pip install firstclass_dotenv
+
+# How to use
+
+```
+import os
+from firstclass_dotenv import Dotenv
+
+if __name__ == "__main__":
+  dotenv = Dotenv
+  
+  # Load .env in current directory
+  dotenv.load()
+  
+  # Load specified .env
+  dotenv.load(".env.test")
+
+  # print specified env value
+  print(os.environ["TESTENVVALUE"])
+```
+
+# Source code
+You can find source code at
+https://github.com/hikarine3/firstclass_dotenv
+<!--
+# How to test this module (This procedure is for developer of this module)
+
+## Preparation
+sudo pip install wheel;
+
+sudo pip install twine;
+
+## Update version
+vi setup.py
+
+## Create distribution
+rm -f dist/*;
+python3 setup.py sdist bdist_wheel
+
+## Register if you haven't
+https://test.pypi.org/
+
+## Upload to Test
+python -m twine upload --repository testpypi dist/*
+
+## Confirm
+https://test.pypi.org/project/firstclass-dotenv/
+
+## Confirm by intallation
+pip install -i https://test.pypi.org/simple/ firstclass-dotenv
+
+## Deploy to production
+python -m twine upload --repository pypi dist/*
+
+## Confirm on Page
+https://pypi.org/project/firstclass-dotenv/
+-->
```

### Comparing `firstclass_dotenv-0.0.6/README.md` & `firstclass_dotenv-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 sudo pip install twine;
 
 ## Update version
 vi setup.py
 
 ## Create distribution
 rm -f dist/*;
-python3 setup.py sdist bdist_wheel;
+python3 setup.py sdist bdist_wheel
 
 ## Register if you haven't
 https://test.pypi.org/
 
 ## Upload to Test
 python -m twine upload --repository testpypi dist/*
```

### Comparing `firstclass_dotenv-0.0.6/firstclass_dotenv/main.py` & `firstclass_dotenv-0.0.7/firstclass_dotenv/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,19 +15,20 @@
         self.dotenv = ".env"
 
     if os.path.exists(self.dotenv):
       with open(self.dotenv, "r") as fh:
         line = fh.readline()
         while line:
           line = line.strip()
-          line = re.sub(r"\s*#.*", "", line)
+          line = re.sub(r"^#.*", "", line)
+          line = re.sub(r"\s#.*", "", line)
           try:
             (key, val) = line.split("=", 1)
             if val:
               val = re.sub('^"|"$', "", val)
-              os.environ[key] = val
+              os.environ[key] = val.trim()
             else:
               os.environ[key] = ""
           except:
             line = fh.readline()
             next
           line = fh.readline()
```

### Comparing `firstclass_dotenv-0.0.6/firstclass_dotenv.egg-info/PKG-INFO` & `firstclass_dotenv-0.0.7/firstclass_dotenv.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: firstclass-dotenv
-Version: 0.0.6
+Version: 0.0.7
 Summary: Read value of .env(dotenv) into ENV values
 Home-page: https://github.com/hikarine3/firstclass_dotenv
 Author: Hajime Kurita
-License: UNKNOWN
-Description: # firstclass-dotenv
-        dotenv package for python
-        
-        # How to install
-        pip install firstclass_dotenv
-        
-        # How to use
-        
-        ```
-        import os
-        from firstclass_dotenv import Dotenv
-        
-        if __name__ == "__main__":
-          dotenv = Dotenv
-          
-          # Load .env in current directory
-          dotenv.load()
-          
-          # Load specified .env
-          dotenv.load(".env.test")
-        
-          # print specified env value
-          print(os.environ["TESTENVVALUE"])
-        ```
-        
-        # Source code
-        You can find source code at
-        https://github.com/hikarine3/firstclass_dotenv
-        <!--
-        # How to test this module (This procedure is for developer of this module)
-        
-        ## Preparation
-        sudo pip install wheel;
-        
-        sudo pip install twine;
-        
-        ## Update version
-        vi setup.py
-        
-        ## Create distribution
-        rm -f dist/*;
-        python3 setup.py sdist bdist_wheel;
-        
-        ## Register if you haven't
-        https://test.pypi.org/
-        
-        ## Upload to Test
-        python -m twine upload --repository testpypi dist/*
-        
-        ## Confirm
-        https://test.pypi.org/project/firstclass-dotenv/
-        
-        ## Confirm by intallation
-        pip install -i https://test.pypi.org/simple/ firstclass-dotenv
-        
-        ## Deploy to production
-        python -m twine upload --repository pypi dist/*
-        
-        ## Confirm on Page
-        https://pypi.org/project/firstclass-dotenv/
-        -->
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# firstclass-dotenv
+dotenv package for python
+
+# How to install
+pip install firstclass_dotenv
+
+# How to use
+
+```
+import os
+from firstclass_dotenv import Dotenv
+
+if __name__ == "__main__":
+  dotenv = Dotenv
+  
+  # Load .env in current directory
+  dotenv.load()
+  
+  # Load specified .env
+  dotenv.load(".env.test")
+
+  # print specified env value
+  print(os.environ["TESTENVVALUE"])
+```
+
+# Source code
+You can find source code at
+https://github.com/hikarine3/firstclass_dotenv
+<!--
+# How to test this module (This procedure is for developer of this module)
+
+## Preparation
+sudo pip install wheel;
+
+sudo pip install twine;
+
+## Update version
+vi setup.py
+
+## Create distribution
+rm -f dist/*;
+python3 setup.py sdist bdist_wheel
+
+## Register if you haven't
+https://test.pypi.org/
+
+## Upload to Test
+python -m twine upload --repository testpypi dist/*
+
+## Confirm
+https://test.pypi.org/project/firstclass-dotenv/
+
+## Confirm by intallation
+pip install -i https://test.pypi.org/simple/ firstclass-dotenv
+
+## Deploy to production
+python -m twine upload --repository pypi dist/*
+
+## Confirm on Page
+https://pypi.org/project/firstclass-dotenv/
+-->
```

### Comparing `firstclass_dotenv-0.0.6/tests/test_1stclass_dotenv.py` & `firstclass_dotenv-0.0.7/tests/test_1stclass_dotenv.py`

 * *Files identical despite different names*

