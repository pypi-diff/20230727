# Comparing `tmp/pylinkandtrack-0.1.0.tar.gz` & `tmp/pylinkandtrack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinkandtrack-0.1.0.tar", max compression
+gzip compressed data, was "pylinkandtrack-0.1.1.tar", max compression
```

## Comparing `pylinkandtrack-0.1.0.tar` & `pylinkandtrack-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1078 2023-07-27 03:27:54.814886 pylinkandtrack-0.1.0/LICENSE
--rw-r--r--   0        0        0     2825 2023-07-27 03:27:54.814886 pylinkandtrack-0.1.0/README.md
--rw-r--r--   0        0        0      125 2023-07-27 03:27:54.818886 pylinkandtrack-0.1.0/linkandtrack/__init__.py
--rw-r--r--   0        0        0       66 2023-07-27 03:27:54.818886 pylinkandtrack-0.1.0/linkandtrack/client_exceptions/__init__.py
--rw-r--r--   0        0        0      137 2023-07-27 03:27:54.818886 pylinkandtrack-0.1.0/linkandtrack/client_exceptions/client_error.py
--rw-r--r--   0        0        0     3866 2023-07-27 03:27:54.818886 pylinkandtrack-0.1.0/linkandtrack/linkandtrack.py
--rw-r--r--   0        0        0     1837 2023-07-27 03:27:54.818886 pylinkandtrack-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3824 1970-01-01 00:00:00.000000 pylinkandtrack-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-27 03:33:47.015750 pylinkandtrack-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2946 2023-07-27 03:33:47.015750 pylinkandtrack-0.1.1/README.md
+-rw-r--r--   0        0        0      125 2023-07-27 03:33:47.019750 pylinkandtrack-0.1.1/linkandtrack/__init__.py
+-rw-r--r--   0        0        0       66 2023-07-27 03:33:47.019750 pylinkandtrack-0.1.1/linkandtrack/client_exceptions/__init__.py
+-rw-r--r--   0        0        0      137 2023-07-27 03:33:47.019750 pylinkandtrack-0.1.1/linkandtrack/client_exceptions/client_error.py
+-rw-r--r--   0        0        0     3866 2023-07-27 03:33:47.019750 pylinkandtrack-0.1.1/linkandtrack/linkandtrack.py
+-rw-r--r--   0        0        0     1837 2023-07-27 03:33:47.019750 pylinkandtrack-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3945 1970-01-01 00:00:00.000000 pylinkandtrack-0.1.1/PKG-INFO
```

### Comparing `pylinkandtrack-0.1.0/LICENSE` & `pylinkandtrack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylinkandtrack-0.1.0/README.md` & `pylinkandtrack-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 <header>
     <div align="center">
         <a href="https://github.com/Diaszano">
-            <img src=".github/assets/diaszano.png" alt="logo" height="300">
+            <img src="https://pylinkandtrack.readthedocs.io/en/latest/assets/logo02.png" alt="logo" height="300">
         </a>
         <h1>
             PyLinkAndTrack
         </h1>
         Interface amigável da <a href="https://linketrack.com/">Link & Track</a>: simplifica rastreamento de encomendas 
         nos Correios através de sua poderosa API.
     </div>
 </header>
 
 [![Documentation Status](https://readthedocs.org/projects/pylinkandtrack/badge/?version=latest)](https://pylinkandtrack.readthedocs.io/en/latest/?badge=latest)
 [![CI](https://github.com/Diaszano/pylinkandtrack/actions/workflows/check.yaml/badge.svg)](https://github.com/Diaszano/pylinkandtrack/actions/workflows/check.yaml)
 [![codecov](https://codecov.io/gh/Diaszano/pylinkandtrack/branch/master/graph/badge.svg?token=VfeUJcEGI7)](https://codecov.io/gh/Diaszano/pylinkandtrack)
-[![PyPI version]()]()
+[![PyPI version](https://badge.fury.io/py/pylinkandtrack.svg)](https://badge.fury.io/py/pylinkandtrack)
+
 
 ## Como instalar o projeto?
 
 Para a instalação do projeto recomendamos que use o `pipx` para fazer essa instalação:
 
 ```bash
 pipx install pylinkandtrack
```

#### html2text {}

```diff
@@ -4,32 +4,34 @@
                     Correios atravÃ©s de sua poderosa API.
  [![Documentation Status](https://readthedocs.org/projects/pylinkandtrack/
 badge/?version=latest)](https://pylinkandtrack.readthedocs.io/en/latest/
 ?badge=latest) [![CI](https://github.com/Diaszano/pylinkandtrack/actions/
 workflows/check.yaml/badge.svg)](https://github.com/Diaszano/pylinkandtrack/
 actions/workflows/check.yaml) [![codecov](https://codecov.io/gh/Diaszano/
 pylinkandtrack/branch/master/graph/badge.svg?token=VfeUJcEGI7)](https://
-codecov.io/gh/Diaszano/pylinkandtrack) [![PyPI version]()]() ## Como instalar o
-projeto? Para a instalaÃ§Ã£o do projeto recomendamos que use o `pipx` para
-fazer essa instalaÃ§Ã£o: ```bash pipx install pylinkandtrack ``` Embora isso
-seja somente uma recomenda uma recomendaÃ§Ã£o! Tu tambÃ©m podes instalar o
-projeto com o gerenciador de sua preferÃªncia. Como `pip`: ```bash pip install
-pylinkandtrack ``` ## Como usar? Este projeto se baseia nas funcionalidades
-oferecidas pela API do [Link&Track](https://linketrack.com/), que possibilita o
-rastreamento de encomendas, sujeito a limites de consultas por minuto. Em nossa
-implementaÃ§Ã£o, todas as requisiÃ§Ãµes Ã  API do [Link&Track](https://
-linketrack.com/) sÃ£o realizadas de forma assÃ­ncrona, proporcionando um
-desempenho otimizado em sua aplicaÃ§Ã£o. Abaixo, apresentaremos como Ã©
-possÃ­vel realizar o rastreamento de uma encomenda por meio da nossa interface:
-Exemplo de Rastreamento de Encomenda: ```python from asyncio import run from
-linkandtrack import LinkAndTrack async def main() -> None: # Crie o seu user e
-token no site do Link&Track # Link: https://linketrack.com/ linkandtrack =
-LinkAndTrack( user='teste', token='1abcd00b2731640e886fb41a8a9671ad14' +
-'34c599dbaa0a0de9a5aa619f29a83f', ) result = await linkandtrack.tracker
-(tracking_code='LX632045407CN') print(result) run(main()) ``` E o resultado do
-print serÃ¡ como este abaixo: ```python result = { 'codigo': 'LX632045407CN',
-'host': 'lt', 'eventos': [], 'time': 1.599, 'quantidade': 0, 'servico':
-'REMESSA INTERNACIONAL', } ``` Desta forma, ao utilizar nossa interface, vocÃª
-poderÃ¡ obter informaÃ§Ãµes sobre o rastreamento de encomendas de maneira
-eficiente e otimizada. Lembre-se de respeitar os limites de consultas por
-minuto estabelecidos pela API do [Link&Track](https://linketrack.com/) para
-garantir o bom funcionamento do serviÃ§o.
+codecov.io/gh/Diaszano/pylinkandtrack) [![PyPI version](https://badge.fury.io/
+py/pylinkandtrack.svg)](https://badge.fury.io/py/pylinkandtrack) ## Como
+instalar o projeto? Para a instalaÃ§Ã£o do projeto recomendamos que use o
+`pipx` para fazer essa instalaÃ§Ã£o: ```bash pipx install pylinkandtrack ```
+Embora isso seja somente uma recomenda uma recomendaÃ§Ã£o! Tu tambÃ©m podes
+instalar o projeto com o gerenciador de sua preferÃªncia. Como `pip`: ```bash
+pip install pylinkandtrack ``` ## Como usar? Este projeto se baseia nas
+funcionalidades oferecidas pela API do [Link&Track](https://linketrack.com/),
+que possibilita o rastreamento de encomendas, sujeito a limites de consultas
+por minuto. Em nossa implementaÃ§Ã£o, todas as requisiÃ§Ãµes Ã  API do
+[Link&Track](https://linketrack.com/) sÃ£o realizadas de forma assÃ­ncrona,
+proporcionando um desempenho otimizado em sua aplicaÃ§Ã£o. Abaixo,
+apresentaremos como Ã© possÃ­vel realizar o rastreamento de uma encomenda por
+meio da nossa interface: Exemplo de Rastreamento de Encomenda: ```python from
+asyncio import run from linkandtrack import LinkAndTrack async def main() -
+> None: # Crie o seu user e token no site do Link&Track # Link: https://
+linketrack.com/ linkandtrack = LinkAndTrack( user='teste',
+token='1abcd00b2731640e886fb41a8a9671ad14' + '34c599dbaa0a0de9a5aa619f29a83f',
+) result = await linkandtrack.tracker(tracking_code='LX632045407CN') print
+(result) run(main()) ``` E o resultado do print serÃ¡ como este abaixo:
+```python result = { 'codigo': 'LX632045407CN', 'host': 'lt', 'eventos': [],
+'time': 1.599, 'quantidade': 0, 'servico': 'REMESSA INTERNACIONAL', } ``` Desta
+forma, ao utilizar nossa interface, vocÃª poderÃ¡ obter informaÃ§Ãµes sobre o
+rastreamento de encomendas de maneira eficiente e otimizada. Lembre-se de
+respeitar os limites de consultas por minuto estabelecidos pela API do
+[Link&Track](https://linketrack.com/) para garantir o bom funcionamento do
+serviÃ§o.
```

### Comparing `pylinkandtrack-0.1.0/linkandtrack/linkandtrack.py` & `pylinkandtrack-0.1.1/linkandtrack/linkandtrack.py`

 * *Files identical despite different names*

### Comparing `pylinkandtrack-0.1.0/pyproject.toml` & `pylinkandtrack-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylinkandtrack"
-version = "0.1.0"
+version = "0.1.1"
 description = "Uma interface amigável para a API de rastreamento de encomendas dos Correios desenvolvida pela Link & Track."
 authors = ["diaszano <luucas.dsantos@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include="linkandtrack"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pylinkandtrack-0.1.0/PKG-INFO` & `pylinkandtrack-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylinkandtrack
-Version: 0.1.0
+Version: 0.1.1
 Summary: Uma interface amigável para a API de rastreamento de encomendas dos Correios desenvolvida pela Link & Track.
 License: MIT
 Author: diaszano
 Author-email: luucas.dsantos@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -20,28 +20,29 @@
 Project-URL: Código, https://github.com/Diaszano/pylinkandtrack
 Project-URL: Documentação, https://pylinkandtrack.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 
 <header>
     <div align="center">
         <a href="https://github.com/Diaszano">
-            <img src=".github/assets/diaszano.png" alt="logo" height="300">
+            <img src="https://pylinkandtrack.readthedocs.io/en/latest/assets/logo02.png" alt="logo" height="300">
         </a>
         <h1>
             PyLinkAndTrack
         </h1>
         Interface amigável da <a href="https://linketrack.com/">Link & Track</a>: simplifica rastreamento de encomendas 
         nos Correios através de sua poderosa API.
     </div>
 </header>
 
 [![Documentation Status](https://readthedocs.org/projects/pylinkandtrack/badge/?version=latest)](https://pylinkandtrack.readthedocs.io/en/latest/?badge=latest)
 [![CI](https://github.com/Diaszano/pylinkandtrack/actions/workflows/check.yaml/badge.svg)](https://github.com/Diaszano/pylinkandtrack/actions/workflows/check.yaml)
 [![codecov](https://codecov.io/gh/Diaszano/pylinkandtrack/branch/master/graph/badge.svg?token=VfeUJcEGI7)](https://codecov.io/gh/Diaszano/pylinkandtrack)
-[![PyPI version]()]()
+[![PyPI version](https://badge.fury.io/py/pylinkandtrack.svg)](https://badge.fury.io/py/pylinkandtrack)
+
 
 ## Como instalar o projeto?
 
 Para a instalação do projeto recomendamos que use o `pipx` para fazer essa instalação:
 
 ```bash
 pipx install pylinkandtrack
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylinkandtrack Version: 0.1.0 Summary: Uma
+Metadata-Version: 2.1 Name: pylinkandtrack Version: 0.1.1 Summary: Uma
 interface amigÃ¡vel para a API de rastreamento de encomendas dos Correios
 desenvolvida pela Link & Track. License: MIT Author: diaszano Author-email:
 luucas.dsantos@gmail.com Requires-Python: >=3.11,<4.0 Classifier: Development
 Status :: 4 - Beta Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Portuguese (Brazilian) Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Adaptive Technologies Classifier: Topic :: Software
@@ -18,32 +18,34 @@
                     Correios atravÃ©s de sua poderosa API.
  [![Documentation Status](https://readthedocs.org/projects/pylinkandtrack/
 badge/?version=latest)](https://pylinkandtrack.readthedocs.io/en/latest/
 ?badge=latest) [![CI](https://github.com/Diaszano/pylinkandtrack/actions/
 workflows/check.yaml/badge.svg)](https://github.com/Diaszano/pylinkandtrack/
 actions/workflows/check.yaml) [![codecov](https://codecov.io/gh/Diaszano/
 pylinkandtrack/branch/master/graph/badge.svg?token=VfeUJcEGI7)](https://
-codecov.io/gh/Diaszano/pylinkandtrack) [![PyPI version]()]() ## Como instalar o
-projeto? Para a instalaÃ§Ã£o do projeto recomendamos que use o `pipx` para
-fazer essa instalaÃ§Ã£o: ```bash pipx install pylinkandtrack ``` Embora isso
-seja somente uma recomenda uma recomendaÃ§Ã£o! Tu tambÃ©m podes instalar o
-projeto com o gerenciador de sua preferÃªncia. Como `pip`: ```bash pip install
-pylinkandtrack ``` ## Como usar? Este projeto se baseia nas funcionalidades
-oferecidas pela API do [Link&Track](https://linketrack.com/), que possibilita o
-rastreamento de encomendas, sujeito a limites de consultas por minuto. Em nossa
-implementaÃ§Ã£o, todas as requisiÃ§Ãµes Ã  API do [Link&Track](https://
-linketrack.com/) sÃ£o realizadas de forma assÃ­ncrona, proporcionando um
-desempenho otimizado em sua aplicaÃ§Ã£o. Abaixo, apresentaremos como Ã©
-possÃ­vel realizar o rastreamento de uma encomenda por meio da nossa interface:
-Exemplo de Rastreamento de Encomenda: ```python from asyncio import run from
-linkandtrack import LinkAndTrack async def main() -> None: # Crie o seu user e
-token no site do Link&Track # Link: https://linketrack.com/ linkandtrack =
-LinkAndTrack( user='teste', token='1abcd00b2731640e886fb41a8a9671ad14' +
-'34c599dbaa0a0de9a5aa619f29a83f', ) result = await linkandtrack.tracker
-(tracking_code='LX632045407CN') print(result) run(main()) ``` E o resultado do
-print serÃ¡ como este abaixo: ```python result = { 'codigo': 'LX632045407CN',
-'host': 'lt', 'eventos': [], 'time': 1.599, 'quantidade': 0, 'servico':
-'REMESSA INTERNACIONAL', } ``` Desta forma, ao utilizar nossa interface, vocÃª
-poderÃ¡ obter informaÃ§Ãµes sobre o rastreamento de encomendas de maneira
-eficiente e otimizada. Lembre-se de respeitar os limites de consultas por
-minuto estabelecidos pela API do [Link&Track](https://linketrack.com/) para
-garantir o bom funcionamento do serviÃ§o.
+codecov.io/gh/Diaszano/pylinkandtrack) [![PyPI version](https://badge.fury.io/
+py/pylinkandtrack.svg)](https://badge.fury.io/py/pylinkandtrack) ## Como
+instalar o projeto? Para a instalaÃ§Ã£o do projeto recomendamos que use o
+`pipx` para fazer essa instalaÃ§Ã£o: ```bash pipx install pylinkandtrack ```
+Embora isso seja somente uma recomenda uma recomendaÃ§Ã£o! Tu tambÃ©m podes
+instalar o projeto com o gerenciador de sua preferÃªncia. Como `pip`: ```bash
+pip install pylinkandtrack ``` ## Como usar? Este projeto se baseia nas
+funcionalidades oferecidas pela API do [Link&Track](https://linketrack.com/),
+que possibilita o rastreamento de encomendas, sujeito a limites de consultas
+por minuto. Em nossa implementaÃ§Ã£o, todas as requisiÃ§Ãµes Ã  API do
+[Link&Track](https://linketrack.com/) sÃ£o realizadas de forma assÃ­ncrona,
+proporcionando um desempenho otimizado em sua aplicaÃ§Ã£o. Abaixo,
+apresentaremos como Ã© possÃ­vel realizar o rastreamento de uma encomenda por
+meio da nossa interface: Exemplo de Rastreamento de Encomenda: ```python from
+asyncio import run from linkandtrack import LinkAndTrack async def main() -
+> None: # Crie o seu user e token no site do Link&Track # Link: https://
+linketrack.com/ linkandtrack = LinkAndTrack( user='teste',
+token='1abcd00b2731640e886fb41a8a9671ad14' + '34c599dbaa0a0de9a5aa619f29a83f',
+) result = await linkandtrack.tracker(tracking_code='LX632045407CN') print
+(result) run(main()) ``` E o resultado do print serÃ¡ como este abaixo:
+```python result = { 'codigo': 'LX632045407CN', 'host': 'lt', 'eventos': [],
+'time': 1.599, 'quantidade': 0, 'servico': 'REMESSA INTERNACIONAL', } ``` Desta
+forma, ao utilizar nossa interface, vocÃª poderÃ¡ obter informaÃ§Ãµes sobre o
+rastreamento de encomendas de maneira eficiente e otimizada. Lembre-se de
+respeitar os limites de consultas por minuto estabelecidos pela API do
+[Link&Track](https://linketrack.com/) para garantir o bom funcionamento do
+serviÃ§o.
```

