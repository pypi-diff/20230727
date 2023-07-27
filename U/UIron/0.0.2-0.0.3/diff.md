# Comparing `tmp/UIron-0.0.2.tar.gz` & `tmp/UIron-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UIron-0.0.2.tar", last modified: Thu Jul 27 16:01:11 2023, max compression
+gzip compressed data, was "UIron-0.0.3.tar", last modified: Thu Jul 27 16:58:54 2023, max compression
```

## Comparing `UIron-0.0.2.tar` & `UIron-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 16:01:11.622731 UIron-0.0.2/
--rw-rw-rw-   0        0        0     1088 2023-07-27 02:09:14.000000 UIron-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      460 2023-07-27 16:01:11.622731 UIron-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 16:01:11.566819 UIron-0.0.2/UIron/
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.2/UIron/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.2/UIron/__main__.py
--rw-rw-rw-   0        0        0      896 2023-07-27 15:57:26.000000 UIron-0.0.2/UIron/config.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:01:11.622731 UIron-0.0.2/UIron/data/
--rw-rw-rw-   0        0        0       60 2023-07-27 15:44:11.000000 UIron-0.0.2/UIron/data/config.json
--rw-rw-rw-   0        0        0     1901 2023-07-27 15:32:53.000000 UIron-0.0.2/UIron/gui.py
--rw-rw-rw-   0        0        0        0 2023-07-27 15:59:43.000000 UIron-0.0.2/UIron/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:01:11.622731 UIron-0.0.2/UIron.egg-info/
--rw-rw-rw-   0        0        0      460 2023-07-27 16:01:11.000000 UIron-0.0.2/UIron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-07-27 16:01:11.000000 UIron-0.0.2/UIron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 16:01:11.000000 UIron-0.0.2/UIron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-27 16:01:11.000000 UIron-0.0.2/UIron.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-27 16:01:11.000000 UIron-0.0.2/UIron.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 16:01:11.622731 UIron-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      789 2023-07-27 16:01:10.000000 UIron-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.892322 UIron-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2023-07-27 02:09:14.000000 UIron-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      460 2023-07-27 16:58:54.892322 UIron-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.856345 UIron-0.0.3/UIron/
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.3/UIron/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-27 02:09:14.000000 UIron-0.0.3/UIron/__main__.py
+-rw-rw-rw-   0        0        0     1269 2023-07-27 16:14:37.000000 UIron-0.0.3/UIron/config.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.892322 UIron-0.0.3/UIron/data/
+-rw-rw-rw-   0        0        0       10 2023-07-27 16:47:20.000000 UIron-0.0.3/UIron/data/config.json
+-rw-rw-rw-   0        0        0     1897 2023-07-27 16:50:20.000000 UIron-0.0.3/UIron/gui.py
+-rw-rw-rw-   0        0        0      958 2023-07-27 16:49:06.000000 UIron-0.0.3/UIron/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-27 16:58:54.882187 UIron-0.0.3/UIron.egg-info/
+-rw-rw-rw-   0        0        0      460 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-27 16:58:54.000000 UIron-0.0.3/UIron.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 16:58:54.892322 UIron-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-07-27 16:58:53.000000 UIron-0.0.3/setup.py
```

### Comparing `UIron-0.0.2/LICENSE` & `UIron-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UIron-0.0.2/UIron/gui.py` & `UIron-0.0.3/UIron/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,15 @@
         super().__init__(master, **kwargs)
 
         # PROPERTIES
         self.base_string = 'Ready to continue...'
         self.text = ttk.StringVar()
         self.text_label = ttk.Label(self, textvariable=self.text)
         self.text_label.pack(anchor='w', padx=10)
-
         self.raise_notification = raise_notification
-
         self.reset()
     
     def raise_notification(self, text: str, type_: str) -> None:
         """Raises a notificacion, is a template"""
         style = 'danger' if type_ == 'error' else type_
         self.config(bootstyle=style)
         self.text_label.config(bootstyle=f'{style}-inverse')
```

### Comparing `UIron-0.0.2/setup.py` & `UIron-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "Package for User Interface"
 LONG_DESCRIPTION = "Package for User Interface"
 
 setup(
     name="UIron",
     version=VERSION,
     author="Armando Chaparro",
```

