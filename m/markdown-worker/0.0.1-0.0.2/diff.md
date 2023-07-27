# Comparing `tmp/markdown_worker-0.0.1.tar.gz` & `tmp/markdown_worker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_worker-0.0.1.tar", last modified: Wed Jul 26 09:57:52 2023, max compression
+gzip compressed data, was "markdown_worker-0.0.2.tar", last modified: Thu Jul 27 06:10:31 2023, max compression
```

## Comparing `markdown_worker-0.0.1.tar` & `markdown_worker-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-26 09:57:52.250038 markdown_worker-0.0.1/
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1073 2023-07-26 09:18:13.000000 markdown_worker-0.0.1/LICENSE
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1484 2023-07-26 09:57:52.249903 markdown_worker-0.0.1/PKG-INFO
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)      921 2023-07-26 09:57:30.000000 markdown_worker-0.0.1/README.md
-drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-26 09:57:52.248802 markdown_worker-0.0.1/markdown_worker/
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)       58 2023-07-26 09:56:36.000000 markdown_worker-0.0.1/markdown_worker/__init__.py
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     4340 2023-07-26 09:40:19.000000 markdown_worker-0.0.1/markdown_worker/markdown_worker.py
-drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-26 09:57:52.249669 markdown_worker-0.0.1/markdown_worker.egg-info/
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1484 2023-07-26 09:57:52.000000 markdown_worker-0.0.1/markdown_worker.egg-info/PKG-INFO
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)      283 2023-07-26 09:57:52.000000 markdown_worker-0.0.1/markdown_worker.egg-info/SOURCES.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)        1 2023-07-26 09:57:52.000000 markdown_worker-0.0.1/markdown_worker.egg-info/dependency_links.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)        6 2023-07-26 09:57:52.000000 markdown_worker-0.0.1/markdown_worker.egg-info/requires.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)       16 2023-07-26 09:57:52.000000 markdown_worker-0.0.1/markdown_worker.egg-info/top_level.txt
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)       38 2023-07-26 09:57:52.250082 markdown_worker-0.0.1/setup.cfg
--rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1084 2023-07-26 09:56:58.000000 markdown_worker-0.0.1/setup.py
+drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-27 06:10:31.244736 markdown_worker-0.0.2/
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1073 2023-07-26 09:18:13.000000 markdown_worker-0.0.2/LICENSE
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1785 2023-07-27 06:10:31.244620 markdown_worker-0.0.2/PKG-INFO
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1222 2023-07-27 06:09:38.000000 markdown_worker-0.0.2/README.md
+drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-27 06:10:31.243733 markdown_worker-0.0.2/markdown_worker/
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)       58 2023-07-26 09:56:36.000000 markdown_worker-0.0.2/markdown_worker/__init__.py
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)     5357 2023-07-27 05:59:02.000000 markdown_worker-0.0.2/markdown_worker/markdown_worker.py
+drwxr-xr-x   0 mantreshkhurana   (501) staff       (20)        0 2023-07-27 06:10:31.244428 markdown_worker-0.0.2/markdown_worker.egg-info/
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1785 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/PKG-INFO
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)      283 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)        1 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)        6 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/requires.txt
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)       16 2023-07-27 06:10:31.000000 markdown_worker-0.0.2/markdown_worker.egg-info/top_level.txt
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)       38 2023-07-27 06:10:31.244773 markdown_worker-0.0.2/setup.cfg
+-rw-r--r--   0 mantreshkhurana   (501) staff       (20)     1084 2023-07-27 06:05:54.000000 markdown_worker-0.0.2/setup.py
```

### Comparing `markdown_worker-0.0.1/LICENSE` & `markdown_worker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_worker-0.0.1/PKG-INFO` & `markdown_worker-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown_worker
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple markdown parsing package.
 Author: Mantresh Khurana
 Author-email: <mantreshkhurana@spyxpo.com>
 Keywords: python,mantresh khurana,parser,markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 # Markdown Worker
 
 This is a simple markdown parser written in Python. It can read, write and parse markdown files. It can read a particular header, write a particular header, and parse a particular header. It can also parse the entire file.
 
 ## Installation
 
 ```bash
+# use these commands to install the package source code to your local machine
 git clone https://github.com/mantreshkhurana/markdown-worker-python.git
 cd markdown-worker-python
 ```
 
 or
 
 ```bash
@@ -36,14 +37,16 @@
 
 ```bash
 pip3 install markdown-worker
 ```
 
 ## Usage
 
+I provided a `example.md` file in the repository. You can use that to test the program, it contains all the [documentation](https://github.com/mantreshkhurana/markdown-worker-python/blob/stable/example.md) of the program.
+
 ```python
 from markdown_worker import MarkdownParser
 
 if __name__ == "__main__":
     file_name = input("Enter the path of the Markdown file: ")
     parser = MarkdownParser(file_name)
```

### Comparing `markdown_worker-0.0.1/README.md` & `markdown_worker-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Markdown Worker
 
 This is a simple markdown parser written in Python. It can read, write and parse markdown files. It can read a particular header, write a particular header, and parse a particular header. It can also parse the entire file.
 
 ## Installation
 
 ```bash
+# use these commands to install the package source code to your local machine
 git clone https://github.com/mantreshkhurana/markdown-worker-python.git
 cd markdown-worker-python
 ```
 
 or
 
 ```bash
@@ -19,14 +20,16 @@
 
 ```bash
 pip3 install markdown-worker
 ```
 
 ## Usage
 
+I provided a `example.md` file in the repository. You can use that to test the program, it contains all the [documentation](https://github.com/mantreshkhurana/markdown-worker-python/blob/stable/example.md) of the program.
+
 ```python
 from markdown_worker import MarkdownParser
 
 if __name__ == "__main__":
     file_name = input("Enter the path of the Markdown file: ")
     parser = MarkdownParser(file_name)
```

### Comparing `markdown_worker-0.0.1/markdown_worker/markdown_worker.py` & `markdown_worker-0.0.2/markdown_worker/markdown_worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import re
 
 class MarkdownParser:
-    def __init__(self, filename):
+    def __init__(self, filename=None):
         self.filename = filename
-        self.markdown_text = self.read_markdown_file()
+        self.markdown_text = self.read_markdown_file() if filename else ""
 
     def read_markdown_file(self):
-        if self.filename.endswith('.md'):
+        if self.filename and self.filename.endswith('.md'):
             with open(self.filename, 'r', encoding='utf-8') as file:
                 markdown_text = file.read()
                 return markdown_text
         else:
             return "File is not a Markdown file."
 
     def extract_headers_and_paragraphs(self):
@@ -111,8 +111,30 @@
         if line_number < len(lines):
             words = lines[line_number].split(' ')
             if word_number < len(words):
                 return words[word_number]
             else:
                 return "Word number out of range."
         else:
-            return "Line number out of range."
+            return "Line number out of range."
+
+    def markdown_to_html(self, markdown_text, output_filename=None):
+        markdown_text = re.sub(r'^(#+)(.*?)$', r'<h\1>\2</h\1>', markdown_text, flags=re.MULTILINE)
+
+        markdown_text = re.sub(r'\*\*(.*?)\*\*', r'<strong>\1</strong>', markdown_text)
+
+        markdown_text = re.sub(r'\*(.*?)\*', r'<em>\1</em>', markdown_text)
+
+        markdown_text = re.sub(r'^\*\s(.*)$', r'<li>\1</li>', markdown_text, flags=re.MULTILINE)
+        markdown_text = re.sub(r'(<li>.*<\/li>)+', r'<ul>\g<0></ul>', markdown_text)
+
+        markdown_text = re.sub(r'^\d+\.\s(.*)$', r'<li>\1</li>', markdown_text, flags=re.MULTILINE)
+        markdown_text = re.sub(r'(<li>.*<\/li>)+', r'<ol>\g<0></ol>', markdown_text)
+
+        markdown_text = re.sub(r'`([^`]+)`', r'<code>\1</code>', markdown_text)
+
+        if output_filename:
+            with open(output_filename, 'w', encoding='utf-8') as output_file:
+                output_file.write(markdown_text)
+
+        return markdown_text
+
```

### Comparing `markdown_worker-0.0.1/markdown_worker.egg-info/PKG-INFO` & `markdown_worker-0.0.2/markdown_worker.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-worker
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple markdown parsing package.
 Author: Mantresh Khurana
 Author-email: <mantreshkhurana@spyxpo.com>
 Keywords: python,mantresh khurana,parser,markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 # Markdown Worker
 
 This is a simple markdown parser written in Python. It can read, write and parse markdown files. It can read a particular header, write a particular header, and parse a particular header. It can also parse the entire file.
 
 ## Installation
 
 ```bash
+# use these commands to install the package source code to your local machine
 git clone https://github.com/mantreshkhurana/markdown-worker-python.git
 cd markdown-worker-python
 ```
 
 or
 
 ```bash
@@ -36,14 +37,16 @@
 
 ```bash
 pip3 install markdown-worker
 ```
 
 ## Usage
 
+I provided a `example.md` file in the repository. You can use that to test the program, it contains all the [documentation](https://github.com/mantreshkhurana/markdown-worker-python/blob/stable/example.md) of the program.
+
 ```python
 from markdown_worker import MarkdownParser
 
 if __name__ == "__main__":
     file_name = input("Enter the path of the Markdown file: ")
     parser = MarkdownParser(file_name)
```

### Comparing `markdown_worker-0.0.1/setup.py` & `markdown_worker-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A simple markdown parsing package.'
 LONG_DESCRIPTION = 'A package that allows to parse, read and write markdown files.'
 
 # Setting up
 setup(
     name="markdown_worker",
     version=VERSION,
```

