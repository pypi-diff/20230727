# Comparing `tmp/feriados_brasileiros-0.0.5.tar.gz` & `tmp/feriados_brasileiros-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feriados_brasileiros-0.0.5.tar", last modified: Tue Jun 20 03:00:07 2023, max compression
+gzip compressed data, was "feriados_brasileiros-0.0.7.tar", last modified: Thu Jul 27 00:37:43 2023, max compression
```

## Comparing `feriados_brasileiros-0.0.5.tar` & `feriados_brasileiros-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/feriados_brasileiros/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/feriados_brasileiros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17405 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/feriados_brasileiros/datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 03:00:07.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 03:00:06.000000 feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 03:00:07.010294 feriados_brasileiros-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 02:59:58.000000 feriados_brasileiros-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:43.954950 feriados_brasileiros-0.0.7/feriados_brasileiros/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/feriados_brasileiros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17423 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/feriados_brasileiros/datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 00:37:43.000000 feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 00:37:43.958950 feriados_brasileiros-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 00:37:34.000000 feriados_brasileiros-0.0.7/setup.py
```

### Comparing `feriados_brasileiros-0.0.5/LICENSE` & `feriados_brasileiros-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.5/MANIFEST.in` & `feriados_brasileiros-0.0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `feriados_brasileiros-0.0.5/PKG-INFO` & `feriados_brasileiros-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: feriados_brasileiros
-Version: 0.0.5
+Version: 0.0.7
 Summary: Feriados Brasileiros
 Home-page: https://github.com/michelmetran/feriados
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
-Keywords: python,dados espaciais,geoprocessamento
+Keywords: python,datas,feriados
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Portuguese
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -81,15 +81,15 @@
 
 <br>
 
 ---
 
 ## Remoção
 
-É possível remover feriados específicos, após ter adicionado todos!.
+É possível remover feriados específicos, após ter adicionado todos!
 
 ```python
 from feriados_brasileiros import datas
 
 # Adiciona todos os feriados de um determinado ano
 feriados = datas.Feriados(ano=2023)
 feriados.add_all()
```

### Comparing `feriados_brasileiros-0.0.5/README.md` & `feriados_brasileiros-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 <br>
 
 ---
 
 ## Remoção
 
-É possível remover feriados específicos, após ter adicionado todos!.
+É possível remover feriados específicos, após ter adicionado todos!
 
 ```python
 from feriados_brasileiros import datas
 
 # Adiciona todos os feriados de um determinado ano
 feriados = datas.Feriados(ano=2023)
 feriados.add_all()
```

### Comparing `feriados_brasileiros-0.0.5/feriados_brasileiros/datas.py` & `feriados_brasileiros-0.0.7/feriados_brasileiros/datas.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,17 @@
         # Results
         return self.dict_tipo[nome]['data']
 
     def add_all(self):
         """
         Adiciona todos os feriados, com as descrições,
         observações e atributos "padrão"
+        :return:
         """
+
         for feriado in self.feriados_disponiveis:
             self.add(nome=feriado)
 
     def add_custom(self, nome, mes, dia, feriado, tipo, obs=None):
         """
         Adiciona um feriado "customizado".
         Ideal para feriados municipais,
```

### Comparing `feriados_brasileiros-0.0.5/feriados_brasileiros.egg-info/PKG-INFO` & `feriados_brasileiros-0.0.7/feriados_brasileiros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: feriados-brasileiros
-Version: 0.0.5
+Version: 0.0.7
 Summary: Feriados Brasileiros
 Home-page: https://github.com/michelmetran/feriados
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
-Keywords: python,dados espaciais,geoprocessamento
+Keywords: python,datas,feriados
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Portuguese
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -81,15 +81,15 @@
 
 <br>
 
 ---
 
 ## Remoção
 
-É possível remover feriados específicos, após ter adicionado todos!.
+É possível remover feriados específicos, após ter adicionado todos!
 
 ```python
 from feriados_brasileiros import datas
 
 # Adiciona todos os feriados de um determinado ano
 feriados = datas.Feriados(ano=2023)
 feriados.add_all()
```

### Comparing `feriados_brasileiros-0.0.5/setup.py` & `feriados_brasileiros-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 requirements = []
 for line in open('requirements.txt', encoding='utf-8'):
     li = line.strip()
     if not li.startswith('#'):
         requirements.append(line.rstrip())
 
-VERSION = (0, 0, 5)
+VERSION = (0, 0, 7)
 __version__ = '.'.join(map(str, VERSION))
 
 setup(
     name='feriados_brasileiros',
     version=__version__,
     author='Michel Metran',
     author_email='michelmetran@gmail.com',
     description='Feriados Brasileiros',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/michelmetran/feriados',
-    keywords='python, dados espaciais, geoprocessamento',
+    keywords='python, datas, feriados',
     # Python and Packages
     python_requires='>=3',
     install_requires=requirements,
     # Classificação
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

