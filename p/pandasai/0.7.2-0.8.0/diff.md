# Comparing `tmp/pandasai-0.7.2.tar.gz` & `tmp/pandasai-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.7.2.tar", max compression
+gzip compressed data, was "pandasai-0.8.0.tar", max compression
```

## Comparing `pandasai-0.7.2.tar` & `pandasai-0.8.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1055 2023-07-24 10:38:30.978324 pandasai-0.7.2/LICENSE
--rw-r--r--   0        0        0     7705 2023-07-24 10:38:30.978324 pandasai-0.7.2/README.md
--rw-r--r--   0        0        0    26143 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/__init__.py
--rw-r--r--   0        0        0      155 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/callbacks/__init__.py
--rw-r--r--   0        0        0      519 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/callbacks/base.py
--rw-r--r--   0        0        0      583 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/callbacks/file.py
--rw-r--r--   0        0        0     1438 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     6404 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3070 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     3507 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4289 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    12126 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      585 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3130 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1578 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1261 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1380 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1256 2023-07-24 10:38:30.986325 pandasai-0.7.2/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1900 2023-07-24 10:38:30.990325 pandasai-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     8919 1970-01-01 00:00:00.000000 pandasai-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-07-27 19:15:30.960351 pandasai-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7853 2023-07-27 19:15:30.960351 pandasai-0.8.0/README.md
+-rw-r--r--   0        0        0    27955 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/callbacks/__init__.py
+-rw-r--r--   0        0        0      519 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/callbacks/base.py
+-rw-r--r--   0        0        0      583 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/callbacks/file.py
+-rw-r--r--   0        0        0     1438 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     6404 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     3631 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/from_google_sheets.py
+-rw-r--r--   0        0        0     1493 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3070 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     2454 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4289 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    12126 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      585 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3130 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     1230 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1578 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1261 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1380 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1256 2023-07-27 19:15:30.968351 pandasai-0.8.0/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1983 2023-07-27 19:15:30.972351 pandasai-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     9152 1970-01-01 00:00:00.000000 pandasai-0.8.0/PKG-INFO
```

### Comparing `pandasai-0.7.2/LICENSE` & `pandasai-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/README.md` & `pandasai-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
 
 After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
 
 ```bash
 pre-commit install
 ```
 
+## Contributors
+
+[![Contributors](https://contrib.rocks/image?repo=gventuri/pandas-ai)](https://github.com/gventuri/pandas-ai/graphs/contributors)
+
 ## 📜 License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Acknowledgements
 
 - This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
```

### Comparing `pandasai-0.7.2/pandasai/__init__.py` & `pandasai-0.8.0/pandasai/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -285,19 +285,50 @@
         """
 
         if self._enforce_privacy:
             # we don't want to send potentially sensitive data to the LLM server
             # if the user has set enforce_privacy to True
             return answer
 
-        generate_response_instruction = self._non_default_prompts.get(
-            "generate_response", GenerateResponsePrompt
-        )(question=question, answer=answer)
+        default_values = {"question": question, "answer": answer}
+        generate_response_instruction, _ = self._get_prompt(
+            "generate_response",
+            default_prompt=GenerateResponsePrompt,
+            default_values=default_values,
+        )
+
         return self._llm.call(generate_response_instruction, "")
 
+    def _get_prompt(
+        self, key: str, default_prompt: Prompt, default_values: Dict = {}, df=None
+    ):
+        prompt = self._non_default_prompts.get(key)
+
+        if prompt and isinstance(prompt, type):
+            prompt = prompt(**default_values)
+
+        if prompt:
+            """Override all the variables with _ prefix with default variable values"""
+            for var in prompt._args:
+                if var[0] == "_" and var[1:] in default_values:
+                    prompt.override_var(var, default_values[var[1:]])
+
+            """Replace all variables with $ prefix with evaluated values"""
+            prompt_text = prompt.text.split(" ")
+            for i in range(len(prompt_text)):
+                word = prompt_text[i]
+
+                if word.startswith("$"):
+                    prompt_text[i] = str(eval(word[1:]))
+            prompt.text = " ".join(prompt_text)
+
+            return prompt, prompt._args
+
+        return default_prompt(**default_values), default_values
+
     def run(
         self,
         data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
@@ -342,50 +373,59 @@
                     heads = [
                         anonymize_dataframe_head(dataframe)
                         if anonymize_df
                         else dataframe.head(rows_to_display)
                         for dataframe in data_frame
                     ]
 
-                    multiple_dataframes_instruction = self._non_default_prompts.get(
-                        "multiple_dataframes", MultipleDataframesPrompt
+                    multiple_dataframes_default_values = {"dataframes": heads}
+                    (
+                        multiple_dataframes_instruction,
+                        multiple_dataframes_instruction_values,
+                    ) = self._get_prompt(
+                        "multiple_dataframes",
+                        default_prompt=MultipleDataframesPrompt,
+                        default_values=multiple_dataframes_default_values,
+                        df=heads,
                     )
+
                     code = self._llm.generate_code(
-                        multiple_dataframes_instruction(dataframes=heads),
+                        multiple_dataframes_instruction,
                         prompt,
                     )
 
-                    self._original_instructions = {
-                        "question": prompt,
-                        "df_head": heads,
-                    }
+                    self._original_instructions = multiple_dataframes_instruction_values
 
                 else:
                     df_head = data_frame.head(rows_to_display)
                     if anonymize_df:
                         df_head = anonymize_dataframe_head(df_head)
                     df_head = df_head.to_csv(index=False)
 
-                    generate_code_instruction = self._non_default_prompts.get(
-                        "generate_python_code", GeneratePythonCodePrompt
-                    )(
-                        df_head=df_head,
-                        num_rows=data_frame.shape[0],
-                        num_columns=data_frame.shape[1],
+                    generate_code_default_values = {
+                        "df_head": df_head,
+                        "num_rows": data_frame.shape[0],
+                        "num_columns": data_frame.shape[1],
+                    }
+
+                    (
+                        generate_code_instruction,
+                        generate_code_instruction_values,
+                    ) = self._get_prompt(
+                        "generate_python_code",
+                        GeneratePythonCodePrompt,
+                        default_values=generate_code_default_values,
+                        df=data_frame,
                     )
+
                     code = self._llm.generate_code(
                         generate_code_instruction,
                         prompt,
                     )
-                    self._original_instructions = {
-                        "question": prompt,
-                        "df_head": df_head,
-                        "num_rows": data_frame.shape[0],
-                        "num_columns": data_frame.shape[1],
-                    }
+                    self._original_instructions = generate_code_instruction_values
 
                 if self.callback:
                     self.callback.on_code(code)
 
                 self.last_code_generated = code
                 self.log(
                     f"""
@@ -592,35 +632,45 @@
             multiple (bool): A boolean to indicate if the code is for multiple
             dataframes
 
         Returns (str): A python code
         """
 
         if multiple:
-            error_correcting_instruction = self._non_default_prompts.get(
+            correct_multiple_dataframes_error_default_values = {
+                "code": code,
+                "error_returned": e,
+                "question": self._original_instructions["question"],
+                "df_head": self._original_instructions["df_head"],
+            }
+
+            error_correcting_instruction, _ = self._get_prompt(
                 "correct_multiple_dataframes_error",
                 CorrectMultipleDataframesErrorPrompt,
-            )(
-                code=code,
-                error_returned=e,
-                question=self._original_instructions["question"],
-                df_head=self._original_instructions["df_head"],
+                default_values=correct_multiple_dataframes_error_default_values,
+                df=self._original_instructions["df_head"],
             )
 
         else:
-            error_correcting_instruction = self._non_default_prompts.get(
-                "correct_error", CorrectErrorPrompt
-            )(
-                code=code,
-                error_returned=e,
-                question=self._original_instructions["question"],
-                df_head=self._original_instructions["df_head"],
-                num_rows=self._original_instructions["num_rows"],
-                num_columns=self._original_instructions["num_columns"],
+            correct_error_default_values = {
+                "code": code,
+                "error_returned": e,
+                "question": self._original_instructions["question"],
+                "df_head": self._original_instructions["df_head"],
+                "num_rows": self._original_instructions["num_rows"],
+                "num_columns": self._original_instructions["num_columns"],
+            }
+
+            error_correcting_instruction, _ = self._get_prompt(
+                "correct_error",
+                CorrectErrorPrompt,
+                correct_error_default_values,
+                df=self._original_instructions["df_head"],
             )
+
         code = self._llm.generate_code(error_correcting_instruction, "")
         if self.callback:
             self.callback.on_code(code)
         return code
 
     def run_code(
         self,
```

### Comparing `pandasai-0.7.2/pandasai/callbacks/base.py` & `pandasai-0.8.0/pandasai/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/callbacks/file.py` & `pandasai-0.8.0/pandasai/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/constants.py` & `pandasai-0.8.0/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/exceptions.py` & `pandasai-0.8.0/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/helpers/_optional.py` & `pandasai-0.8.0/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/helpers/anonymizer.py` & `pandasai-0.8.0/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/helpers/cache.py` & `pandasai-0.8.0/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/helpers/from_excel.py` & `pandasai-0.8.0/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/helpers/notebook.py` & `pandasai-0.8.0/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/helpers/openai_info.py` & `pandasai-0.8.0/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/helpers/save_chart.py` & `pandasai-0.8.0/pandasai/helpers/save_chart.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,30 @@
 """Helper functions to save charts to a file, if plt.show() is called."""
 import ast
 import logging
 import os
-from itertools import zip_longest
 from os.path import dirname
-from typing import Union
 
 import astor
 
 
-def compare_ast(
-    node1: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
-    node2: Union[ast.expr, list[ast.expr], ast.stmt, ast.AST],
-    ignore_args=False,
-) -> bool:
-    """
-    Compare two AST nodes for equality.
-    Source: https://stackoverflow.com/a/66733795/11080806
-
-    Args:
-        node1 (ast.AST): First AST node to compare.
-        node2 (ast.AST): Second AST node to compare.
-        ignore_args (bool, optional): Whether to ignore the arguments of the nodes.
-            Defaults to False.
-
-    Returns:
-        bool: True if the nodes are equal, False otherwise.
-
-    """
-    if type(node1) is not type(node2):
+def is_show_node(node: ast.Call) -> bool:
+    if not hasattr(node, "value"):
         return False
 
-    if isinstance(node1, ast.AST):
-        for k, node in vars(node1).items():
-            if k in {"lineno", "end_lineno", "col_offset", "end_col_offset", "ctx"}:
-                continue
-            if ignore_args and k == "args":
-                continue
-            if not compare_ast(node, getattr(node2, k), ignore_args):
-                return False
-        return True
-
-    if isinstance(node1, list) and isinstance(node2, list):
-        return all(
-            compare_ast(n1, n2, ignore_args) for n1, n2 in zip_longest(node1, node2)
+    value = node.value
+    return (
+        isinstance(value, ast.Call)
+        and value.func
+        and (
+            isinstance(value.func, ast.Attribute)
+            and value.func.attr == "show"
+            and value.func.value.id == "plt"
         )
-
-    return node1 == node2
+    )
 
 
 def add_save_chart(
     code: str,
     folder_name: str,
     save_charts_path: str = None,
     print_save_dir: bool = True,
@@ -77,31 +51,28 @@
         charts_root_dir = dirname(dirname(dirname(__file__)))
 
     chart_save_dir = os.path.join(charts_root_dir, "exports", "charts", folder_name)
 
     tree = ast.parse(code)
 
     # count number of plt.show() calls
-    show_count = sum(
-        compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True)
-        for node in ast.walk(tree)
-    )
+    show_count = sum(1 for node in ast.walk(tree) if is_show_node(node))
 
     # if there are no plt.show() calls, return the original code
     if show_count == 0:
         return code
 
     if not os.path.exists(chart_save_dir):
         os.makedirs(chart_save_dir)
 
     # iterate through the AST and add plt.savefig() calls before plt.show() calls
     counter = ord("a")
     new_body = []
     for node in tree.body:
-        if compare_ast(node, ast.parse("plt.show()").body[0], ignore_args=True):
+        if is_show_node(node):
             filename = "chart"
             if show_count > 1:
                 filename += f"_{chr(counter)}"
                 counter += 1
 
             chart_save_path = os.path.join(chart_save_dir, f"{filename}.png")
             new_body.append(ast.parse(f"plt.savefig(r'{chart_save_path}')"))
```

### Comparing `pandasai-0.7.2/pandasai/helpers/shortcuts.py` & `pandasai-0.8.0/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/azure_openai.py` & `pandasai-0.8.0/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/base.py` & `pandasai-0.8.0/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/fake.py` & `pandasai-0.8.0/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/falcon.py` & `pandasai-0.8.0/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/google_palm.py` & `pandasai-0.8.0/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/langchain.py` & `pandasai-0.8.0/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/openai.py` & `pandasai-0.8.0/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/llm/starcoder.py` & `pandasai-0.8.0/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/middlewares/base.py` & `pandasai-0.8.0/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/middlewares/charts.py` & `pandasai-0.8.0/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/middlewares/streamlit.py` & `pandasai-0.8.0/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/prompts/base.py` & `pandasai-0.8.0/pandasai/prompts/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Base class to implement a new Prompt
 In order to better handle the instructions, this prompt module is written.
 """
 
 from pandasai.exceptions import MethodNotImplementedError
+from string import Formatter
 
 
 class Prompt:
     """Base class to implement a new Prompt"""
 
     text = None
     _args = {}
@@ -16,12 +17,26 @@
         __init__ method of Base class of Prompt Module
         Args:
             **kwargs: Inferred Keyword Arguments
         """
         if kwargs:
             self._args = kwargs
 
+        """Set all the variables with underscore prefix with default value as DEFAULT
+        This will prevent any possible key errors if anyone tries to print 
+        prompt before running .run method"""
+        if self.text:
+            vars = [
+                fn for _, fn, _, _ in Formatter().parse(self.text) if fn is not None
+            ]
+            for var in vars:
+                if var[0] == "_" and var not in self._args:
+                    self._args[var] = var
+
+    def override_var(self, var, value):
+        self._args[var] = value
+
     def __str__(self):
         if self.text is None:
             raise MethodNotImplementedError
 
         return self.text.format(**self._args)
```

### Comparing `pandasai-0.7.2/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.8.0/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.8.0/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/prompts/generate_python_code.py` & `pandasai-0.8.0/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.8.0/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.7.2/pyproject.toml` & `pandasai-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.7.2"
+version = "0.8.0"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
@@ -14,14 +14,15 @@
 astor = "^0.8.1"
 openai = "^0.27.5"
 ipython = "^8.13.1"
 matplotlib = "^3.7.1"
 google-generativeai = { version = "^0.1.0rc2", optional = true }
 google-cloud-aiplatform = { version = "^1.26.1", optional = true }
 langchain = { version = "^0.0.199", optional = true}
+beautifulsoup4 = { version = "^4.12.2", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 ruff = "^0.0.220"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
@@ -32,14 +33,15 @@
 [tool.poetry.group.extras.dependencies]
 google-cloud-aiplatform = "^1.26.1"
 
 [tool.poetry.extras]
 google = ["google-generativeai"]
 tests = ["numpy", "seaborn"]
 langchain = ["langchain"]
+bs4 = ["beautifulsoup4"]
 google-cloud = ["google-cloud-aiplatform"]
 
 [tool.poetry.group.whitelist.dependencies]
 statsmodels = {version = "^0.14.0", optional = true}
 scikit-learn = {version = "^1.2.2", optional = true}
 seaborn = {version = "^0.12.2", optional = true}
 plotly = {version = "^5.14.1", optional = true}
```

### Comparing `pandasai-0.7.2/PKG-INFO` & `pandasai-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.7.2
+Version: 0.8.0
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: bs4
 Provides-Extra: google
 Provides-Extra: google-cloud
 Provides-Extra: langchain
 Provides-Extra: tests
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) ; extra == "bs4"
 Requires-Dist: google-cloud-aiplatform (>=1.26.1,<2.0.0) ; extra == "google-cloud"
 Requires-Dist: google-generativeai (>=0.1.0rc2,<0.2.0) ; extra == "google"
 Requires-Dist: ipython (>=8.13.1,<9.0.0)
 Requires-Dist: langchain (>=0.0.199,<0.0.200) ; extra == "langchain"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: openai (>=0.27.5,<0.28.0)
 Requires-Dist: pandas (==1.5.3)
@@ -199,14 +201,18 @@
 
 After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
 
 ```bash
 pre-commit install
 ```
 
+## Contributors
+
+[![Contributors](https://contrib.rocks/image?repo=gventuri/pandas-ai)](https://github.com/gventuri/pandas-ai/graphs/contributors)
+
 ## 📜 License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Acknowledgements
 
 - This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
```

