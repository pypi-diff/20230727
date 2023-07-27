# Comparing `tmp/minlog-0.3.0.tar.gz` & `tmp/minlog-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minlog-0.3.0.tar", max compression
+gzip compressed data, was "minlog-0.3.1.tar", max compression
```

## Comparing `minlog-0.3.0.tar` & `minlog-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.3.0/README.md
--rw-r--r--   0        0        0     4869 2023-07-27 05:55:47.270050 minlog-0.3.0/minlog/__init__.py
--rw-r--r--   0        0        0      523 2023-07-27 05:52:40.500198 minlog-0.3.0/minlog/_test.py
--rw-r--r--   0        0        0      297 2023-07-27 05:36:03.383457 minlog-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 minlog-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.3.1/README.md
+-rw-r--r--   0        0        0     4947 2023-07-27 06:10:47.792342 minlog-0.3.1/minlog/__init__.py
+-rw-r--r--   0        0        0      523 2023-07-27 05:52:40.500198 minlog-0.3.1/minlog/_test.py
+-rw-r--r--   0        0        0      297 2023-07-27 06:11:00.115657 minlog-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 minlog-0.3.1/PKG-INFO
```

### Comparing `minlog-0.3.0/minlog/__init__.py` & `minlog-0.3.1/minlog/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,16 +72,17 @@
         # then print the message
         meta_str = f"{self.short_verbosity(message_verbosity)}"
         message_str = message
 
         if self.backend == Backend.RICH:
             # mprint(message)
             meta_style_rich = self.get_style_rich(message_verbosity)
-            self.rich_console.print(f"\[{meta_str}]", style=meta_style_rich, end=" ")
-            self.rich_console.print(message_str)
+            self.rich_console.print(f"\[{meta_str}]", style=meta_style_rich, end="")
+            message_str_escaped = message_str.replace("[", "\[")
+            self.rich_console.print(f" {message_str_escaped}")
         elif self.backend == Backend.COLORAMA:
             meta_bg = Back.BLACK
             meta_fg = self.get_fg_color_colorama(message_verbosity)
             message_bg = Back.RESET
             message_fg = Fore.RESET
 
             meta_frm = f"{meta_bg}{meta_fg}[{meta_str}]{Style.RESET_ALL}"
```

### Comparing `minlog-0.3.0/minlog/_test.py` & `minlog-0.3.1/minlog/_test.py`

 * *Files identical despite different names*

