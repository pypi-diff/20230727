# Comparing `tmp/usefulgram-0.0.0a6.tar.gz` & `tmp/usefulgram-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulgram-0.0.0a6.tar", max compression
+gzip compressed data, was "usefulgram-0.0.0a7.tar", max compression
```

## Comparing `usefulgram-0.0.0a6.tar` & `usefulgram-0.0.0a7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a6/LICENSE
--rw-r--r--   0        0        0      751 2023-07-27 00:49:17.178696 usefulgram-0.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a6/README.md
--rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a6/usefulgram/__init__.py
--rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a6/usefulgram/enums/__init__.py
--rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a6/usefulgram/enums/const.py
--rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a6/usefulgram/exceptions/__init__.py
--rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a6/usefulgram/exceptions/exceptions.py
--rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a6/usefulgram/filters/__init__.py
--rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a6/usefulgram/filters/database_filters.py
--rw-r--r--   0        0        0     6685 2023-07-26 18:02:46.375010 usefulgram-0.0.0a6/usefulgram/filters/parse_filters.py
--rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a6/usefulgram/keyboard/__init__.py
--rw-r--r--   0        0        0     3698 2023-07-27 00:47:38.667882 usefulgram-0.0.0a6/usefulgram/keyboard/builder.py
--rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a6/usefulgram/keyboard/buttons.py
--rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a6/usefulgram/keyboard/rows.py
--rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a6/usefulgram/lazy/__init__.py
--rw-r--r--   0        0        0     2066 2023-07-20 12:11:40.025890 usefulgram-0.0.0a6/usefulgram/lazy/editor.py
--rw-r--r--   0        0        0     8289 2023-07-20 23:58:44.464844 usefulgram-0.0.0a6/usefulgram/lazy/lazy_editing.py
--rw-r--r--   0        0        0     1774 2023-07-20 12:10:31.068816 usefulgram-0.0.0a6/usefulgram/lazy/sender.py
--rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a6/usefulgram/middlewares/__init__.py
--rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a6/usefulgram/middlewares/stacker.py
--rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a6/usefulgram/middlewares/trottling.py
--rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a6/usefulgram/parsing/__init__.py
--rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a6/usefulgram/parsing/decode.py
--rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a6/usefulgram/parsing/encode.py
--rw-r--r--   0        0        0        0 2023-07-27 00:03:27.735654 usefulgram-0.0.0a6/usefulgram/utils/__init__.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-07 20:49:54.066720 usefulgram-0.0.0a7/LICENSE
+-rw-r--r--   0        0        0      751 2023-07-27 00:55:19.909963 usefulgram-0.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     3053 2023-07-21 00:40:55.695271 usefulgram-0.0.0a7/README.md
+-rw-r--r--   0        0        0      247 2023-07-12 21:45:25.235118 usefulgram-0.0.0a7/usefulgram/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-07 21:21:58.969929 usefulgram-0.0.0a7/usefulgram/enums/__init__.py
+-rw-r--r--   0        0        0      289 2023-07-20 23:58:44.461878 usefulgram-0.0.0a7/usefulgram/enums/const.py
+-rw-r--r--   0        0        0      309 2023-07-20 23:10:48.507629 usefulgram-0.0.0a7/usefulgram/exceptions/__init__.py
+-rw-r--r--   0        0        0      869 2023-07-20 23:10:48.511619 usefulgram-0.0.0a7/usefulgram/exceptions/exceptions.py
+-rw-r--r--   0        0        0      168 2023-07-07 21:21:58.956995 usefulgram-0.0.0a7/usefulgram/filters/__init__.py
+-rw-r--r--   0        0        0      784 2023-06-25 19:32:18.676643 usefulgram-0.0.0a7/usefulgram/filters/database_filters.py
+-rw-r--r--   0        0        0     6685 2023-07-26 18:02:46.375010 usefulgram-0.0.0a7/usefulgram/filters/parse_filters.py
+-rw-r--r--   0        0        0      123 2023-07-20 20:45:03.943904 usefulgram-0.0.0a7/usefulgram/keyboard/__init__.py
+-rw-r--r--   0        0        0     3673 2023-07-27 00:54:59.805545 usefulgram-0.0.0a7/usefulgram/keyboard/builder.py
+-rw-r--r--   0        0        0     2761 2023-07-20 20:15:49.534299 usefulgram-0.0.0a7/usefulgram/keyboard/buttons.py
+-rw-r--r--   0        0        0      515 2023-07-20 20:15:49.549286 usefulgram-0.0.0a7/usefulgram/keyboard/rows.py
+-rw-r--r--   0        0        0       43 2023-07-07 21:21:58.939012 usefulgram-0.0.0a7/usefulgram/lazy/__init__.py
+-rw-r--r--   0        0        0     2066 2023-07-20 12:11:40.025890 usefulgram-0.0.0a7/usefulgram/lazy/editor.py
+-rw-r--r--   0        0        0     8289 2023-07-20 23:58:44.464844 usefulgram-0.0.0a7/usefulgram/lazy/lazy_editing.py
+-rw-r--r--   0        0        0     1774 2023-07-20 12:10:31.068816 usefulgram-0.0.0a7/usefulgram/lazy/sender.py
+-rw-r--r--   0        0        0       89 2023-07-07 21:21:58.945022 usefulgram-0.0.0a7/usefulgram/middlewares/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-20 23:55:38.146961 usefulgram-0.0.0a7/usefulgram/middlewares/stacker.py
+-rw-r--r--   0        0        0     1510 2023-07-19 23:25:39.503139 usefulgram-0.0.0a7/usefulgram/middlewares/trottling.py
+-rw-r--r--   0        0        0       44 2023-07-07 21:21:58.963945 usefulgram-0.0.0a7/usefulgram/parsing/__init__.py
+-rw-r--r--   0        0        0     3946 2023-07-20 21:32:27.645449 usefulgram-0.0.0a7/usefulgram/parsing/decode.py
+-rw-r--r--   0        0        0     2774 2023-07-19 21:09:49.679939 usefulgram-0.0.0a7/usefulgram/parsing/encode.py
+-rw-r--r--   0        0        0        0 2023-07-27 00:03:27.735654 usefulgram-0.0.0a7/usefulgram/utils/__init__.py
+-rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 usefulgram-0.0.0a7/PKG-INFO
```

### Comparing `usefulgram-0.0.0a6/LICENSE` & `usefulgram-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/pyproject.toml` & `usefulgram-0.0.0a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "usefulgram"
-version = "0.0.0a6"
+version = "0.0.0a7"
 description = "Like aiogram but more easy"
 license = "MIT"
 authors = ["Alexandr Bortnik <sambonsttt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/Sethis/usefulgram"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `usefulgram-0.0.0a6/README.md` & `usefulgram-0.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/exceptions/exceptions.py` & `usefulgram-0.0.0a7/usefulgram/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/filters/database_filters.py` & `usefulgram-0.0.0a7/usefulgram/filters/database_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/filters/parse_filters.py` & `usefulgram-0.0.0a7/usefulgram/filters/parse_filters.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/keyboard/builder.py` & `usefulgram-0.0.0a7/usefulgram/keyboard/builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
         buttons: list[T] = []
 
         for button_row in rows:
             for button in button_row:
                 buttons.append(button)
 
         rows_len = len(buttons)
-        print(rows_len)
 
         result: list[list[T]] = []
         row: list[T] = []
 
         for index in range(0, rows_len):
             row.append(buttons[index])
```

### Comparing `usefulgram-0.0.0a6/usefulgram/keyboard/buttons.py` & `usefulgram-0.0.0a7/usefulgram/keyboard/buttons.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/keyboard/rows.py` & `usefulgram-0.0.0a7/usefulgram/keyboard/rows.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/lazy/editor.py` & `usefulgram-0.0.0a7/usefulgram/lazy/editor.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/lazy/lazy_editing.py` & `usefulgram-0.0.0a7/usefulgram/lazy/lazy_editing.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/lazy/sender.py` & `usefulgram-0.0.0a7/usefulgram/lazy/sender.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/middlewares/stacker.py` & `usefulgram-0.0.0a7/usefulgram/middlewares/stacker.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/middlewares/trottling.py` & `usefulgram-0.0.0a7/usefulgram/middlewares/trottling.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/parsing/decode.py` & `usefulgram-0.0.0a7/usefulgram/parsing/decode.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/usefulgram/parsing/encode.py` & `usefulgram-0.0.0a7/usefulgram/parsing/encode.py`

 * *Files identical despite different names*

### Comparing `usefulgram-0.0.0a6/PKG-INFO` & `usefulgram-0.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usefulgram
-Version: 0.0.0a6
+Version: 0.0.0a7
 Summary: Like aiogram but more easy
 Home-page: https://github.com/Sethis/usefulgram
 License: MIT
 Author: Alexandr Bortnik
 Author-email: sambonsttt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
```

