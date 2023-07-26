# Comparing `tmp/minecraft_script-0.1.405.tar.gz` & `tmp/minecraft_script-0.1.406.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.405.tar", last modified: Wed Jul 26 17:50:01 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.406.tar", last modified: Wed Jul 26 22:05:35 2023, max compression
```

## Comparing `minecraft_script-0.1.405.tar` & `minecraft_script-0.1.406.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.465750 minecraft_script-0.1.405/
--rw-rw-rw-   0        0        0     2070 2023-07-26 17:50:01.464748 minecraft_script-0.1.405/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.447593 minecraft_script-0.1.405/minecraft_script/
--rw-rw-rw-   0        0        0     1449 2023-07-26 17:49:37.000000 minecraft_script-0.1.405/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.405/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.405/minecraft_script/build_interpreter.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.461746 minecraft_script-0.1.405/minecraft_script/build_templates/
--rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/build_templates/function_tags.json
--rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/build_templates/pack.mcmeta
--rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.405/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       51 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/common.py
--rw-rw-rw-   0        0        0     1837 2023-07-26 12:37:44.000000 minecraft_script-0.1.405/minecraft_script/errors.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.463748 minecraft_script-0.1.405/minecraft_script/grammar/
--rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/grammar/LANG_KEYWORDS.json
--rw-rw-rw-   0        0        0      483 2023-07-26 12:47:05.000000 minecraft_script-0.1.405/minecraft_script/grammar/LANG_TOKENS.json
--rw-rw-rw-   0        0        0     4526 2023-07-26 17:42:04.000000 minecraft_script-0.1.405/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     4435 2023-07-26 16:04:57.000000 minecraft_script-0.1.405/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     3197 2023-07-26 17:12:09.000000 minecraft_script-0.1.405/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     6276 2023-07-26 17:44:50.000000 minecraft_script-0.1.405/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.405/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     3515 2023-07-26 17:16:21.000000 minecraft_script-0.1.405/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:50:01.460744 minecraft_script-0.1.405/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     2070 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 17:50:01.000000 minecraft_script-0.1.405/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:50:01.465750 minecraft_script-0.1.405/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-07-26 17:49:34.000000 minecraft_script-0.1.405/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.626016 minecraft_script-0.1.406/
+-rw-rw-rw-   0        0        0     2943 2023-07-26 22:05:35.626016 minecraft_script-0.1.406/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.597988 minecraft_script-0.1.406/minecraft_script/
+-rw-rw-rw-   0        0        0     1449 2023-07-26 22:04:12.000000 minecraft_script-0.1.406/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.406/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     1168 2023-07-26 12:31:03.000000 minecraft_script-0.1.406/minecraft_script/build_interpreter.py
+drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.618008 minecraft_script-0.1.406/minecraft_script/build_templates/
+-rw-rw-rw-   0        0        0       41 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/build_templates/function_tags.json
+-rw-rw-rw-   0        0        0      131 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/build_templates/pack.mcmeta
+-rw-rw-rw-   0        0        0     2276 2023-07-26 12:32:37.000000 minecraft_script-0.1.406/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       51 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     2070 2023-07-26 21:29:02.000000 minecraft_script-0.1.406/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.625016 minecraft_script-0.1.406/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0       88 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      545 2023-07-26 20:23:02.000000 minecraft_script-0.1.406/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     5202 2023-07-26 21:29:02.000000 minecraft_script-0.1.406/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     4791 2023-07-26 20:54:59.000000 minecraft_script-0.1.406/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     3826 2023-07-26 21:14:45.000000 minecraft_script-0.1.406/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     7950 2023-07-26 21:16:41.000000 minecraft_script-0.1.406/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-25 21:27:11.000000 minecraft_script-0.1.406/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     5159 2023-07-26 21:57:47.000000 minecraft_script-0.1.406/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-26 22:05:35.611001 minecraft_script-0.1.406/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     2943 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      763 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 22:05:35.000000 minecraft_script-0.1.406/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 22:05:35.626016 minecraft_script-0.1.406/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2023-07-26 22:04:20.000000 minecraft_script-0.1.406/setup.py
```

### Comparing `minecraft_script-0.1.405/PKG-INFO` & `minecraft_script-0.1.406/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.405
+Version: 0.1.406
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,14 +21,23 @@
 # Commands
 ```cmd
 python -m minecraft_script help
 python -m minecraft_script run [files: optional, multiple allowed]
 python -m minecraft_script build [file]
 ```
 
+## Data Types
+Minecraft-script can only work with integers. This is due to the fact that strings aren't a thing in minecraft, and floating point numbers don't work in most cases, specifically scoreboards.
+This also means that the only division available is euclidean division.
+
+```js
+var number = 423  // number, has to be an integer
+var array = [1, 2, 3, 4, 5]  // array of numbers
+```
+
 ## Objects
 ### Variables
 The var keyword can be used to initialize new variables.
 Use it by following it by the variable's name, then an equals sign and a value.
 
 ```js
 var hello2 = 500  // initialized variable "hello2" with value 500
@@ -52,10 +61,32 @@
 ### log
 The log functions allows you to keep track of values in the console.
 It is equivalent to JavaScript's console.log() or Python's print() function.
 
 ```js
 var hello1 = 500
 
-log(200 + 200)  // logs "400" in console
+log(400)  // logs "400" in console
 log(hello1, 300)  // logs "500, 300" in console
+```
+
+### append
+Append a value to a list. The first argument has to be a list.
+```js
+var test = [3, 5, 4]
+
+append(test, 2)  // append 2 to the list
+append(test, [3, 4])  // append [3, 4] to the list
+
+log(test)  // logs "[3, 5, 4, 2, [3, 4]]"
+```
+
+### extend
+Extend a list by another list. Both arguments need to be lists.
+```js
+var list_1 = [5, 2]
+var list_2 = [2, 3]
+
+extend(list_1, list_2)
+
+log(list_1)  // logs "[5, 2, 2, 3]"
 ```
```

### Comparing `minecraft_script-0.1.405/minecraft_script/__init__.py` & `minecraft_script-0.1.406/minecraft_script/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .lexer import Lexer
 from .parser import Parser
 from .interpreter import Interpreter, Context, SymbolTable
 
-version = "0.1.405"
+version = "0.1.406"
 
 
 def run(text: str):
     global_symbol_table = SymbolTable()
 
     run_lexer = Lexer(text)
     tokens = run_lexer.tokenize()
```

### Comparing `minecraft_script-0.1.405/minecraft_script/build_interpreter.py` & `minecraft_script-0.1.406/minecraft_script/build_interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.405/minecraft_script/builder.py` & `minecraft_script-0.1.406/minecraft_script/builder.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.405/minecraft_script/errors.py` & `minecraft_script-0.1.406/minecraft_script/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,11 +45,16 @@
 
 
 class MCSNameError(MCSError):
     def __init__(self, details: str, line_number: int = None):
         details = f'Name {text_underline(f"{details !r}")} is not defined'
         super().__init__(details, "Name Error", line_number)
 
+class MCSIndexError(MCSError):
+    def __init__(self, details: str, line_number: int = None):
+        details = f'Index {text_underline(f"{details}")} out of range'
+        super().__init__(details, "Index Error", line_number)
+
 
 if __name__ == '__main__':
     a = MCSTypeError('const')
     print(a)
```

### Comparing `minecraft_script-0.1.405/minecraft_script/interpreter.py` & `minecraft_script-0.1.406/minecraft_script/interpreter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .text_additions import text_error, text_underline
-from .types import Number, Function, BuiltinFunction
-from .errors import MCSNameError
+from .types import Number, List, Function, BuiltinFunction
+from .errors import MCSNameError, MCSTypeError, MCSIndexError
 
 
 class Context:
     def __init__(self, display_name: str, symbol_table, parent=None):
         self.display_name = display_name
         self.parent: None | Context = parent
         self.symbol_table: SymbolTable = symbol_table
@@ -18,15 +18,16 @@
 
 class SymbolTable:
     def __init__(self, parent=None, *, load_builtins=True):
         self.symbols: dict = {}
         self.parent = parent
 
         if load_builtins:
-            self.set('log', BuiltinFunction('log'))
+            for name in BuiltinFunction.names:
+                self.set(name, BuiltinFunction(name))
 
     def get(self, variable_name):
         value = self.symbols.get(variable_name, None)
 
         if value is None and self.parent:
             return self.parent.get(variable_name)
 
@@ -47,56 +48,78 @@
 
 class Interpreter:
     def visit(self, node, context: Context):
         method_name = f'visit_{type(node).__name__}'
         method = getattr(self, method_name, self.no_visit_node)
         return method(node, context)
 
-    def visit_NumberNode(self, node, context: Context) -> int:
+    def visit_NumberNode(self, node, context) -> int:
         return node.get_value()
 
-    def visit_VariableAccessNode(self, node, context: Context) -> any:
+    def visit_ListNode(self, node, context):
+        value_array = [self.visit(element, context) for element in node.array]
+        return List(value_array)
+
+    def visit_ListGetNode(self, node, context):
+        name = node.name_token.value
+        index = self.visit(node.index, context)
+        variable = context.symbol_table.get(name)
+
+        if type(variable).__name__ == 'List':
+            value = variable.get_index(index)
+
+            if not value:
+                MCSIndexError(f'{index}')
+                exit()
+
+            return value
+
+        else:
+            MCSTypeError(f'{variable} is not a list')
+            exit()
+
+    def visit_VariableAccessNode(self, node, context) -> any:
         var_name: str = node.get_name()
         var_value = context.symbol_table.get(var_name)
 
         if var_value is None:
             MCSNameError(var_name)
             exit()
 
         return var_value
 
-    def visit_VariableAssignNode(self, node, context: Context) -> any:
+    def visit_VariableAssignNode(self, node, context) -> any:
         var_name: str = node.get_name()
         var_new_value = self.visit(node.value_node, context)
 
         context.symbol_table.set(var_name, var_new_value)
         return var_new_value
 
-    def visit_FunctionAssignNode(self, node, context: Context) -> Function:
+    def visit_FunctionAssignNode(self, node, context) -> Function:
         func_name = node.name_token.value if node.name_token else None
         parameter_names = [param_token.value for param_token in node.parameter_name_tokens]
         body_node = node.body_node
 
         function = Function(func_name, parameter_names, body_node, context)
 
         if func_name:
             context.symbol_table.set(func_name, function)
 
         return function
 
-    def visit_FunctionCallNode(self, node, context: Context) -> any:
+    def visit_FunctionCallNode(self, node, context) -> any:
         func_name = node.name_token.value
         arguments = [self.visit(arg_token, context) for arg_token in node.argument_nodes]
 
         function = context.symbol_table.get(func_name)
         result = function.call(arguments)
 
         return result
 
-    def visit_BinaryOperationNode(self, node, context: Context) -> int:
+    def visit_BinaryOperationNode(self, node, context) -> int:
         operator = node.operator.value
         left_expression = Number(self.visit(node.left_node, context))
         right_expression = Number(self.visit(node.right_node, context))
         result = 0
 
         if operator == '+':
             result = left_expression.add(right_expression)
@@ -107,28 +130,28 @@
         elif operator == '/':
             result = left_expression.divide(right_expression)
         elif operator == '%':
             result = left_expression.modulus(right_expression)
 
         return result
 
-    def visit_UnaryOperationNode(self, node, context: Context) -> int:
+    def visit_UnaryOperationNode(self, node, context) -> int:
         operator = node.operator.value
         right_node = Number(self.visit(node.right_node, context))
         result = 0
 
         if operator == '+':
             result = Number(0).add(right_node)
         elif operator == '-':
             result = Number(0).subtract(right_node)
 
         return result
 
     def visit_MultipleStatementsNode(self, node, context):
         return [self.visit(statement, context) for statement in node.statements]
 
-    def no_visit_node(self, node, context: Context):
+    def no_visit_node(self, node, context):
         print(text_error(f'No visit method defined for {text_underline(type(node).__name__)}'))
 
 
 if __name__ == '__main__':
     Interpreter()
```

### Comparing `minecraft_script-0.1.405/minecraft_script/lexer.py` & `minecraft_script-0.1.406/minecraft_script/lexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,30 +67,38 @@
                 tokens.append(Token(self.current_char, 'TT_LEFT_PARENTHESIS'))
                 self.advance()
 
             elif self.current_char == LANG_TOKENS['TT_RIGHT_PARENTHESIS']:
                 tokens.append(Token(self.current_char, 'TT_RIGHT_PARENTHESIS'))
                 self.advance()
 
+            elif self.current_char == LANG_TOKENS['TT_LEFT_BRACKET']:
+                tokens.append(Token(self.current_char, 'TT_LEFT_BRACKET'))
+                self.advance()
+
+            elif self.current_char == LANG_TOKENS['TT_RIGHT_BRACKET']:
+                tokens.append(Token(self.current_char, 'TT_RIGHT_BRACKET'))
+                self.advance()
+
             elif self.current_char == LANG_TOKENS['TT_COMMA']:
                 tokens.append(Token(self.current_char, 'TT_COMMA'))
                 self.advance()
 
             elif self.current_char in LANG_TOKENS['TT_NEWLINE']:
                 if self.bracket_depth == 0:
                     tokens.append(Token(self.current_char, 'TT_NEWLINE'))
                 self.advance()
 
-            elif self.current_char == LANG_TOKENS['TT_LEFT_BRACKET']:
-                tokens.append(Token(self.current_char, 'TT_LEFT_BRACKET'))
+            elif self.current_char == LANG_TOKENS['TT_LEFT_BRACE']:
+                tokens.append(Token(self.current_char, 'TT_LEFT_BRACE'))
                 self.bracket_depth += 1
                 self.advance()
 
-            elif self.current_char == LANG_TOKENS['TT_RIGHT_BRACKET']:
-                tokens.append(Token(self.current_char, 'TT_RIGHT_BRACKET'))
+            elif self.current_char == LANG_TOKENS['TT_RIGHT_BRACE']:
+                tokens.append(Token(self.current_char, 'TT_RIGHT_BRACE'))
                 self.bracket_depth -= 1
                 self.advance()
 
             elif self.current_char == LANG_TOKENS['TT_EQUALS']:
                 token_value = self.make_equals()
 
                 if token_value == LANG_TOKENS['TT_FUNCTION_ARROW']:
```

### Comparing `minecraft_script-0.1.405/minecraft_script/nodes.py` & `minecraft_script-0.1.406/minecraft_script/nodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,40 @@
     def __str__(self):
         return f'{self.token.tt_type}:{self.token.value}'
 
     def __repr__(self):
         return f'NumberNode({self.token !r})'
 
 
+class ListNode:
+    def __init__(self, array: list):
+        self.array = array
+
+    def get_index(self, index: int):
+        return self.array[index]
+
+    def __str__(self):
+        return f'array node: {self.array}'
+
+    def __repr__(self):
+        return f'ListNode({self.array !r})'
+
+
+class ListGetNode:
+    def __init__(self, name_token, index):
+        self.name_token = name_token
+        self.index = index
+
+    def __str__(self):
+        return f'array get: {self.name_token.value} {self.index}'
+
+    def __repr__(self):
+        return f'ListGetNode({self.name_token !r}, {self.index !r})'
+
+
 class VariableAssignNode:
     def __init__(self, name_token: Token, value_node):
         self.name_token = name_token
         self.value_node = value_node
 
     def get_name(self) -> str:
         return self.name_token.value
@@ -99,8 +125,8 @@
     def __init__(self, statements: list):
         self.statements = statements
 
     def __str__(self):
         return f'statements: {self.statements}'
 
     def __repr__(self):
-        return f'MultipleStatementsNode({self.statements})'
+        return f'MultipleStatementsNode({self.statements})'
```

### Comparing `minecraft_script-0.1.405/minecraft_script/parser.py` & `minecraft_script-0.1.406/minecraft_script/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .tokens import Token
 from .errors import MCSSyntaxError
 from .text_additions import text_underline
 from .nodes import NumberNode, BinaryOperationNode, UnaryOperationNode, VariableAssignNode, VariableAccessNode, \
-    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode
+    FunctionAssignNode, FunctionCallNode, MultipleStatementsNode, ListNode, ListGetNode
 
 
 class Parser:
     def __init__(self, token_list: list[Token]):
         self.token_list = token_list
         self.current_index = -1
         self.current_token = None
@@ -18,37 +18,43 @@
         if self.current_index < len(self.token_list):
             self.current_token = self.token_list[self.current_index]
 
     def parse(self):
         result = self.statement()
         return result
 
-    def factor(self) -> NumberNode | UnaryOperationNode | BinaryOperationNode | VariableAccessNode | FunctionCallNode:
+    def factor(self) -> NumberNode | UnaryOperationNode | BinaryOperationNode | VariableAccessNode | FunctionCallNode | ListNode:
         token = self.current_token
 
         if token.value in ['+', '-']:
             self.advance()
             factor = self.factor()
             return UnaryOperationNode(token, factor)
 
         elif token.tt_type == 'TT_NAME':
             self.advance()
 
             if self.current_token.tt_type == 'TT_LEFT_PARENTHESIS':
                 return self.function_call(token)
 
+            elif self.current_token.tt_type == 'TT_LEFT_BRACKET':
+                return self.array_get(token)
+
             return VariableAccessNode(token)
 
         elif token.tt_type == 'TT_LEFT_PARENTHESIS':
             self.advance()
             expression = self.expression()
             if self.current_token.tt_type == 'TT_RIGHT_PARENTHESIS':
                 self.advance()
                 return expression
 
+        elif token.tt_type == 'TT_LEFT_BRACKET':
+            return self.array()
+
         elif token.tt_type == 'TT_NUMBER':
             self.advance()
             return NumberNode(token)
 
     def term(self) -> BinaryOperationNode:
         return self.binary_operation(self.factor, ['*', '/', '%'])
 
@@ -154,14 +160,59 @@
             self.advance()
             argument_tokens.append(self.factor())
 
         if self.current_token.tt_type == 'TT_RIGHT_PARENTHESIS':
             self.advance()
             return FunctionCallNode(name_token, argument_tokens)
 
+    def array(self) -> ListNode:
+        if self.current_token.tt_type != 'TT_LEFT_BRACKET':
+            MCSSyntaxError(f'Expected "[". Got {self.current_token.value} instead.')
+            exit()
+        self.advance()
+
+        array_contents = []
+
+        if self.current_token.tt_type != 'TT_RIGHT_BRACKET':
+            array_contents.append(self.expression())
+        else:
+            self.advance()
+            return ListNode(array_contents)
+
+        while self.current_token.tt_type == 'TT_COMMA':
+            self.advance()
+            if self.current_token.tt_type == 'TT_RIGHT_BRACKET':
+                self.advance()
+                return ListNode(array_contents)
+
+            array_contents.append(self.expression())
+
+        if self.current_token.tt_type == 'TT_RIGHT_BRACKET':
+            self.advance()
+            return ListNode(array_contents)
+
+        else:
+            MCSSyntaxError(f'Expected "]". Got {self.current_token.value} instead.')
+            exit()
+
+    def array_get(self, name_token) -> ListGetNode:
+        if self.current_token.tt_type != 'TT_LEFT_BRACKET':
+            MCSSyntaxError(f'Expected "[". Got {self.current_token.value} instead.')
+            exit()
+        self.advance()
+
+        index = self.term()
+
+        if self.current_token.tt_type == 'TT_RIGHT_BRACKET':
+            self.advance()
+            return ListGetNode(name_token, index)
+
+
+
+
 
 if __name__ == '__main__':
     tokens = [Token(5, 'TT_NUMBER'), Token('+', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
               Token('*', 'TT_BINARY_OPERATOR'), Token('(', 'TT_LEFT_PARENTHESIS'), Token(3, 'TT_NUMBER'),
               Token('+', 'TT_BINARY_OPERATOR'), Token('-', 'TT_BINARY_OPERATOR'), Token(5, 'TT_NUMBER'),
               Token(')', 'TT_RIGHT_PARENTHESIS')]
     print(Parser(tokens).parse())
```

### Comparing `minecraft_script-0.1.405/minecraft_script/shell_commands.py` & `minecraft_script-0.1.406/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.405/minecraft_script/text_additions.py` & `minecraft_script-0.1.406/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.405/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.1.406/minecraft_script.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-script
-Version: 0.1.405
+Version: 0.1.406
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
@@ -21,14 +21,23 @@
 # Commands
 ```cmd
 python -m minecraft_script help
 python -m minecraft_script run [files: optional, multiple allowed]
 python -m minecraft_script build [file]
 ```
 
+## Data Types
+Minecraft-script can only work with integers. This is due to the fact that strings aren't a thing in minecraft, and floating point numbers don't work in most cases, specifically scoreboards.
+This also means that the only division available is euclidean division.
+
+```js
+var number = 423  // number, has to be an integer
+var array = [1, 2, 3, 4, 5]  // array of numbers
+```
+
 ## Objects
 ### Variables
 The var keyword can be used to initialize new variables.
 Use it by following it by the variable's name, then an equals sign and a value.
 
 ```js
 var hello2 = 500  // initialized variable "hello2" with value 500
@@ -52,10 +61,32 @@
 ### log
 The log functions allows you to keep track of values in the console.
 It is equivalent to JavaScript's console.log() or Python's print() function.
 
 ```js
 var hello1 = 500
 
-log(200 + 200)  // logs "400" in console
+log(400)  // logs "400" in console
 log(hello1, 300)  // logs "500, 300" in console
+```
+
+### append
+Append a value to a list. The first argument has to be a list.
+```js
+var test = [3, 5, 4]
+
+append(test, 2)  // append 2 to the list
+append(test, [3, 4])  // append [3, 4] to the list
+
+log(test)  // logs "[3, 5, 4, 2, [3, 4]]"
+```
+
+### extend
+Extend a list by another list. Both arguments need to be lists.
+```js
+var list_1 = [5, 2]
+var list_2 = [2, 3]
+
+extend(list_1, list_2)
+
+log(list_1)  // logs "[5, 2, 2, 3]"
 ```
```

### Comparing `minecraft_script-0.1.405/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.406/minecraft_script.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.405/setup.py` & `minecraft_script-0.1.406/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.405'
+VERSION = '0.1.406'
 DESCRIPTION = 'Minecraft Script Programming language'
 
 # Setting up
 setup(
     name="minecraft_script",
     version=VERSION,
     author="Joyful-Bard",
```

