# Comparing `tmp/AppiumExtended-0.0.2.tar.gz` & `tmp/AppiumExtended-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppiumExtended-0.0.2.tar", last modified: Wed Jul 26 17:49:58 2023, max compression
+gzip compressed data, was "AppiumExtended-0.1.3.tar", last modified: Thu Jul 27 20:46:21 2023, max compression
```

## Comparing `AppiumExtended-0.0.2.tar` & `AppiumExtended-0.1.3.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.978569 AppiumExtended-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.927042 AppiumExtended-0.0.2/AppiumExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:45.000000 AppiumExtended-0.0.2/AppiumExtended/__init__.py
--rw-rw-rw-   0        0        0     2694 2023-07-26 16:13:14.000000 AppiumExtended-0.0.2/AppiumExtended/appium_base.py
--rw-rw-rw-   0        0        0    28523 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_extended.py
--rw-rw-rw-   0        0        0    15339 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_get.py
--rw-rw-rw-   0        0        0     2505 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_is.py
--rw-rw-rw-   0        0        0     2259 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_swipe.py
--rw-rw-rw-   0        0        0     1888 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_tap.py
--rw-rw-rw-   0        0        0     7107 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_wait.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.935042 AppiumExtended-0.0.2/AppiumExtended.egg-info/
--rw-rw-rw-   0        0        0      472 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1310 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      232 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/requires.txt
--rw-rw-rw-   0        0        0      131 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.939486 AppiumExtended-0.0.2/AppiumGraph/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:49.000000 AppiumExtended-0.0.2/AppiumGraph/__init__.py
--rw-rw-rw-   0        0        0      486 2023-07-26 16:29:27.000000 AppiumExtended-0.0.2/AppiumGraph/appium_graph.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.944879 AppiumExtended-0.0.2/AppiumHelpers/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:54.000000 AppiumExtended-0.0.2/AppiumHelpers/__init__.py
--rw-rw-rw-   0        0        0    18033 2023-07-26 16:33:16.000000 AppiumExtended-0.0.2/AppiumHelpers/appium_helpers.py
--rw-rw-rw-   0        0        0    32167 2023-07-26 16:36:11.000000 AppiumExtended-0.0.2/AppiumHelpers/appium_image.py
--rw-rw-rw-   0        0        0    19788 2023-07-26 17:49:07.000000 AppiumExtended-0.0.2/AppiumHelpers/helpers_decorators.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.949016 AppiumExtended-0.0.2/AppiumNavigator/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:58.000000 AppiumExtended-0.0.2/AppiumNavigator/__init__.py
--rw-rw-rw-   0        0        0     7435 2023-07-26 16:41:36.000000 AppiumExtended-0.0.2/AppiumNavigator/appium_navigator.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.952009 AppiumExtended-0.0.2/AppiumServer/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:03.000000 AppiumExtended-0.0.2/AppiumServer/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-07-26 16:53:52.000000 AppiumExtended-0.0.2/AppiumServer/appium_server.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.966894 AppiumExtended-0.0.2/AppiumWebElementExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:07.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/__init__.py
--rw-rw-rw-   0        0        0        6 2023-05-31 18:50:55.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_actions.py
--rw-rw-rw-   0        0        0     9210 2023-07-26 16:51:39.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_adb_actions.py
--rw-rw-rw-   0        0        0    11345 2023-07-26 16:53:53.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_click.py
--rw-rw-rw-   0        0        0    14511 2023-07-26 16:56:52.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_dom.py
--rw-rw-rw-   0        0        0    17174 2023-07-26 16:56:57.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_extended.py
--rw-rw-rw-   0        0        0    23257 2023-07-26 16:58:06.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_get.py
--rw-rw-rw-   0        0        0    11658 2023-07-26 16:59:35.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_scroll.py
--rw-rw-rw-   0        0        0    12723 2023-07-26 16:59:35.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_tap.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.969468 AppiumExtended-0.0.2/AppiumWebElementsExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:11.000000 AppiumExtended-0.0.2/AppiumWebElementsExtended/__init__.py
--rw-rw-rw-   0        0        0      493 2023-07-26 16:59:35.000000 AppiumExtended-0.0.2/AppiumWebElementsExtended/web_elements_extended.py
--rw-rw-rw-   0        0        0      472 2023-07-26 17:49:58.978569 AppiumExtended-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.972473 AppiumExtended-0.0.2/adb/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:39.000000 AppiumExtended-0.0.2/adb/__init__.py
--rw-rw-rw-   0        0        0    27262 2023-07-26 16:49:36.000000 AppiumExtended-0.0.2/adb/adb.py
--rw-rw-rw-   0        0        0       42 2023-07-26 17:49:58.978569 AppiumExtended-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-07-26 17:49:48.000000 AppiumExtended-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.976564 AppiumExtended-0.0.2/utils/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:21.000000 AppiumExtended-0.0.2/utils/__init__.py
--rw-rw-rw-   0        0        0    16209 2023-07-26 16:53:52.000000 AppiumExtended-0.0.2/utils/operations.py
--rw-rw-rw-   0        0        0     6955 2023-07-26 17:07:41.000000 AppiumExtended-0.0.2/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.273734 AppiumExtended-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.204734 AppiumExtended-0.1.3/AppiumExtended/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:45.000000 AppiumExtended-0.1.3/AppiumExtended/__init__.py
+-rw-rw-rw-   0        0        0     2564 2023-07-27 15:28:50.000000 AppiumExtended-0.1.3/AppiumExtended/appium_base.py
+-rw-rw-rw-   0        0        0    28523 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_extended.py
+-rw-rw-rw-   0        0        0    15339 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_get.py
+-rw-rw-rw-   0        0        0     2505 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_is.py
+-rw-rw-rw-   0        0        0     2259 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_swipe.py
+-rw-rw-rw-   0        0        0     1888 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_tap.py
+-rw-rw-rw-   0        0        0     7107 2023-07-26 16:28:56.000000 AppiumExtended-0.1.3/AppiumExtended/appium_wait.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.213737 AppiumExtended-0.1.3/AppiumExtended.egg-info/
+-rw-rw-rw-   0        0        0      486 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1328 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      232 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      131 2023-07-27 20:46:21.000000 AppiumExtended-0.1.3/AppiumExtended.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.218738 AppiumExtended-0.1.3/AppiumGraph/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:49.000000 AppiumExtended-0.1.3/AppiumGraph/__init__.py
+-rw-rw-rw-   0        0        0      486 2023-07-26 16:29:27.000000 AppiumExtended-0.1.3/AppiumGraph/appium_graph.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.226733 AppiumExtended-0.1.3/AppiumHelpers/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:54.000000 AppiumExtended-0.1.3/AppiumHelpers/__init__.py
+-rw-rw-rw-   0        0        0    18033 2023-07-26 16:33:16.000000 AppiumExtended-0.1.3/AppiumHelpers/appium_helpers.py
+-rw-rw-rw-   0        0        0    32167 2023-07-26 16:36:11.000000 AppiumExtended-0.1.3/AppiumHelpers/appium_image.py
+-rw-rw-rw-   0        0        0    19788 2023-07-26 17:49:07.000000 AppiumExtended-0.1.3/AppiumHelpers/helpers_decorators.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.230735 AppiumExtended-0.1.3/AppiumNavigator/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:58.000000 AppiumExtended-0.1.3/AppiumNavigator/__init__.py
+-rw-rw-rw-   0        0        0     7472 2023-07-27 16:28:38.000000 AppiumExtended-0.1.3/AppiumNavigator/appium_navigator.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.237745 AppiumExtended-0.1.3/AppiumServer/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:03.000000 AppiumExtended-0.1.3/AppiumServer/__init__.py
+-rw-rw-rw-   0        0        0     2211 2023-07-27 20:06:25.000000 AppiumExtended-0.1.3/AppiumServer/appium_server.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.256736 AppiumExtended-0.1.3/AppiumWebElementExtended/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:07.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-05-31 18:50:55.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_actions.py
+-rw-rw-rw-   0        0        0     9210 2023-07-26 16:51:39.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_adb_actions.py
+-rw-rw-rw-   0        0        0    11345 2023-07-26 16:53:53.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_click.py
+-rw-rw-rw-   0        0        0    14511 2023-07-26 16:56:52.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_dom.py
+-rw-rw-rw-   0        0        0    17174 2023-07-26 16:56:57.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_extended.py
+-rw-rw-rw-   0        0        0    23257 2023-07-26 16:58:06.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_get.py
+-rw-rw-rw-   0        0        0    11658 2023-07-26 16:59:35.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_scroll.py
+-rw-rw-rw-   0        0        0    12723 2023-07-26 16:59:35.000000 AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_tap.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.259734 AppiumExtended-0.1.3/AppiumWebElementsExtended/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:11.000000 AppiumExtended-0.1.3/AppiumWebElementsExtended/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-07-26 16:59:35.000000 AppiumExtended-0.1.3/AppiumWebElementsExtended/web_elements_extended.py
+-rw-rw-rw-   0        0        0     1090 2023-07-26 20:30:30.000000 AppiumExtended-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      486 2023-07-27 20:46:21.273734 AppiumExtended-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-07-27 17:44:37.000000 AppiumExtended-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.264734 AppiumExtended-0.1.3/adb/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:39.000000 AppiumExtended-0.1.3/adb/__init__.py
+-rw-rw-rw-   0        0        0    27262 2023-07-26 16:49:36.000000 AppiumExtended-0.1.3/adb/adb.py
+-rw-rw-rw-   0        0        0       42 2023-07-27 20:46:21.274733 AppiumExtended-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-07-27 20:44:43.000000 AppiumExtended-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 20:46:21.271734 AppiumExtended-0.1.3/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:21.000000 AppiumExtended-0.1.3/utils/__init__.py
+-rw-rw-rw-   0        0        0    16209 2023-07-26 16:53:52.000000 AppiumExtended-0.1.3/utils/operations.py
+-rw-rw-rw-   0        0        0     6955 2023-07-26 17:07:41.000000 AppiumExtended-0.1.3/utils/utils.py
```

### Comparing `AppiumExtended-0.0.2/AppiumExtended/appium_base.py` & `AppiumExtended-0.1.3/AppiumExtended/appium_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,10 +68,7 @@
             self.driver = None
         if not self.keep_alive_server:
             self.server.stop()
 
     def is_running(self):
         return self.driver.is_running()
 
-    def get_session(self):
-        self.logger.debug("get_session(self)")
-        self.logger.debug(self.driver.get_session())
```

### Comparing `AppiumExtended-0.0.2/AppiumExtended/appium_extended.py` & `AppiumExtended-0.1.3/AppiumExtended/appium_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumExtended/appium_get.py` & `AppiumExtended-0.1.3/AppiumExtended/appium_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumExtended/appium_is.py` & `AppiumExtended-0.1.3/AppiumExtended/appium_is.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumExtended/appium_swipe.py` & `AppiumExtended-0.1.3/AppiumExtended/appium_swipe.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumExtended/appium_tap.py` & `AppiumExtended-0.1.3/AppiumExtended/appium_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumExtended/appium_wait.py` & `AppiumExtended-0.1.3/AppiumExtended/appium_wait.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumExtended.egg-info/SOURCES.txt` & `AppiumExtended-0.1.3/AppiumExtended.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+README.md
 setup.py
 AppiumExtended/__init__.py
 AppiumExtended/appium_base.py
 AppiumExtended/appium_extended.py
 AppiumExtended/appium_get.py
 AppiumExtended/appium_is.py
 AppiumExtended/appium_swipe.py
```

### Comparing `AppiumExtended-0.0.2/AppiumHelpers/appium_helpers.py` & `AppiumExtended-0.1.3/AppiumHelpers/appium_helpers.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumHelpers/appium_image.py` & `AppiumExtended-0.1.3/AppiumHelpers/appium_image.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumHelpers/helpers_decorators.py` & `AppiumExtended-0.1.3/AppiumHelpers/helpers_decorators.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumNavigator/appium_navigator.py` & `AppiumExtended-0.1.3/AppiumNavigator/appium_navigator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,16 @@
         # Находим путь от текущей страницы к целевой странице
         path = self.find_path(current_page, destination_page)
 
         if not path:
             raise ValueError(f"No path found from {current_page} to {destination_page}")
 
         # Выполняем навигацию, следуя найденному пути
-        self.perform_navigation(path)
+        self.perform_navigation(path, timeout)
 
-        # Ожидаем, пока не появится изображение целевой страницы
-        self.app.wait_for(image=destination_page.page_images, timeout=timeout)
 
     def find_path(self, start_page: Any, target_page: Any) -> Optional[List[Any]]:
         """
         Находит путь от стартовой страницы до целевой страницы.
 
         Этот метод использует поиск в ширину (BFS) для нахождения пути от стартовой страницы до целевой.
         Он обходит граф переходов между страницами, сохраняя текущий путь и посещенные страницы.
@@ -94,15 +92,15 @@
                 # Если соседняя страница не была посещена, добавляем ее в очередь для дальнейшего поиска
                 if next_window not in visited:
                     queue.append((next_window, path + [current_window]))
 
         # Возвращаем None, если путь не найден
         return None
 
-    def perform_navigation(self, path: List[Any]) -> None:
+    def perform_navigation(self, path: List[Any], timeout: int = 55) -> None:
         """
         Выполняет навигацию по заданному пути.
 
         Этот метод принимает список страниц, который представляет собой путь для навигации.
         Он выполняет переходы между соседними страницами, чтобы достичь целевой страницы.
 
         Args:
@@ -118,11 +116,13 @@
             current_page = path[page]
             next_page = path[page + 1]
             try:
                 # Получаем метод перехода между текущей и следующей страницами
                 transition_method = current_page.edges[next_page]
                 # Выполняем переход
                 transition_method()
+                # Ожидаем, пока не появится изображение целевой страницы
+                self.app.wait_for(image=next_page.page_images, timeout=timeout)
             except KeyError as e:
                 # В случае ошибки выводим сообщение о неудачном переходе
                 self.logger.error("perform_navigation() Не найден способ перехода")
                 self.logger.exception(e)
```

### Comparing `AppiumExtended-0.0.2/AppiumServer/appium_server.py` & `AppiumExtended-0.1.3/AppiumServer/appium_server.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self, port: int = 4723, log_level='error'):
         self.logger = logging.getLogger(config.APPIUM_LOG_NAME)
         self.port = port
         self.log_level = log_level
 
     def start(self) -> bool:
         self.logger.info("Start Appium server")
-        cmd = f'appium server --log-level {self.log_level} --use-plugins images -p {self.port} -a 127.0.0.1 -pa /wd/hub'
+        cmd = f'appium server -ka 800 --log-level {self.log_level} --use-plugins=device-farm,appium-dashboard -p {self.port} -a 0.0.0.0 -pa /wd/hub --plugin-device-farm-platform=android'
         try:
             subprocess.Popen(cmd, shell=True)
             return True
         except subprocess.CalledProcessError:
             self.logger.error("Error starting Appium server: subprocess.CalledProcessError")
             return False
         except OSError:
```

### Comparing `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_adb_actions.py` & `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_adb_actions.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_click.py` & `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_click.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_dom.py` & `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_dom.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_extended.py` & `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_get.py` & `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_scroll.py` & `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_scroll.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_tap.py` & `AppiumExtended-0.1.3/AppiumWebElementExtended/web_element_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/adb/adb.py` & `AppiumExtended-0.1.3/adb/adb.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/setup.py` & `AppiumExtended-0.1.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='AppiumExtended',
-    version='0.0.2',
+    version='0.1.3',
     description='An extension library for adding ease of use Appium-Python-Client',
-    author='open source community',
+    author='molokov-klim',
     packages=find_packages(),
     install_requires=[
         'Appium-Python-Client==2.11.1',
         'allure-pytest==2.13.2',
         'zlib-compress==0.0.1',
         'zlib-decompress==0.0.2',
         'pylibjpeg==1.4.0',
```

### Comparing `AppiumExtended-0.0.2/utils/operations.py` & `AppiumExtended-0.1.3/utils/operations.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.2/utils/utils.py` & `AppiumExtended-0.1.3/utils/utils.py`

 * *Files identical despite different names*

