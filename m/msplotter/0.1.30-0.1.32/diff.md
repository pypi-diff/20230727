# Comparing `tmp/msplotter-0.1.30.tar.gz` & `tmp/msplotter-0.1.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msplotter-0.1.30.tar", last modified: Mon Jul 24 18:43:42 2023, max compression
+gzip compressed data, was "msplotter-0.1.32.tar", last modified: Thu Jul 27 15:52:58 2023, max compression
```

## Comparing `msplotter-0.1.30.tar` & `msplotter-0.1.32.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.851086 msplotter-0.1.30/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.30/LICENSE
--rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-24 18:43:42.850517 msplotter-0.1.30/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)     4123 2023-07-22 19:56:11.000000 msplotter-0.1.30/README.md
--rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-22 00:36:53.000000 msplotter-0.1.30/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-24 18:43:42.851261 msplotter-0.1.30/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.808425 msplotter-0.1.30/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.825260 msplotter-0.1.30/src/msp/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.30/src/msp/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.30/src/msp/__main__.py
--rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.30/src/msp/arrows.py
--rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.30/src/msp/colormap_picker.py
--rw-r--r--   0 msp        (501) staff       (20)    19061 2023-07-24 05:29:03.000000 msplotter-0.1.30/src/msp/gui.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.846279 msplotter-0.1.30/src/msp/images/
--rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.30/src/msp/images/Blues.png
--rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/BuGn.png
--rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/BuPu.png
--rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/GnBu.png
--rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Greens.png
--rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Greys.png
--rw-r--r--   0 msp        (501) staff       (20)   353491 2023-07-22 04:33:21.000000 msplotter-0.1.30/src/msp/images/MSPlotter_gui.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/OrRd.png
--rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Oranges.png
--rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/PuBu.png
--rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/PuBuGn.png
--rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/PuRd.png
--rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Purples.png
--rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/RdPu.png
--rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Reds.png
--rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlGn.png
--rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlGnBu.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlOrBr.png
--rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlOrRd.png
--rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/logo.png
--rw-r--r--   0 msp        (501) staff       (20)    36197 2023-07-24 05:39:10.000000 msplotter-0.1.30/src/msp/msplotter.py
--rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.30/src/msp/plot.py
--rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.30/src/msp/slider_widget.py
--rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.30/src/msp/spinbox.py
--rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.30/src/msp/user_input.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.849731 msplotter-0.1.30/src/msplotter.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      966 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.242394 msplotter-0.1.32/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.32/LICENSE
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-27 15:52:58.241084 msplotter-0.1.32/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)     4123 2023-07-22 19:56:11.000000 msplotter-0.1.32/README.md
+-rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-27 15:24:07.000000 msplotter-0.1.32/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-27 15:52:58.242534 msplotter-0.1.32/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.205446 msplotter-0.1.32/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.217405 msplotter-0.1.32/src/msp/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.32/src/msp/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.32/src/msp/__main__.py
+-rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.32/src/msp/arrows.py
+-rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.32/src/msp/colormap_picker.py
+-rw-r--r--   0 msp        (501) staff       (20)    20747 2023-07-27 15:24:07.000000 msplotter-0.1.32/src/msp/gui.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.235094 msplotter-0.1.32/src/msp/images/
+-rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.32/src/msp/images/Blues.png
+-rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/BuGn.png
+-rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/BuPu.png
+-rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/GnBu.png
+-rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Greens.png
+-rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Greys.png
+-rw-r--r--   0 msp        (501) staff       (20)   353491 2023-07-22 04:33:21.000000 msplotter-0.1.32/src/msp/images/MSPlotter_gui.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/OrRd.png
+-rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Oranges.png
+-rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/PuBu.png
+-rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/PuBuGn.png
+-rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/PuRd.png
+-rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Purples.png
+-rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/RdPu.png
+-rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/Reds.png
+-rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlGn.png
+-rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlGnBu.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlOrBr.png
+-rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/YlOrRd.png
+-rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.32/src/msp/images/logo.png
+-rw-r--r--   0 msp        (501) staff       (20)    36197 2023-07-24 05:39:10.000000 msplotter-0.1.32/src/msp/msplotter.py
+-rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.32/src/msp/plot.py
+-rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.32/src/msp/slider_widget.py
+-rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.32/src/msp/spinbox.py
+-rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.32/src/msp/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-27 15:52:58.239799 msplotter-0.1.32/src/msplotter.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      966 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-27 15:52:58.000000 msplotter-0.1.32/src/msplotter.egg-info/top_level.txt
```

### Comparing `msplotter-0.1.30/LICENSE` & `msplotter-0.1.32/LICENSE`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/PKG-INFO` & `msplotter-0.1.32/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.30
+Version: 0.1.32
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.30/README.md` & `msplotter-0.1.32/README.md`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/pyproject.toml` & `msplotter-0.1.32/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msplotter"
-version = "0.1.30"
+version = "0.1.32"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Make a graphical representation of a blastn alignment"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
```

### Comparing `msplotter-0.1.30/src/msp/arrows.py` & `msplotter-0.1.32/src/msp/arrows.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/colormap_picker.py` & `msplotter-0.1.32/src/msp/colormap_picker.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/gui.py` & `msplotter-0.1.32/src/msp/gui.py`

 * *Files 21% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         # if self.annotate_sequences is True, self.sequence_name is used for
         # annotating the sequences.
         self.sequence_name: str = "accession"
         self.annotate_genes: bool = False
         self.annotate_genes_from: str = "gene_tag"
 
         # -- Set layout parameters --------------------------------------------
-        self.geometry('750x600')
+        self.geometry('850x500')
         self.title('MSPlotter')
         self.grid_rowconfigure(1, weight=1)
         self.grid_columnconfigure((2,3), weight=1)
         self.grid_columnconfigure((0,1), weight=0)
         # Protocol to close app, including plot if exist.
         self.protocol('WM_DELETE_WINDOW', self.on_closing)
         # Variable to store the ColormapPicker class used in the
@@ -50,15 +50,15 @@
         # -- Navigation frame -------------------------------------------------
         # Create navigation frame.
         self.navigation_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.navigation_frame.grid(row=0, column=0, columnspan=4, sticky='nsew')
         self.navigation_frame.grid_columnconfigure(0, weight=1)
         # Logo label
         self.logo_label = customtkinter.CTkLabel(
-            self.navigation_frame, text='MSPloter',
+            self.navigation_frame, text='MSPlotter',
             font=customtkinter.CTkFont(size=24, weight='bold')
         )
         self.logo_label.grid(row=0, column=0, padx=(10,5), pady=20)
         # Select button
         self.select_button = customtkinter.CTkButton(
             self.navigation_frame, text='Select',
             command=self.get_files_path
@@ -84,167 +84,203 @@
         # -- Appearance frame -------------------------------------------------
         self.appearance_frame = customtkinter.CTkFrame(
             self, corner_radius=5,
         )
         self.appearance_frame.grid(
             row=1, column=0, columnspan=2, padx=(10, 5), pady=10, sticky='nsew'
         )
-        self.appearance_frame.grid_rowconfigure(9, weight=1)
+        self.appearance_frame.grid_rowconfigure(2, weight=1)
         self.appearance_frame.grid_columnconfigure((0,1), weight=0)
         # Appearance label
         self.appearance_label = customtkinter.CTkLabel(
             self.appearance_frame,
             text='Appearance',
             font=customtkinter.CTkFont(size=18, weight='bold'),
             width=120,
             height=50,
             corner_radius=5,
             # fg_color=self.appearance_fg_color,
         )
         self.appearance_label.grid(
-            row=0, column=0, columnspan=2, pady=(10,10), sticky='nswe'
+            row=0, column=0, columnspan=2, sticky='nswe'
         )
+        # Reset button
+        self.reset_button = customtkinter.CTkButton(
+            self.appearance_frame, text='Reset', fg_color='transparent',
+            text_color=('gray10', '#DCE4EE'), border_width=2,
+            command=self.reset_appearance
+        )
+        self.reset_button.grid(row=2, column=0, columnspan=2)
+        # -----> Tabview General <----- #
+        self.tabview = customtkinter.CTkTabview(
+            self.appearance_frame, width=380, height=300
+        )
+        self.tabview.grid(
+            row=1, column=0, columnspan=2, pady=(0, 10), padx=(10, 10), sticky='nsew'
+        )
+        self.tabview.add('General')
+        # self.tabview.tab('General').grid_rowconfigure(0, weight=1)
+        # self.tabview.tab('General').grid_columnconfigure((0,1), weight=0)
         # Align plot label
         self.align_plot_label = customtkinter.CTkLabel(
-            self.appearance_frame, text='Align plot:'
+            self.tabview.tab('General'), text='Align plot:'
         )
         self.align_plot_label.grid(row=1, column=0, pady=(10, 0))
         # Variable to store align_plot menu selection
         self.align_plot_var = customtkinter.StringVar(self, 'Left')
         # Align plot menu
         self.align_plot = customtkinter.CTkOptionMenu(
-            self.appearance_frame,
+            self.tabview.tab('General'),
             values=['Left', 'Center', 'Right'],
             variable=self.align_plot_var,
         )
         self.align_plot.grid(row=2, column=0, padx=20, pady=(0, 10))
         # Annotate sequences label
         self.annotate_seq_label = customtkinter.CTkLabel(
-            self.appearance_frame, text='Annotate sequences:'
+            self.tabview.tab('General'), text='Annotate sequences:'
         )
         self.annotate_seq_label.grid(row=3, column=0, pady=(10, 0))
         # Variable to store annotate_seq menu selection
         self.annotate_seq_var = customtkinter.StringVar(self, 'No')
         # Annotate sequences menu
         self.annotate_seq_menu = customtkinter.CTkOptionMenu(
-            self.appearance_frame,
+            self.tabview.tab('General'),
             values=['No', 'From acc number', 'From file name'],
             variable=self.annotate_seq_var,
             command=lambda _:self.update_annotate_seq()
         )
         self.annotate_seq_menu.grid(row=4, column=0, pady=(0,10))
         # Annotate genes label
         self.annotate_genes_label = customtkinter.CTkLabel(
-            self.appearance_frame, text='Annotate genes:'
+            self.tabview.tab('General'), text='Annotate genes:'
         )
         self.annotate_genes_label.grid(row=5, column=0, pady=(10,0))
         # Variable to store annotate_genes menu selection
         self.annotate_genes_var = customtkinter.StringVar(self, 'No')
         # Annotate genes menu
         self.annotate_genes_menu = customtkinter.CTkOptionMenu(
-            self.appearance_frame,
+            self.tabview.tab('General'),
             values=['No', 'From gene tag', 'From product tag'],
             variable=self.annotate_genes_var,
             command=lambda _:self.update_annotate_genes()
         )
         self.annotate_genes_menu.grid(row=6, column=0, pady=(0,10))
         # Homology color label
         self.homology_label = customtkinter.CTkLabel(
-            self.appearance_frame, text='Homology color:',
+            self.tabview.tab('General'), text='Homology color:',
         )
         self.homology_label.grid(row=1, column=1, pady=(10,0))
         # Colormap picker
         self.format_button = customtkinter.CTkButton(
-            self.appearance_frame,
+            self.tabview.tab('General'),
             text='Choose colormap',
             command=self.launch_colormap_picker
         )
         self.format_button.grid(row=2, column=1, padx=20, pady=(0, 10))
         # Scale bar label
         self.scale_bar_label = customtkinter.CTkLabel(
-            self.appearance_frame, text='Scale bar:'
+            self.tabview.tab('General'), text='Scale bar:'
         )
         self.scale_bar_label.grid(row=3, column=1, pady=(10,0))
         # Variable to store scale_bar menu selection
         self.scale_bar_var = customtkinter.StringVar(self, 'No')
         # Scale bar menu
         self.scale_bar_menu = customtkinter.CTkOptionMenu(
-            self.appearance_frame,
+            self.tabview.tab('General'),
             values=['No', 'Yes'],
             variable=self.scale_bar_var,
             command=lambda _:self.update_scale_bar()
         )
         self.scale_bar_menu.grid(row=4, column=1, pady=(0,10))
         # Color map position label
         self.cmap_position_label = customtkinter.CTkLabel(
-            self.appearance_frame, text='Position colormap:'
+            self.tabview.tab('General'), text='Position colormap:'
         )
         self.cmap_position_label.grid(row=5, column=1, pady=(10, 0))
         # Color map position spinbox
         self.cmap_position_spinbox = FloatSpinbox(
-            self.appearance_frame,
+            self.tabview.tab('General'),
             width=140,
             height=28,
             command=self.update_y_limit
         )
         self.cmap_position_spinbox.grid(row=6, column=1, pady=(0, 10))
+        # -----> Tabview Size <----- #
+        self.tabview.add('Size')
+        self.size_textbox = customtkinter.CTkTextbox(
+            self.tabview.tab('Size'), wrap='word', fg_color='transparent',
+            height=110
+        )
+        self.size_textbox.grid(
+            row=0, column=0, columnspan=2, padx=(10,0), pady=(5, 0),
+            sticky='nsew'
+        )
+        self.size_textbox.insert(
+            'end',
+            'MSPlotter adjusts the size automatically.\n'
+            'A plot with four or less alignments has a size of 6.4 x 4.8 '
+            'inches.\n\n'
+            "If your plot looks congested, change the figure size."
+        )
+        # self.size_textbox.tag_config('justified', justify="center")
+        # self.size_textbox.tag_add('justified', '1.0', 'end')
+        self.size_textbox.configure(state='disabled')
+        # Enter data label
+        self.enter_data_label = customtkinter.CTkLabel(
+            self.tabview.tab('Size'), text='Enter values in inches'
+        )
+        self.enter_data_label.grid(
+            row=1, column=0, columnspan=2, sticky='we', pady=(5, 5)
+        )
         # Create a validation function to check for float input in entry boxes
         self.validation = self.register(self.validate_input)
         # Change width check box variable
         self.width_check_var = customtkinter.StringVar(value='off')
         # Change width check box
         self.width_check = customtkinter.CTkCheckBox(
-            self.appearance_frame,
+            self.tabview.tab('Size'),
             text='Change figure width:',
             variable=self.width_check_var,
             onvalue='on',
             offvalue='off',
             command=self.change_figure_width_event
         )
         self.width_check.grid(
-            row=7, column=0, sticky='w', padx=(10,0), pady=(20, 10))
+            row=2, column=0, sticky='w', padx=(10,0), pady=(5, 10))
         # Change width entry box
         self.width_entry = customtkinter.CTkEntry(
-            self.appearance_frame,
+            self.tabview.tab('Size'),
             validate='key',
             validatecommand=(self.validation, '%P'),
         )
         self.width_entry.grid(
-            row=7, column=1, sticky='we', padx=(0,10), pady=(20, 10))
+            row=2, column=1, sticky='we', padx=(0,10), pady=(0, 10))
         self.width_entry.configure(state='disabled')
         # Change height check box variable
         self.height_check_var = customtkinter.StringVar(value='off')
         # Change height check box
         self.height_check = customtkinter.CTkCheckBox(
-            self.appearance_frame,
+            self.tabview.tab('Size'),
             text='Change figure height:',
             variable=self.height_check_var,
             onvalue='on',
             offvalue='off',
             command=self.change_figure_height_event
         )
         self.height_check.grid(
-            row=8, column=0, sticky='w', padx=(10,0), pady=(10))
+            row=3, column=0, sticky='w', padx=(10,5), pady=(10))
         # Change height entry box
         self.height_entry = customtkinter.CTkEntry(
-            self.appearance_frame,
+            self.tabview.tab('Size'),
             validate='key',
             validatecommand=(self.validation, '%P'),
         )
         self.height_entry.grid(
-            row=8, column=1, sticky='we', padx=(0,10), pady=(10))
+            row=3, column=1, sticky='we', padx=(0,10), pady=(10))
         self.height_entry.configure(state='disabled')
-        # Reset button
-        self.reset_button = customtkinter.CTkButton(
-            self.appearance_frame, text='Reset', fg_color='transparent',
-            text_color=('gray10', '#DCE4EE'), border_width=2,
-            command=self.reset_appearance
-        )
-        self.reset_button.grid(row=9, column=0, columnspan=2, pady=(10, 10))
-
         # -- Display frame ---------------------------------------------------
         # Create display frame
         self.display_frame = customtkinter.CTkFrame(
             self, corner_radius=0,
             fg_color='transparent'
         )
         self.display_frame.grid(row=1, column=2, columnspan=2, sticky='nsew')
@@ -254,15 +290,15 @@
             self.display_frame, wrap='word'
         )
         self.display_window.grid(row=0, column=0, padx=(5, 10), pady=10,
             sticky='nsew'
         )
         self.display_window.insert(
             'end',
-            '\n\n\n\nWelcome to MSPlotter!\n\n' +
+            '\n\n\n\nWelcome to MSPlotter!\n\n'
             'Select your GenBank sequences, plot, and save.\n\n'
             "If you don't like the default parameters, change the appearance."
         )
         self.display_window.configure(state='disabled')
 
     # =========================================================================
     # Functionality
@@ -455,17 +491,17 @@
             sequence_name=self.sequence_name,
             annotate_genes=self.annotate_genes,
             annotate_genes_from=self.annotate_genes_from,
             scale_bar=self.scale_bar,
             y_limit=self.y_limit,
             use_gui=True
         )
-        # Plot figure using the Plot class
+        # Make figure with matplotlib via MakeFigure class.
         self.figure_plt = self.figure_msp.make_figure()
-        # Plot figure
+        # Plot using FigureCanvasTkAgg via Plot class.
         Plot(self.figure_plt, self.figure_msp)
 
     def on_closing(self):
         if self.figure_plt is not None:
             self.figure_msp.close_figure()
         self.quit()
         self.destroy()
```

### Comparing `msplotter-0.1.30/src/msp/images/Blues.png` & `msplotter-0.1.32/src/msp/images/Blues.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/BuGn.png` & `msplotter-0.1.32/src/msp/images/BuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/BuPu.png` & `msplotter-0.1.32/src/msp/images/BuPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/GnBu.png` & `msplotter-0.1.32/src/msp/images/GnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/Greens.png` & `msplotter-0.1.32/src/msp/images/Greens.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/MSPlotter_gui.png` & `msplotter-0.1.32/src/msp/images/MSPlotter_gui.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/OrRd.png` & `msplotter-0.1.32/src/msp/images/OrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/Oranges.png` & `msplotter-0.1.32/src/msp/images/Oranges.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/PuBu.png` & `msplotter-0.1.32/src/msp/images/PuBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/PuBuGn.png` & `msplotter-0.1.32/src/msp/images/PuBuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/PuRd.png` & `msplotter-0.1.32/src/msp/images/PuRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/Purples.png` & `msplotter-0.1.32/src/msp/images/Purples.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/RdPu.png` & `msplotter-0.1.32/src/msp/images/RdPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/Reds.png` & `msplotter-0.1.32/src/msp/images/Reds.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/YlGn.png` & `msplotter-0.1.32/src/msp/images/YlGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/YlGnBu.png` & `msplotter-0.1.32/src/msp/images/YlGnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/YlOrBr.png` & `msplotter-0.1.32/src/msp/images/YlOrBr.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/YlOrRd.png` & `msplotter-0.1.32/src/msp/images/YlOrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/images/logo.png` & `msplotter-0.1.32/src/msp/images/logo.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/msplotter.py` & `msplotter-0.1.32/src/msp/msplotter.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/plot.py` & `msplotter-0.1.32/src/msp/plot.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/slider_widget.py` & `msplotter-0.1.32/src/msp/slider_widget.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/spinbox.py` & `msplotter-0.1.32/src/msp/spinbox.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msp/user_input.py` & `msplotter-0.1.32/src/msp/user_input.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.30/src/msplotter.egg-info/PKG-INFO` & `msplotter-0.1.32/src/msplotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.30
+Version: 0.1.32
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.30/src/msplotter.egg-info/SOURCES.txt` & `msplotter-0.1.32/src/msplotter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

