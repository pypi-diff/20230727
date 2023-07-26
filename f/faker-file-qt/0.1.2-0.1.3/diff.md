# Comparing `tmp/faker-file-qt-0.1.2.tar.gz` & `tmp/faker-file-qt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faker-file-qt-0.1.2.tar", last modified: Tue Jul 25 22:32:00 2023, max compression
+gzip compressed data, was "faker-file-qt-0.1.3.tar", last modified: Wed Jul 26 23:00:35 2023, max compression
```

## Comparing `faker-file-qt-0.1.2.tar` & `faker-file-qt-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      807 2023-07-25 22:20:01.000000 faker-file-qt-0.1.2/CHANGELOG.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2023-07-23 20:21:53.000000 faker-file-qt-0.1.2/LICENSE.rst
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2023-07-23 20:21:53.000000 faker-file-qt-0.1.2/MANIFEST.in
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4953 2023-07-23 21:44:30.000000 faker-file-qt-0.1.2/README.rst
-drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/faker_file_qt.egg-info/
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/PKG-INFO
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      323 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/SOURCES.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/dependency_links.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       53 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/entry_points.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      114 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/requires.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-07-25 22:32:00.000000 faker-file-qt-0.1.2/faker_file_qt.egg-info/top_level.txt
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    14712 2023-07-25 22:21:33.000000 faker-file-qt-0.1.2/faker_file_qt.py
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2077 2023-07-24 20:06:13.000000 faker-file-qt-0.1.2/pyproject.toml
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      328 2023-07-25 22:32:00.769000 faker-file-qt-0.1.2/setup.cfg
--rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2051 2023-07-25 22:21:40.000000 faker-file-qt-0.1.2/setup.py
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-26 23:00:35.360399 faker-file-qt-0.1.3/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      901 2023-07-26 22:51:19.000000 faker-file-qt-0.1.3/CHANGELOG.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     1077 2023-07-23 20:21:53.000000 faker-file-qt-0.1.3/LICENSE.rst
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       61 2023-07-23 20:21:53.000000 faker-file-qt-0.1.3/MANIFEST.in
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-26 23:00:35.360399 faker-file-qt-0.1.3/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     4953 2023-07-25 22:33:15.000000 faker-file-qt-0.1.3/README.rst
+drwxrwxr-x   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        0 2023-07-26 23:00:35.360399 faker-file-qt-0.1.3/faker_file_qt.egg-info/
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     6132 2023-07-26 23:00:35.000000 faker-file-qt-0.1.3/faker_file_qt.egg-info/PKG-INFO
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      323 2023-07-26 23:00:35.000000 faker-file-qt-0.1.3/faker_file_qt.egg-info/SOURCES.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)        1 2023-07-26 23:00:35.000000 faker-file-qt-0.1.3/faker_file_qt.egg-info/dependency_links.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       53 2023-07-26 23:00:35.000000 faker-file-qt-0.1.3/faker_file_qt.egg-info/entry_points.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      122 2023-07-26 23:00:35.000000 faker-file-qt-0.1.3/faker_file_qt.egg-info/requires.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)       14 2023-07-26 23:00:35.000000 faker-file-qt-0.1.3/faker_file_qt.egg-info/top_level.txt
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)    16199 2023-07-26 22:51:19.000000 faker-file-qt-0.1.3/faker_file_qt.py
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2077 2023-07-25 22:33:15.000000 faker-file-qt-0.1.3/pyproject.toml
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)      328 2023-07-26 23:00:35.360399 faker-file-qt-0.1.3/setup.cfg
+-rw-rw-r--   0 delusionalinsanity  (1000) delusionalinsanity  (1000)     2059 2023-07-26 22:51:19.000000 faker-file-qt-0.1.3/setup.py
```

### Comparing `faker-file-qt-0.1.2/CHANGELOG.rst` & `faker-file-qt-0.1.3/CHANGELOG.rst`

 * *Files 24% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 - It's always safe to upgrade within the same minor version (for example, from
   0.3 to 0.3.4).
 - Minor version changes might be backwards incompatible. Read the
   release notes carefully before upgrading (for example, when upgrading from
   0.3.4 to 0.4).
 - All backwards incompatible changes are mentioned in this document.
 
+0.1.3
+-----
+2023-07-28
+
+- Set minimal required version of faker-file to 0.17.2.
+- Add menus.
+
 0.1.2
 -----
 2023-07-26
 
 - UI improvements.
 - Added JSON file provider.
 - Improved tests.
```

### Comparing `faker-file-qt-0.1.2/LICENSE.rst` & `faker-file-qt-0.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1.2/PKG-INFO` & `faker-file-qt-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-file-qt
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyQT UI for faker-file.
 Home-page: https://github.com/barseghyanartur/faker-file-qt/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file-qt/issues
 Project-URL: Documentation, https://faker-file-qt.readthedocs.io/
```

### Comparing `faker-file-qt-0.1.2/README.rst` & `faker-file-qt-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1.2/faker_file_qt.egg-info/PKG-INFO` & `faker-file-qt-0.1.3/faker_file_qt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faker-file-qt
-Version: 0.1.2
+Version: 0.1.3
 Summary: PyQT UI for faker-file.
 Home-page: https://github.com/barseghyanartur/faker-file-qt/
 Author: Artur Barseghyan
 Author-email: artur.barseghyan@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/barseghyanartur/faker-file-qt/issues
 Project-URL: Documentation, https://faker-file-qt.readthedocs.io/
```

### Comparing `faker-file-qt-0.1.2/faker_file_qt.py` & `faker-file-qt-0.1.3/faker_file_qt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 import inspect
 import logging
+import os
 import platform
 import subprocess
 import sys
 from typing import Any, AnyStr, Dict, List, Tuple, Union, get_args, get_origin
 
 import qdarkstyle
 from faker import Faker
@@ -54,33 +55,37 @@
 from faker_file.providers.webp_file import (
     GraphicWebpFileProvider,
     WebpFileProvider,
 )
 from faker_file.providers.xlsx_file import XlsxFileProvider
 from faker_file.providers.xml_file import XmlFileProvider
 from faker_file.providers.zip_file import ZipFileProvider
+from faker_file.storages.filesystem import FileSystemStorage
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import (
+    QAction,
     QApplication,
     QFormLayout,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QListWidget,
     QListWidgetItem,
+    QMainWindow,
+    QMessageBox,
     QPushButton,
     QSizePolicy,
     QTextEdit,
     QVBoxLayout,
     QWidget,
 )
 
-__title__ = "faker_file_qt"
-__version__ = "0.1.2"
+__title__ = "faker-file-qt"
+__version__ = "0.1.3"
 __author__ = "Artur Barseghyan <artur.barseghyan@gmail.com>"
 __copyright__ = "2022-2023 Artur Barseghyan"
 __license__ = "MIT"
 __all__ = (
     "FakerFileApp",
     "get_item_key",
     "get_label_text",
@@ -178,14 +183,16 @@
     TxtFileProvider.txt_file.__name__: TxtFileProvider,
     WebpFileProvider.webp_file.__name__: WebpFileProvider,
     XlsxFileProvider.xlsx_file.__name__: XlsxFileProvider,
     XmlFileProvider.xml_file.__name__: XmlFileProvider,
     ZipFileProvider.zip_file.__name__: ZipFileProvider,
 }
 
+STORAGE = FileSystemStorage()
+
 # Names that should show a multi-line text box
 MULTI_LINE_INPUTS = [
     "content",
     "data_columns",
     "options",
     "mp3_generator_kwargs",
     "pdf_generator_kwargs",
@@ -256,27 +263,48 @@
         subprocess.run(("open", file_path))
     elif platform.system() == "Windows":  # Windows
         subprocess.run(("start", file_path), shell=True)
     else:  # linux variants
         subprocess.run(("xdg-open", file_path))
 
 
-class FakerFileApp(QWidget):
+class FakerFileApp(QMainWindow):
     def __init__(self: "FakerFileApp") -> None:
         super().__init__()
 
         # Initialize
         self.param_widgets = {}
         self.param_annotations = {}
         self.initUI()
 
     def initUI(self: "FakerFileApp") -> None:
         # Set window size
         self.setGeometry(200, 200, 960, 720)
 
+        # Create menu bar
+        menu_bar = self.menuBar()
+
+        # Create menus
+        file_menu = menu_bar.addMenu("&File")
+        help_menu = menu_bar.addMenu("&Help")
+
+        browse_files_action = QAction("&Browse Files", self)
+        browse_files_action.setStatusTip(
+            "Open storage location using default file browser"
+        )
+        browse_files_action.triggered.connect(self.browse_files_menu_action)
+
+        about_action = QAction("&About", self)
+        about_action.setStatusTip(f"About {__title__}")
+        about_action.triggered.connect(self.about_message_menu_action)
+
+        # Add actions to menus
+        file_menu.addAction(browse_files_action)
+        help_menu.addAction(about_action)
+
         # Create a QHBoxLayout
         layout = QHBoxLayout()
 
         self.list_widget = QListWidget()
         self.list_widget.itemClicked.connect(self.show_form)
         list_group = QGroupBox("File type")  # create a group box
         list_layout = QVBoxLayout()  # create a layout for the group box
@@ -314,14 +342,35 @@
         self.list_widget.itemClicked.emit(self.list_widget.currentItem())
 
         layout.addWidget(list_group, -1)
         layout.addWidget(form_group, 3)
         layout.addWidget(result_group, 3)
         self.setLayout(layout)
 
+        self.setCentralWidget(
+            QWidget()
+        )  # QMainWindow requires a central widget
+        self.centralWidget().setLayout(layout)
+
+    def about_message_menu_action(self):
+        QMessageBox.about(
+            self,
+            f"About {__title__}",
+            (
+                f"{__title__} version {__version__}.\n\n"
+                f"Author: {__author__}\n"
+                f"License: {__license__}\n"
+            ),
+        )
+
+    def browse_files_menu_action(self):
+        open_file_with_default_app(
+            os.path.join(STORAGE.root_path, STORAGE.rel_path)
+        )
+
     def show_form(self: "FakerFileApp", item: "QListWidgetItem") -> None:
         file_type = get_item_key(item)
         provider = PROVIDERS[file_type]
 
         method = getattr(provider(FAKER), file_type)
         method_specs = inspect.getfullargspec(method)
```

### Comparing `faker-file-qt-0.1.2/pyproject.toml` & `faker-file-qt-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `faker-file-qt-0.1.2/setup.py` & `faker-file-qt-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 
 from setuptools import setup
 
-version = "0.1.2"
+version = "0.1.3"
 
 try:
     readme = open(os.path.join(os.path.dirname(__file__), "README.rst")).read()
 except OSError:
     readme = ""
 
 install_requires = [
     "Faker",
-    "faker-file[common]",
+    "faker-file[common]>=0.17.2",
     "QDarkStyle",
     "PyQt5",
-    "Pillow<=9.5.0",
+    "Pillow<10.0.0",
 ]
 
 extras_require = {
     "dev": [
         "black",
         "detect-secrets",
         "doc8",
```

