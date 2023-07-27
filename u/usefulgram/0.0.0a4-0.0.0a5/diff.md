# Comparing `tmp/usefulgram-0.0.0a4.tar.gz` & `tmp/usefulgram-0.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulgram-0.0.0a4.tar", max compression
+gzip compressed data, was "usefulgram-0.0.0a5.tar", max compression
```

## Comparing `usefulgram-0.0.0a4.tar` & `usefulgram-0.0.0a5.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a4/LICENSE
--rw-r--r--   0        0        0      751 2023-07-20 13:00:49.747638 usefulgram-0.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a4/README.md
--rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a4/usefulgram/__init__.py
--rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a4/usefulgram/enums/__init__.py
--rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a4/usefulgram/enums/const.py
--rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a4/usefulgram/exceptions/__init__.py
--rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a4/usefulgram/exceptions/exceptions.py
--rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a4/usefulgram/filters/__init__.py
--rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a4/usefulgram/filters/database_filters.py
--rw-r--r--   0        0        0     5991 2023-07-20 23:26:12.344647 usefulgram-0.0.0a4/usefulgram/filters/parse_filters.py
--rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a4/usefulgram/keyboard/__init__.py
--rw-r--r--   0        0        0     3615 2023-07-20 21:15:40.376031 usefulgram-0.0.0a4/usefulgram/keyboard/builder.py
--rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a4/usefulgram/keyboard/buttons.py
--rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a4/usefulgram/keyboard/rows.py
--rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a4/usefulgram/lazy/__init__.py
--rw-r--r--   0        0        0     2066 2023-07-20 12:11:40.025890 usefulgram-0.0.0a4/usefulgram/lazy/editor.py
--rw-r--r--   0        0        0     8289 2023-07-20 23:58:44.464844 usefulgram-0.0.0a4/usefulgram/lazy/lazy_editing.py
--rw-r--r--   0        0        0     1774 2023-07-20 12:10:31.068816 usefulgram-0.0.0a4/usefulgram/lazy/sender.py
--rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a4/usefulgram/middlewares/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a4/usefulgram/middlewares/stacker.py
--rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a4/usefulgram/middlewares/trottling.py
--rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a4/usefulgram/parsing/__init__.py
--rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a4/usefulgram/parsing/decode.py
--rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a4/usefulgram/parsing/encode.py
--rw-r--r--   0        0        0       52 2023-06-18 09:35:26.952475 usefulgram-0.0.0a4/usefulgram/utils/__init__.py
--rw-r--r--   0        0        0      233 2023-06-18 09:36:46.396163 usefulgram-0.0.0a4/usefulgram/utils/autorepr.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a5/LICENSE
+-rw-r--r--   0        0        0      751 2023-07-27 00:03:27.731665 usefulgram-0.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a5/README.md
+-rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a5/usefulgram/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a5/usefulgram/enums/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a5/usefulgram/enums/const.py
+-rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a5/usefulgram/exceptions/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a5/usefulgram/exceptions/exceptions.py
+-rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a5/usefulgram/filters/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a5/usefulgram/filters/database_filters.py
+-rw-r--r--   0        0        0     6685 2023-07-26 18:02:46.375010 usefulgram-0.0.0a5/usefulgram/filters/parse_filters.py
+-rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a5/usefulgram/keyboard/__init__.py
+-rw-r--r--   0        0        0     3615 2023-07-20 21:15:40.376031 usefulgram-0.0.0a5/usefulgram/keyboard/builder.py
+-rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a5/usefulgram/keyboard/buttons.py
+-rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a5/usefulgram/keyboard/rows.py
+-rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a5/usefulgram/lazy/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-20 12:11:40.025890 usefulgram-0.0.0a5/usefulgram/lazy/editor.py
+-rw-r--r--   0        0        0     8289 2023-07-20 23:58:44.464844 usefulgram-0.0.0a5/usefulgram/lazy/lazy_editing.py
+-rw-r--r--   0        0        0     1774 2023-07-20 12:10:31.068816 usefulgram-0.0.0a5/usefulgram/lazy/sender.py
+-rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a5/usefulgram/middlewares/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a5/usefulgram/middlewares/stacker.py
+-rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a5/usefulgram/middlewares/trottling.py
+-rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a5/usefulgram/parsing/__init__.py
+-rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a5/usefulgram/parsing/decode.py
+-rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a5/usefulgram/parsing/encode.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:03:27.735654 usefulgram-0.0.0a5/usefulgram/utils/__init__.py
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a5/PKG-INFO
```

### Comparing `usefulgram-0.0.0a4/LICENSE` & `usefulgram-0.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/pyproject.toml` & `usefulgram-0.0.0a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "usefulgram"
-version = "0.0.0a4"
+version = "0.0.0a5"
 description = "Like aiogram but more easy"
 license = "MIT"
 authors = ["Alexandr Bortnik <sambonsttt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Sethis/usefulgram"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `usefulgram-0.0.0a4/README.md` & `usefulgram-0.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/exceptions/exceptions.py` & `usefulgram-0.0.0a5/usefulgram/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/filters/database_filters.py` & `usefulgram-0.0.0a5/usefulgram/filters/database_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/filters/parse_filters.py` & `usefulgram-0.0.0a5/usefulgram/filters/parse_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 
-from typing import Optional, Union, Dict, Any, Tuple
-from abc import ABC
+from typing import Optional, Union, Dict, Any, Tuple, Iterable
+from abc import ABC, abstractmethod
 
 from pydantic import BaseModel
 
 from aiogram.filters import BaseFilter
 from aiogram.types import CallbackQuery
 
 from aiogram.filters.magic_data import MagicData
@@ -53,26 +53,38 @@
             return self.__getattribute__("_magic_filter")
 
         except AttributeError:
             return None
 
 
 class _BaseDataclassesFilter(_BaseMagicFilter, ABC):
-    async def __call__(
+    @abstractmethod
+    async def __call__(self, callback: CallbackQuery, decoder: DecodeCallbackData):
+        """
+        This abstract method should use the get_filter method
+        :param callback:
+        :param decoder:
+        :return:
+        """
+        pass
+
+    async def get_filter(
             self,
             callback: CallbackQuery,
-            decoder: DecodeCallbackData) -> Union[bool, Dict[str, Any]]:
+            decoder: DecodeCallbackData,
+            fields_name: Iterable[str]
+    ) -> Union[bool, Dict[str, Any]]:
 
         try:
             callback_data_model = decoder.to_format(type(self), add_prefix=True)
 
         except (AttributeError, ValueError, IndexError):
             return False
 
-        for item_name in self.__annotations__.keys():
+        for item_name in fields_name:
             if item_name == "_magic_filter":
                 continue
 
             filter_value = self.__getattribute__(item_name)
 
             if filter_value is None:
                 continue
@@ -96,14 +108,28 @@
 
         return decoder.class_to_dict(callback_data_model)
 
 
 class BasePydanticFilter(_BaseDataclassesFilter, BaseModel, BaseFilter):
     prefix: Optional[str] = None
 
+    async def __call__(
+            self,
+            callback: CallbackQuery,
+            decoder: DecodeCallbackData
+    ) -> Union[bool, Dict[str, Any]]:
+
+        fields = self.model_fields.keys()
+
+        return await self.get_filter(
+            callback=callback,
+            decoder=decoder,
+            fields_name=fields
+        )
+
 
 class CallbackPrefixFilter(BaseFilter):
     def __init__(self, prefix: str):
         """
 
         :param prefix: first argument in callback data
         """
```

### Comparing `usefulgram-0.0.0a4/usefulgram/keyboard/builder.py` & `usefulgram-0.0.0a5/usefulgram/keyboard/builder.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/keyboard/buttons.py` & `usefulgram-0.0.0a5/usefulgram/keyboard/buttons.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/keyboard/rows.py` & `usefulgram-0.0.0a5/usefulgram/keyboard/rows.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/lazy/editor.py` & `usefulgram-0.0.0a5/usefulgram/lazy/editor.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/lazy/lazy_editing.py` & `usefulgram-0.0.0a5/usefulgram/lazy/lazy_editing.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/lazy/sender.py` & `usefulgram-0.0.0a5/usefulgram/lazy/sender.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/middlewares/stacker.py` & `usefulgram-0.0.0a5/usefulgram/middlewares/stacker.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/middlewares/trottling.py` & `usefulgram-0.0.0a5/usefulgram/middlewares/trottling.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/parsing/decode.py` & `usefulgram-0.0.0a5/usefulgram/parsing/decode.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/usefulgram/parsing/encode.py` & `usefulgram-0.0.0a5/usefulgram/parsing/encode.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a4/PKG-INFO` & `usefulgram-0.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usefulgram
-Version: 0.0.0a4
+Version: 0.0.0a5
 Summary: Like aiogram but more easy
 Home-page: https://github.com/Sethis/usefulgram
 License: MIT
 Author: Alexandr Bortnik
 Author-email: sambonsttt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

