# Comparing `tmp/nsj_queue_lib-0.3.0.tar.gz` & `tmp/nsj_queue_lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_queue_lib-0.3.0.tar", last modified: Wed Jul 26 18:47:05 2023, max compression
+gzip compressed data, was "nsj_queue_lib-0.4.0.tar", last modified: Wed Jul 26 23:16:42 2023, max compression
```

## Comparing `nsj_queue_lib-0.3.0.tar` & `nsj_queue_lib-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1976 2023-07-21 22:40:47.000000 nsj_queue_lib-0.3.0/README.md
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/nsj_queue_lib/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/__init__.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/exception.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/lock_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)    10609 2023-07-26 17:36:54.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/main_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3938 2023-07-25 19:59:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/notify_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/purge_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4624 2023-07-26 17:21:11.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/queue_client.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/retry_thread.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/retry_util.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1960 2023-07-25 19:58:20.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/settings.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     9205 2023-07-26 18:03:22.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/tarefa_dao.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      368 2023-07-26 18:13:34.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_fila_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2733 2023-07-26 17:51:10.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_pub_sub_base.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      509 2023-07-25 22:43:19.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_pub_sub_teste.py
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.3.0/nsj_queue_lib/worker_webhook.py
-drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/
--rw-rw-r--   0 sergio    (1000) sergio    (1000)     2542 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/PKG-INFO
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      742 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/requires.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-26 18:47:05.000000 nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/top_level.txt
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.3.0/pyproject.toml
--rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-26 18:47:05.797599 nsj_queue_lib-0.3.0/setup.cfg
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37028 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    36463 2023-07-26 22:53:35.000000 nsj_queue_lib-0.4.0/README.md
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:16:42.485020 nsj_queue_lib-0.4.0/nsj_queue_lib/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        0 2023-07-19 18:24:10.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/__init__.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       98 2023-07-25 22:33:41.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/exception.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1090 2023-07-22 22:37:18.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/lock_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    10845 2023-07-26 20:42:13.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/main_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4814 2023-07-26 20:46:48.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/notify_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3243 2023-07-22 23:57:02.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/purge_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4670 2023-07-26 22:19:35.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/queue_client.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     4913 2023-07-22 23:57:41.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/retry_thread.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     5259 2023-07-26 18:39:19.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/retry_util.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2032 2023-07-26 20:47:28.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/settings.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     9746 2023-07-26 20:45:47.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/tarefa_dao.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1756 2023-07-26 17:45:30.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      580 2023-07-26 21:58:04.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_fila_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     3204 2023-07-26 23:08:43.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_pub_sub_base.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     1392 2023-07-26 23:11:44.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_pub_sub_teste.py
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)     2162 2023-07-26 17:51:34.000000 nsj_queue_lib-0.4.0/nsj_queue_lib/worker_webhook.py
+drwxrwxr-x   0 sergio    (1000) sergio    (1000)        0 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)    37028 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      742 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)        1 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       64 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/requires.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)       14 2023-07-26 23:16:42.000000 nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/top_level.txt
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      103 2023-07-21 22:32:09.000000 nsj_queue_lib-0.4.0/pyproject.toml
+-rw-rw-r--   0 sergio    (1000) sergio    (1000)      786 2023-07-26 23:16:42.489020 nsj_queue_lib-0.4.0/setup.cfg
```

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/lock_dao.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/lock_dao.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/main_thread.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/main_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,23 @@
     DB_USER,
     DB_PASS,
     QUEUE_NAME,
     GLOBAL_RUN,
     QUEUE_MAX_RETRY,
     QUEUE_TABLE,
     QUEUE_SUBSCRIBER_TABLE,
+    QUEUE_WAIT_NOTIFY_INTERVAL,
     logger,
 )
 
 
 class MainThread:
     def __init__(self, worker):
         self.worker = worker
+        self._notificacao_inicial = False
 
     def run(self):
         """
         Método de entrada da Thread, reponsável pelo loop infinito,
         e por abrir conexão com o BD.
         """
         logger.info("Thread de principal iniciada.")
@@ -57,17 +59,22 @@
         # Como a variável é escrita, neste escopo, é preciso declarar que estamos usando
         # a mesma variável definida fora do escopo
         global GLOBAL_RUN
 
         with conn.cursor() as curs:
             curs.execute(f"LISTEN {QUEUE_NAME}")
 
+            # Iniciando espera por notificações da fila
             logger.info(f"Esperando notificações na fila.")
             while GLOBAL_RUN:
-                if select.select([conn], [], [], 5) == ([], [], []):
+                if select.select([conn], [], [], QUEUE_WAIT_NOTIFY_INTERVAL) == (
+                    [],
+                    [],
+                    [],
+                ):
                     logger.debug(
                         "Timeout - Na espera de dados do descritor de arquivo que representa a conexão com o BD. Estratégia para evitar espera ocupada."
                     )
                 else:
                     conn.poll()
                     while conn.notifies:
                         notify = conn.notifies.pop(0)
```

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/notify_thread.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/notify_thread.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     DB_PORT,
     DB_BASE,
     DB_USER,
     DB_PASS,
     QUEUE_NAME,
     QUEUE_MINUTE_NOTIFY_THREAD,
     QUEUE_TABLE,
+    QUEUE_WAIT_NOTIFY_INTERVAL,
     GLOBAL_RUN,
     logger,
 )
 
 
 class NotifyThread(threading.Thread):
     def __init__(self):
@@ -69,30 +70,31 @@
                                 "Desistindo do notify, porque já há outro worker operando o mesmo."
                             )
                             continue
 
                         logger.info("Iniciando tratamento de notify...")
 
                         dao = TarefaDAO(db, QUEUE_TABLE)
-                        self._notify(dao)
+                        self._notify_agendadas(dao)
+                        self._notify_perdidas(dao)
 
                     finally:
                         if lock:
                             lock_dao.unlock_notify()
 
             except Exception as e:
                 logger.exception(f"Erro desconhecido: {e}", e, stack_info=True)
                 logger.info(
                     "Aguardando 5 segundos, para tentar nova conexão com o banco de dados."
                 )
                 time.sleep(5)
 
         logger.info("Thread de purge finalizada.")
 
-    def _notify(self, dao: TarefaDAO):
+    def _notify_agendadas(self, dao: TarefaDAO):
         """
         Recupera as tarefas agendadas que precisam de notify,
         marcando-as como pendentes, disparando o notify para elas.
         """
 
         agendadas, count = dao.list_agendadas_para_notificacao()
         logger.info(
@@ -115,7 +117,27 @@
                 dao.notify(QUEUE_NAME)
 
                 # Commitando transação
                 dao.db.commit()
             finally:
                 # Fazendo rollback (se houver commit anterior, não faz nada)
                 dao.db.rollback()
+
+    def _notify_perdidas(self, dao: TarefaDAO):
+        """
+        Recupera as tarefas pendentes há mais tempo que o intervalo de espera por uma notificação,
+        definido para os workers.
+
+        Isso é necessário para garantir que uma notificação não foi disparada no exato momento que
+        não havia ninguém ouvindo.
+        """
+
+        contagem, _ = dao.count_pendentes_perdidas(QUEUE_WAIT_NOTIFY_INTERVAL)
+
+        qtd = contagem[0]["qtd"]
+        logger.info(
+            f"Contando as tarefas pendentes, porém não pegas há mais tempo que o intervalo padrão de espera por notificações. Quantidade de tarefas: {qtd}"
+        )
+
+        if qtd > 0:
+            # Notificando a fila (para acordar os workers)
+            dao.notify(QUEUE_NAME)
```

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/purge_thread.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/purge_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/queue_client.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/queue_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 from nsj_sql_utils_lib.dbadapter3 import DBAdapter3
 
 from tarefa_dao import TarefaDAO
 
 
 class QueueClient:
-    def __init__(self, bd_conn, queue_table: str, queue_subscriber_table: str) -> None:
+    def __init__(
+        self,
+        bd_conn,
+        queue_table: str,
+        queue_subscriber_table: str = None,
+    ) -> None:
         self._tarefa_dao = TarefaDAO(
             DBAdapter3(bd_conn), queue_table, queue_subscriber_table
         )
 
     def _insert_task(
         self,
         origem: str,
```

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/retry_thread.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/retry_thread.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/retry_util.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/retry_util.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/settings.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 QUEUE_MINUTE_NOTIFY_THREAD = os.getenv(
     "QUEUE_MINUTE_NOTIFY_THREAD", "0,5,10,15,20,25,30,35,40,45,50,55"
 )
 
 QUEUE_PURGE_MAX_AGE = int(os.getenv("QUEUE_PURGE_MAX_AGE", "60"))
 QUEUE_PURGE_LIMIT = int(os.getenv("QUEUE_PURGE_LIMIT", "1000"))
 
+QUEUE_WAIT_NOTIFY_INTERVAL = int(os.getenv("QUEUE_PURGE_LIMIT", "30"))
+
 DEFAULT_WEBHOOK_TIMEOUT = int(os.getenv("DEFAULT_WEBHOOK_TIMEOUT", "20"))
 
 ENV = os.getenv("ENV", "DEV").upper()
 GRAFANA_URL = os.getenv("GRAFANA_URL")
 LOG_DEBUG = os.getenv("LOG_DEBUG", "False").upper() == "TRUE"
 
 # Resolvendo as constantes e variáveis globais
```

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/tarefa_dao.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/tarefa_dao.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,29 @@
             where
                 status = 'agendada'
                 and data_hora <= clock_timestamp()
             order by data_hora
         """
         return self.db.execute(sql)
 
+    def count_pendentes_perdidas(self, wait_notify_interval: int):
+        """
+        Conta as tarefas que estiverem pendentes há mais tempo que o intervalo padrão de espera pelas notificações.
+        """
+        sql = f"""
+            select
+                count(*) as qtd
+            from
+                {self.queue_table} as tarefa
+            where
+                status = 'pendente'
+                and clock_timestamp() >= data_hora + interval '{wait_notify_interval} seconds'
+        """
+        return self.db.execute(sql)
+
     def insert(self, tarefa: dict[str, any]):
         # Calculando o hash do payload
         if (
             "payload" in tarefa
             and tarefa["payload"] is not None
             and tarefa["payload"] != ""
         ):
```

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/worker_base.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_base.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/worker_pub_sub_base.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_pub_sub_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 import abc
 
 from nsj_gcf_utils.json_util import json_loads
 
 from nsj_queue_lib.exception import SubscriberNotRegistered
 from nsj_queue_lib.settings import logger
 from nsj_queue_lib.worker_base import WorkerBase
+from nsj_queue_lib.worker_webhook import WorkerWebhook
 
 
 class Subscriber:
     METHOD_SUBSCRIBER_DICT = {}
 
     def __init__(self, subscriber_id: str) -> None:
         self.subscriber_id = subscriber_id
 
     def __call__(self, func):
         Subscriber.METHOD_SUBSCRIBER_DICT[self.subscriber_id] = func
         return func
 
 
+class SubscriberWebhook:
+    METHOD_WEBHOOK_SUBSCRIBE_DICT = set()
+
+    def __init__(self, subscriber_id: str) -> None:
+        self.subscriber_id = subscriber_id
+
+    def __call__(self, obj):
+        SubscriberWebhook.METHOD_WEBHOOK_SUBSCRIBE_DICT.add(self.subscriber_id)
+        return obj
+
+
 class DeadSubscriber:
     METHOD_DEAD_SUBSCRIBER_DICT = {}
 
     def __init__(self, subscriber_id: str) -> None:
         self.subscriber_id = subscriber_id
 
     def __call__(self, func):
@@ -35,29 +47,30 @@
         logger.debug(f"Dados da tarefa: {tarefa}")
 
         # Recuperando os dados da tarefa
         payload = json_loads(payload)
         subscription = payload["subscription"]
         subscriber_id = subscription["id"]
 
-        # Recuperando a função registrada para subscriber_id
-        if subscriber_id not in Subscriber.METHOD_SUBSCRIBER_DICT:
+        # Executando o método registrado para o subscriber_id
+        if subscriber_id in Subscriber.METHOD_SUBSCRIBER_DICT:
+            return Subscriber.METHOD_SUBSCRIBER_DICT[subscriber_id](
+                self,
+                payload,
+                subscription,
+                tarefa,
+                bd_conn,
+            )
+        elif subscriber_id in SubscriberWebhook.METHOD_WEBHOOK_SUBSCRIBE_DICT:
+            return WorkerWebhook().execute(payload, tarefa, bd_conn)
+        else:
             raise SubscriberNotRegistered(
                 f"Subscriber '{subscriber_id}' não registrado."
             )
 
-        # Executando o método registrado para o subscriber_id
-        return Subscriber.METHOD_SUBSCRIBER_DICT[subscriber_id](
-            self,
-            payload,
-            subscription,
-            tarefa,
-            bd_conn,
-        )
-
     def execute_dead(self, payload: str, tarefa: dict[str, any], bd_conn) -> str:
         """
         Sobreescreva esse método, se desejar customizar o comportamento da fila de mortos.
 
         O comportamento padrão é o simples registro em log.
         """
         logger.info(f"Executando fila de mortos da tarefa PubSub de ID: {tarefa['id']}")
```

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib/worker_webhook.py` & `nsj_queue_lib-0.4.0/nsj_queue_lib/worker_webhook.py`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.3.0/nsj_queue_lib.egg-info/SOURCES.txt` & `nsj_queue_lib-0.4.0/nsj_queue_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nsj_queue_lib-0.3.0/setup.cfg` & `nsj_queue_lib-0.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nsj_queue_lib
-version = 0.3.0
+version = 0.4.0
 author = Nasajon Sistemas
 author_email = contact.dev@nasajon.com.br
 description = Biblioteca para facilitar a implementação de filas e workers.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nasajon/nsj-queue-lib
 project_urls =
```

