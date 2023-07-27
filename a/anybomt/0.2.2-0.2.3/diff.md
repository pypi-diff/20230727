# Comparing `tmp/anybomt-0.2.2.tar.gz` & `tmp/anybomt-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anybomt-0.2.2.tar", last modified: Thu Jul 27 00:43:52 2023, max compression
+gzip compressed data, was "anybomt-0.2.3.tar", last modified: Thu Jul 27 07:09:07 2023, max compression
```

## Comparing `anybomt-0.2.2.tar` & `anybomt-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 00:43:51.998278 anybomt-0.2.2/
--rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.2.2/LICENSE
--rw-rw-rw-   0        0        0    24402 2023-07-27 00:43:51.998278 anybomt-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    23973 2023-07-22 09:55:41.000000 anybomt-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 00:43:51.989732 anybomt-0.2.2/anybomt.egg-info/
--rw-rw-rw-   0        0        0    24402 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    90193 2023-07-27 00:43:06.000000 anybomt-0.2.2/anybomt.py
--rw-rw-rw-   0        0        0       42 2023-07-27 00:43:51.998278 anybomt-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      970 2023-07-27 00:43:23.000000 anybomt-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 07:09:07.666002 anybomt-0.2.3/
+-rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0    24402 2023-07-27 07:09:07.664998 anybomt-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    23973 2023-07-22 09:55:41.000000 anybomt-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 07:09:07.661457 anybomt-0.2.3/anybomt.egg-info/
+-rw-rw-rw-   0        0        0    24402 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 07:09:07.000000 anybomt-0.2.3/anybomt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    90356 2023-07-27 07:07:31.000000 anybomt-0.2.3/anybomt.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 07:09:07.667047 anybomt-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      980 2023-07-27 07:08:50.000000 anybomt-0.2.3/setup.py
```

### Comparing `anybomt-0.2.2/LICENSE` & `anybomt-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anybomt-0.2.2/PKG-INFO` & `anybomt-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anybomt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Uma biblioteca para facilitar sua jornada em matemática
 Author: AnyBoMath
 Author-email: bidjorys@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anybomt-0.2.2/README.md` & `anybomt-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `anybomt-0.2.2/anybomt.egg-info/PKG-INFO` & `anybomt-0.2.3/anybomt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anybomt
-Version: 0.2.2
+Version: 0.2.3
 Summary: Uma biblioteca para facilitar sua jornada em matemática
 Author: AnyBoMath
 Author-email: bidjorys@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anybomt-0.2.2/anybomt.py` & `anybomt-0.2.3/anybomt.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 def potencia(base, exponent):
     try:
         return base ** exponent
     except Exception as e:
         return e
 
 # Função para calcular o máximo entre dois números inteiros
-def valor_maximo(a, b):
+def valor_maximo(*args):
     try:
-        return max(a, b)
+        return max(args)
     except Exception as e:
         return e
       
 # Função para calcular o mínimo entre dois números inteiros
-def valor_minimo(a, b):
+def valor_minimo(*args):
     try:
-        return min(a, b)
+        return min(args)
     except Exception as e:
         return e
 
 # Função para calcular a raiz quadrada de um número
 def raiz_quadrada(num):
     try:
         import math
@@ -56,14 +56,24 @@
     
 def em_ordem(*args):
     try:
         return sorted(args)
     except Exception as e:
         return e
 
+def limpa():
+    import os
+    import platform
+    if platform.system() == "Windows":
+        os.system('cls')
+    else:
+        os.system('clear')
+
+
+
 # Classe Trigonometria
 class Trigonometria:
     # Função para calcular o seno de um ângulo em radianos
     def seno(angle):
         try:
             import math
             return math.sin(angle)
```

### Comparing `anybomt-0.2.2/setup.py` & `anybomt-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Leitura do arquivo README.md
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 # Configuração do pacote
 setup(
     name='anybomt',
-    version='0.2.2',
+    version='0.2.3',
     license='MIT',
     author='AnyBoMath',
     author_email='bidjorys@gmail.com',
     description='Uma biblioteca para facilitar sua jornada em matemática',
     long_description=long_description,
     long_description_content_type='text/markdown',
   # Substitua com o link do seu repositório no GitHub
@@ -22,11 +22,12 @@
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'scipy',
         'numpy',
         'sympy',
         'mpmath',
+        
         # outras dependências da sua biblioteca
     ],
     python_requires='>=3.6',
 )
```

