# Comparing `tmp/selene-2.0.0rc3.tar.gz` & `tmp/selene-2.0.0rc3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selene-2.0.0rc3.tar", max compression
+gzip compressed data, was "selene-2.0.0rc3.post1.tar", max compression
```

## Comparing `selene-2.0.0rc3.tar` & `selene-2.0.0rc3.post1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc3/LICENSE
--rw-r--r--   0        0        0    16589 2023-07-21 19:40:03.696730 selene-2.0.0rc3/README.md
--rw-r--r--   0        0        0     7937 2023-07-21 20:19:06.512747 selene-2.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     6045 2023-07-21 20:13:43.937671 selene-2.0.0rc3/selene/__init__.py
--rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc3/selene/_managed.py
--rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc3/selene/api/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc3/selene/api/base/__init__.py
--rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc3/selene/api/shared/__init__.py
--rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc3/selene/common/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc3/selene/common/data_structures/__init__.py
--rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc3/selene/common/data_structures/persistent.py
--rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc3/selene/common/fp.py
--rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc3/selene/common/helpers.py
--rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc3/selene/common/none_object.py
--rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc3/selene/common/predicate.py
--rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc3/selene/core/__init__.py
--rw-r--r--   0        0        0     9379 2023-07-01 11:09:18.988781 selene-2.0.0rc3/selene/core/command.py
--rw-r--r--   0        0        0     6672 2023-07-01 11:00:30.192218 selene-2.0.0rc3/selene/core/condition.py
--rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc3/selene/core/conditions.py
--rw-r--r--   0        0        0    61335 2023-07-21 19:02:34.547994 selene-2.0.0rc3/selene/core/configuration.py
--rw-r--r--   0        0        0     9441 2023-04-12 19:41:51.757408 selene-2.0.0rc3/selene/core/configuration.pyi
--rw-r--r--   0        0        0    44433 2023-07-01 11:09:18.989737 selene-2.0.0rc3/selene/core/entity.py
--rw-r--r--   0        0        0    12087 2023-04-12 19:44:29.895473 selene-2.0.0rc3/selene/core/entity.pyi
--rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc3/selene/core/exceptions.py
--rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc3/selene/core/locator.py
--rw-r--r--   0        0        0    17246 2023-07-01 11:09:18.990179 selene-2.0.0rc3/selene/core/match.py
--rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc3/selene/core/query.py
--rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc3/selene/core/wait.py
--rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc3/selene/py.typed
--rw-r--r--   0        0        0      120 2023-07-21 19:00:31.406121 selene-2.0.0rc3/selene/support/__init__.py
--rw-r--r--   0        0        0       32 2023-07-21 19:00:05.654941 selene-2.0.0rc3/selene/support/_extensions/__init__.py
--rw-r--r--   0        0        0       20 2023-07-21 19:00:05.662165 selene-2.0.0rc3/selene/support/_extensions/webdriver_manager/__init__.py
--rw-r--r--   0        0        0     7336 2023-07-21 20:05:15.134209 selene-2.0.0rc3/selene/support/_extensions/webdriver_manager/patch.py
--rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc3/selene/support/_logging.py
--rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc3/selene/support/by.py
--rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc3/selene/support/conditions/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc3/selene/support/conditions/be.py
--rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc3/selene/support/conditions/have.py
--rw-r--r--   0        0        0     9093 2023-07-01 10:59:38.230736 selene-2.0.0rc3/selene/support/conditions/not_.py
--rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc3/selene/support/shared/__init__.py
--rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc3/selene/support/shared/browser.py
--rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc3/selene/support/shared/config.py
--rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc3/selene/support/shared/jquery_style.py
--rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc3/selene/support/webdriver.py
--rw-r--r--   0        0        0    18226 1970-01-01 00:00:00.000000 selene-2.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc3.post1/LICENSE
+-rw-r--r--   0        0        0    16589 2023-07-21 19:40:03.696730 selene-2.0.0rc3.post1/README.md
+-rw-r--r--   0        0        0     7942 2023-07-27 13:49:44.978059 selene-2.0.0rc3.post1/pyproject.toml
+-rw-r--r--   0        0        0     6050 2023-07-27 13:56:57.965322 selene-2.0.0rc3.post1/selene/__init__.py
+-rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc3.post1/selene/_managed.py
+-rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc3.post1/selene/api/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc3.post1/selene/api/base/__init__.py
+-rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc3.post1/selene/api/shared/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc3.post1/selene/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc3.post1/selene/common/data_structures/__init__.py
+-rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc3.post1/selene/common/data_structures/persistent.py
+-rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc3.post1/selene/common/fp.py
+-rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc3.post1/selene/common/helpers.py
+-rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc3.post1/selene/common/none_object.py
+-rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc3.post1/selene/common/predicate.py
+-rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc3.post1/selene/core/__init__.py
+-rw-r--r--   0        0        0     8731 2023-07-27 13:08:17.397537 selene-2.0.0rc3.post1/selene/core/command.py
+-rw-r--r--   0        0        0     6672 2023-07-01 11:00:30.192218 selene-2.0.0rc3.post1/selene/core/condition.py
+-rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc3.post1/selene/core/conditions.py
+-rw-r--r--   0        0        0    61351 2023-07-27 13:56:27.749605 selene-2.0.0rc3.post1/selene/core/configuration.py
+-rw-r--r--   0        0        0     9441 2023-04-12 19:41:51.757408 selene-2.0.0rc3.post1/selene/core/configuration.pyi
+-rw-r--r--   0        0        0    44433 2023-07-01 11:09:18.989737 selene-2.0.0rc3.post1/selene/core/entity.py
+-rw-r--r--   0        0        0    12087 2023-04-12 19:44:29.895473 selene-2.0.0rc3.post1/selene/core/entity.pyi
+-rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc3.post1/selene/core/exceptions.py
+-rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc3.post1/selene/core/locator.py
+-rw-r--r--   0        0        0    17295 2023-07-25 14:23:47.850912 selene-2.0.0rc3.post1/selene/core/match.py
+-rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc3.post1/selene/core/query.py
+-rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc3.post1/selene/core/wait.py
+-rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc3.post1/selene/py.typed
+-rw-r--r--   0        0        0      120 2023-07-21 19:00:31.406121 selene-2.0.0rc3.post1/selene/support/__init__.py
+-rw-r--r--   0        0        0       32 2023-07-27 13:43:32.337434 selene-2.0.0rc3.post1/selene/support/_extensions/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-27 13:48:23.832967 selene-2.0.0rc3.post1/selene/support/_extensions/webdriver_manager/__init__.py
+-rw-r--r--   0        0        0     8693 2023-07-27 13:55:40.670448 selene-2.0.0rc3.post1/selene/support/_extensions/webdriver_manager/patch.py
+-rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc3.post1/selene/support/_logging.py
+-rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc3.post1/selene/support/by.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc3.post1/selene/support/conditions/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc3.post1/selene/support/conditions/be.py
+-rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc3.post1/selene/support/conditions/have.py
+-rw-r--r--   0        0        0     9093 2023-07-01 10:59:38.230736 selene-2.0.0rc3.post1/selene/support/conditions/not_.py
+-rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc3.post1/selene/support/shared/__init__.py
+-rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc3.post1/selene/support/shared/browser.py
+-rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc3.post1/selene/support/shared/config.py
+-rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc3.post1/selene/support/shared/jquery_style.py
+-rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc3.post1/selene/support/webdriver.py
+-rw-r--r--   0        0        0    18232 1970-01-01 00:00:00.000000 selene-2.0.0rc3.post1/PKG-INFO
```

### Comparing `selene-2.0.0rc3/LICENSE` & `selene-2.0.0rc3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/README.md` & `selene-2.0.0rc3.post1/README.md`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/pyproject.toml` & `selene-2.0.0rc3.post1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selene"
-version = "2.0.0rc3"
+version = "2.0.0rc3post1"
 description = "User-oriented browser tests in Python (Selenide port)"
 authors = ["Iakiv Kramarenko <yashaka@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
 	"testing",
 	"selenium",
```

### Comparing `selene-2.0.0rc3/selene/__init__.py` & `selene-2.0.0rc3.post1/selene/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,8 +223,8 @@
 """
 
 # """
 # Just types...
 # """
 from selene.core.entity import Element, Collection  # noqa
 
-__version__ = '2.0.0rc3'
+__version__ = '2.0.0rc3post1'
```

### Comparing `selene-2.0.0rc3/selene/api/__init__.py` & `selene-2.0.0rc3.post1/selene/api/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/api/base/__init__.py` & `selene-2.0.0rc3.post1/selene/api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/api/shared/__init__.py` & `selene-2.0.0rc3.post1/selene/api/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/common/data_structures/persistent.py` & `selene-2.0.0rc3.post1/selene/common/data_structures/persistent.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/common/fp.py` & `selene-2.0.0rc3.post1/selene/common/fp.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/common/helpers.py` & `selene-2.0.0rc3.post1/selene/common/helpers.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/common/none_object.py` & `selene-2.0.0rc3.post1/selene/common/none_object.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/common/predicate.py` & `selene-2.0.0rc3.post1/selene/common/predicate.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/__init__.py` & `selene-2.0.0rc3.post1/selene/core/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/command.py` & `selene-2.0.0rc3.post1/selene/core/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,35 +69,14 @@
     .locate()
     .send_keys(
         (Keys.COMMAND if sys.platform == 'darwin' else Keys.CONTROL) + 'a' + Keys.NULL,
     ),
 )
 
 
-def _drag_to(destination: Element):
-    def func(source: Element):
-        located_source = source.locate()
-        located_destination = destination.locate()
-        driver = source.config.driver
-        actions: ActionChains = ActionChains(driver)
-
-        actions.w3c_actions = ActionBuilder(
-            driver, mouse=PointerInput(interaction.POINTER_MOUSE, 'mouse')
-        )
-        (
-            actions.w3c_actions.pointer_action.move_to(located_source)
-            .pointer_down()
-            .move_to(located_destination)
-            .release()
-        )
-        actions.perform()
-
-    return Command(f'drag to -> {destination}', func)
-
-
 # TODO: can we make it work for both mobile and web?
 #       should we selectively choose proper interaction.POINTER_TOUCH below?
 def _long_press(duration=1.0):
     def func(element: Element):
         located_element = element.locate()
         driver = element.config.driver
         actions: ActionChains = ActionChains(driver)
```

### Comparing `selene-2.0.0rc3/selene/core/condition.py` & `selene-2.0.0rc3.post1/selene/core/condition.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/conditions.py` & `selene-2.0.0rc3.post1/selene/core/conditions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/configuration.py` & `selene-2.0.0rc3.post1/selene/core/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,20 +59,20 @@
         Edge,
     )
 
     from selenium.webdriver.chrome.service import Service as ChromeService
     from selenium.webdriver.firefox.service import Service as FirefoxService
     from selenium.webdriver.edge.service import Service as EdgeService  # type: ignore
 
+    from selene.support._extensions.webdriver_manager import ChromeType  # type: ignore
+
     from webdriver_manager.chrome import ChromeDriverManager  # type: ignore
     from webdriver_manager.firefox import GeckoDriverManager  # type: ignore
     from webdriver_manager.microsoft import EdgeChromiumDriverManager  # type: ignore
 
-    from webdriver_manager.core.utils import ChromeType  # type: ignore
-
     def install_and_build_chrome():
         # TODO: consider simplifying the logic... to much of ifs
         #       probably all ifs were already before calling this function
         #       see example of simplification in install_and_build_firefox
         if config.driver_options and not isinstance(
             config.driver_options, ChromeOptions
         ):
```

### Comparing `selene-2.0.0rc3/selene/core/configuration.pyi` & `selene-2.0.0rc3.post1/selene/core/configuration.pyi`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/entity.py` & `selene-2.0.0rc3.post1/selene/core/entity.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/entity.pyi` & `selene-2.0.0rc3.post1/selene/core/entity.pyi`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/exceptions.py` & `selene-2.0.0rc3.post1/selene/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/locator.py` & `selene-2.0.0rc3.post1/selene/core/locator.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/match.py` & `selene-2.0.0rc3.post1/selene/core/match.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,17 @@
             )
 
     return ConditionWithValues(
         str(raw_attribute_condition), raw_attribute_condition.call
     )
 
 
-element_is_selected: Condition[Element] = element_has_attribute('elementIsSelected')
+element_is_selected: Condition[Element] = ElementCondition.raise_if_not(
+    'is selected', lambda element: element().is_selected()
+)
 
 
 def element_has_value(expected: str) -> Condition[Element]:
     return element_has_attribute('value').value(expected)
 
 
 def element_has_value_containing(expected: str) -> Condition[Element]:
```

### Comparing `selene-2.0.0rc3/selene/core/query.py` & `selene-2.0.0rc3.post1/selene/core/query.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/core/wait.py` & `selene-2.0.0rc3.post1/selene/core/wait.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/_extensions/webdriver_manager/patch.py` & `selene-2.0.0rc3.post1/selene/support/_extensions/webdriver_manager/patch.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,98 +43,120 @@
     """
 
     from webdriver_manager.core import logger as wdm_logger
     from packaging import version
     from webdriver_manager.core import utils as wdm_utils
     from webdriver_manager.core.utils import ChromeType
 
+    # We alias driver object from driver_manager as driver_utils
+    # for lesser confusion.
+    # In fact wdm driver object is more a bunch of utility functions.
+    # From OOP perspective,
+    # it's not a pure object representing actual "low level driver binary".
+    # And 'driver' name also conflicts with common 'driver' client object from selenium.
     driver_utils = driver_manager.driver
     http_client = driver_utils._http_client
 
     def chrome_apis_url(endpoint):
         return f'https://googlechromelabs.github.io/chrome-for-testing/{endpoint}'
 
     good_binary_version = None
     good_binary_url = None
     installed_browser_version = driver_utils.get_browser_version_from_os()
 
-    if not installed_browser_version:
+    if installed_browser_version:
+        if version.parse(installed_browser_version) < version.parse('115.0.5763.0'):
+            # if browser version is less than 115.0.5763.0
+            # then we use old wdm logic
+            # and just return the driver_manager as is
+            return driver_manager
+
+        # patching wdm_utils.PATTERN
+        # we need all 4 sub-versions not just 3 of them
+        wdm_utils.PATTERN[ChromeType.GOOGLE] = r"\d+\.\d+\.\d+.\d+"
+        # retaking version from os after patched pattern
+        good_binary_version = wdm_utils.get_browser_version_from_os(
+            driver_utils.get_browser_type()
+        )
+        # let's reset _browser_version to the new 4-sub-versions value
+        # from here, we assume that
+        # "good" binary version is the same as "good" browser version
+        driver_utils._browser_version = good_binary_version
+
+        known_good_versions = (
+            http_client.get(chrome_apis_url('known-good-versions-with-downloads.json'))
+            .json()
+            .get('versions', [])
+        )
+
+        matched_version_downloads_chromedriver_per_platform: list = next(
+            iter(
+                info.get('downloads', {}).get('chromedriver', [])
+                for info in known_good_versions
+                if info.get('version', None) == good_binary_version
+            ),
+            [],
+        )
+
+        good_binary_url = next(
+            iter(
+                info.get('url', None)
+                for info in matched_version_downloads_chromedriver_per_platform
+                if info.get('platform') == driver_utils.get_os_type().replace('_', '-')
+            ),
+            None,
+        )
+
+    if (not installed_browser_version) or (not good_binary_url):
         wdm_logger.log(
             'Failed to get version of Chrome installed at your OS '
-            f'(detected os type: {driver_utils.os_type}).'
+            f'(detected os type: {driver_utils._os_type}).'
             f'Going to install the chromedriver binary '
             f'matching latest known stable version of Chrome...'
         )
         last_known_good_versions_with_downloads = http_client.get(
             chrome_apis_url('last-known-good-versions-with-downloads.json')
         ).json()
         stable_channel = last_known_good_versions_with_downloads.get(
             'channels', {}
         ).get('Stable', {})
 
-        last_known_good_version = (stable_channel.get('version', {})) or None
+        # Above and below, we allways use get('key', default) instead of just ['key']
+        # to provide default value in case of missing key
+        # and make further processing easier and safer
+        # (we don't need to check for None when processing via comprehensions).
+        # Sometimes, like below we use `get('key', '') or None`
+        # instead of just `get('key', None)` or even `get('key)`
+        # in order to hint the type of result of the value by the key to get
+        # (in this case - string by hinting it via default empty string '').
+        # We could use just type hinting on a variable,
+        # but we prefer the style consistent with other similar parts of this code...
+        last_known_good_version = (stable_channel.get('version', '')) or None
         platform_and_url_pairs = stable_channel.get('downloads', {}).get(
             'chromedriver', []
         )
         url_where_platform_is_os_type = next(
             iter(
+                # url is obviously a string and if absent we are interested in None
+                # emphasizing this by providing it explicitly
                 pair.get('url', None)
                 for pair in platform_and_url_pairs
-                if pair.get('platform', None) == driver_utils.get_os_type()
+                # .get_os_type() may return None, hence '' as default in get is intended
+                if pair.get('platform', '')
+                == driver_utils.get_os_type().replace('_', '-')
             ),
             None,
         )
         wdm_logger.log(
             f'latest known stable version of Chrome: {last_known_good_version}'
         )
 
         good_binary_version = last_known_good_version
         good_binary_url = url_where_platform_is_os_type
 
-    if installed_browser_version:
-        if version.parse(installed_browser_version) >= version.parse('115.0.5763.0'):
-            # patching wdm_utils.PATTERN
-            # we need all 4 sub-versions not just 3 of them
-            wdm_utils.PATTERN[ChromeType.GOOGLE] = r"\d+\.\d+\.\d+.\d+"
-            # retaking version from os after patched pattern
-            good_binary_version = wdm_utils.get_browser_version_from_os(
-                driver_utils.get_browser_type()
-            )
-            # let's reset _browser_version to the new 4-sub-versions value
-            # from here, we assume that
-            # "good" binary version is the same as "good" browser version
-            driver_utils._browser_version = good_binary_version
-
-            known_good_versions = (
-                http_client.get(
-                    chrome_apis_url('known-good-versions-with-downloads.json')
-                )
-                .json()
-                .get('versions', [])
-            )
-
-            matched_version_downloads_chromedriver_per_platform: list = next(
-                iter(
-                    info.get('downloads', {}).get('chromedriver', [])
-                    for info in known_good_versions
-                    if info.get('version', None) == good_binary_version
-                ),
-                [],
-            )
-
-            good_binary_url = next(
-                iter(
-                    info.get('url', None)
-                    for info in matched_version_downloads_chromedriver_per_platform
-                    if info.get('platform')
-                    == driver_utils.get_os_type().replace('_', '-')
-                ),
-                None,
-            )
-
     if good_binary_url:
         # it happened that we found good binary url on our own
         # let's monkey patch WDM classes and objects they know it too ;P
 
         # now we provide exactly correct and ready for download url
         driver_utils._url = good_binary_url
```

### Comparing `selene-2.0.0rc3/selene/support/_logging.py` & `selene-2.0.0rc3.post1/selene/support/_logging.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/by.py` & `selene-2.0.0rc3.post1/selene/support/by.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/conditions/be.py` & `selene-2.0.0rc3.post1/selene/support/conditions/be.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/conditions/have.py` & `selene-2.0.0rc3.post1/selene/support/conditions/have.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/conditions/not_.py` & `selene-2.0.0rc3.post1/selene/support/conditions/not_.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/shared/__init__.py` & `selene-2.0.0rc3.post1/selene/support/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/shared/browser.py` & `selene-2.0.0rc3.post1/selene/support/shared/browser.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/shared/config.py` & `selene-2.0.0rc3.post1/selene/support/shared/config.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/shared/jquery_style.py` & `selene-2.0.0rc3.post1/selene/support/shared/jquery_style.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/selene/support/webdriver.py` & `selene-2.0.0rc3.post1/selene/support/webdriver.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3/PKG-INFO` & `selene-2.0.0rc3.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selene
-Version: 2.0.0rc3
+Version: 2.0.0rc3.post1
 Summary: User-oriented browser tests in Python (Selenide port)
 Home-page: https://yashaka.github.io/selene/
 License: MIT
 Keywords: testing,selenium,selenide,browser,pageobject,widget,wrapper
 Author: Iakiv Kramarenko
 Author-email: yashaka@gmail.com
 Requires-Python: >=3.7,<4.0
```

