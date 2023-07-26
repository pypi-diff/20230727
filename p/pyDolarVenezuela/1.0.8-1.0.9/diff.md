# Comparing `tmp/pyDolarVenezuela-1.0.8-py3-none-any.whl.zip` & `tmp/pyDolarVenezuela-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5956 bytes, number of entries: 10
+Zip file size: 6050 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-26 05:29 pyDolarVenezuela/__init__.py
 -rw-rw-rw-  2.0 fat      389 b- defN 23-Jul-26 03:29 pyDolarVenezuela/module_bcv.py
 -rw-rw-rw-  2.0 fat      573 b- defN 23-Jul-26 04:17 pyDolarVenezuela/request.py
--rw-rw-rw-  2.0 fat     2584 b- defN 23-Jul-26 06:02 pyDolarVenezuela/scraping_monitor.py
+-rw-rw-rw-  2.0 fat     2897 b- defN 23-Jul-26 23:31 pyDolarVenezuela/scraping_monitor.py
 -rw-rw-rw-  2.0 fat       81 b- defN 23-Jul-26 04:18 pyDolarVenezuela/util.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3555 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      855 b- defN 23-Jul-26 06:38 pyDolarVenezuela-1.0.8.dist-info/RECORD
-10 files, 9338 bytes uncompressed, 4476 bytes compressed:  52.1%
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-26 23:35 pyDolarVenezuela-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3560 b- defN 23-Jul-26 23:35 pyDolarVenezuela-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 23:35 pyDolarVenezuela-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-26 23:35 pyDolarVenezuela-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      855 b- defN 23-Jul-26 23:35 pyDolarVenezuela-1.0.9.dist-info/RECORD
+10 files, 9656 bytes uncompressed, 4570 bytes compressed:  52.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pyDolarVenezuela/scraping_monitor.py
 Comment: 
 
 Filename: pyDolarVenezuela/util.py
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.8.dist-info/LICENSE
+Filename: pyDolarVenezuela-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.8.dist-info/METADATA
+Filename: pyDolarVenezuela-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.8.dist-info/WHEEL
+Filename: pyDolarVenezuela-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.8.dist-info/top_level.txt
+Filename: pyDolarVenezuela-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pyDolarVenezuela-1.0.8.dist-info/RECORD
+Filename: pyDolarVenezuela-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyDolarVenezuela/scraping_monitor.py

```diff
@@ -1,40 +1,48 @@
 from bs4 import BeautifulSoup
+import re
 
 from pyDolarVenezuela.request import get_content_page
 from pyDolarVenezuela.util import PAGINA_PRINCIPAL_EXCHANGE_MONITOR
 
 def _get_values_monitors(soup: BeautifulSoup):
     return [value for value in soup]
 
+def _get_date_value(soup: BeautifulSoup):
+    return str(soup.find('p')).split("<br/>")[-1].replace("</p>", "")
+
 class Monitor(object):
     """
     La clase Monitor permite consultar los precios del dólar en diversos monitores en Venezuela. \n
     El método `_load` carga los datos de los monitores a través del scraping de la página web de referencia, donde los datos son almacenados en un diccionario. \ 
     El método `get_value_monitors` permite acceder a los datos almacenados en el diccionario.
     """
     def _load(self):
         soup = BeautifulSoup(get_content_page(PAGINA_PRINCIPAL_EXCHANGE_MONITOR), "html.parser")
         section_dolar_venezuela = soup.find_all("div", "col-xs-12 col-sm-6 col-md-4 col-tabla")
+        section_fecha_valor = soup.find("div", "col-xs-12 text-center")
+
+        date = _get_date_value(section_fecha_valor)
         all_monitors = _get_values_monitors(section_dolar_venezuela)
 
         self.all_monitors = {}
+        self.all_monitors['value'] = {"date": date}
         i: int = 0
         for monitor in all_monitors:
             monitor = monitor.find("div", "module-table module-table-fecha")
             data = {
                 "name": monitor.find('h6', 'nombre').text,
                 "unit": monitor.find('p', 'unidad').text,
                 "price": str(monitor.find('p', 'precio').text).replace(',', '.'),
                 "last_update": monitor.find('p', 'fecha').text
             }
-            self.all_monitors[i] = data
+            self.all_monitors[f"{i}"] = data
             i += 1
     
-    def get_value_monitors(self, monitor_code: int = None, name_property: str = None, prettify: bool = False):
+    def get_value_monitors(self, monitor_code: str = None, name_property: str = None, prettify: bool = False):
         """
         El parámetro `monitor_code` indica el código del monitor del cual se desea obtener información, \
         mientras que el parámetro `prettify` permite mostrar los precios en formato de moneda con el símbolo de Bolívares. \
         Si se proporciona un nombre de propiedad válido, se devolverá el valor correspondiente para ese monitor.
         """
         self._load()
```

## Comparing `pyDolarVenezuela-1.0.8.dist-info/LICENSE` & `pyDolarVenezuela-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyDolarVenezuela-1.0.8.dist-info/METADATA` & `pyDolarVenezuela-1.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.0.8
+Version: 1.0.9
 Summary: esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/pydolarvenezuela
 Project-URL: Bug Tracker, https://github.com/fcoagz/pydolarvenezuela/issues
@@ -43,18 +43,18 @@
 
 monitor = pdv.Monitor()
 
 # Obtener los valores de todos los monitores
 values = monitor.get_value_monitors()
 
 # Obtener el valor del dólar en EnParaleloVzla
-get_value_enparalelovzla = monitor.get_value_monitors(monitor_code=2, name_property='price', prettify=True)
+get_value_enparalelovzla = monitor.get_value_monitors(monitor_code='2', name_property='price', prettify=True)
 
 # Obtener la ultima actualizacion del dólar en Binance
-get_value_binance = monitor.get_value_monitors(monitor_code=17, name_property='last_update' prettify=False)
+get_value_binance = monitor.get_value_monitors(monitor_code='17', name_property='last_update', prettify=False)
 ```
 
 La clase `Bcv` tiene el siguiente metodo:
 
 - `Bcv().get_rates()`: Te muestra los valores de las tasas de cambio del Banco Central de Venezuela. EUR, CNY, TRY, USD.
 
 Los parametros del metodo ante mencionado son los siguientes:
```

## Comparing `pyDolarVenezuela-1.0.8.dist-info/RECORD` & `pyDolarVenezuela-1.0.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pyDolarVenezuela/__init__.py,sha256=0GTmqLZwCOSXXMeTQ5l-GVI8bzSHdG1ptbaK8dNUjoo,98
 pyDolarVenezuela/module_bcv.py,sha256=IcxghFAml6nLh8LmHasJG3DFLzPSDF-7wXrfdGFP93M,389
 pyDolarVenezuela/request.py,sha256=55_ZjAKw-SupS4ugtXZWhSEZgqVy9mgz5DKUchQKH_4,573
-pyDolarVenezuela/scraping_monitor.py,sha256=HUDoYZIAgJM_-2ZfD8hf-Hvt9Lti0q4LcIYQYZ0Rxrc,2584
+pyDolarVenezuela/scraping_monitor.py,sha256=AClW6LMQQ-MR1DwZg18MXwrkxUWX1YxRejbplViy8wg,2897
 pyDolarVenezuela/util.py,sha256=9zypmUe_jZTpMkzyizPj5N9hJoH78tRyUHdfNw3EFfI,81
-pyDolarVenezuela-1.0.8.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
-pyDolarVenezuela-1.0.8.dist-info/METADATA,sha256=INmb3kWrKHONCl1fIWUwDPg51Ha-PjtloBrzeJ7TI9g,3555
-pyDolarVenezuela-1.0.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-pyDolarVenezuela-1.0.8.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
-pyDolarVenezuela-1.0.8.dist-info/RECORD,,
+pyDolarVenezuela-1.0.9.dist-info/LICENSE,sha256=yhyzG4KlBwvAy1K47aCyZbF5x8p9Evp9ehLARqdm4mM,1094
+pyDolarVenezuela-1.0.9.dist-info/METADATA,sha256=sVhPkKez79ndVaENtKjlRUxwF24XhVDJq3X8DGdIhq0,3560
+pyDolarVenezuela-1.0.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+pyDolarVenezuela-1.0.9.dist-info/top_level.txt,sha256=DqT65xfdAAw8yCgxoWQ1UWnzpZ-LGoBUkgMVnY0N8ro,17
+pyDolarVenezuela-1.0.9.dist-info/RECORD,,
```

