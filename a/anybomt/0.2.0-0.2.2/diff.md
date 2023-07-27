# Comparing `tmp/anybomt-0.2.0.tar.gz` & `tmp/anybomt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anybomt-0.2.0.tar", last modified: Sat Jul 22 09:56:01 2023, max compression
+gzip compressed data, was "anybomt-0.2.2.tar", last modified: Thu Jul 27 00:43:52 2023, max compression
```

## Comparing `anybomt-0.2.0.tar` & `anybomt-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 09:56:01.782758 anybomt-0.2.0/
--rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    24402 2023-07-22 09:56:01.781729 anybomt-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    23973 2023-07-22 09:55:41.000000 anybomt-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 09:56:01.779604 anybomt-0.2.0/anybomt.egg-info/
--rw-rw-rw-   0        0        0    24402 2023-07-22 09:56:01.000000 anybomt-0.2.0/anybomt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-07-22 09:56:01.000000 anybomt-0.2.0/anybomt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:56:01.000000 anybomt-0.2.0/anybomt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:56:01.000000 anybomt-0.2.0/anybomt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    90267 2023-07-22 09:54:27.000000 anybomt-0.2.0/anybomt.py
--rw-rw-rw-   0        0        0       42 2023-07-22 09:56:01.782758 anybomt-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      815 2023-07-22 09:54:58.000000 anybomt-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 00:43:51.998278 anybomt-0.2.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-21 08:26:10.000000 anybomt-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    24402 2023-07-27 00:43:51.998278 anybomt-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    23973 2023-07-22 09:55:41.000000 anybomt-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 00:43:51.989732 anybomt-0.2.2/anybomt.egg-info/
+-rw-rw-rw-   0        0        0    24402 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 00:43:51.000000 anybomt-0.2.2/anybomt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    90193 2023-07-27 00:43:06.000000 anybomt-0.2.2/anybomt.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 00:43:51.998278 anybomt-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-07-27 00:43:23.000000 anybomt-0.2.2/setup.py
```

### Comparing `anybomt-0.2.0/LICENSE` & `anybomt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anybomt-0.2.0/PKG-INFO` & `anybomt-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anybomt
-Version: 0.2.0
+Version: 0.2.2
 Summary: Uma biblioteca para facilitar sua jornada em matemática
 Author: AnyBoMath
 Author-email: bidjorys@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anybomt-0.2.0/README.md` & `anybomt-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `anybomt-0.2.0/anybomt.egg-info/PKG-INFO` & `anybomt-0.2.2/anybomt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anybomt
-Version: 0.2.0
+Version: 0.2.2
 Summary: Uma biblioteca para facilitar sua jornada em matemática
 Author: AnyBoMath
 Author-email: bidjorys@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anybomt-0.2.0/anybomt.py` & `anybomt-0.2.2/anybomt.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,26 @@
 
 def somar(*args):
     try:
         return sum(args)
     except Exception as e:
         return e
 
+def comprimento_de(*args):
+    try:
+        return len(args)
+    except Exception as e:
+        return e
+    
+def em_ordem(*args):
+    try:
+        return sorted(args)
+    except Exception as e:
+        return e
+
 # Classe Trigonometria
 class Trigonometria:
     # Função para calcular o seno de um ângulo em radianos
     def seno(angle):
         try:
             import math
             return math.sin(angle)
@@ -152,90 +164,67 @@
         import math
         return math.exp(num)
     except Exception as e:
         return e
     
 def PI():
     try:
-        from mpmath import mp
-        mp.dps = 20
-        pi_value = mp.pi
+        pi_value = 3.14159265358979323846
         return pi_value
     except Exception as e:
         return e
 
 def PI_Long():
     try:
-        from mpmath import mp
-        mp.dps = 200
-        pi_value = mp.pi
+        pi_value =3.1415926535897932384626433832795028841971693993751058209749445923078164062862089986280348253421170679
         return pi_value
     except Exception as e: return e
 
 def E_long():
     try:
-        from mpmath import mp
-        mp.dps = 200
-        euler_value = mp.e
+        euler_value = 2.7182818284590452353602874713526624977572470936999595749669676277240766303535475945713821785251664274
         return euler_value
     except Exception as e:
         return e
 
 def E():
     try:
-        from mpmath import mp
-        # Define a precisão para 200 casas decimais
-        mp.dps = 20
-
         # Obtém o valor de e com 200 casas decimais
-        euler_value = mp.e
+        euler_value = 2.71828182845904523536
 
         return euler_value
     except Exception as e: return e
 
 
 def Num_Au_long():
     try:
-        from mpmath import mp
-        mp.dps = 200
+        import math as mp
         phi = (1 + mp.sqrt(5)) / 2
         return phi
     except Exception as e: return e
 
 def Num_Au():
     try:
-        from mpmath import mp
-        mp.dps = 20
+        import math as mp
         phi = (1 + mp.sqrt(5)) / 2
         return phi
     except Exception as e: return e
 
 
 
-def Num_catalan():
-    try:
-        from mpmath import mp
-        mp.dps = 20
-        catalan = mp.catalan
-        return catalan
-    except Exception as e: return e
-
-def Num_catalan_long():
+def Num_catalan(n):
     try:
-        from mpmath import mp
-        mp.dps = 200
-        catalan = mp.catalan
-        return catalan
+        import math 
+        numero = math.factorial(2*n) // (math.factorial(n+1) * math.factorial(n))
+        return numero
     except Exception as e: return e
 
 
 def feigenbaum_delta_long():
     try:
-        from mpmath import mp
-        mp.dps = 200
         feigenbaum_delta = 4.669201609102990671853203821578
         return feigenbaum_delta
     except Exception as e: return e
 
 def feigenbaum_delta():
     try:
         from mpmath import mp
```

### Comparing `anybomt-0.2.0/setup.py` & `anybomt-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,23 +3,30 @@
 # Leitura do arquivo README.md
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 # Configuração do pacote
 setup(
     name='anybomt',
-    version='0.2.0',
+    version='0.2.2',
     license='MIT',
     author='AnyBoMath',
     author_email='bidjorys@gmail.com',
     description='Uma biblioteca para facilitar sua jornada em matemática',
     long_description=long_description,
     long_description_content_type='text/markdown',
   # Substitua com o link do seu repositório no GitHub
     packages=[''],  # Lista de pacotes que serão incluídos
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    install_requires=[
+        'scipy',
+        'numpy',
+        'sympy',
+        'mpmath',
+        # outras dependências da sua biblioteca
+    ],
     python_requires='>=3.6',
 )
```

