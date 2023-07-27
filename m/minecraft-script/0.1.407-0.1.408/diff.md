# Comparing `tmp/minecraft_script-0.1.407.tar.gz` & `tmp/minecraft_script-0.1.408.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.407.tar", last modified: Thu Jul 27 19:43:27 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.408.tar", last modified: Thu Jul 27 21:12:11 2023, max compression
```

## Comparing `minecraft_script-0.1.407.tar` & `minecraft_script-0.1.408.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.415776 minecraft_script-0.1.407/
--rw-rw-rw-   0        0        0     1684 2023-07-27 19:43:27.415776 minecraft_script-0.1.407/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.393012 minecraft_script-0.1.407/minecraft_script/
--rw-rw-rw-   0        0        0     1426 2023-07-26 22:22:30.000000 minecraft_script-0.1.407/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      378 2023-07-26 22:23:11.000000 minecraft_script-0.1.407/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.407/minecraft_script/build_interpreter.py
-drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.412773 minecraft_script-0.1.407/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.407/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       72 2023-07-27 19:42:41.000000 minecraft_script-0.1.407/minecraft_script/common.py
--rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.407/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.414775 minecraft_script-0.1.407/minecraft_script/grammar/
--rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      579 2023-07-27 17:14:29.000000 minecraft_script-0.1.407/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     5202 2023-07-26 21:29:02.000000 minecraft_script-0.1.407/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     5048 2023-07-27 19:30:20.000000 minecraft_script-0.1.407/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     3826 2023-07-26 21:14:45.000000 minecraft_script-0.1.407/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     7950 2023-07-26 21:16:41.000000 minecraft_script-0.1.407/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.407/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     5159 2023-07-26 21:57:47.000000 minecraft_script-0.1.407/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-27 19:43:27.405764 minecraft_script-0.1.407/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     1684 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-27 19:43:27.000000 minecraft_script-0.1.407/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 19:43:27.416777 minecraft_script-0.1.407/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-07-27 14:00:51.000000 minecraft_script-0.1.407/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.229390 minecraft_script-0.1.408/
+-rw-rw-rw-   0        0        0     1684 2023-07-27 21:12:11.229390 minecraft_script-0.1.408/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.208375 minecraft_script-0.1.408/minecraft_script/
+-rw-rw-rw-   0        0        0     1426 2023-07-26 22:22:30.000000 minecraft_script-0.1.408/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      378 2023-07-26 22:23:11.000000 minecraft_script-0.1.408/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.408/minecraft_script/build_interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.226388 minecraft_script-0.1.408/minecraft_script/build_templates/
+-rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/build_templates/function_tags.json
+-rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.408/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       72 2023-07-27 21:10:53.000000 minecraft_script-0.1.408/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.408/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.228389 minecraft_script-0.1.408/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      579 2023-07-27 17:14:29.000000 minecraft_script-0.1.408/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     5512 2023-07-27 21:07:11.000000 minecraft_script-0.1.408/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     4883 2023-07-27 20:35:04.000000 minecraft_script-0.1.408/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     4085 2023-07-27 20:20:40.000000 minecraft_script-0.1.408/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     9244 2023-07-27 20:43:18.000000 minecraft_script-0.1.408/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.408/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     5159 2023-07-26 21:57:47.000000 minecraft_script-0.1.408/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-27 21:12:11.222382 minecraft_script-0.1.408/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     1684 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-27 21:12:11.000000 minecraft_script-0.1.408/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-27 21:12:11.229390 minecraft_script-0.1.408/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-07-27 14:00:51.000000 minecraft_script-0.1.408/setup.py
```

### Comparing `minecraft_script-0.1.407/PKG-INFO` & `minecraft_script-0.1.408/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.407
+Version: 0.1.408
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.407/minecraft_script/__init__.py` & `minecraft_script-0.1.408/minecraft_script/__init__.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script/build_interpreter.py` & `minecraft_script-0.1.408/minecraft_script/build_interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script/builder.py` & `minecraft_script-0.1.408/minecraft_script/builder.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script/errors.py` & `minecraft_script-0.1.408/minecraft_script/errors.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script/grammar/LANG_TOKENS.json` & `minecraft_script-0.1.408/minecraft_script/grammar/LANG_TOKENS.json`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script/interpreter.py` & `minecraft_script-0.1.408/minecraft_script/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,13 +145,19 @@
             result = Number(0).subtract(right_node)
 
         return result
 
     def visit_MultipleStatementsNode(self, node, context):
         return [self.visit(statement, context) for statement in node.statements]
 
+    def visit_CodeBlockNode(self, node, context):
+        local_symbol_table = SymbolTable(context.symbol_table, load_builtins=False)
+        local_context = Context(f'code_block at {id(node)}', local_symbol_table)
+
+        return [self.visit(statement, local_context) for statement in node.statements]
+
     def no_visit_node(self, node, context):
         print(text_error(f'No visit method defined for {text_underline(type(node).__name__)}'))
 
 
 if __name__ == '__main__':
     Interpreter()
```

### Comparing `minecraft_script-0.1.407/minecraft_script/lexer.py` & `minecraft_script-0.1.408/minecraft_script/lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 class Lexer:
     def __init__(self, text: str):
         self.text = text
         self.current_index = -1
         self.current_char = None
         self.current_line = 0
 
-        self.bracket_depth = 0
-
         self.advance()
 
     def advance(self) -> None:
         self.current_index += 1
         self.current_char = self.text[self.current_index] if self.current_index < len(self.text) else None
 
         if self.current_char == '\n':
@@ -80,26 +78,23 @@
                 self.advance()
 
             elif self.current_char == LANG_TOKENS['TT_COMMA']:
                 tokens.append(Token(self.current_char, 'TT_COMMA'))
                 self.advance()
 
             elif self.current_char in LANG_TOKENS['TT_NEWLINE']:
-                if self.bracket_depth == 0:
-                    tokens.append(Token(self.current_char, 'TT_NEWLINE'))
+                tokens.append(Token(self.current_char, 'TT_NEWLINE'))
                 self.advance()
 
             elif self.current_char == LANG_TOKENS['TT_LEFT_BRACE']:
                 tokens.append(Token(self.current_char, 'TT_LEFT_BRACE'))
-                self.bracket_depth += 1
                 self.advance()
 
             elif self.current_char == LANG_TOKENS['TT_RIGHT_BRACE']:
                 tokens.append(Token(self.current_char, 'TT_RIGHT_BRACE'))
-                self.bracket_depth -= 1
                 self.advance()
 
             elif self.current_char == LANG_TOKENS['TT_EQUALS']:
                 token_value = self.make_equals()
 
                 if token_value == LANG_TOKENS['TT_FUNCTION_ARROW']:
                     tokens.append(Token(token_value, 'TT_FUNCTION_ARROW'))
```

### Comparing `minecraft_script-0.1.407/minecraft_script/nodes.py` & `minecraft_script-0.1.408/minecraft_script/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,7 +126,18 @@
         self.statements = statements
 
     def __str__(self):
         return f'statements: {self.statements}'
 
     def __repr__(self):
         return f'MultipleStatementsNode({self.statements})'
+
+
+class CodeBlockNode:
+    def __init__(self, statements: list):
+        self.statements = statements
+
+    def __str__(self):
+        return f'Code Block: {self.statements}'
+
+    def __repr__(self):
+        return f'CodeBlockNode({self.statements})'
```

### Comparing `minecraft_script-0.1.407/minecraft_script/parser.py` & `minecraft_script-0.1.408/minecraft_script/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .tokens import Token
 from .errors import MCSSyntaxError
 from .text_additions import text_underline
 from .nodes import NumberNode, BinaryOperationNode, UnaryOperationNode, VariableAssignNode, VariableAccessNode, \
-    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode, ListNode, ListGetNode
+    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode, ListNode, ListGetNode, CodeBlockNode
 
 
 class Parser:
     def __init__(self, token_list: list[Token]):
         self.token_list = token_list
         self.current_index = -1
         self.current_token = None
@@ -54,15 +54,15 @@
         elif token.tt_type == 'TT_NUMBER':
             self.advance()
             return NumberNode(token)
 
     def term(self) -> BinaryOperationNode:
         return self.binary_operation(self.factor, ['*', '/', '%'])
 
-    def expression(self) -> BinaryOperationNode | VariableAssignNode | FunctionAssignNode:
+    def expression(self) -> BinaryOperationNode | VariableAssignNode | FunctionAssignNode | CodeBlockNode:
         if self.current_token.tt_type == 'VAR_DEFINE':
             self.advance()
             if self.current_token.tt_type != 'TT_NAME':
                 MCSSyntaxError(f'Expected name. Got {text_underline(f"{self.current_token.value !r}")} instead.')
                 exit()
 
             var_name_token = self.current_token
@@ -74,14 +74,17 @@
 
             self.advance()
             return VariableAssignNode(var_name_token, self.expression())
 
         elif self.current_token.tt_type == 'FUNC_DEFINE':
             return self.function_define()
 
+        elif self.current_token.tt_type == 'TT_LEFT_BRACE':
+            return self.code_block()
+
         return self.binary_operation(self.term, ['+', '-'])
 
     def binary_operation(self, function, operators) -> BinaryOperationNode:
         left_node = function()
         # self.current_token is now the operator
 
         while self.current_token.value in operators:
@@ -202,15 +205,48 @@
 
         index = self.term()
 
         if self.current_token.tt_type == 'TT_RIGHT_BRACKET':
             self.advance()
             return ListGetNode(name_token, index)
 
+    def code_block(self):
+        if self.current_token.tt_type != 'TT_LEFT_BRACE':
+            MCSSyntaxError('Expected "{". Got "%s" instead' % self.current_token.value)
+            exit()
+        self.advance()
+
+        statements = []
+
+        if self.current_token.tt_type == 'TT_RIGHT_BRACE':
+            self.advance()
+            return CodeBlockNode(statements)
+
+        while self.current_token.tt_type == 'TT_NEWLINE':
+            self.advance()
+
+        statements.append(self.expression())
+
+        while self.current_token.tt_type == 'TT_NEWLINE':
+            self.advance()
+            while self.current_token.tt_type == 'TT_NEWLINE':
+                self.advance()
+
+            if self.current_token.tt_type == 'TT_RIGHT_BRACE':
+                self.advance()
+                return CodeBlockNode(statements)
+
+            statements.append(self.expression())
 
+        if self.current_token.tt_type == 'TT_RIGHT_BRACE':
+            self.advance()
+            return CodeBlockNode(statements)
+        else:
+            MCSSyntaxError('Expected "}". Got "%s" instead.' % self.current_token.value)
+            exit()
 
 
 
 if __name__ == '__main__':
     tokens = [Token(5, 'TT_NUMBER'), Token('+', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
               Token('*', 'TT_BINARY_OPERATOR'), Token('(', 'TT_LEFT_PARENTHESIS'), Token(3, 'TT_NUMBER'),
               Token('+', 'TT_BINARY_OPERATOR'), Token('-', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
```

### Comparing `minecraft_script-0.1.407/minecraft_script/shell_commands.py` & `minecraft_script-0.1.408/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script/text_additions.py` & `minecraft_script-0.1.408/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script/types.py` & `minecraft_script-0.1.408/minecraft_script/types.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.1.408/minecraft_script.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-script
-Version: 0.1.407
+Version: 0.1.408
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.407/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.408/minecraft_script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.407/setup.py` & `minecraft_script-0.1.408/setup.py`

 * *Files identical despite different names*

