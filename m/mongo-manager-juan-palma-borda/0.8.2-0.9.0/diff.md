# Comparing `tmp/mongo-manager-juan-palma-borda-0.8.2.tar.gz` & `tmp/mongo-manager-juan-palma-borda-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo-manager-juan-palma-borda-0.8.2.tar", last modified: Wed May 31 09:57:03 2023, max compression
+gzip compressed data, was "mongo-manager-juan-palma-borda-0.9.0.tar", last modified: Thu Jul 27 09:53:01 2023, max compression
```

## Comparing `mongo-manager-juan-palma-borda-0.8.2.tar` & `mongo-manager-juan-palma-borda-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.983829 mongo-manager-juan-palma-borda-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-31 09:57:03.983829 mongo-manager-juan-palma-borda-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 09:57:03.983829 mongo-manager-juan-palma-borda-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.979829 mongo-manager-juan-palma-borda-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.979829 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.979829 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/aggregations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/aggregations/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.979829 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/entity/objeto_mongo_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/mongo_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/mongo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.979829 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/patrones/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/patrones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/patrones/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.983829 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-31 09:56:41.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/repository/repository_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:57:03.983829 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager_juan_palma_borda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-31 09:57:03.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager_juan_palma_borda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-31 09:57:03.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager_juan_palma_borda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:57:03.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager_juan_palma_borda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 09:57:03.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager_juan_palma_borda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 09:57:03.000000 mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager_juan_palma_borda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.154715 mongo-manager-juan-palma-borda-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-27 09:53:01.154715 mongo-manager-juan-palma-borda-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-27 09:53:01.154715 mongo-manager-juan-palma-borda-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.146715 mongo-manager-juan-palma-borda-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.150715 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.150715 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/agg_op_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/agg_op_logical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/agg_op_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/agg_op_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/aggregation_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/aggregation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/aggregation_stages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/agreggation_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/aggregations/utils_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.150715 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/entity/objeto_mongo_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/mongo_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/mongo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.150715 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/patrones/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/patrones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/patrones/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.150715 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-27 09:52:50.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/repository/repository_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:53:01.154715 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager_juan_palma_borda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-27 09:53:01.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager_juan_palma_borda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-27 09:53:01.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager_juan_palma_borda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:53:01.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager_juan_palma_borda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 09:53:01.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager_juan_palma_borda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-27 09:53:01.000000 mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager_juan_palma_borda.egg-info/top_level.txt
```

### Comparing `mongo-manager-juan-palma-borda-0.8.2/LICENSE` & `mongo-manager-juan-palma-borda-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.8.2/LICENSE.txt` & `mongo-manager-juan-palma-borda-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.8.2/PKG-INFO` & `mongo-manager-juan-palma-borda-0.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,8 @@
-Metadata-Version: 2.1
-Name: mongo-manager-juan-palma-borda
-Version: 0.8.2
-Summary: Libreria para manejar objetos almacenados en MongoDB, usando la referencia de los CRUDRepository de SpringBoot
-Home-page: https://github.com/muerterauda/mongo_manager
-Author: Juan Palma Borda
-Author-email: juanpalmaborda@hotmail.com
-Project-URL: Bug Tracker, https://github.com/muerterauda/mongo_manager/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE.txt
-
-# Mongo Manager (0.8.2)
+# Mongo Manager (0.9.0.test)
 
 Libreria para el manejo de Objetos almacenados en base de datos MongoDB
 
 ## Clases
 
 ### MongoManager
 
@@ -48,21 +32,15 @@
 
 Repositorio base de mongo, recibe como parametros en el constructor,
 la coleccion a la que se hace referencia y el objeto al que va a convertir
 los resultados de las query que se realicen.
 
 En caso de querer usar una coleccion no perteneciente a la base de datos instanciada,
 se puede pasar el atributo *connection_collection* que debe ser una instancia de la conexion 
-MongoClient para la coleccion a tratar por el repositorio.
-
-### Aggregates
-
-Todavia no se han implementado ninguna clase que las trate a fondo, pero se pueden
-usar la mayoria de las *stages* y *operators* definidos en mongo_utils. Una vez definida la clase o 
-clases para tratar los Aggregates se compenetrara con estas funciones.
+*MongoClient* para la coleccion a tratar por el repositorio.
 
 ## Ejemplo 1
 
 En este ejemplo veremos el uso de la libreria definiendo un objeto <i>Book</i> 
 que hereda de ObjetoMongoAbstract y para el que implementa un <i>RepositoryBook</i>
  para poder manejar el objeto de manera más comoda.
 
@@ -92,20 +70,20 @@
                 return cls(name=dictionary.get('nombre'))
 
 
             def __str__(self) -> str:
                 return "{}".format(self.name)
 
     class RepositoryBook(RepositoryBase[Book]):
-        def __init__(self) -> None:
-            super().__init__('book', Book)
+        def __init__(self, conection_collection=None) -> None:
+            super().__init__('book', Book, conection_collection)
 
     class RepositoryBookOverrided(RepositoryBase[BookOverrided]):
-        def __init__(self) -> None:
-            super().__init__('book', BookOverrided)
+        def __init__(self, conection_collection=None) -> None:
+            super().__init__('book', BookOverrided, conection_collection)
 
     def main():
         a = RepositoryBook()
         b = Book('test')
         c = RepositoryBookOverrided()
         d = BookOverrided('test')
         a.insert_one(b)
@@ -113,7 +91,41 @@
         print(a.find_all()[-1])
         print(c.find_all()[-1])
 
 
     if __name__ == '__main__':
         MongoManager('user', 'psw', 'bd', 'authenticationDatabase')
         main()
+
+
+### Aggregates
+
+Los Aggregates se han dispuesto para poder ser creados de dos maneras distintas.
+
+ - Usando los decoradores definidos en el fichero _aggregation_decorator.py_ en combinacion
+con las clases _AggregationStage_ y _AggregationOperation_ cuyos hijos implementan los distintas 
+funciones permitidas en MongoDB, asi como los parametros que reciben.
+
+   El decorador permite a la función definida dentro de una clase que herede de _RepositoryBase_, recibir un
+AggregationExecutor que se ejecutar una vez finalizada la función, para ello todas las funciones usen estos decoradores
+deberán devolver dicho parametro.
+
+   Un ejemplo se puede ver a continuación, en el que se realiza un match a todos los libros que tengan en su nombre una *s* mayuscula 
+o minuscula, agrupa el resultado por nombre y cuenta los integrantes de cada grupo y finalmente genera el resultado con
+el formato {name: book_name_group, counter: total_books}:
+
+       class RepositoryBook(RepositoryBase[Book]):
+           def __init__(self, conection_collection=None) -> None:
+               super().__init__('book', Book, conection_collection)
+       
+           @agg_de.aggregation_decorator
+           def test_aggregation(self, agg: AggregationExecutor):
+               a = agg_st.AggStMatch()
+               a['nombre'] = agg_op_re.AggOpRegex('test',
+                                                  agg_op_re.AggOpRegex.get_options_regex(insensitive=True))
+               b = agg_st.AggStGroup(id_mapping={'name': '$name'})
+               b['counter'] = {'$sum': 1}
+               c = agg_st.AggStProject({'name': '$_id.name', 'counter': 1})
+               agg.add_steps(a, b, c)
+               return agg
+
+ - Usando los antigüos metodos definidos en el _mongo_utils.py_ que sirven de ayuda para poder generar los aggregates.
```

### Comparing `mongo-manager-juan-palma-borda-0.8.2/setup.cfg` & `mongo-manager-juan-palma-borda-0.9.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mongo-manager-juan-palma-borda
-version = 0.8.2
+version = 0.9.0
 author = Juan Palma Borda
 author_email = juanpalmaborda@hotmail.com
 description = Libreria para manejar objetos almacenados en MongoDB, usando la referencia de los CRUDRepository de SpringBoot
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/muerterauda/mongo_manager
 project_urls =
```

### Comparing `mongo-manager-juan-palma-borda-0.8.2/setup.py` & `mongo-manager-juan-palma-borda-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mongo-manager-juan-palma-borda",
-    version="0.8.2",
+    version="0.9.0",
     author='Juan Palma Borda',
     author_email='juanpalmaborda@hotmail.com',
     description='Libreria para manejar objetos almacenados en MongoDB, '
                 'usando la referencia de los CRUDRepository de SpringBoot',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/muerterauda/mongo_manager",
```

### Comparing `mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/entity/objeto_mongo_abstract.py` & `mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/entity/objeto_mongo_abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
                 d[x] = y.generar_list_dicts_from_list_objects(d[x], False, False)
             else:
                 d[x] = d[x].get_dict(False, False)
         return d
 
     def get_dict_no_id(self) -> dict:
         """
-        Fachade for get_dict(id_mongo=False). Return all variables from this object, similar to vars(object) with exception for _id
+        Facade for get_dict(id_mongo=False). Return all variables from this object, similar to vars(object)
+         with exception for _id
         @return: dict with object variables, similar to vars(object)
         """
         return self.get_dict(id_mongo=False)
 
     def serialize(self, id_mongo=True) -> str:
         """
         Serialize object to JSON format
@@ -81,22 +82,28 @@
     @classmethod
     def generar_object_from_dict(cls, dictionary):
         if dictionary is None:
             return None
         return cls(**cls.prepare_dict_for_generated_object(dictionary,
                                                            cls.get_attr_nested_objects()))
 
+    def __repr__(self):
+        return str(self.get_dict(True, True))
+
+    def __str__(self):
+        return f'Class: {self.__class__.__name__} -> ObjectID {self._id}'
+
     @classmethod
     def generar_objects_from_list_dicts(cls, dictionaries: list | Cursor):
         return [cls.generar_object_from_dict(dictionary) for dictionary in dictionaries]
 
     @staticmethod
     def generar_list_dicts_from_list_objects(lista_objetos: list, id_mongo=True, id_as_string=False):
         return [c.get_dict(id_mongo=id_mongo, id_as_string=id_as_string) for c in lista_objetos]
 
     @staticmethod
     def get_attr_nested_objects() -> dict:
         """
-        Attributes which are objects of the class ObjetoMongoAbstract, all of them. Overrides parents methods.
+        Attributes which are objects of the class ObjetoMongoAbstract, all of them. Override parents methods.
         @return: dict format {name_attr: class_attr}
         """
         return {}
```

### Comparing `mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/mongo_manager.py` & `mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/mongo_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from pymongo import MongoClient
 
-from .patrones.singleton import SingletonMeta
+from .patrones import SingletonMeta
 
 _mongo_manager_gl = None
 
 
 class MongoManager(metaclass=SingletonMeta):
     __bd = None
```

### Comparing `mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/mongo_utils.py` & `mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/patrones/singleton.py` & `mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/patrones/singleton.py`

 * *Files identical despite different names*

### Comparing `mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager/repository/repository_base.py` & `mongo-manager-juan-palma-borda-0.9.0/src/mongo_manager/repository/repository_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from __future__ import annotations
 
 from typing import TypeVar, Type, Generic, Optional
 
 import pymongo
 from pymongo.results import UpdateResult, InsertManyResult, InsertOneResult, DeleteResult
 
-from ..entity.objeto_mongo_abstract import ObjetoMongoAbstract
-from ..mongo_manager import SingletonMeta
+from .. import ObjetoMongoAbstract, MongoManagerException
+from ..patrones import SingletonMeta
+from ..aggregations.aggregation import AggregationExecutor
 from ..mongo_utils import aggregate_out, aggregate_match
 from bson import ObjectId
 
 T_O = TypeVar('T_O', bound=ObjetoMongoAbstract)
 
 
 class RepositoryBase(Generic[T_O], metaclass=SingletonMeta):
 
-    def __init__(self, collection, clase: Type[T_O], connection_collection=None) -> None:
+    def __init__(self, collection: str, clase: Type[T_O], connection_collection=None) -> None:
         __metaclass__ = SingletonMeta
         if connection_collection is None:
             from ..mongo_manager import _mongo_manager_gl as mongo_manager_gl
+            if mongo_manager_gl is None:
+                raise MongoManagerException(
+                    '\nNo se ha inicializado la base de datos, crear con MongoManager(),'
+                    ' ni se ha dado una conexion al repositorio.'
+                    '\nMongoManager is not initialized, pls create it with MongoManager(),'
+                    ' or provide a different connection to the repository.')
             connection_collection = mongo_manager_gl.collection(collection)
         self.__collection = connection_collection
         self.__clase = clase
 
     @property
     def collection(self) -> pymongo.collection.Collection:
         """
@@ -33,14 +40,17 @@
     @property
     def clase(self):
         """
         @return: Class used in the repository to convert data o objects| Clase del repositorio
         """
         return self.__clase
 
+    def _generate_aggregation_executor(self) -> AggregationExecutor:
+        return AggregationExecutor(collection_to_execute=self.collection)
+
     def count_many(self, filter_dict: dict = None) -> int:
         if filter_dict is None:
             filter_dict = {}
         return self.collection.count_documents(filter_dict)
 
     def count_all(self) -> int:
         return self.collection.count_documents({})
```

### Comparing `mongo-manager-juan-palma-borda-0.8.2/src/mongo_manager_juan_palma_borda.egg-info/PKG-INFO` & `mongo-manager-juan-palma-borda-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: mongo-manager-juan-palma-borda
-Version: 0.8.2
+Version: 0.9.0
 Summary: Libreria para manejar objetos almacenados en MongoDB, usando la referencia de los CRUDRepository de SpringBoot
 Home-page: https://github.com/muerterauda/mongo_manager
 Author: Juan Palma Borda
 Author-email: juanpalmaborda@hotmail.com
 Project-URL: Bug Tracker, https://github.com/muerterauda/mongo_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
-# Mongo Manager (0.8.2)
+# Mongo Manager (0.9.0.test)
 
 Libreria para el manejo de Objetos almacenados en base de datos MongoDB
 
 ## Clases
 
 ### MongoManager
 
@@ -48,21 +48,15 @@
 
 Repositorio base de mongo, recibe como parametros en el constructor,
 la coleccion a la que se hace referencia y el objeto al que va a convertir
 los resultados de las query que se realicen.
 
 En caso de querer usar una coleccion no perteneciente a la base de datos instanciada,
 se puede pasar el atributo *connection_collection* que debe ser una instancia de la conexion 
-MongoClient para la coleccion a tratar por el repositorio.
-
-### Aggregates
-
-Todavia no se han implementado ninguna clase que las trate a fondo, pero se pueden
-usar la mayoria de las *stages* y *operators* definidos en mongo_utils. Una vez definida la clase o 
-clases para tratar los Aggregates se compenetrara con estas funciones.
+*MongoClient* para la coleccion a tratar por el repositorio.
 
 ## Ejemplo 1
 
 En este ejemplo veremos el uso de la libreria definiendo un objeto <i>Book</i> 
 que hereda de ObjetoMongoAbstract y para el que implementa un <i>RepositoryBook</i>
  para poder manejar el objeto de manera más comoda.
 
@@ -92,20 +86,20 @@
                 return cls(name=dictionary.get('nombre'))
 
 
             def __str__(self) -> str:
                 return "{}".format(self.name)
 
     class RepositoryBook(RepositoryBase[Book]):
-        def __init__(self) -> None:
-            super().__init__('book', Book)
+        def __init__(self, conection_collection=None) -> None:
+            super().__init__('book', Book, conection_collection)
 
     class RepositoryBookOverrided(RepositoryBase[BookOverrided]):
-        def __init__(self) -> None:
-            super().__init__('book', BookOverrided)
+        def __init__(self, conection_collection=None) -> None:
+            super().__init__('book', BookOverrided, conection_collection)
 
     def main():
         a = RepositoryBook()
         b = Book('test')
         c = RepositoryBookOverrided()
         d = BookOverrided('test')
         a.insert_one(b)
@@ -113,7 +107,41 @@
         print(a.find_all()[-1])
         print(c.find_all()[-1])
 
 
     if __name__ == '__main__':
         MongoManager('user', 'psw', 'bd', 'authenticationDatabase')
         main()
+
+
+### Aggregates
+
+Los Aggregates se han dispuesto para poder ser creados de dos maneras distintas.
+
+ - Usando los decoradores definidos en el fichero _aggregation_decorator.py_ en combinacion
+con las clases _AggregationStage_ y _AggregationOperation_ cuyos hijos implementan los distintas 
+funciones permitidas en MongoDB, asi como los parametros que reciben.
+
+   El decorador permite a la función definida dentro de una clase que herede de _RepositoryBase_, recibir un
+AggregationExecutor que se ejecutar una vez finalizada la función, para ello todas las funciones usen estos decoradores
+deberán devolver dicho parametro.
+
+   Un ejemplo se puede ver a continuación, en el que se realiza un match a todos los libros que tengan en su nombre una *s* mayuscula 
+o minuscula, agrupa el resultado por nombre y cuenta los integrantes de cada grupo y finalmente genera el resultado con
+el formato {name: book_name_group, counter: total_books}:
+
+       class RepositoryBook(RepositoryBase[Book]):
+           def __init__(self, conection_collection=None) -> None:
+               super().__init__('book', Book, conection_collection)
+       
+           @agg_de.aggregation_decorator
+           def test_aggregation(self, agg: AggregationExecutor):
+               a = agg_st.AggStMatch()
+               a['nombre'] = agg_op_re.AggOpRegex('test',
+                                                  agg_op_re.AggOpRegex.get_options_regex(insensitive=True))
+               b = agg_st.AggStGroup(id_mapping={'name': '$name'})
+               b['counter'] = {'$sum': 1}
+               c = agg_st.AggStProject({'name': '$_id.name', 'counter': 1})
+               agg.add_steps(a, b, c)
+               return agg
+
+ - Usando los antigüos metodos definidos en el _mongo_utils.py_ que sirven de ayuda para poder generar los aggregates.
```

