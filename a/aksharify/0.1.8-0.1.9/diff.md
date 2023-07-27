# Comparing `tmp/aksharify-0.1.8.tar.gz` & `tmp/aksharify-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.8.tar", max compression
+gzip compressed data, was "aksharify-0.1.9.tar", max compression
```

## Comparing `aksharify-0.1.8.tar` & `aksharify-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.8/LICENSE.md
--rw-r--r--   0        0        0      674 2023-07-26 09:26:53.034009 aksharify-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.8/README.md
--rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.8/src/aksharify/__init__.py
--rw-r--r--   0        0        0     5632 2023-07-26 09:23:20.805879 aksharify-0.1.8/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5327 2023-07-25 04:07:23.752855 aksharify-0.1.8/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1615 2023-07-24 16:06:14.067631 aksharify-0.1.8/src/aksharify/image.py
--rw-r--r--   0        0        0     1191 2023-07-25 06:47:53.889912 aksharify-0.1.8/src/aksharify/interactive.py
--rw-r--r--   0        0        0     4946 2023-07-24 12:43:24.100266 aksharify-0.1.8/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6659 1970-01-01 00:00:00.000000 aksharify-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0      674 2023-07-27 05:39:03.743172 aksharify-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5977 2023-07-26 18:35:45.363211 aksharify-0.1.9/README.md
+-rw-r--r--   0        0        0       63 2023-07-26 19:10:39.011428 aksharify-0.1.9/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     5632 2023-07-26 09:23:20.805879 aksharify-0.1.9/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5327 2023-07-25 04:07:23.752855 aksharify-0.1.9/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1615 2023-07-24 16:06:14.067631 aksharify-0.1.9/src/aksharify/image.py
+-rw-r--r--   0        0        0     1191 2023-07-25 06:47:53.889912 aksharify-0.1.9/src/aksharify/interactive.py
+-rw-r--r--   0        0        0     4946 2023-07-24 12:43:24.100266 aksharify-0.1.9/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     6648 1970-01-01 00:00:00.000000 aksharify-0.1.9/PKG-INFO
```

### Comparing `aksharify-0.1.8/LICENSE.md` & `aksharify-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.8/pyproject.toml` & `aksharify-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aksharify"
-version = "0.1.8"
+version = "0.1.9"
 description = "Ascii Art + Emoji Art python Package"
 authors = ["Prime Patel <primespatel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aksharify", from = "src"}]
 license = "MIT"
 homepage = "https://primepatel.github.io/aksharify/"
 repository = "https://github.com/primepatel/aksharify"
```

### Comparing `aksharify-0.1.8/README.md` & `aksharify-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from aksharify import AksharArt
 from aksharify.image import Image
 from aksharify.distributions import Linear
 from aksharify.outputs import SVG
 ```
 
 ```python
-image = Image("..\images\julia1.png")
+image = Image("images\julia1.png")
 image.set_dim(200)
 image.show()
 ```
 
 ```python
 lin = Linear("01")
 lin.show()
@@ -70,20 +70,20 @@
 ```python
 art = AksharArt(image, lin)
 art.aksharify(show=True)
 ```
 
 ```python
 config = SVG()
-config.file_name = "..\\art"
+config.file_name = "art"
 config.bold = True
 ```
 
 ```python
-art.svg_output(config)
+art.export(config)
 ```
 
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
```

### Comparing `aksharify-0.1.8/src/aksharify/aksharify.py` & `aksharify-0.1.9/src/aksharify/aksharify.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.8/src/aksharify/distributions.py` & `aksharify-0.1.9/src/aksharify/distributions.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.8/src/aksharify/image.py` & `aksharify-0.1.9/src/aksharify/image.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.8/src/aksharify/interactive.py` & `aksharify-0.1.9/src/aksharify/interactive.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.8/src/aksharify/outputs.py` & `aksharify-0.1.9/src/aksharify/outputs.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.8/PKG-INFO` & `aksharify-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ascii Art + Emoji Art python Package
 Home-page: https://primepatel.github.io/aksharify/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -75,15 +75,15 @@
 from aksharify import AksharArt
 from aksharify.image import Image
 from aksharify.distributions import Linear
 from aksharify.outputs import SVG
 ```
 
 ```python
-image = Image("..\images\julia1.png")
+image = Image("images\julia1.png")
 image.set_dim(200)
 image.show()
 ```
 
 ```python
 lin = Linear("01")
 lin.show()
@@ -92,20 +92,20 @@
 ```python
 art = AksharArt(image, lin)
 art.aksharify(show=True)
 ```
 
 ```python
 config = SVG()
-config.file_name = "..\\art"
+config.file_name = "art"
 config.bold = True
 ```
 
 ```python
-art.svg_output(config)
+art.export(config)
 ```
 
 _For examples from user community, please refer to the [primepatel.github.io/aksharify](https://primepatel.github.io/aksharify)_
 
 
 <!-- ROADMAP -->
 ## Roadmap
```

