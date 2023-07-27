# Comparing `tmp/minecraft_script-0.1.406.tar.gz` & `tmp/minecraft_script-0.1.407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.406.tar", last modified: Wed Jul 26 22:05:35 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.407.tar", last modified: Thu Jul 27 19:43:27 2023, max compression
```

## Comparing `minecraft_script-0.1.406.tar` & `minecraft_script-0.1.407.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.626016 minecraft_script-0.1.406/
--rw-rw-rw-   0        0        0     2943 2023-07-26 22:05:35.626016 minecraft_script-0.1.406/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.597988 minecraft_script-0.1.406/minecraft_script/
--rw-rw-rw-   0        0        0     1449 2023-07-26 22:04:12.000000 minecraft_script-0.1.406/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.406/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.406/minecraft_script/build_interpreter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.618008 minecraft_script-0.1.406/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.406/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       51 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/common.py
--rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.406/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.625016 minecraft_script-0.1.406/minecraft_script/grammar/
--rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      545 2023-07-26 20:23:02.000000 minecraft_script-0.1.406/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     5202 2023-07-26 21:29:02.000000 minecraft_script-0.1.406/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     4791 2023-07-26 20:54:59.000000 minecraft_script-0.1.406/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     3826 2023-07-26 21:14:45.000000 minecraft_script-0.1.406/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     7950 2023-07-26 21:16:41.000000 minecraft_script-0.1.406/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     5159 2023-07-26 21:57:47.000000 minecraft_script-0.1.406/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.611001 minecraft_script-0.1.406/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     2943 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 22:05:35.626016 minecraft_script-0.1.406/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-07-26 22:04:20.000000 minecraft_script-0.1.406/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.415776 minecraft_script-0.1.407/
+-rw-rw-rw-   0        0        0     1684 2023-07-27 19:43:27.415776 minecraft_script-0.1.407/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.393012 minecraft_script-0.1.407/minecraft_script/
+-rw-rw-rw-   0        0        0     1426 2023-07-26 22:22:30.000000 minecraft_script-0.1.407/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      378 2023-07-26 22:23:11.000000 minecraft_script-0.1.407/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.407/minecraft_script/build_interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.412773 minecraft_script-0.1.407/minecraft_script/build_templates/
+-rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/build_templates/function_tags.json
+-rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.407/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       72 2023-07-27 19:42:41.000000 minecraft_script-0.1.407/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.407/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.414775 minecraft_script-0.1.407/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      579 2023-07-27 17:14:29.000000 minecraft_script-0.1.407/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     5202 2023-07-26 21:29:02.000000 minecraft_script-0.1.407/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     5048 2023-07-27 19:30:20.000000 minecraft_script-0.1.407/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     3826 2023-07-26 21:14:45.000000 minecraft_script-0.1.407/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     7950 2023-07-26 21:16:41.000000 minecraft_script-0.1.407/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     5159 2023-07-26 21:57:47.000000 minecraft_script-0.1.407/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.405764 minecraft_script-0.1.407/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     1684 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 19:43:27.416777 minecraft_script-0.1.407/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-07-27 14:00:51.000000 minecraft_script-0.1.407/setup.py
```

### Comparing `minecraft_script-0.1.406/minecraft_script/__init__.py` & `minecraft_script-0.1.407/minecraft_script/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from .lexer import Lexer
 from .parser import Parser
 from .interpreter import Interpreter, Context, SymbolTable
 
-version = "0.1.406"
-
 
 def run(text: str):
     global_symbol_table = SymbolTable()
 
     run_lexer = Lexer(text)
     tokens = run_lexer.tokenize()
     print(repr(tokens))
```

### Comparing `minecraft_script-0.1.406/minecraft_script/build_interpreter.py` & `minecraft_script-0.1.407/minecraft_script/build_interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/builder.py` & `minecraft_script-0.1.407/minecraft_script/builder.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/errors.py` & `minecraft_script-0.1.407/minecraft_script/errors.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/grammar/LANG_TOKENS.json` & `minecraft_script-0.1.407/minecraft_script/grammar/LANG_TOKENS.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'TT_COMMENT'": "'//'"}*

```diff
@@ -1,10 +1,11 @@
 {
     "TT_BINARY_OPERATOR": "+-*/%",
     "TT_COMMA": ",",
+    "TT_COMMENT": "//",
     "TT_EQUALS": "=",
     "TT_FUNCTION_ARROW": "=>",
     "TT_IGNORE": " \t",
     "TT_LEFT_BRACE": "{",
     "TT_LEFT_BRACKET": "[",
     "TT_LEFT_PARENTHESIS": "(",
     "TT_NAME": "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ_",
```

### Comparing `minecraft_script-0.1.406/minecraft_script/interpreter.py` & `minecraft_script-0.1.407/minecraft_script/interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/lexer.py` & `minecraft_script-0.1.407/minecraft_script/lexer.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,17 +109,24 @@
                 # don't self.advance() since that is already done in self.make_equals()
 
             elif self.current_char in LANG_TOKENS['TT_NUMBER']:
                 number = self.make_number()
                 tokens.append(Token(number, 'TT_NUMBER'))
 
             elif self.current_char in LANG_TOKENS['TT_BINARY_OPERATOR']:
-                tokens.append(Token(self.current_char, 'TT_BINARY_OPERATOR'))
+                current_char = self.current_char
                 self.advance()
 
+                if f'{current_char}{self.current_char}' == LANG_TOKENS['TT_COMMENT']:
+                    while self.current_char != '\n':
+                        self.advance()
+
+                else:
+                    tokens.append(Token(current_char, 'TT_BINARY_OPERATOR'))
+
             elif self.current_char in LANG_TOKENS['TT_NAME']:
                 name = self.make_name()
                 if LANG_KEYWORDS.get(name, False):
                     tokens.append(Token(name, LANG_KEYWORDS[name]))
                 else:
                     tokens.append(Token(name, "TT_NAME"))
```

### Comparing `minecraft_script-0.1.406/minecraft_script/nodes.py` & `minecraft_script-0.1.407/minecraft_script/nodes.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/parser.py` & `minecraft_script-0.1.407/minecraft_script/parser.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/shell_commands.py` & `minecraft_script-0.1.407/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/text_additions.py` & `minecraft_script-0.1.407/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script/types.py` & `minecraft_script-0.1.407/minecraft_script/types.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.407/minecraft_script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.406/setup.py` & `minecraft_script-0.1.407/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
+from minecraft_script.common import version
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.406'
 DESCRIPTION = 'Minecraft Script Programming language'
 
 # Setting up
 setup(
     name="minecraft_script",
-    version=VERSION,
+    version=version,
     author="Joyful-Bard",
     author_email="<thisis@notarealemail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     package_data={'minecraft_script': [
```

