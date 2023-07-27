# Comparing `tmp/mcptbr-0.1.8.tar.gz` & `tmp/mcptbr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcptbr-0.1.8.tar", last modified: Thu Jul 27 20:50:41 2023, max compression
+gzip compressed data, was "mcptbr-0.1.9.tar", last modified: Thu Jul 27 20:53:52 2023, max compression
```

## Comparing `mcptbr-0.1.8.tar` & `mcptbr-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 20:50:40.995519 mcptbr-0.1.8/
--rw-rw-rw-   0        0        0      718 2023-07-27 20:50:40.995519 mcptbr-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 20:50:40.979903 mcptbr-0.1.8/mcptbr/
--rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.8/mcptbr/__init__.py
--rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.8/mcptbr/model.py
-drwxrwxrwx   0        0        0        0 2023-07-27 20:50:40.995519 mcptbr-0.1.8/mcptbr.egg-info/
--rw-rw-rw-   0        0        0      718 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 20:50:40.000000 mcptbr-0.1.8/mcptbr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 20:50:40.995519 mcptbr-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      608 2023-07-27 20:50:32.000000 mcptbr-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:53:52.155262 mcptbr-0.1.9/
+-rw-rw-rw-   0        0        0      694 2023-07-27 20:53:52.155262 mcptbr-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 20:53:52.139641 mcptbr-0.1.9/mcptbr/
+-rw-rw-rw-   0        0        0        0 2023-07-24 11:28:31.000000 mcptbr-0.1.9/mcptbr/__init__.py
+-rw-rw-rw-   0        0        0     2202 2023-07-27 20:17:14.000000 mcptbr-0.1.9/mcptbr/model.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:53:52.155262 mcptbr-0.1.9/mcptbr.egg-info/
+-rw-rw-rw-   0        0        0      694 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-07-27 20:53:52.000000 mcptbr-0.1.9/mcptbr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-27 20:53:51.000000 mcptbr-0.1.9/mcptbr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:53:52.155262 mcptbr-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      626 2023-07-27 20:53:27.000000 mcptbr-0.1.9/setup.py
```

### Comparing `mcptbr-0.1.8/PKG-INFO` & `mcptbr-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # mcptbr
 
 
-mcptbr Ã© uma pequena biblioteca que permite o usuÃ¡rio a manipular blocos do Minecraft com python.
+mcptbr é uma pequena biblioteca que permite o usuário a manipular blocos do Minecraft com python.
 
 ## Para quem serve?
-Material criado para os alunos do curso de programaÃ§Ã£o em python no Minecraft.
+Material criado para os alunos do curso de programação em python no Minecraft.
 
-ObservaÃ§Ã£o: VersÃ£o em portuguÃªs de outras bibliotecas jÃ¡ existentes.
+Observação: Versão em português de outras bibliotecas já existentes.
 
 
 
-## InstalaÃ§Ã£o
-VÃ¡ ao CMD e digite pip install mcptbr.
+## Instalação
+Vá ao CMD e digite pip install mcptbr.
 
 
 
 ## Exemplo de uso
 ```
 from mcptbr.model import *
```

### Comparing `mcptbr-0.1.8/mcptbr/model.py` & `mcptbr-0.1.9/mcptbr/model.py`

 * *Files identical despite different names*

### Comparing `mcptbr-0.1.8/mcptbr.egg-info/PKG-INFO` & `mcptbr-0.1.9/mcptbr.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: mcptbr
-Version: 0.1.8
+Version: 0.1.9
 Summary: Biblioteca para manipular o Minecraft através do python.
 Author: Lucas Pereira
 Author-email: lucasthe2@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 
 # mcptbr
 
 
-mcptbr Ã© uma pequena biblioteca que permite o usuÃ¡rio a manipular blocos do Minecraft com python.
+mcptbr é uma pequena biblioteca que permite o usuário a manipular blocos do Minecraft com python.
 
 ## Para quem serve?
-Material criado para os alunos do curso de programaÃ§Ã£o em python no Minecraft.
+Material criado para os alunos do curso de programação em python no Minecraft.
 
-ObservaÃ§Ã£o: VersÃ£o em portuguÃªs de outras bibliotecas jÃ¡ existentes.
+Observação: Versão em português de outras bibliotecas já existentes.
 
 
 
-## InstalaÃ§Ã£o
-VÃ¡ ao CMD e digite pip install mcptbr.
+## Instalação
+Vá ao CMD e digite pip install mcptbr.
 
 
 
 ## Exemplo de uso
 ```
 from mcptbr.model import *
```

### Comparing `mcptbr-0.1.8/setup.py` & `mcptbr-0.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mcptbr',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=[
         "mcpi", # Dependências necessárias para sua biblioteca (se houver).
     ],
     author='Lucas Pereira',
     author_email='lucasthe2@gmail.com',
     description='Biblioteca para manipular o Minecraft através do python.',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     #url='https://github.com/seu_usuario/minha_biblioteca',
     license='MIT',  # Substitua pela licença adequada.
 )
```

