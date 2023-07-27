# Comparing `tmp/neoscr-2.0.0.tar.gz` & `tmp/neoscr-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neoscr-2.0.0.tar", last modified: Sun Jul 23 20:53:54 2023, max compression
+gzip compressed data, was "neoscr-2.1.0.tar", last modified: Thu Jul 27 20:00:49 2023, max compression
```

## Comparing `neoscr-2.0.0.tar` & `neoscr-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-23 20:53:54.626762 neoscr-2.0.0/
--rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-01-20 02:50:04.000000 neoscr-2.0.0/LICENSE
--rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-01-20 02:50:04.000000 neoscr-2.0.0/MANIFEST.in
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4039 2023-07-23 20:53:54.626615 neoscr-2.0.0/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)     3245 2023-07-23 20:45:11.000000 neoscr-2.0.0/README.md
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-23 20:53:54.624801 neoscr-2.0.0/neoscr/
--rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-07-23 20:50:53.000000 neoscr-2.0.0/neoscr/__init__.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2083 2023-07-23 20:50:53.000000 neoscr-2.0.0/neoscr/_modidx.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     2024 2023-07-23 20:50:53.000000 neoscr-2.0.0/neoscr/cli.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)     5965 2023-07-23 20:50:53.000000 neoscr-2.0.0/neoscr/core.py
--rw-r--r--   0 joaonogueira   (501) staff       (20)      834 2023-07-23 20:50:53.000000 neoscr-2.0.0/neoscr/utils.py
-drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-23 20:53:54.626386 neoscr-2.0.0/neoscr.egg-info/
--rw-r--r--   0 joaonogueira   (501) staff       (20)     4039 2023-07-23 20:53:54.000000 neoscr-2.0.0/neoscr.egg-info/PKG-INFO
--rw-r--r--   0 joaonogueira   (501) staff       (20)      344 2023-07-23 20:53:54.000000 neoscr-2.0.0/neoscr.egg-info/SOURCES.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-07-23 20:53:54.000000 neoscr-2.0.0/neoscr.egg-info/dependency_links.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)      173 2023-07-23 20:53:54.000000 neoscr-2.0.0/neoscr.egg-info/entry_points.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-03-10 22:07:48.000000 neoscr-2.0.0/neoscr.egg-info/not-zip-safe
--rw-r--r--   0 joaonogueira   (501) staff       (20)       46 2023-07-23 20:53:54.000000 neoscr-2.0.0/neoscr.egg-info/requires.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-07-23 20:53:54.000000 neoscr-2.0.0/neoscr.egg-info/top_level.txt
--rw-r--r--   0 joaonogueira   (501) staff       (20)      999 2023-07-23 20:46:56.000000 neoscr-2.0.0/settings.ini
--rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-07-23 20:53:54.626825 neoscr-2.0.0/setup.cfg
--rw-rw-r--   0 joaonogueira   (501) staff       (20)     2560 2023-01-20 02:50:04.000000 neoscr-2.0.0/setup.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-27 20:00:49.580377 neoscr-2.1.0/
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)    11337 2023-01-20 02:50:04.000000 neoscr-2.1.0/LICENSE
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)      111 2023-01-20 02:50:04.000000 neoscr-2.1.0/MANIFEST.in
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     4752 2023-07-27 20:00:49.580204 neoscr-2.1.0/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     3958 2023-07-27 19:54:52.000000 neoscr-2.1.0/README.md
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-27 20:00:49.578327 neoscr-2.1.0/neoscr/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       22 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/__init__.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     2339 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/_modidx.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     2024 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/cli.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     8431 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/core.py
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     3773 2023-07-27 19:55:21.000000 neoscr-2.1.0/neoscr/utils.py
+drwxr-xr-x   0 joaonogueira   (501) staff       (20)        0 2023-07-27 20:00:49.579985 neoscr-2.1.0/neoscr.egg-info/
+-rw-r--r--   0 joaonogueira   (501) staff       (20)     4752 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/PKG-INFO
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      344 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/SOURCES.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/dependency_links.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      173 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/entry_points.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        1 2023-03-10 22:07:48.000000 neoscr-2.1.0/neoscr.egg-info/not-zip-safe
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       46 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/requires.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)        7 2023-07-27 20:00:49.000000 neoscr-2.1.0/neoscr.egg-info/top_level.txt
+-rw-r--r--   0 joaonogueira   (501) staff       (20)      999 2023-07-27 19:55:21.000000 neoscr-2.1.0/settings.ini
+-rw-r--r--   0 joaonogueira   (501) staff       (20)       38 2023-07-27 20:00:49.580440 neoscr-2.1.0/setup.cfg
+-rw-rw-r--   0 joaonogueira   (501) staff       (20)     2560 2023-01-20 02:50:04.000000 neoscr-2.1.0/setup.py
```

### Comparing `neoscr-2.0.0/LICENSE` & `neoscr-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neoscr-2.0.0/PKG-INFO` & `neoscr-2.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoscr
-Version: 2.0.0
+Version: 2.1.0
 Summary: Wrapper to query the SCR api
 Home-page: https://github.com/datarisk-io/neoscr
 Author: João Nogueira
 Author-email: joao.nogueira@datarisk.io
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -50,47 +50,52 @@
 )
 ```
 
 <div>
 
 > **Warning**
 >
-> You should have the credentials to access the SCR API stored in your
-> OS environment variables.
+> You have the choice to not pass the API credentials on the
+> [`ConsultaSCR`](https://datarisk-io.github.io/neoscr/core.html#consultascr)
+> instantiation, but for that you should have the credentials to access
+> the SCR API stored in your OS environment variables.
 
 </div>
 
 ``` python
 cpf = "867.168.046-09" # fake cpf
 ano = 2022
 mes = 12
 
-# retorna dois dataframes
-df_cpf_traduzido, df_cpf_modalidade = scr.get_cpf_data(cpf, ano, mes)
+# retorna três dataframes
+df_cpf_traduzido, df_cpf_modalidade, df_cpf_resumo_lista_das_operacoes = scr.get_cpf_data(cpf, ano, mes)
 ```
 
 <div>
 
 > **Note**
 >
 > `neoscr` will save each request made into `.neoscr` folder located at
 > your home directory.
 >
 > For the example above, the saved file will be:
-> `~/.neoscr/00000000000_2022_12.json`
+> `~/.neoscr/86716804609_2022_12.json`
+>
+> Next time you do the same request, it will load from the local
+> storage.
 
 </div>
 
 ``` python
 cnpj = "79.322.561/0001-67" # fake cnpj
 ano = 2022
 mes = 12
 
-# retorna dois dataframes
-df_cnpj_traduzido, df_cnpj_modalidade = scr.get_cnpj_data(cnpj, ano, mes)
+# retorna três dataframes
+df_cnpj_traduzido, df_cnpj_modalidade, df_cnpj_resumo_lista_das_operacoes = scr.get_cnpj_data(cnpj, ano, mes)
 ```
 
 # Batch Query
 
 Execute the code below to query a list of cpfs or cnpjs (under
 modification) and download the data
 
@@ -112,20 +117,15 @@
 from neoscr.utils import let_only_digits
 
 # carregando a lista de cpfs
 df = pd.read_csv("dataset.csv")
 lista_de_cpfs = df['cpf'].tolist()
 
 # instanciando o objeto ConsultaSCR
-scr = ConsultaSCR(
-    user=os.environ["SCR_USER"],
-    password=os.environ["SCR_PASSWORD"],
-    code=os.environ["SCR_CODE"],
-    api_key=os.environ["SCR_API_KEY"]
-)
+scr = ConsultaSCR()
 
 # instanciando o objeto logger
 logger = logging.getLogger('database_updater')
 logger.setLevel(logging.DEBUG)
 
 # criando o file handler
 file_handler = logging.FileHandler('querylog.log')
@@ -135,18 +135,19 @@
 logger.addHandler(file_handler)
 
 # iterando sobre a lista de cpfs e enriquecendo
 ano = 2022
 mes = 12
 for cpf in tqdm(lista_de_cpfs):
     try:
-        df_traduzido, df_modalidade = scr.get_cpf_data(cpf, ano, mes)                               
+        df_traduzido, df_modalidade, df_cnpj_resumo_lista_das_operacoes = scr.get_cpf_data(cpf, ano, mes)                               
         cpf_only_digits = let_only_digits(cpf)
         df_traduzido.to_csv(f"data/scr/raw/{cpf_only_digits}_traduzido.csv", index=False)
         df_modalidade.to_csv(f"data/scr/raw/{cpf_only_digits}_modalidade.csv", index=False)
+        df_cnpj_resumo_lista_das_operacoes.to_csv(f"data/scr/raw/{cpf_only_digits}_resumo_lista_das_operacoes.csv", index=False)
     except:
         logger.error(f"Erro no CPF {cpf}")
         continue
 ```
 
 After download the data, you may want to get all the raw data together
 in one big table:
@@ -160,10 +161,16 @@
         df_traduzido_full = pd.concat([df_traduzido_full, df_traduzido])
 
 df_modalidade_full = pd.DataFrame()
 for file in os.listdir(".data/scr/raw"):
     if file.endswith("_modalidade.csv"):
         df_modalidade = pd.read_csv(f"data/scr/raw/{file}")
         df_modalidade_full = pd.concat([df_modalidade_full, df_modalidade])
+
+df_cnpj_resumo_lista_das_operacoes_full = pd.DataFrame()
+for file in os.listdir("data/scr/raw/"):
+    if file.endswith("_resumo_lista_das_operacoes.csv"):
+        df_cnpj_resumo_lista_das_operacoes = pd.read_csv(f"data/scr/raw/{file}")
+        df_cnpj_resumo_lista_das_operacoes_full = pd.concat([df_cnpj_resumo_lista_das_operacoes_full, df_cnpj_resumo_lista_das_operacoes])
 ```
```

### Comparing `neoscr-2.0.0/neoscr/_modidx.py` & `neoscr-2.1.0/neoscr/_modidx.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
   'syms': { 'neoscr.cli': { 'neoscr.cli.build_package': ('cli.html#build_package', 'neoscr/cli.py'),
                             'neoscr.cli.consulta_scr': ('cli.html#consulta_scr', 'neoscr/cli.py'),
                             'neoscr.cli.install_package': ('cli.html#install_package', 'neoscr/cli.py')},
             'neoscr.core': { 'neoscr.core.ConsultaSCR': ('core.html#consultascr', 'neoscr/core.py'),
                              'neoscr.core.ConsultaSCR.__init__': ('core.html#consultascr.__init__', 'neoscr/core.py'),
                              'neoscr.core.ConsultaSCR._get_resumo_cliente_traduzido': ( 'core.html#consultascr._get_resumo_cliente_traduzido',
                                                                                         'neoscr/core.py'),
+                             'neoscr.core.ConsultaSCR._get_resumo_lista_das_operacoes': ( 'core.html#consultascr._get_resumo_lista_das_operacoes',
+                                                                                          'neoscr/core.py'),
                              'neoscr.core.ConsultaSCR._get_resumo_modalidade': ( 'core.html#consultascr._get_resumo_modalidade',
                                                                                  'neoscr/core.py'),
                              'neoscr.core.ConsultaSCR._request': ('core.html#consultascr._request', 'neoscr/core.py'),
                              'neoscr.core.ConsultaSCR.get_cnpj_data': ('core.html#consultascr.get_cnpj_data', 'neoscr/core.py'),
                              'neoscr.core.ConsultaSCR.get_cpf_data': ('core.html#consultascr.get_cpf_data', 'neoscr/core.py')},
             'neoscr.utils': { 'neoscr.utils.fill_zeros': ('utils.html#fill_zeros', 'neoscr/utils.py'),
                               'neoscr.utils.format_cnpj': ('utils.html#format_cnpj', 'neoscr/utils.py'),
```

### Comparing `neoscr-2.0.0/neoscr/cli.py` & `neoscr-2.1.0/neoscr/cli.py`

 * *Files identical despite different names*

### Comparing `neoscr-2.0.0/neoscr/core.py` & `neoscr-2.1.0/neoscr/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['ConsultaSCR']
 
 # %% ../nbs/00_core.ipynb 3
+import os
 import json
 import requests
 import pandas as pd
 from typing import Tuple
 from pathlib import Path
 from datetime import datetime
 
 from .utils import let_only_digits
+from .utils import codigos_vencimentos
 
 # %% ../nbs/00_core.ipynb 4
 class ConsultaSCR:
     def __init__(self, 
-                 user: str,     # SCR user
-                 password: str, # SCR password
-                 code: str,     # SCR code
-                 api_key: str   # SCR api key
+                 user: str = None,     # SCR user
+                 password: str = None, # SCR password
+                 code: str = None,     # SCR code
+                 api_key: str = None  # SCR api key
     ):
         "Class to query SCR"
-        self.user = user
-        self.password = password
-        self.code = code                                                
-        self.key = api_key
+        self.user = os.environ['SCR_USER'] if user is None else user
+        self.password = os.environ['SCR_PASSWORD'] if password is None else password
+        self.code = os.environ['SCR_CODE'] if code is None else code
+        self.key = os.environ['SCR_API_KEY'] if api_key is None else api_key
         self.headers = {'Content-Type': 'application/json'}
         self.url = "https://bmpdigital.moneyp.com.br/api/BMPDigital/ConsultaSCR"
         self.params = {
             "auth": {
                 "Usuario": self.user,
                 "Senha": self.password,
                 "CodigoParametro": self.code,
@@ -82,43 +84,73 @@
 
         df = pd.DataFrame(response_json.get("ResumoDoClienteTraduzido"), columns=response_json.get("ResumoDoClienteTraduzido").keys(), index = [0])
         df.insert(0, "doc", kwargs.get("doc"))
         df.insert(1, "data_consulta", kwargs.get("data_consulta"))
         df.insert(2, "mes_referencia", kwargs.get("mes_referencia"))
         df.insert(3, "msg", response_json.get("MensagemOperador"))
         return df
-    
+
+
     def _get_resumo_modalidade(self, 
                                response_json: dict, # Response from the SCR API 
                                **kwargs: dict       # Keyword arguments
     ) -> pd.DataFrame:
         "Return a DataFrame with the modalities client summary"
 
         df = pd.DataFrame(response_json.get("ResumoModalidade"))
         df.insert(0, "doc", kwargs.get("doc"))
         df.insert(1, "data_consulta", kwargs.get("data_consulta"))
         df.insert(2, "mes_referencia", kwargs.get("mes_referencia"))
         return df
 
+
+    def _get_resumo_lista_das_operacoes(self,
+                                        response_json: dict, # Response from the SCR API 
+                                        **kwargs: dict       # Keyword arguments
+    ) -> pd.DataFrame:
+        df_aux = pd.DataFrame(response_json.get('ResumoDoCliente').get('ListaDeResumoDasOperacoes'))
+        df_aux_exploded = df_aux.explode('ListaDeVencimentos').reset_index(drop=True)
+        df = pd.concat([
+                df_aux_exploded[['Modalidade', 'VariacaoCambial']],
+                df_aux_exploded['ListaDeVencimentos'].apply(pd.Series)
+            ], axis=1)
+        df.insert(0, "doc", kwargs.get("doc"))
+        df.insert(1, "data_consulta", kwargs.get("data_consulta"))
+        df.insert(2, "mes_referencia", kwargs.get("mes_referencia"))
+        df = pd.merge(df, codigos_vencimentos, on='CodigoVencimento', how='left').filter([
+                                                                                        'doc',
+                                                                                        'data_consulta',
+                                                                                        'mes_referencia',
+                                                                                        'Modalidade',
+                                                                                        'VariacaoCambial',
+                                                                                        'CodigoVencimento',
+                                                                                        'Descrição',
+                                                                                        'ValorVencimento',
+                                                                                        'ValorVencimentoSpecified'])
+
+        return df
+
+
     def get_cpf_data(self, 
                      cpf: str,      # CPF
                      ano: int,      # Year to be consulted. Ex: 2022
                      mes: int       # Month to be consulted. Ex: 8, 10
     ) -> Tuple[pd.DataFrame, pd.DataFrame]:
         "Query CPFs and return a tuple of DataFrames: (df_cpf_resumo_cliente_traduzido, df_cpf_resumo_modalidade)"
         
         data_consulta = datetime.today().strftime("%d/%m/%Y")
         response_json = self._request(cpf, ano, mes)
         if response_json.get("Erro"):
             raise Exception(response_json.get("Msg").strip() + f": {cpf}")
         
         df_traduzido = self._get_resumo_cliente_traduzido(response_json, doc=cpf, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         df_modalidade = self._get_resumo_modalidade(response_json, doc=cpf, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
+        df_resumo_lista_das_operacoes = self._get_resumo_lista_das_operacoes(response_json, doc=cpf, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         
-        return df_traduzido, df_modalidade
+        return df_traduzido, df_modalidade, df_resumo_lista_das_operacoes
 
     
     def get_cnpj_data(self, 
                       cnpj: str,     # CNPJ
                       ano: int,      # Year to be consulted. Ex: 2022
                       mes: int       # Month to be consulted. Ex: 8, 10
     ) -> Tuple[pd.DataFrame, pd.DataFrame]:
@@ -126,9 +158,10 @@
         data_consulta = datetime.today().strftime("%d/%m/%Y")
         response_json = self._request(cnpj, ano, mes)
         if response_json.get("Erro"):
             raise Exception(response_json.get("Msg").strip() + f": {cnpj}")
         
         df_traduzido = self._get_resumo_cliente_traduzido(response_json, doc=cnpj, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
         df_modalidade = self._get_resumo_modalidade(response_json, doc=cnpj, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
+        df_resumo_lista_das_operacoes = self._get_resumo_lista_das_operacoes(response_json, doc=cnpj, data_consulta=data_consulta, mes_referencia=f"{ano}{mes:02d}")
 
-        return df_traduzido, df_modalidade
+        return df_traduzido, df_modalidade, df_resumo_lista_das_operacoes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neoscr-2.0.0/neoscr.egg-info/PKG-INFO` & `neoscr-2.1.0/neoscr.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neoscr
-Version: 2.0.0
+Version: 2.1.0
 Summary: Wrapper to query the SCR api
 Home-page: https://github.com/datarisk-io/neoscr
 Author: João Nogueira
 Author-email: joao.nogueira@datarisk.io
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -50,47 +50,52 @@
 )
 ```
 
 <div>
 
 > **Warning**
 >
-> You should have the credentials to access the SCR API stored in your
-> OS environment variables.
+> You have the choice to not pass the API credentials on the
+> [`ConsultaSCR`](https://datarisk-io.github.io/neoscr/core.html#consultascr)
+> instantiation, but for that you should have the credentials to access
+> the SCR API stored in your OS environment variables.
 
 </div>
 
 ``` python
 cpf = "867.168.046-09" # fake cpf
 ano = 2022
 mes = 12
 
-# retorna dois dataframes
-df_cpf_traduzido, df_cpf_modalidade = scr.get_cpf_data(cpf, ano, mes)
+# retorna três dataframes
+df_cpf_traduzido, df_cpf_modalidade, df_cpf_resumo_lista_das_operacoes = scr.get_cpf_data(cpf, ano, mes)
 ```
 
 <div>
 
 > **Note**
 >
 > `neoscr` will save each request made into `.neoscr` folder located at
 > your home directory.
 >
 > For the example above, the saved file will be:
-> `~/.neoscr/00000000000_2022_12.json`
+> `~/.neoscr/86716804609_2022_12.json`
+>
+> Next time you do the same request, it will load from the local
+> storage.
 
 </div>
 
 ``` python
 cnpj = "79.322.561/0001-67" # fake cnpj
 ano = 2022
 mes = 12
 
-# retorna dois dataframes
-df_cnpj_traduzido, df_cnpj_modalidade = scr.get_cnpj_data(cnpj, ano, mes)
+# retorna três dataframes
+df_cnpj_traduzido, df_cnpj_modalidade, df_cnpj_resumo_lista_das_operacoes = scr.get_cnpj_data(cnpj, ano, mes)
 ```
 
 # Batch Query
 
 Execute the code below to query a list of cpfs or cnpjs (under
 modification) and download the data
 
@@ -112,20 +117,15 @@
 from neoscr.utils import let_only_digits
 
 # carregando a lista de cpfs
 df = pd.read_csv("dataset.csv")
 lista_de_cpfs = df['cpf'].tolist()
 
 # instanciando o objeto ConsultaSCR
-scr = ConsultaSCR(
-    user=os.environ["SCR_USER"],
-    password=os.environ["SCR_PASSWORD"],
-    code=os.environ["SCR_CODE"],
-    api_key=os.environ["SCR_API_KEY"]
-)
+scr = ConsultaSCR()
 
 # instanciando o objeto logger
 logger = logging.getLogger('database_updater')
 logger.setLevel(logging.DEBUG)
 
 # criando o file handler
 file_handler = logging.FileHandler('querylog.log')
@@ -135,18 +135,19 @@
 logger.addHandler(file_handler)
 
 # iterando sobre a lista de cpfs e enriquecendo
 ano = 2022
 mes = 12
 for cpf in tqdm(lista_de_cpfs):
     try:
-        df_traduzido, df_modalidade = scr.get_cpf_data(cpf, ano, mes)                               
+        df_traduzido, df_modalidade, df_cnpj_resumo_lista_das_operacoes = scr.get_cpf_data(cpf, ano, mes)                               
         cpf_only_digits = let_only_digits(cpf)
         df_traduzido.to_csv(f"data/scr/raw/{cpf_only_digits}_traduzido.csv", index=False)
         df_modalidade.to_csv(f"data/scr/raw/{cpf_only_digits}_modalidade.csv", index=False)
+        df_cnpj_resumo_lista_das_operacoes.to_csv(f"data/scr/raw/{cpf_only_digits}_resumo_lista_das_operacoes.csv", index=False)
     except:
         logger.error(f"Erro no CPF {cpf}")
         continue
 ```
 
 After download the data, you may want to get all the raw data together
 in one big table:
@@ -160,10 +161,16 @@
         df_traduzido_full = pd.concat([df_traduzido_full, df_traduzido])
 
 df_modalidade_full = pd.DataFrame()
 for file in os.listdir(".data/scr/raw"):
     if file.endswith("_modalidade.csv"):
         df_modalidade = pd.read_csv(f"data/scr/raw/{file}")
         df_modalidade_full = pd.concat([df_modalidade_full, df_modalidade])
+
+df_cnpj_resumo_lista_das_operacoes_full = pd.DataFrame()
+for file in os.listdir("data/scr/raw/"):
+    if file.endswith("_resumo_lista_das_operacoes.csv"):
+        df_cnpj_resumo_lista_das_operacoes = pd.read_csv(f"data/scr/raw/{file}")
+        df_cnpj_resumo_lista_das_operacoes_full = pd.concat([df_cnpj_resumo_lista_das_operacoes_full, df_cnpj_resumo_lista_das_operacoes])
 ```
```

### Comparing `neoscr-2.0.0/settings.ini` & `neoscr-2.1.0/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = neoscr
 lib_name = neoscr
-version = 2.0.0
+version = 2.1.0
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = neoscr
 nbs_path = nbs
 recursive = True
```

### Comparing `neoscr-2.0.0/setup.py` & `neoscr-2.1.0/setup.py`

 * *Files identical despite different names*

