# Comparing `tmp/nsj_queue_lib-0.4.0.tar.gz` & `tmp/nsj_queue_lib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.4.0.tar", last modified: Wed Jul 26 23:16:42 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.5.0.tar", last modified: Wed Jul 26 23:47:33 2023, max compression
```

## Comparing `nsj_queue_lib-0.4.0.tar` & `nsj_queue_lib-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37028 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    36463 2023-07-26 22:53:35.000000 nsj_queue_lib-0.4.0/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:16:42.485020 nsj_queue_lib-0.4.0/nsj_queue_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/lock_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/main_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/notify_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/purge_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4670 2023-07-26 22:19:35.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/queue_client.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/retry_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/retry_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2032 2023-07-26 20:47:28.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/settings.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/tarefa_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_fila_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_pub_sub_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-26 23:11:44.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_pub_sub_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_webhook.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    37028 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      742 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.4.0/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:47:33.684914 nsj_queue_lib-0.5.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37264 2023-07-26 23:47:33.688914 nsj_queue_lib-0.5.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    36699 2023-07-26 23:45:45.000000 nsj_queue_lib-0.5.0/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:47:33.684914 nsj_queue_lib-0.5.0/nsj_queue_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2954 2023-07-26 23:38:36.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/db_gen.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/lock_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/main_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/notify_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/purge_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4670 2023-07-26 22:19:35.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/queue_client.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/retry_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/retry_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2032 2023-07-26 20:47:28.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/settings.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/tarefa_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/worker_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/worker_fila_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/worker_pub_sub_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-26 23:11:44.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/worker_pub_sub_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.5.0/nsj_queue_lib/worker_webhook.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:47:33.684914 nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37264 2023-07-26 23:47:33.000000 nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      768 2023-07-26 23:47:33.000000 nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-26 23:47:33.000000 nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-26 23:47:33.000000 nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-26 23:47:33.000000 nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.5.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-26 23:47:33.688914 nsj_queue_lib-0.5.0/setup.cfg
```

### Comparing `nsj_queue_lib-0.4.0/PKG-INFO` & `nsj_queue_lib-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj_queue_lib
-Version: 0.4.0
+Version: 0.5.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -49,14 +49,20 @@
 
 Nna prática, cada worker será uma máquina virtual, ou POD, rodando no ambiente de produção, com diferentes variáveis de ambiente, e diferentes entrypoints. Mas, todoo código pode estar num único repositório.
 
 ### Passos para criar um novo Worker
 
 1. Adicionar a biblioteca `nsj-queue-lib` como dependencia de seu projeto (disponível no pypi.org).
 2. Criar a estrutura de banco, que deve ser similar ao exemplo contido no arquivo ```database/sump/0001 - fila teste.sql```, bastando renomear a tabela de fila, a tabela de assinantes (caso seja usada), os índices, a trigger, a função da trigger e o nome do canal que sofre notificação (pela trigger).
+   1. Para facilitar esse passo, foi implementado um utilitário na biblioteca, que pode ser executado por meio do comando a seguir (que imprime o modelo de banco gerado):
+
+```sh
+python -m nsj_queue_lib.db_gen <schema> <nome_fila>
+```
+
 3. Estender alguma das classes base de worker (no caso de webhooks, não é preciso estender nenhuma classe), e implementar o código de processamento das tarefas.
    1. Pode-se usar os módulos `woker_fila_teste.py` e `worker_pub_sub_teste.py` como exmplos para esse passo.
 4. Definir uma imagem com o entrypoint apontando para o worker implementado (ou para o worker de webhook), conforme exemplificado no arquivo `docker-compose.yml`.
 5. Executar o worker.
 6. Inserir tarefas na fila.
    1. Sugere-se utiliza o módulo `queue_client.py` para facilitar a inserção de tarefas na fila, mas, o insert direto na tabela de filas também funcionará (devendo-se respeitar o significado de cada coluna, conforme explicado em sessão à frente).
```

### Comparing `nsj_queue_lib-0.4.0/README.md` & `nsj_queue_lib-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 
 Nna prática, cada worker será uma máquina virtual, ou POD, rodando no ambiente de produção, com diferentes variáveis de ambiente, e diferentes entrypoints. Mas, todoo código pode estar num único repositório.
 
 ### Passos para criar um novo Worker
 
 1. Adicionar a biblioteca `nsj-queue-lib` como dependencia de seu projeto (disponível no pypi.org).
 2. Criar a estrutura de banco, que deve ser similar ao exemplo contido no arquivo ```database/sump/0001 - fila teste.sql```, bastando renomear a tabela de fila, a tabela de assinantes (caso seja usada), os índices, a trigger, a função da trigger e o nome do canal que sofre notificação (pela trigger).
+   1. Para facilitar esse passo, foi implementado um utilitário na biblioteca, que pode ser executado por meio do comando a seguir (que imprime o modelo de banco gerado):
+
+```sh
+python -m nsj_queue_lib.db_gen <schema> <nome_fila>
+```
+
 3. Estender alguma das classes base de worker (no caso de webhooks, não é preciso estender nenhuma classe), e implementar o código de processamento das tarefas.
    1. Pode-se usar os módulos `woker_fila_teste.py` e `worker_pub_sub_teste.py` como exmplos para esse passo.
 4. Definir uma imagem com o entrypoint apontando para o worker implementado (ou para o worker de webhook), conforme exemplificado no arquivo `docker-compose.yml`.
 5. Executar o worker.
 6. Inserir tarefas na fila.
    1. Sugere-se utiliza o módulo `queue_client.py` para facilitar a inserção de tarefas na fila, mas, o insert direto na tabela de filas também funcionará (devendo-se respeitar o significado de cada coluna, conforme explicado em sessão à frente).
```

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/lock_dao.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/lock_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/main_thread.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/main_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/notify_thread.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/notify_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/purge_thread.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/purge_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/queue_client.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/queue_client.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/retry_thread.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/retry_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/retry_util.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/retry_util.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/settings.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/tarefa_dao.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/tarefa_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_base.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/worker_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_fila_teste.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/worker_fila_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_pub_sub_base.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/worker_pub_sub_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_pub_sub_teste.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/worker_pub_sub_teste.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_webhook.py` & `nsj_queue_lib-0.5.0/nsj_queue_lib/worker_webhook.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/PKG-INFO` & `nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-queue-lib
-Version: 0.4.0
+Version: 0.5.0
 Summary: Biblioteca para facilitar a implementação de filas e workers.
 Home-page: https://github.com/Nasajon/nsj-queue-lib
 Author: Nasajon Sistemas
 Author-email: contact.dev@nasajon.com.br
 Project-URL: Source, https://github.com/Nasajon/nsj-queue-lib
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -49,14 +49,20 @@
 
 Nna prática, cada worker será uma máquina virtual, ou POD, rodando no ambiente de produção, com diferentes variáveis de ambiente, e diferentes entrypoints. Mas, todoo código pode estar num único repositório.
 
 ### Passos para criar um novo Worker
 
 1. Adicionar a biblioteca `nsj-queue-lib` como dependencia de seu projeto (disponível no pypi.org).
 2. Criar a estrutura de banco, que deve ser similar ao exemplo contido no arquivo ```database/sump/0001 - fila teste.sql```, bastando renomear a tabela de fila, a tabela de assinantes (caso seja usada), os índices, a trigger, a função da trigger e o nome do canal que sofre notificação (pela trigger).
+   1. Para facilitar esse passo, foi implementado um utilitário na biblioteca, que pode ser executado por meio do comando a seguir (que imprime o modelo de banco gerado):
+
+```sh
+python -m nsj_queue_lib.db_gen <schema> <nome_fila>
+```
+
 3. Estender alguma das classes base de worker (no caso de webhooks, não é preciso estender nenhuma classe), e implementar o código de processamento das tarefas.
    1. Pode-se usar os módulos `woker_fila_teste.py` e `worker_pub_sub_teste.py` como exmplos para esse passo.
 4. Definir uma imagem com o entrypoint apontando para o worker implementado (ou para o worker de webhook), conforme exemplificado no arquivo `docker-compose.yml`.
 5. Executar o worker.
 6. Inserir tarefas na fila.
    1. Sugere-se utiliza o módulo `queue_client.py` para facilitar a inserção de tarefas na fila, mas, o insert direto na tabela de filas também funcionará (devendo-se respeitar o significado de cada coluna, conforme explicado em sessão à frente).
```

### Comparing `nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/SOURCES.txt` & `nsj_queue_lib-0.5.0/nsj_queue_lib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 setup.cfg
 ./nsj_queue_lib/__init__.py
+./nsj_queue_lib/db_gen.py
 ./nsj_queue_lib/exception.py
 ./nsj_queue_lib/lock_dao.py
 ./nsj_queue_lib/main_thread.py
 ./nsj_queue_lib/notify_thread.py
 ./nsj_queue_lib/purge_thread.py
 ./nsj_queue_lib/queue_client.py
 ./nsj_queue_lib/retry_thread.py
```

### Comparing `nsj_queue_lib-0.4.0/setup.cfg` & `nsj_queue_lib-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.4.0
+version = 0.5.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls =
```

