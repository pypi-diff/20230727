# Comparing `tmp/pg_save-0.2.0.tar.gz` & `tmp/pg_save-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_save-0.2.0.tar", last modified: Thu Mar 23 16:06:33 2023, max compression
+gzip compressed data, was "pg_save-0.3.0.tar", max compression
```

## Comparing `pg_save-0.2.0.tar` & `pg_save-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     8893 2023-03-23 16:06:33.104511 pg_save-0.2.0/PKG-INFO
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     8338 2022-12-09 17:32:14.000000 pg_save-0.2.0/README.md
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/pg_save/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)      485 2023-03-23 15:32:08.000000 pg_save-0.2.0/pg_save/__init__.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)    12192 2023-03-23 15:59:06.000000 pg_save-0.2.0/pg_save/__main__.py
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/pg_save/database_description/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     4596 2023-03-23 15:57:12.000000 pg_save-0.2.0/pg_save/database_description/__init__.py
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/pg_save/exceptions/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)      341 2023-03-23 15:44:36.000000 pg_save-0.2.0/pg_save/exceptions/__init__.py
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/pg_save/export/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     5259 2023-03-23 15:55:29.000000 pg_save-0.2.0/pg_save/export/__init__.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)      978 2023-03-23 15:55:29.000000 pg_save-0.2.0/pg_save/export/csv.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)       75 2023-03-23 14:10:29.000000 pg_save-0.2.0/pg_save/export/default_crs.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     1216 2023-03-23 15:55:29.000000 pg_save-0.2.0/pg_save/export/excel.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     3618 2023-03-23 15:55:29.000000 pg_save-0.2.0/pg_save/export/geojson.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     2405 2023-03-23 15:55:29.000000 pg_save-0.2.0/pg_save/export/json.py
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/pg_save/query/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     5196 2023-03-23 15:55:29.000000 pg_save-0.2.0/pg_save/query/__init__.py
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/pg_save/utils/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)      605 2023-03-23 15:44:36.000000 pg_save-0.2.0/pg_save/utils/__init__.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     2052 2023-03-23 15:55:29.000000 pg_save-0.2.0/pg_save/utils/dotenv.py
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     4287 2023-03-23 15:59:30.000000 pg_save-0.2.0/pg_save/utils/interactive.py
-drwxrwxr-x   0 kanu      (1000) kanu      (1000)        0 2023-03-23 16:06:33.104511 pg_save-0.2.0/pg_save.egg-info/
--rw-rw-r--   0 kanu      (1000) kanu      (1000)     8893 2023-03-23 16:06:33.000000 pg_save-0.2.0/pg_save.egg-info/PKG-INFO
--rw-rw-r--   0 kanu      (1000) kanu      (1000)      547 2023-03-23 16:06:33.000000 pg_save-0.2.0/pg_save.egg-info/SOURCES.txt
--rw-rw-r--   0 kanu      (1000) kanu      (1000)        1 2023-03-23 16:06:33.000000 pg_save-0.2.0/pg_save.egg-info/dependency_links.txt
--rw-rw-r--   0 kanu      (1000) kanu      (1000)      107 2023-03-23 16:06:33.000000 pg_save-0.2.0/pg_save.egg-info/requires.txt
--rw-rw-r--   0 kanu      (1000) kanu      (1000)        8 2023-03-23 16:06:33.000000 pg_save-0.2.0/pg_save.egg-info/top_level.txt
--rw-rw-r--   0 kanu      (1000) kanu      (1000)      996 2023-03-23 16:01:29.000000 pg_save-0.2.0/pyproject.toml
--rw-rw-r--   0 kanu      (1000) kanu      (1000)       38 2023-03-23 16:06:33.104511 pg_save-0.2.0/setup.cfg
+-rw-r--r--   0        0        0     1070 2023-07-27 14:58:46.717392 pg_save-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9040 2023-07-27 14:54:33.982038 pg_save-0.3.0/README.md
+-rw-r--r--   0        0        0      251 2023-07-27 13:25:00.040219 pg_save-0.3.0/pg_save/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-27 13:25:24.683419 pg_save-0.3.0/pg_save/__main__.py
+-rw-r--r--   0        0        0      618 2023-07-27 13:25:24.695418 pg_save-0.3.0/pg_save/cli/__init__.py
+-rw-r--r--   0        0        0      850 2023-07-27 14:22:21.739561 pg_save-0.3.0/pg_save/cli/describe_table.py
+-rw-r--r--   0        0        0     1827 2023-07-27 13:28:01.498381 pg_save-0.3.0/pg_save/cli/group.py
+-rw-r--r--   0        0        0     5833 2023-07-27 13:43:07.493623 pg_save-0.3.0/pg_save/cli/interactive.py
+-rw-r--r--   0        0        0      609 2023-07-27 14:39:50.413115 pg_save-0.3.0/pg_save/cli/list_tables.py
+-rw-r--r--   0        0        0     3522 2023-07-27 13:57:01.111348 pg_save-0.3.0/pg_save/cli/query.py
+-rw-r--r--   0        0        0     1770 2023-07-27 13:56:56.755434 pg_save-0.3.0/pg_save/cli/select_table.py
+-rw-r--r--   0        0        0      172 2023-07-27 12:20:55.650666 pg_save-0.3.0/pg_save/database_description/__init__.py
+-rw-r--r--   0        0        0     3164 2023-07-27 14:21:00.426265 pg_save-0.3.0/pg_save/database_description/table_info.py
+-rw-r--r--   0        0        0     1884 2023-07-27 14:20:47.110717 pg_save-0.3.0/pg_save/database_description/tables_list.py
+-rw-r--r--   0        0        0       86 2023-07-27 11:45:31.028016 pg_save-0.3.0/pg_save/dtos/__init__.py
+-rw-r--r--   0        0        0     1944 2023-07-27 13:40:42.258773 pg_save-0.3.0/pg_save/dtos/database.py
+-rw-r--r--   0        0        0      151 2023-07-27 12:20:47.702883 pg_save-0.3.0/pg_save/exceptions/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-27 13:21:32.155102 pg_save-0.3.0/pg_save/exceptions/db_connect.py
+-rw-r--r--   0        0        0      274 2023-07-27 13:21:35.007006 pg_save-0.3.0/pg_save/exceptions/table_not_fonud.py
+-rw-r--r--   0        0        0      183 2023-07-27 12:19:43.388641 pg_save-0.3.0/pg_save/exceptions/unsafe_expression.py
+-rw-r--r--   0        0        0      269 2023-07-27 12:21:19.142024 pg_save-0.3.0/pg_save/export/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-27 10:25:40.528671 pg_save-0.3.0/pg_save/export/csv.py
+-rw-r--r--   0        0        0       73 2023-07-27 10:25:44.660484 pg_save-0.3.0/pg_save/export/default_crs.py
+-rw-r--r--   0        0        0     1415 2023-07-27 12:01:38.273562 pg_save-0.3.0/pg_save/export/excel.py
+-rw-r--r--   0        0        0     3850 2023-07-27 13:40:32.135082 pg_save-0.3.0/pg_save/export/geojson.py
+-rw-r--r--   0        0        0     2603 2023-07-27 10:25:59.195829 pg_save-0.3.0/pg_save/export/json.py
+-rw-r--r--   0        0        0     4677 2023-07-27 13:40:58.382281 pg_save-0.3.0/pg_save/export/united.py
+-rw-r--r--   0        0        0      217 2023-07-27 13:25:02.332145 pg_save-0.3.0/pg_save/querying/__init__.py
+-rw-r--r--   0        0        0     3039 2023-07-27 10:59:43.371246 pg_save-0.3.0/pg_save/querying/query.py
+-rw-r--r--   0        0        0     2156 2023-07-27 13:25:24.695418 pg_save-0.3.0/pg_save/querying/table.py
+-rw-r--r--   0        0        0      134 2023-07-27 13:24:51.992482 pg_save-0.3.0/pg_save/utils/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-27 13:39:33.916862 pg_save-0.3.0/pg_save/utils/dotenv.py
+-rw-r--r--   0        0        0     4396 2023-07-27 14:38:46.934840 pg_save-0.3.0/pg_save/utils/interactive.py
+-rw-r--r--   0        0        0      488 2023-07-27 10:28:26.757510 pg_save-0.3.0/pg_save/utils/np_encoder.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:39:50.129122 pg_save-0.3.0/pg_save/utils/print.py
+-rw-r--r--   0        0        0     1417 2023-07-27 14:59:56.603121 pg_save-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9959 1970-01-01 00:00:00.000000 pg_save-0.3.0/PKG-INFO
```

### Comparing `pg_save-0.2.0/PKG-INFO` & `pg_save-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,123 @@
 Metadata-Version: 2.1
-Name: pg_save
-Version: 0.2.0
-Summary: An utility to save Postgres table data to csv, xlsx, json or geojson without a need of GeoPandas
-Author-email: Aleksei Sokol <kanootoko@gmail.com>, George Kontsevik <george.kontsevik@gmail.com>
+Name: pg-save
+Version: 0.3.0
+Summary: An utility to export Postgres table data to a various formats without having GeoPandas as a requirement
+Home-page: https://github.com/kanootoko/pg-save
 License: MIT
-Project-URL: Homepage, https://github.com/GKI98/df_saver_cli
-Project-URL: Bug Tracker, https://github.com/GKI98/df_saver_cli/issues
-Classifier: Programming Language :: Python :: 3
+Author: Aleksei Sokol
+Author-email: kanootoko@gmail.com
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.6,<9.0.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: numpy (>=1.25.1,<2.0.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: psycopg2 (>=2.9.6,<3.0.0)
+Requires-Dist: pyxlsx (>=1.1.3,<2.0.0)
+Project-URL: Bug Tracker, https://github.com/kanootoko/pg-save/issues
+Project-URL: Repository, https://github.com/kanootoko/pg-save
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 
-# pg-save - сохранение данных из базы данных Postgresql в различные форматы
+# pg-save - Утилита для сохранения данных из базы данных PostgreSQL в различные форматы
 
-Данная утилита позволяет экспортировать данные таблиц в csv, json, xlsx и geojson форматы посредством выгрузки из базы данных
-  с помощью драйвера `psycopg2` и обработки и сохранения средствами `pandas`. Сохранение geojson происходит без использования `geopandas`,
-  вся нагрузка по преобразованию геометрии ложится на `PostGIS` в базе данных.
+Данная утилита позволяет экспортировать данные таблиц в csv, json, xlsx и geojson форматы посредством
+    выгрузки из базы данных с помощью драйвера `psycopg2` и обработки и сохранения средствами `pandas`.
+    
+Сохранение geojson происходит без использования `geopandas`,
+    вся нагрузка по преобразованию геометрии ложится на `PostGIS` в базе данных.
 
 ## Установка из исходного кода
 
-1. Установить [python3](https://python3.org) (тестировалось на версии 3.10)
-2. Скачать содержимое репозитория и открыть терминал в папке
-3. Установить зависимости через `python -m pip install .`
-4. Запустить через `python -m pg_save запрос/название_таблицы`
+1. Установить \[python3\](https://python3.org) версии не меньше 3.9
+2. Скачать содержимое репозитория и открыть терминал в директории
+3. Установить с помощью `pipx install .` или `pip install .`
+4. Запустить через `pg-save --help`
 
-## Установка через pip
+## Установка через pipx (pip)
 
-Выполнить `pip install pg-save`.  
-В случае ошибки сборки psycopg2 нужно поставить необходимые зависимости, либо устанавливать из исходного кода с заменой `psycopg2` на `psycopg2-binary` в [pyproject.toml](pyproject.toml).
+Выполнить `pipx install pg-save`.
+
+В случае ошибки сборки psycopg2 нужно поставить необходимые зависимости, либо устанавливать из исходного кода
+с заменой `psycopg2` на `psycopg2-binary` в \[pyproject.toml\](pyproject.toml).
 
 ## Аргументы запуска
 
 Единственный принимаемый аргумент - запрос, название таблицы или имя файла с запросом/названием таблицы.
-  Приоритеты: имя файла (если есть такой файл) -> запрос (если начинается со слова SELECT в любом регистре) -> название таблицы (если не подошли другие варианты).  
+    Приоритеты: имя файла (если есть такой файл) -> запрос (если начинается со слова SELECT в любом регистре)
+    -> название таблицы (если не подошли другие варианты).
+
 Если аргумент не указан (а также не указаны команды получения списка таблиц, получения свойств заданной таблицы,
-  или запуска интерактивного режима), то программа завершается с ошибкой.
+    или запуска интерактивного режима), то программа завершается с ошибкой.
 
 ### Параметры подключения к базе данных
 
 Могут быть установлены через следующие аргументы:
-- --db_addr / -H - адрес сервера (по-умолчанию *localhost*)
-- --db_port / -P - порт сервера (по-умолчанию *5342*)
-- --db_name / -D - название базы данных (по-умолчанию *city_db_final*)
-- --db_user / -U - имя пользователя (по-умолчанию *postgres*)
-- --db_pass / -W - пароль пользователя (по-умолчанию *postgres*)
+- --db_addr / -h - адрес сервера (по-умолчанию *localhost*)
+- --db_port / -p - порт сервера (по-умолчанию *5342*)
+- --db_name / -d - название базы данных (по-умолчанию *city_db_final*)
+- --db_user / -u - имя пользователя (по-умолчанию *postgres*)
+- --db_pass / -w - пароль пользователя (по-умолчанию *postgres*)
+- --verbose_level / -v - уровень работы логгера (ERROR, WARNING, INFO, DEBUG, TRACE) - также может быть загружен из
+    переменной окружения VERBOSE_LEVEL
 
-Кроме того, эти же параметры могут быть заданы через переменные окружения, пример - [env_default](env_default.txt) .  
-Задать имя файла для загрузки переменных окружения можно через переменную окружения ENVFILE, по-умолчанию будет попытка использования файла `.env` в директории запуска.
+Кроме того, эти же параметры могут быть заданы через переменные окружения, пример - \[env_default\](env_default.txt) .
+
+Задать имя файла для загрузки переменных окружения можно через переменную окружения ENVFILE, по-умолчанию будет
+    попытка использования файла `.env` в директории запуска.
 Для удобства рекомендуется скопировать и изменить файл, назвав его **env**
 
-### Варианты работы, отличные от выгрузки данных
+### Выполнение заданного select-запроса
 
-Если задан хотя бы один из этих аргументов, то запрос обработан не будет, даже если он задан.  
-Список таблиц стоит выше по приоритету, чем получение информации о таблице.
+Команда `query` позволяет выполнить заданный select-запрос. Доступные параметры:
 
-- --list_tables / -l - получение списка таблиц в базе данных
-- --describe_table / -d - получение информации о выбранной таблице
+- --geometry_column / -g - установка столбца геометрии (для вывода в geojson)
+- --execute_as_is / -r (флаг) - не выполнять автоматически ST_AsGeoJSON() для геометрий объектов
+- --output_filename / -o - сохранение в файл, формат по расширению (.csv, .xlsx, .geojson или .json). Для сохранения
+    в geojson необходимо указать столбец геометрии (по-умолчанию *goemetry*)
 
-### Прочие параметры
+### Сохранение всех данных таблицы
+
+Команда `select-table` позволяет выполнить запрос вида `SELECT * FROM <table>`. Доступные параметры:
 
 - --geometry_column / -g - установка столбца геометрии (для вывода в geojson)
 - --use_centroids / -c (флаг) - сохранять только центроиды объектов (для выгрузки таблицы, с запросом ничего не делает)
-- --verbose_level / -v - уровень работы логгера (ERROR, WARNING, INFO, DEBUG) - также может быть загружен из переменной
-    окружения VERBOSE_LEVEL
-- --filename / -f - сохранение в файл, формат по расширению (.csv, .xlsx, .geojson или .json). Для сохранения в geojson необходимо указать столбец геометрии (по-умолчанию *goemetry*)
-- --interactive / -i - интерактивный режим
+- --output_filename / -o - сохранение в файл, формат по расширению (.csv, .xlsx, .geojson или .json). Для сохранения
+    в geojson необходимо указать столбец геометрии (по-умолчанию *goemetry*)
+
+### Варианты работы, отличные от выгрузки данных
+
+- list-tables - получение списка таблиц в базе данных
+- describe-table - получение информации о выбранной таблице/представлении/материализованном представлении
+- interactive - запуск интерактивного режима (о нем ниже)
 
 ## Интерактивный режим
 
-При запуске с параметром --interactive запускается интерактивный режим, позволяющий последовательно вводить
- команды без перезапуска утилиты и переподключения к базе данных  
+Данный режим позволяет последовательно вводить команды без перезапуска утилиты и переподключения к базе данных.
+
 Доступные команды:
 
-- \<query/filename\> [> filename] (запрос или путь до файла с запросом, опционально стрелочка и имя файла (в кавычках или нет)) -
-    выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения не задан, резултат просто выводится на экран.
-- "\<query/filename\>" [> filename] (запрос или путь до файла с запросом в кавычках, опционально стрелочка и имя файла (в кавычках или нет)) -
-    выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения не задан, резултат просто выводится на экран.
-    Запрос можно разносить на несколько строк, а также использовать внутри экранированные кавычки => аналогично запуску с запрсом.  
+- \<query/filename\> \[> filename\] (запрос или путь до файла с запросом, опционально стрелочка и имя файла
+    (в кавычках или нет)) - выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения
+    не задан, резултат просто выводится на экран.
+- "\<query/filename\>" \[> filename\] (запрос или путь до файла с запросом в кавычках, опционально стрелочка и имя файла
+    (в кавычках или нет)) - выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения не
+    задан, резултат просто выводится на экран. Запрос можно разносить на несколько строк, а также использовать внутри
+    экранированные кавычки => аналогично запуску с запрсом.
+
     Приоритет между файлом и запросом отдается в сторону файла (если такой файл есть).
-- \s \<table_name\> [> filename] (имя таблицы после \s, опционально стрелочка и имя файла) - получение всего, что находится в
-    таблице с опциональным сохранением в файл => аналогично запуском с аргументом - названием таблицы.
-- \dt \[schema\] - получение списка таблиц, опционально можно задать схему (по-умолчанию выводятся все не-системные таблицы) =>
-    аналогично ключу --list_tables.
-- \d \[schema\].\<table\> - Получение описания таблицы (столбцы, типы данных, возможность нахождения null'а и наличие значения
-    по-умолчанию) => аналогично ключу --describe_table.
-- \geometry_column, \g - изменение названия колонки геометрии для сохранения таблиц в geojson => аналогично ключу --geometry_column
-- \use_centroids, \c - Переключение режима использования центроидов (используется в случае загрузки таблиц) =>
+- \\s \<table_name\> \[> filename\] (имя таблицы после \s, опционально стрелочка и имя файла) - получение всего, что
+    находится в таблице с опциональным сохранением в файл => аналогично запуском с аргументом - названием таблицы.
+- \\dt \[schema\] - получение списка таблиц, опционально можно задать схему
+    (по-умолчанию выводятся все не-системные таблицы) => аналогично ключу --list_tables.
+- \\d \[schema\].\<table\> - Получение описания таблицы (столбцы, типы данных, возможность нахождения null'а и
+    наличие значения по-умолчанию) => аналогично ключу --describe_table.
+- \\geometry_column, \\g - изменение названия колонки геометрии для сохранения таблиц в geojson => аналогично
+    ключу --geometry_column
+- \\use_centroids, \\c - Переключение режима использования центроидов (используется в случае загрузки таблиц) =>
     аналогично ключу --use_centroids.
-- q, quit, exit, два Ctrl+C подряд - выход из интерактивного режима
+- q, quit, exit, два нажатия Ctrl+C подряд - выход из интерактивного режима
```

### Comparing `pg_save-0.2.0/README.md` & `pg_save-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,98 @@
-# pg-save - сохранение данных из базы данных Postgresql в различные форматы
+# pg-save - Утилита для сохранения данных из базы данных PostgreSQL в различные форматы
 
-Данная утилита позволяет экспортировать данные таблиц в csv, json, xlsx и geojson форматы посредством выгрузки из базы данных
-  с помощью драйвера `psycopg2` и обработки и сохранения средствами `pandas`. Сохранение geojson происходит без использования `geopandas`,
-  вся нагрузка по преобразованию геометрии ложится на `PostGIS` в базе данных.
+Данная утилита позволяет экспортировать данные таблиц в csv, json, xlsx и geojson форматы посредством
+    выгрузки из базы данных с помощью драйвера `psycopg2` и обработки и сохранения средствами `pandas`.
+    
+Сохранение geojson происходит без использования `geopandas`,
+    вся нагрузка по преобразованию геометрии ложится на `PostGIS` в базе данных.
 
 ## Установка из исходного кода
 
-1. Установить [python3](https://python3.org) (тестировалось на версии 3.10)
-2. Скачать содержимое репозитория и открыть терминал в папке
-3. Установить зависимости через `python -m pip install .`
-4. Запустить через `python -m pg_save запрос/название_таблицы`
+1. Установить \[python3\](https://python3.org) версии не меньше 3.9
+2. Скачать содержимое репозитория и открыть терминал в директории
+3. Установить с помощью `pipx install .` или `pip install .`
+4. Запустить через `pg-save --help`
 
-## Установка через pip
+## Установка через pipx (pip)
 
-Выполнить `pip install pg-save`.  
-В случае ошибки сборки psycopg2 нужно поставить необходимые зависимости, либо устанавливать из исходного кода с заменой `psycopg2` на `psycopg2-binary` в [pyproject.toml](pyproject.toml).
+Выполнить `pipx install pg-save`.
+
+В случае ошибки сборки psycopg2 нужно поставить необходимые зависимости, либо устанавливать из исходного кода
+с заменой `psycopg2` на `psycopg2-binary` в \[pyproject.toml\](pyproject.toml).
 
 ## Аргументы запуска
 
 Единственный принимаемый аргумент - запрос, название таблицы или имя файла с запросом/названием таблицы.
-  Приоритеты: имя файла (если есть такой файл) -> запрос (если начинается со слова SELECT в любом регистре) -> название таблицы (если не подошли другие варианты).  
+    Приоритеты: имя файла (если есть такой файл) -> запрос (если начинается со слова SELECT в любом регистре)
+    -> название таблицы (если не подошли другие варианты).
+
 Если аргумент не указан (а также не указаны команды получения списка таблиц, получения свойств заданной таблицы,
-  или запуска интерактивного режима), то программа завершается с ошибкой.
+    или запуска интерактивного режима), то программа завершается с ошибкой.
 
 ### Параметры подключения к базе данных
 
 Могут быть установлены через следующие аргументы:
-- --db_addr / -H - адрес сервера (по-умолчанию *localhost*)
-- --db_port / -P - порт сервера (по-умолчанию *5342*)
-- --db_name / -D - название базы данных (по-умолчанию *city_db_final*)
-- --db_user / -U - имя пользователя (по-умолчанию *postgres*)
-- --db_pass / -W - пароль пользователя (по-умолчанию *postgres*)
+- --db_addr / -h - адрес сервера (по-умолчанию *localhost*)
+- --db_port / -p - порт сервера (по-умолчанию *5342*)
+- --db_name / -d - название базы данных (по-умолчанию *city_db_final*)
+- --db_user / -u - имя пользователя (по-умолчанию *postgres*)
+- --db_pass / -w - пароль пользователя (по-умолчанию *postgres*)
+- --verbose_level / -v - уровень работы логгера (ERROR, WARNING, INFO, DEBUG, TRACE) - также может быть загружен из
+    переменной окружения VERBOSE_LEVEL
+
+Кроме того, эти же параметры могут быть заданы через переменные окружения, пример - \[env_default\](env_default.txt) .
 
-Кроме того, эти же параметры могут быть заданы через переменные окружения, пример - [env_default](env_default.txt) .  
-Задать имя файла для загрузки переменных окружения можно через переменную окружения ENVFILE, по-умолчанию будет попытка использования файла `.env` в директории запуска.
+Задать имя файла для загрузки переменных окружения можно через переменную окружения ENVFILE, по-умолчанию будет
+    попытка использования файла `.env` в директории запуска.
 Для удобства рекомендуется скопировать и изменить файл, назвав его **env**
 
-### Варианты работы, отличные от выгрузки данных
+### Выполнение заданного select-запроса
+
+Команда `query` позволяет выполнить заданный select-запрос. Доступные параметры:
 
-Если задан хотя бы один из этих аргументов, то запрос обработан не будет, даже если он задан.  
-Список таблиц стоит выше по приоритету, чем получение информации о таблице.
+- --geometry_column / -g - установка столбца геометрии (для вывода в geojson)
+- --execute_as_is / -r (флаг) - не выполнять автоматически ST_AsGeoJSON() для геометрий объектов
+- --output_filename / -o - сохранение в файл, формат по расширению (.csv, .xlsx, .geojson или .json). Для сохранения
+    в geojson необходимо указать столбец геометрии (по-умолчанию *goemetry*)
 
-- --list_tables / -l - получение списка таблиц в базе данных
-- --describe_table / -d - получение информации о выбранной таблице
+### Сохранение всех данных таблицы
 
-### Прочие параметры
+Команда `select-table` позволяет выполнить запрос вида `SELECT * FROM <table>`. Доступные параметры:
 
 - --geometry_column / -g - установка столбца геометрии (для вывода в geojson)
 - --use_centroids / -c (флаг) - сохранять только центроиды объектов (для выгрузки таблицы, с запросом ничего не делает)
-- --verbose_level / -v - уровень работы логгера (ERROR, WARNING, INFO, DEBUG) - также может быть загружен из переменной
-    окружения VERBOSE_LEVEL
-- --filename / -f - сохранение в файл, формат по расширению (.csv, .xlsx, .geojson или .json). Для сохранения в geojson необходимо указать столбец геометрии (по-умолчанию *goemetry*)
-- --interactive / -i - интерактивный режим
+- --output_filename / -o - сохранение в файл, формат по расширению (.csv, .xlsx, .geojson или .json). Для сохранения
+    в geojson необходимо указать столбец геометрии (по-умолчанию *goemetry*)
+
+### Варианты работы, отличные от выгрузки данных
+
+- list-tables - получение списка таблиц в базе данных
+- describe-table - получение информации о выбранной таблице/представлении/материализованном представлении
+- interactive - запуск интерактивного режима (о нем ниже)
 
 ## Интерактивный режим
 
-При запуске с параметром --interactive запускается интерактивный режим, позволяющий последовательно вводить
- команды без перезапуска утилиты и переподключения к базе данных  
+Данный режим позволяет последовательно вводить команды без перезапуска утилиты и переподключения к базе данных.
+
 Доступные команды:
 
-- \<query/filename\> [> filename] (запрос или путь до файла с запросом, опционально стрелочка и имя файла (в кавычках или нет)) -
-    выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения не задан, резултат просто выводится на экран.
-- "\<query/filename\>" [> filename] (запрос или путь до файла с запросом в кавычках, опционально стрелочка и имя файла (в кавычках или нет)) -
-    выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения не задан, резултат просто выводится на экран.
-    Запрос можно разносить на несколько строк, а также использовать внутри экранированные кавычки => аналогично запуску с запрсом.  
+- \<query/filename\> \[> filename\] (запрос или путь до файла с запросом, опционально стрелочка и имя файла
+    (в кавычках или нет)) - выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения
+    не задан, резултат просто выводится на экран.
+- "\<query/filename\>" \[> filename\] (запрос или путь до файла с запросом в кавычках, опционально стрелочка и имя файла
+    (в кавычках или нет)) - выполнение select-запроса с возможностью сохранения в файл. Если файл для сохранения не
+    задан, резултат просто выводится на экран. Запрос можно разносить на несколько строк, а также использовать внутри
+    экранированные кавычки => аналогично запуску с запрсом.
+
     Приоритет между файлом и запросом отдается в сторону файла (если такой файл есть).
-- \s \<table_name\> [> filename] (имя таблицы после \s, опционально стрелочка и имя файла) - получение всего, что находится в
-    таблице с опциональным сохранением в файл => аналогично запуском с аргументом - названием таблицы.
-- \dt \[schema\] - получение списка таблиц, опционально можно задать схему (по-умолчанию выводятся все не-системные таблицы) =>
-    аналогично ключу --list_tables.
-- \d \[schema\].\<table\> - Получение описания таблицы (столбцы, типы данных, возможность нахождения null'а и наличие значения
-    по-умолчанию) => аналогично ключу --describe_table.
-- \geometry_column, \g - изменение названия колонки геометрии для сохранения таблиц в geojson => аналогично ключу --geometry_column
-- \use_centroids, \c - Переключение режима использования центроидов (используется в случае загрузки таблиц) =>
+- \\s \<table_name\> \[> filename\] (имя таблицы после \s, опционально стрелочка и имя файла) - получение всего, что
+    находится в таблице с опциональным сохранением в файл => аналогично запуском с аргументом - названием таблицы.
+- \\dt \[schema\] - получение списка таблиц, опционально можно задать схему
+    (по-умолчанию выводятся все не-системные таблицы) => аналогично ключу --list_tables.
+- \\d \[schema\].\<table\> - Получение описания таблицы (столбцы, типы данных, возможность нахождения null'а и
+    наличие значения по-умолчанию) => аналогично ключу --describe_table.
+- \\geometry_column, \\g - изменение названия колонки геометрии для сохранения таблиц в geojson => аналогично
+    ключу --geometry_column
+- \\use_centroids, \\c - Переключение режима использования центроидов (используется в случае загрузки таблиц) =>
     аналогично ключу --use_centroids.
-- q, quit, exit, два Ctrl+C подряд - выход из интерактивного режима
+- q, quit, exit, два нажатия Ctrl+C подряд - выход из интерактивного режима
```

### Comparing `pg_save-0.2.0/pg_save/export/__init__.py` & `pg_save-0.3.0/pg_save/export/united.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Export pandas DataFrame to file or buffer with given format is defined here.
-"""
+"""United export to a given format methods are defined here."""
 from typing import BinaryIO, Literal, TextIO
 
 import pandas as pd
 from loguru import logger
 
 from pg_save.export.csv import to_csv
 from pg_save.export.default_crs import DEFAULT_CRS
@@ -27,103 +25,87 @@
         crs (dict[str, int] | int | None, optional): Coordinate system given by name (string), EPSG code (int) or
         by mapping {column: crs}. Used only in export to GeoJSON. Defaults to None.
         geometry_column (str | None, optional): Column with geometry. Used only in export to GeoJSON. Defaults to None.
     """
     if "." not in filename:
         logger.warning("File does not have extension, using csv")
         filename += ".csv"
-    file_format = filename.split(".")[-1]
+    file_format = filename.split(".")[-1].lower()
     if file_format.lower() not in ("csv", "xlsx", "json", "geojson"):
-        logger.error(f'File has wrong extension ("{file_format}"), switching to .csv')
+        logger.error('File has wrong extension ("{}"), switching to .csv', file_format)
         filename += ".csv"
         file_format = "csv"
     logger.info(f"Saving file in {file_format} format")
-    match file_format.lower():
-        case "csv":
-            to_csv(dataframe, filename)
-        case "xlsx":
-            to_excel(dataframe, filename)
-        case "geojson":
-            if crs is None:
-                logger.warning("No CRS is given, using {}", DEFAULT_CRS)
+    if file_format == "csv":
+        to_csv(dataframe, filename)
+    elif file_format == "xlsx":
+        to_excel(dataframe, filename)
+    elif file_format == "geojson":
+        if crs is None:
+            logger.warning("No CRS is given, using {}", DEFAULT_CRS)
+            crs = DEFAULT_CRS
+        elif isinstance(crs, dict):
+            if geometry_column in crs:
+                crs = crs[geometry_column]
+            else:
+                logger.warning(
+                    "crs given as a dict, but geometry column ({}) is not in its keys ({}). Using {}",
+                    geometry_column,
+                    ", ".join(crs.keys()),
+                    DEFAULT_CRS,
+                )
                 crs = DEFAULT_CRS
-            elif isinstance(crs, dict):
-                if geometry_column in crs:
-                    crs = crs[geometry_column]
-                else:
-                    logger.warning(
-                        "crs given as a dict, but geometry column ({}) is not in its keys ({}). Using {}",
-                        geometry_column,
-                        ", ".join(crs.keys()),
-                        DEFAULT_CRS,
-                    )
-                    crs = DEFAULT_CRS
-            if geometry_column is None:
-                logger.error('Geometry column is not set, but is required. Falling back to "geometry"')
-                geometry_column = "geometry"
-            to_geojson(dataframe, filename, geometry_column, crs)  # type: ignore
-        case "json":
-            to_json(dataframe, filename)
-        case _:
-            raise NotImplementedError(f"Cannot export DataFrame to file named {filename} - unknown extension.")
+        if geometry_column is None:
+            logger.error('Geometry column is not set, but is required. Falling back to "geometry"')
+            geometry_column = "geometry"
+        to_geojson(dataframe, filename, geometry_column, crs)
+    elif file_format == "json":
+        to_json(dataframe, filename)
 
 
 def to_buffer(
     dataframe: pd.DataFrame,
     buffer: TextIO | BinaryIO,
-    format: Literal["csv", "xlsx", "geojson", "json"],  # pylint: disable=redefined-builtin
+    file_format: Literal["csv", "xlsx", "geojson", "json"],
     crs: dict[str, str | int] | int | str | None = None,
     geometry_column: str | None = None,
 ) -> None:
     """Export pandas DataFrame to buffer.
 
     Args:
         dataframe (pd.DataFrame): DataFrame to export.
         buffer (TextIO | BinaryIO): StringIO (for csv, json, geojson) or BytesIO (for xlsx) to export DataFrame to.
         format (Literal["csv", "xlsx", "geojson", "json"]): file format to export to buffer.
         crs (int | str, optional): Coordinate system given by name (string), EPSG code (int) or
         by mapping {column: crs}. Used only in export to GeoJSON. Defaults to None.
         geometry_column (str): Column with geometry. Used only in export to GeoJSON. Defaults to None.
     """
-    format = format.lower()
-    if format not in ("csv", "xlsx", "json", "geojson"):
-        logger.error(f'Format is not supported ("{format}"), switching to csv')
-        format = "csv"
-    logger.info(f"Saving file in {format} format")
-    match format:
-        case "csv":
-            to_csv(dataframe, buffer)  # type: ignore
-        case "xlsx":
-            to_excel(dataframe, buffer)  # type: ignore
-        case "geojson":
-            if crs is None:
-                logger.warning("No CRS is given, using {}", DEFAULT_CRS)
+    file_format = file_format.lower()
+    if file_format not in ("csv", "xlsx", "json", "geojson"):
+        logger.error('Format is not supported ("{}"), switching to csv', file_format)
+        file_format = "csv"
+    logger.info(f"Saving file in {file_format} format")
+    if file_format == "csv":
+        to_csv(dataframe, buffer)
+    elif file_format == "xlsx":
+        to_excel(dataframe, buffer)
+    elif file_format == "geojson":
+        if crs is None:
+            logger.warning("No CRS is given, using {}", DEFAULT_CRS)
+            crs = DEFAULT_CRS
+        elif isinstance(crs, dict):
+            if geometry_column in crs:
+                crs = crs[geometry_column]
+            else:
+                logger.warning(
+                    "crs given as a dict, but geometry column ({}) is not in its keys ({}). Using {}",
+                    geometry_column,
+                    ", ".join(crs.keys()),
+                    DEFAULT_CRS,
+                )
                 crs = DEFAULT_CRS
-            elif isinstance(crs, dict):
-                if geometry_column in crs:
-                    crs = crs[geometry_column]
-                else:
-                    logger.warning(
-                        "crs given as a dict, but geometry column ({}) is not in its keys ({}). Using {}",
-                        geometry_column,
-                        ", ".join(crs.keys()),
-                        DEFAULT_CRS,
-                    )
-                    crs = DEFAULT_CRS
-            if geometry_column is None:
-                logger.error('Geometry column is not set, but is required. Falling back to "geometry"')
-                geometry_column = "geometry"
-            to_geojson(dataframe, buffer, geometry_column, crs)  # type: ignore
-        case "json":
-            to_json(dataframe, buffer)  # type: ignore
-        case _:
-            raise NotImplementedError(f"Cannot export DataFrame to unsupported format - {format}")
-
-
-__all__ = [
-    "DEFAULT_CRS",
-    "to_csv",
-    "to_excel",
-    "to_geojson",
-    "to_json",
-    "to_file",
-]
+        if geometry_column is None:
+            logger.error('Geometry column is not set, but is required. Falling back to "geometry"')
+            geometry_column = "geometry"
+        to_geojson(dataframe, buffer, geometry_column, crs)
+    elif file_format == "json":
+        to_json(dataframe, buffer)
```

### Comparing `pg_save-0.2.0/pg_save/export/excel.py` & `pg_save-0.3.0/pg_save/export/csv.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-"""
-Logic of exporting pandas DataFrame to excel is defined here.
-"""
-from typing import BinaryIO
+"""Logic of exporting pandas DataFrame to csv is defined here."""
+from __future__ import annotations
+
+from typing import TextIO
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 
 
-def to_excel(dataframe: pd.DataFrame, filename_or_buf: str | BinaryIO) -> None:
-    """Export pandas DataFrame to excel format.
+def to_csv(dataframe: pd.DataFrame, filename_or_buf: str | TextIO) -> None:
+    """Export pandas DataFrame to csv format.
 
     Args:
         dataframe (pd.DataFrame): DataFrame to export.
-        filename_or_buf (str | BinaryIO): filename or BytesIO buffer.
+        filename_or_buf (str | TextIO): filename or StringIO buffer.
     """
-    logger.debug("Saving excel" + (f" to {filename_or_buf}" if isinstance(filename_or_buf, str) else ""))
+    logger.debug("Saving csv" + (f' to "{filename_or_buf}"' if isinstance(filename_or_buf, str) else ""))
 
     dataframe = dataframe.copy()
+    if not isinstance(dataframe.index, pd.RangeIndex) or not all(dataframe.index == pd.RangeIndex(dataframe.shape[0])):
+        dataframe = dataframe.reset_index()
+
     for i in range(dataframe.shape[1]):
         dataframe.iloc[:, i] = pd.Series(
             map(
                 lambda x: int(x) if isinstance(x, float) and x.is_integer() else x,
                 dataframe.iloc[:, i],
             ),
             dtype=object,
         )
     dataframe = dataframe.replace({np.nan: None})
-    if isinstance(filename_or_buf, str):
-        dataframe.to_excel(filename_or_buf, header=True, index=False)
-    else:
-        with pd.ExcelWriter(filename_or_buf) as writer:  # pylint: disable=abstract-class-instantiated
-            dataframe.to_excel(writer, header=True, index=False)
+    dataframe.to_csv(filename_or_buf, header=True, index=False)
 
     logger.debug("Saved")
```

### Comparing `pg_save-0.2.0/pg_save/export/geojson.py` & `pg_save-0.3.0/pg_save/export/geojson.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""
-Logic of exporting pandas DataFrame to GeoJSON is defined here.
-"""
+"""Logic of exporting pandas DataFrame to GeoJSON is defined here."""
+from __future__ import annotations
+
 import json
 from typing import TextIO
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 
@@ -27,32 +27,35 @@
         crs (int | str, optional): Coordinate system EPSG code or full geometry description name given as string.
         Defaults to 4326.
     """
     logger.debug("Saving geojson" + (f' to "{filename_or_buf}"' if isinstance(filename_or_buf, str) else ""))
     serializable_types = ["object", "int64", "float64", "bool"]
 
     if geometry_column not in dataframe.columns:
-        logger.error(f'Geometry column "{geometry_column}" is not present, aborting')
+        logger.error('Geometry column "{}" is not present, aborting', geometry_column)
         return
 
     geometry_series = dataframe[geometry_column]
-    dataframe = dataframe.drop(geometry_column, axis=1)
+    dataframe = dataframe.drop(geometry_column, axis=1).copy()
+    if not isinstance(dataframe.index, pd.RangeIndex) or not all(dataframe.index == pd.RangeIndex(dataframe.shape[0])):
+        dataframe = dataframe.reset_index()
 
     for col in set(dataframe.columns):
         if isinstance(dataframe[col], pd.DataFrame):
             logger.warning(f'Table contains multiple columns having with the same name: "{col}", renaming')
             overlapping_columns_number_range = iter(range(dataframe.shape[1] + 1))
             dataframe = dataframe.rename(
                 lambda name, col=col, rng=overlapping_columns_number_range: name
                 if name != col
                 else f"{col}_{next(rng)}",
                 axis=1,
             )
             for col_idx in range(next(overlapping_columns_number_range)):
-                if dataframe[col_name:=f"{col}_{col_idx}"].dtypes not in serializable_types:
+                col_name = f"{col}_{col_idx}"
+                if dataframe[col_name].dtypes not in serializable_types:
                     logger.warning(f'Dropping non-serializable "{col_name}" column')
                     dataframe = dataframe.drop(col_name, axis=1)
         else:
             if dataframe[col].dtypes not in serializable_types:
                 logger.warning(f'Dropping non-serializable "{col}" column')
                 dataframe = dataframe.drop(col, axis=1)
```

### Comparing `pg_save-0.2.0/pg_save/export/json.py` & `pg_save-0.3.0/pg_save/export/json.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""
-Logic of exporting pandas DataFrame to json is defined here.
-"""
+"""Logic of exporting pandas DataFrame to json is defined here."""
+from __future__ import annotations
+
 import json
 from typing import Any, TextIO
 
 import numpy as np
 import pandas as pd
 from loguru import logger
 
@@ -16,14 +16,16 @@
 
     Args:
         dataframe (pd.DataFrame): DataFrame to export.
         filename_or_buf (str | TextIO): filename or StringIO buffer.
     """
     logger.debug("Saving json" + f' to "{filename_or_buf}"' if isinstance(filename_or_buf, str) else "")
     dataframe = dataframe.copy()
+    if not isinstance(dataframe.index, pd.RangeIndex) or not all(dataframe.index == pd.RangeIndex(dataframe.shape[0])):
+        dataframe = dataframe.reset_index()
 
     serializable_types = ["object", "int64", "float64", "bool"]
 
     for col in set(dataframe.columns):
         if isinstance(dataframe[col], pd.DataFrame):
             logger.warning(f'Table has more than one column with the same name: "{col}", renaming')
             overlapping_columns_number_range = iter(range(dataframe.shape[1] + 1))
```

### Comparing `pg_save-0.2.0/pg_save/utils/dotenv.py` & `pg_save-0.3.0/pg_save/utils/dotenv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,49 @@
-"""
-Read envfile function is defined here.
-"""
+"""Read envfile function is defined here."""
+from __future__ import annotations
+
 import os
+
 from loguru import logger
 
 
-def read_envfile(envfile_path: str | list[str], stop_after_first_success: bool = True) -> int:
+def try_read_envfile(envfile_path: str | list[str] = ..., stop_after_first_success: bool = True) -> int:
     """Read variables and set them to os.env from the given file/list of files.
     If multiple files are given, `stop_after_first_success` indicates if more than one should be read
-    (with priority of identical variables given to the first files)
+    (with priority of identical variables given to the first files).
 
     Args:
         envfile_path (str | list[str]): path to envfile or list of paths to multiple (first files have higher priority)
         stop_after_first_success (bool, optional): indicates whether process should stop after
         first successful envfile read. Defaults to True.
 
     Returns:
-        int: _description_
+        int: number of environment files processed.
     """
+    if envfile_path is ...:
+        envfile_path = [os.environ.get("ENVFILE", ".env")]
     if isinstance(envfile_path, str):
         envfile_path = [envfile_path]
     files_read = 0
     for envfile in envfile_path:
         if os.path.exists(envfile):
-            logger.info("reading envfile file located at {}", envfile)
+            logger.info("Reading envfile file located at {}", envfile)
             with open(envfile, "r", encoding="utf-8") as file:
                 for line in file:
                     try:
                         if len(line) == 0 or line.startswith("#"):
                             continue
                         if line.startswith("export "):
                             line = line[len("export ") :].strip()
                         name, value = line.split("=", 1)
                         if " #" in value:
                             value = value[: value.index(" #")].strip()
                         if name in os.environ:
                             logger.info(
-                                'skipping env variable "{}" from envfile as it is already set',
+                                'Skipping env variable "{}" from envfile as it is already set',
                                 name,
                             )
                         else:
                             os.environ[name] = value.strip()
                     except RuntimeError:
                         pass
             files_read += 1
```

### Comparing `pg_save-0.2.0/pg_save/utils/interactive.py` & `pg_save-0.3.0/pg_save/utils/interactive.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""
-Interactive methods of the project are defined here.
-"""
+"""Interactive methods of the project are defined here."""
 import os
+import sys
 
 import psycopg2  # pylint: disable=unused-import
 from loguru import logger
 
 import pg_save.export as export_df
-import pg_save.query as query_db
+import pg_save.querying as query_db
+from pg_save.utils.print import print_df
 
 
 def select_table(command: str, conn: "psycopg2.connection") -> None:
     """Select table helper
 
     Args:
         command (str): command to execute.
@@ -21,105 +21,101 @@
         print("You must use \\s with table name after it, aborting")
         return
     filename = None
     table_end = len(command)
     if ">" in command:
         filename = command[command.rfind(">") + 1 :].strip().strip("'\"")
         table_end = command.rfind(">")
-        logger.debug(f'saving table select to file "{filename}"')
+        logger.debug('Saving table select to file "{}"', filename)
 
     table_name = command[2:table_end].strip()
-    logger.debug(f"selecting table {table_name}")
+    logger.debug("Selecting table {}", table_name)
     table_data, _ = query_db.get_table(conn, table_name)
 
-    print(table_data)
+    print_df(table_data)
 
     if filename is not None:
         export_df.to_file(table_data, filename)
 
 
 def quoted_command(command: str, conn: "psycopg2.connection", geometry_column: str, execute_as_is: bool) -> None:
-    """Quoted command helper, launches when command starts with a double quote.
+    """Quoted command helper. Launched when command starts with a double quote.
 
     Args:
         command (str): command to execute.
         conn (psycopg2.connection): psycopg2 connection to the database.
         geometry_column (str): geometry column for GeoJSON export.
         execute_as_is (bool): indicates whether geometry columns will not be casted by ST_AsGeoJSON.
     """
-    if command.find('"', 1) == -1 or command.count('"') - command.count('\\"') == 0:
+    if '"' not in command[1:] or command.count('"') - command.count('\\"') == 0:
         while True:
             try:
                 line = input('>>>"')
                 command += f" {line}"
-                if line.find('"', 1) != -1 or line.count('"') - line.count('\\"') != 0:
+                if line.count('"') - line.count('\\"') != 0:
                     break
             except KeyboardInterrupt:
-                print("Ctrl+C hit, aborting query")
+                print("Ctrl+C hit, aborting multi-line query")
                 command = ""
                 break
-        if command == "":
+        if command.strip() == "":
             return
     filename = None
     query_end = command.rfind('"')
 
-    if ">" in command:
-        filename = command[command.rfind(">") + 1 :].strip().strip("'\"")
+    if line.rfind(">") > line.rfind('"'):
+        filename = line[line.rfind(">") + 1 :].strip("'\" ").strip()
         query_end = command.rfind('"', 2, command.rfind(">"))
-        logger.debug(f'Saving query results to file "{filename}"')
+        logger.debug('Saving query results to file "{}"', filename)
 
     query = command[1:query_end].strip()
+    query = query.replace('\\"', '"')
     if os.path.isfile(query):
-        logger.info("query is treated as filename, reading query from file")
+        logger.info("Query is treated as filename, reading query from file")
         try:
             with open(query, "r", encoding="utf-8") as file:
                 query = file.read()
-        except RuntimeError as ex:
-            logger.error(f"Exception on file read: {ex}")
+        except RuntimeError as exc:
+            logger.error("Exception on file read: {!r}", exc)
 
-    logger.debug("executing query: {}", query)
+    logger.debug("Executing query: {}", query)
 
     table_data, crs_dict = query_db.select(conn, query, execute_as_is)
     print(table_data)
 
     if filename is not None:
         export_df.to_file(table_data, filename, crs_dict, geometry_column)
 
 
 def command_with_save(command: str, conn: "psycopg2.connection", geometry_column: str, execute_as_is: bool) -> None:
-    """Command with export to flie helper.
+    """Execute query with optional export to flie if '>' is in command.
 
     Args:
         command (str): command to execute.
         conn (psycopg2.connection): psycopg2 connection to the database.
         geometry_column (str): geometry column to use with export to GeoJSON.
         execute_as_is (bool): indicates whether geometry columns will not be casted by ST_AsGeoJSON.
     """
     if ">" in command:
-        query = command[: command.find(">")].strip()
-        filename = command[command.find(">") + 1 :].strip().strip("'\"")
+        query = command[: command.rfind(">")].strip()
+        filename = command[command.rfind(">") + 1 :].strip().strip("'\"")
     else:
         query = command
         filename = None
 
     if os.path.isfile(query):
-        logger.info("query is treated as filename, reading query from file")
+        logger.info("Query is treated as filename, reading query from file")
         try:
             with open(query, "r", encoding="utf-8") as file:
                 query = file.read()
-        except RuntimeError as ex:
-            logger.error(f"Exception on file read: {ex}")
+        except Exception as exc:  # pylint: disable=broad-except
+            logger.error("Exception on file read: {!r}", exc)
+            sys.exit(1)
 
-    logger.debug("executing query (no options left): {}", query)
+    logger.debug("Executing query (no options left): {}", query)
+
+    table_data, crs_dict = query_db.select(conn, query, execute_as_is)
 
-    table_data, crs_dict = query_db.select(conn, command, execute_as_is)
     print(table_data)
 
     if filename is not None:
         export_df.to_file(table_data, filename, crs_dict, geometry_column)
-
-
-__all__ = [
-    "select_table",
-    "quoted_command",
-    "command_with_save",
-]
```

### Comparing `pg_save-0.2.0/pyproject.toml` & `pg_save-0.3.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,63 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "pg_save"
-version = "0.2.0"
+[tool.poetry]
+name = "pg-save"
+version = "0.3.0"
+description = "An utility to export Postgres table data to a various formats without having GeoPandas as a requirement"
 authors = [
-    { name = "Aleksei Sokol", email = "kanootoko@gmail.com" },
-    { name = "George Kontsevik", email = "george.kontsevik@gmail.com" },
+    "Aleksei Sokol <kanootoko@gmail.com>",
+    "George Kontsevik <george.kontsevik@gmail.com>",
 ]
-description = "An utility to save Postgres table data to csv, xlsx, json or geojson without a need of GeoPandas"
+license = "MIT"
 readme = "README.md"
-requires-python = ">=3.10"
-license = { text = "MIT" }
-
-dependencies = [
-    "click>=8.0",
-    "pandas>=1.5",
-    "numpy>=1.22",
-    "loguru>=0.6",
-    "pyxlsx>=1.1",
-    "psycopg2>=2.9",
-]
+packages = [{ include = "pg_save" }]
+repository = "https://github.com/kanootoko/pg-save"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-[project.optional-dependencies]
-dev = ["black>=22", "isort", "pre-commit"]
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/kanootoko/pg-save/issues"
+
+[tool.poetry.scripts]
+pg-save = "pg_save.cli:main"
+
+[tool.poetry.dependencies]
+python = "^3.9"
+click = "^8.1.6"
+pandas = "^2.0.3"
+numpy = "^1.25.1"
+loguru = "^0.7.0"
+pyxlsx = "^1.1.3"
+psycopg2 = "^2.9.6"
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.7.0"
+pylint = "^2.17.5"
+isort = "^5.12.0"
+pre-commit = "^3.3.3"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-[project.urls]
-"Homepage" = "https://github.com/GKI98/df_saver_cli"
-"Bug Tracker" = "https://github.com/GKI98/df_saver_cli/issues"
 
 [tool.black]
-line-length = 120
+target-version = ['py39']
+line_length = 120
+
+[tool.pylint.format]
+max-line-length = 120
+ignored-modules = ["psycopg2.errors"]
+disable = ["duplicate-code"]
+
+[tool.isort]
+py_version = 39
+lines_after_imports = 2
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+ensure_newline_before_comments = true
+line_length = 120
```

