# Comparing `tmp/promptz-0.0.7.tar.gz` & `tmp/promptz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptz-0.0.7.tar", last modified: Tue Jul 25 16:38:40 2023, max compression
+gzip compressed data, was "promptz-0.0.8.tar", last modified: Thu Jul 27 14:01:55 2023, max compression
```

## Comparing `promptz-0.0.7.tar` & `promptz-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:38:40.459707 promptz-0.0.7/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:38:40.459707 promptz-0.0.7/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)    14608 2023-07-25 15:57:54.000000 promptz-0.0.7/README.md
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:38:40.459707 promptz-0.0.7/promptz/
--rw-r--r--   0 rjl       (1000) rjl       (1000)    38967 2023-07-25 16:37:29.000000 promptz-0.0.7/promptz/__init__.py
--rw-r--r--   0 rjl       (1000) rjl       (1000)      151 2023-05-17 11:33:35.000000 promptz-0.0.7/promptz/main.py
-drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-25 16:38:40.459707 promptz-0.0.7/promptz.egg-info/
--rw-r--r--   0 rjl       (1000) rjl       (1000)      165 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/PKG-INFO
--rw-r--r--   0 rjl       (1000) rjl       (1000)      208 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/SOURCES.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/dependency_links.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)     2089 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/requires.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-25 16:38:40.000000 promptz-0.0.7/promptz.egg-info/top_level.txt
--rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-25 16:38:40.459707 promptz-0.0.7/setup.cfg
--rw-r--r--   0 rjl       (1000) rjl       (1000)      278 2023-07-25 16:37:35.000000 promptz-0.0.7/setup.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-27 14:01:55.297938 promptz-0.0.8/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    11357 2023-07-26 07:18:43.000000 promptz-0.0.8/LICENSE
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      187 2023-07-27 14:01:55.297938 promptz-0.0.8/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    14911 2023-07-26 07:07:09.000000 promptz-0.0.8/README.md
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-27 14:01:55.297938 promptz-0.0.8/promptz/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)    38207 2023-07-27 10:06:43.000000 promptz-0.0.8/promptz/__init__.py
+drwxr-xr-x   0 rjl       (1000) rjl       (1000)        0 2023-07-27 14:01:55.297938 promptz-0.0.8/promptz.egg-info/
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      187 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/PKG-INFO
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      200 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/SOURCES.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        1 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/dependency_links.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)     2089 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/requires.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)        8 2023-07-27 14:01:55.000000 promptz-0.0.8/promptz.egg-info/top_level.txt
+-rw-r--r--   0 rjl       (1000) rjl       (1000)       38 2023-07-27 14:01:55.297938 promptz-0.0.8/setup.cfg
+-rw-r--r--   0 rjl       (1000) rjl       (1000)      278 2023-07-27 14:01:45.000000 promptz-0.0.8/setup.py
```

### Comparing `promptz-0.0.7/README.md` & `promptz-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # promptz
 
 A lightweight library, built on top of pandas and pydantic, that lets you interact with language models and store the output as queryable embeddings.
 
 ## Getting starting
 
-To follow along and run the examples interactively using [./getting-started.ipynb]() or on [colab]().
+To follow along and run the examples interactively you can use [./getting-started.ipynb](https://github.com/layterz/promptz/blob/main/getting-started.ipynb) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/layterz/promptz/blob/main/getting-started.ipynb)
 
 ```python
 pip install promptz
 ```
 
+*Note: if install hangs or returns `Killed`, try running `pip install promptz --no-cache-dir`*
+
 First, you need to initialize the library, specifying the language model and embedding function to use.
 
 ```python
 import os
 import promptz
 from chromadb.utils.embedding_functions import OpenAIEmbeddingFunction
 
@@ -53,15 +55,15 @@
 His face is covered by a mask, leaving only his piercing blue eyes visible.
                                                                                 
 Personality: Intense, determined, and highly disciplined. Bruce Wayne is known
 for his relentless pursuit of justice and his unwavering commitment to
 protecting Gotham City. He is intensely focused, often seen as aloof and...
 ```
 
-The response is a raw string of the response from the model. This might be what you want if you're writing an email or asking a question, but other times you'll need to convert the response into structured data.
+The response is a raw string from the model output. This might be what you want if you're writing an email or asking a question, but other times you'll need to convert the response into structured data.
 
 To do that, you can pass a `pydantic.BaseModel` as `output=` when calling `prompt`. This will add format instructions, based on the pydantic schema and field annotations, and return an instance of the output model using the generated data.
 
 ```python
 from typing import List
 from pydantic import BaseModel, Field
 from promptz import prompt
@@ -192,15 +194,15 @@
 ```
 
 For example, `[{name: 'Batman'}, {description: 'Batman, also known as...'}, {age: 35}]` would be converted into 3 embeddings for the first item. You can then query collections using those field embeddings.
 
 ```python
 from promptz import query
 
-villains = query('they are a villain').first
+villains = query('they are a villain')
 ```
 ```
     id	                                    description	                                        type	    name	            age
 26	7143239c-9a6a-4dc3-84a6-f4c53faf8dda	Nightstrike is a former Gotham City Police off...	character	Nightstrike	        35
 27	03f387bd-3264-4add-a296-fa74a7e9fa5d	Crimson Shade is a master of deception and ill...	character	Crimson Shade	    29
 17	1bad4da4-a6d1-408e-a785-61649fbe7a8e	The Enforcer is a highly trained martial artis...	character	The Enforcer	    28
 6	61896717-f5f5-4d79-9f46-268232b2a1b0	Nightshade is a mysterious vigilante who uses ...	character	Nightshade	        34
```

### Comparing `promptz-0.0.7/promptz/__init__.py` & `promptz-0.0.8/promptz/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import uuid
 import textwrap
 import json
 from json import JSONDecodeError
 from enum import Enum
 from typing import Type, Callable, List, Tuple, Dict, Union, Any, Literal 
 from abc import abstractmethod
+import base64
+from IPython.display import display, HTML, Image
 import torch
 from torch import nn
 import numpy as np
 import pandas as pd
 from jinja2 import Template
 from pydantic import BaseModel, ValidationError 
 from datetime import datetime
@@ -20,153 +22,73 @@
 import openai
 from openai.error import RateLimitError
 import chromadb
 import colorama
 
 colorama.just_fix_windows_console()
 
+FORMAT_INSTRUCTIONS = logging.DEBUG + 1
+CONTEXT = logging.DEBUG + 2
+EXAMPLES = logging.DEBUG + 3
+METRICS = logging.DEBUG + 4
+HISTORY = logging.DEBUG + 5
+INSTRUCTIONS = logging.INFO + 1
+INPUT = logging.INFO + 2
+OUTPUT = logging.INFO + 3
+
+logging.addLevelName(FORMAT_INSTRUCTIONS, "FORMAT INSTRUCTIONS")
+logging.addLevelName(CONTEXT, "CONTEXT")
+logging.addLevelName(EXAMPLES, "EXAMPLES")
+logging.addLevelName(INSTRUCTIONS, "INSTRUCTIONS")
+logging.addLevelName(INPUT, "INPUT")
+logging.addLevelName(OUTPUT, "OUTPUT")
+logging.addLevelName(METRICS, "METRICS")
+logging.addLevelName(HISTORY, "HISTORY")
 
-class PromptLogger(logging.Logger):
-
-    FORMAT_INSTRUCTIONS = logging.DEBUG + 1
-    CONTEXT = logging.DEBUG + 2
-    EXAMPLES = logging.DEBUG + 3
-    METRICS = logging.DEBUG + 4
-    HISTORY = logging.DEBUG + 5
-    INSTRUCTIONS = logging.INFO + 1
-    INPUT = logging.INFO + 2
-    OUTPUT = logging.INFO + 3
+class NotebookFormatter(logging.Formatter):
 
     colors = {
         FORMAT_INSTRUCTIONS: colorama.Fore.CYAN,
         CONTEXT: colorama.Fore.BLACK + colorama.Back.YELLOW,
         EXAMPLES: colorama.Fore.MAGENTA,
         METRICS: colorama.Fore.WHITE + colorama.Style.DIM,
         HISTORY: colorama.Back.WHITE + colorama.Fore.BLACK,
         INSTRUCTIONS: colorama.Fore.YELLOW,
         INPUT: colorama.Fore.BLUE,
         OUTPUT: colorama.Fore.GREEN,
         logging.ERROR: colorama.Fore.RED,
         logging.INFO: colorama.Fore.WHITE,
         logging.DEBUG: colorama.Style.DIM,
     }
-    
-    def __init__(self, name, level=logging.DEBUG, formatter=None):
-        super().__init__(name)
-        logging.addLevelName(self.FORMAT_INSTRUCTIONS, "FORMAT INSTRUCTIONS")
-        logging.addLevelName(self.CONTEXT, "CONTEXT")
-        logging.addLevelName(self.EXAMPLES, "EXAMPLES")
-        logging.addLevelName(self.INSTRUCTIONS, "INSTRUCTIONS")
-        logging.addLevelName(self.INPUT, "INPUT")
-        logging.addLevelName(self.OUTPUT, "OUTPUT")
-        logging.addLevelName(self.METRICS, "METRICS")
-        logging.addLevelName(self.HISTORY, "HISTORY")
-
-        if formatter is None:
-            formatter = logging.Formatter('%(message)s')
-        ch = logging.StreamHandler()
-        ch.setLevel(level)
-        ch.setFormatter(formatter)
-        self.addHandler(ch)
-        self.setLevel(level)
 
-    def format_instructions(self, msg, *args, **kwargs):
-        self._log(self.FORMAT_INSTRUCTIONS, msg, args, **kwargs)
+    def __init__(self, width=80, **kwargs):
+        super().__init__(**kwargs)
+        self.width = width
+
+    def format(self, record) -> str:
+        color = self.colors.get(record.levelno, None)
+        msg = f'{color}{record.getMessage()}{colorama.Style.RESET_ALL}'
+        return '\n'.join([
+            textwrap.fill(line.strip(), width=self.width).ljust(self.width, ' ')
+            for line in msg.split('\n')
+        ])
 
-    def context(self, msg, *args, **kwargs):
-        self._log(self.CONTEXT, msg, args, **kwargs)
 
-    def examples(self, msg, *args, **kwargs):
-        self._log(self.EXAMPLES, msg, args, **kwargs)
-    
-    def instructions(self, msg, *args, **kwargs):
-        self._log(self.INSTRUCTIONS, msg, args, **kwargs)
-
-    def input(self, msg, *args, **kwargs):
-        self._log(self.INPUT, msg, args, **kwargs)
-
-    def output(self, msg, *args, **kwargs):
-        self._log(self.OUTPUT, msg, args, **kwargs)
-    
-    def error(self, msg, *args, **kwargs):
-        self._log(logging.ERROR, msg, args, **kwargs)
-    
-    def debug(self, msg, *args, **kwargs):
-        self._log(logging.DEBUG, msg, args, **kwargs)
-    
-    def metrics(self, msg, *args, **kwargs):
-        self._log(self.METRICS, msg, args, **kwargs)
-    
-    def history(self, msg, *args, **kwargs):
-        self._log(self.HISTORY, msg, args, **kwargs)
-
-
-class NotebookLogger(PromptLogger):
-    
-    def _log(self, level, msg, *args, wrap=False, **kwargs):
-        color = self.colors.get(level, None)
-        if wrap:
-            width = 80
-            msg = '\n'.join([
-                textwrap.fill(line.strip(), width=80).ljust(width, ' ')
-                for line in msg.split('\n')
-            ])
-        msg = f'{color}{msg}{colorama.Style.RESET_ALL}'
-        return super()._log(level, msg, *args, **kwargs)
-    
-    def format_instructions(self, msg, *args, **kwargs):
-        self._log(self.FORMAT_INSTRUCTIONS, f'''
-        FORMAT
-        ===
-        {msg}
-        ''', args, wrap=True, **kwargs)
-
-    def context(self, msg, *args, **kwargs):
-        self._log(self.CONTEXT, f'CONTEXT: {msg}', args, wrap=True, **kwargs)
-
-    def examples(self, msg, *args, **kwargs):
-        self._log(self.EXAMPLES, f'''
-        EXAMPLES
-        ===
-        {msg}
-        ''', args, wrap=True, **kwargs)
-    
-    def instructions(self, msg, *args, **kwargs):
-        self._log(self.INSTRUCTIONS, f'''
-        INSTRUCTIONS
-        ===
-        {msg}
-        ''', args, wrap=True, **kwargs)
-
-    def input(self, msg, *args, **kwargs):
-        self._log(self.INPUT, f'''
-        INPUT:
-        ===
-        {msg}
-        ''', args, wrap=True, **kwargs)
-
-    def output(self, msg, *args, **kwargs):
-        self._log(self.OUTPUT, f'''
-        OUTPUT
-        ===
-        {msg}
-        ''', args, wrap=True, **kwargs)
-    
-    def error(self, msg, *args, **kwargs):
-        self._log(logging.ERROR, f'ERROR', args, wrap=True, **kwargs)
-        self._log(logging.ERROR, msg, args, wrap=True, **kwargs)
-    
-    def debug(self, msg, *args, **kwargs):
-        self._log(logging.DEBUG, msg, args, wrap=True, **kwargs)
-    
-    def metrics(self, msg, *args, **kwargs):
-        self._log(self.METRICS, msg, args, **kwargs)
-    
-    def history(self, msg, *args, **kwargs):
-        self._log(self.HISTORY, msg, args, wrap=True, **kwargs)
+class JSONLogFormatter(logging.Formatter):
+    def format(self, record):
+        msg = super().format(record)
+        log_entry = {
+            "timestamp": record.created,
+            "level": record.levelname,
+            "message": msg,
+            "filename": record.filename,
+            "lineno": record.lineno,
+            "funcName": record.funcName,
+        }
+        return json.dumps(log_entry)
 
 
 class Callback(BaseModel):
     name: str
     params: Dict[str, Any] = None
 
 
@@ -294,14 +216,42 @@
                 model=f'{self.__class__.__name__}.{self.model}',
                 input_tokens=output.usage.get('prompt_tokens'),
                 output_tokens=output.usage.get('completion_tokens')
             ),
         )
 
 
+class ImageResponse(Response):
+    
+    def __repr__(self) -> str:
+        image_bytes = base64.b64decode(self.raw)
+        display(Image(data=image_bytes))
+
+
+class DALL_E(LLM):
+    
+    def __init__(self, api_key=None, org_id=None):
+        openai.api_key = api_key or os.environ.get('OPENAI_API_KEY')
+        openai.organization = org_id or os.environ.get('OPENAI_ORG_ID')
+
+    def generate(self, x, **kwargs) -> Response:
+        output = openai.Image.create(
+            prompt=x,
+            n=1,
+            size='512x512',
+            response_format='b64_json',
+        )
+        return ImageResponse(
+            raw=output['data'][0]['b64_json'],
+            metrics=Metrics(
+                input_tokens=len(x),
+            )
+        )
+
+
 class HuggingfaceTransformer(LLM):
     model: PreTrainedModel
     tokenizer: PreTrainedTokenizer
     max_length: int
 
     def __init__(self, model, tokenizer, max_length=50, **kwargs):
         self.model = model
@@ -462,25 +412,15 @@
     num_examples: int = 1
     output: Type[BaseModel] = None
     llm: LLM = MockLLM()
 
     def __init__(self, instructions=None, output=None, context=None, template=None, examples=None, num_examples=None, history=None, llm=None, logger=None, debug=False, silent=False, tools: ToolList = None):
         super().__init__()
 
-        if logger is None:
-            logger = NotebookLogger(f'prompt.{self.__class__.__name__}')
-
-        level = logging.INFO
-        if debug:
-            level = logging.DEBUG
-        elif silent:
-            level = logging.ERROR
-        logger.setLevel(level)
         self.logger = logger
-
         self.name = self.__class__.__name__
         self.llm = llm or self.llm
         self.context = context or self.context
         self.history = history or self.history
         self.output = output or self.output
         instructions = instructions or self.__doc__
         if instructions is None:
@@ -613,57 +553,59 @@
                 return self.output(**d)
             return Collection(rows)
         else:
             return output
     
     def forward(self, x, retries=3, dryrun=False, **kwargs):
         if retries and retries <= 0:
-            raise MaxRetriesExceeded(f'{self.name} failed to forward {x}')
+            e = MaxRetriesExceeded(f'{self.name} failed to forward {x}')
+            self.logger.error(e)
+            raise e
         
         if dryrun:
             self.logger.debug(f'Dryrun: {self.output}')
             llm = MockLLM(output=self.output)
         else:
             llm = self.llm
         
         px = self.parse(x)
             
         if self.template is not None and self.template != '':
             prompt_input = self.render({'input': px})
             if self.context: self.logger.context(self.context)
-            self.logger.history('\n\n\n'.join([f'''
+            self.logger.log(HISTORY, '\n\n\n'.join([f'''
             {log.input}
             {log.output}
             ''' for log in self.history]))
-            self.logger.instructions(self.instructions)
-            if len(self.examples): self.logger.examples(self.render_examples())
-            if len(px): self.logger.input(px)
+            self.logger.log(INSTRUCTIONS, self.instructions)
+            if len(self.examples): self.logger.log(EXAMPLES, self.render_examples())
+            if len(px): self.logger.log(INPUT, px)
             tools = [t.info for t in self.tools]
             response = llm.generate(prompt_input, context=self.context, history=self.history, tools=tools)
             if response.callback is not None:
                 function_name = response.callback.name
                 tool = next(t for t in self.tools if t.name == function_name)
                 params = {p['name']: response.callback.params.get(p['name']) 
                           for p in tool.parameters}
                 rsp = tool(**params)
                 return None
-            if self.output: self.logger.format_instructions(self.render_format(px))
+            if self.output: self.logger.log(FORMAT_INSTRUCTIONS, self.render_format(px))
             try:
-                self.logger.output(response.raw)
+                self.logger.log(OUTPUT, response.raw)
                 response.content = self.process(px, response.raw, **kwargs)
             except ValidationError as e:
-                self.logger.error(f'Output validation failed: {e} {response.content}')
+                self.logger.warn(f'Output validation failed: {e} {response.content}')
                 return self.forward(x, retries=retries-1, **kwargs)
             except JSONDecodeError as e:
-                self.logger.error(f'Failed to decode JSON from {response.content}: {e}')
+                self.logger.warn(f'Failed to decode JSON from {response.content}: {e}')
                 return self.forward(x, retries=retries-1, **kwargs)
             except RateLimitError as e:
-                self.logger.error(f'Hit rate limit for {self}: {e}')
+                self.logger.warn(f'Hit rate limit for {self}: {e}')
                 return self.forward(x, retries=retries-1, **kwargs)
-            self.logger.metrics(response.metrics)
+            self.logger.log(METRICS, response.metrics)
             return response
 
 
 class Query:
 
     def __init__(self, query=None, where=None, collection=None, **kwargs):
         self.query = query
@@ -716,14 +658,32 @@
         arbitrary_types_allowed = True
     
     def __init__(self, **data):
         super().__init__(**data)
     
     def __repr__(self):
         return self.json()
+    
+    def display(self):
+        # Check if we're in an IPython environment
+        try:
+            get_ipython
+        except NameError:
+            # If we're not in an IPython environment, fall back to json
+            return self.json()
+
+        # Convert the dictionary to a HTML table
+        html = '<table>'
+        for field, value in self.dict().items():
+            html += f'<tr><td>{field}</td><td>{value}</td></tr>'
+        html += '</table>'
+
+        # Display the table
+        display(HTML(html))
+        return self.json()
 
 
 class EntitySeries(pd.Series):
 
     @property
     def _constructor(self):
         return EntitySeries
@@ -888,15 +848,15 @@
         self.name = name
         self.db = db
         self.llm = llm
         self.ef = ef
         self._collection = default_collection
         if collections is not None:
             self._collections = collections 
-        self.logger = logger or NotebookLogger(name)
+        self.logger = logger
         self._history = []
         self.use_cache = use_cache
     
     def activate(self):
         set_default_session(self)
     
     def _run_prompt(self, p, input, dryrun=False, retries=3, **kwargs):
@@ -927,31 +887,37 @@
         except MaxRetriesExceeded as e:
             self.logger.error(f'Max retries exceeded: {e}')
             return None
     
     def _run_batch(self, p, inputs, dryrun=False, retries=3, **kwargs):
         for input in inputs:
             o = self._run_prompt(p, input, dryrun=dryrun, retries=retries, **kwargs)
-            yield o
+            yield o.content
 
     def prompt(self, instructions=None, input=None, output=None, prompt=None, context=None, template=None, llm=None, examples=None, num_examples=1, history=None, tools=None, dryrun=False, retries=3, debug=False, silent=False, **kwargs):
+        logger = self.logger.getChild('prompt')
+        level = logging.INFO
+        if debug: level = logging.DEBUG
+        elif silent: level = logging.ERROR
+        logger.setLevel(level)
+
         if prompt is None:
             p = Prompt(
                 output=output,
                 instructions=instructions,
                 llm=llm or self.llm,
                 context=context,
                 examples=examples,
                 num_examples=num_examples,
                 history=history,
                 tools=tools,
                 template=template,
                 debug=debug,
                 silent=silent,
-                logger=self.logger,
+                logger=logger,
             )
         else:
             p = prompt
             p.llm = llm or self.llm
             p.logger = self.logger
             p.debug = debug
             p.silent = silent
@@ -967,22 +933,22 @@
         if isinstance(item, str):
             return self.ef([item])[0]
         elif isinstance(item, BaseModel):
             return self.ef([item.json()])[0]
         elif isinstance(item, list):
             return [self.embed(i, field=field) for i in item]
     
-    def query(self, query=None, field=None, where=None, collection=None):
+    def query(self, *texts, field=None, where=None, collection=None):
         c = self.collection(collection)
-        if query is None and field is None and where is None:
+        if len(texts) == 0 and field is None and where is None:
             return c
         where = where or {}
         if field is not None:
             where['field'] = field
-        return c(query, where=where)
+        return c(*texts, where=where)
 
     def store(self, *items, collection=None):
         def flatten(lst):
             return [
                 item for sublist in lst 
                 for item in (
                     flatten(sublist) if isinstance(sublist, list) else [sublist]
@@ -1085,31 +1051,42 @@
             raise NotImplementedError
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         return self.process(*args, **kwds)
 
 
 class World:
+    name: str
     sessions: List[Session]
     collections: Dict[str, Collection]
     systems: List[System]
 
-    def __init__(self, systems=None, llm=None, ef=None, logger=None, db=None):
+    def __init__(self, name, systems=None, llm=None, ef=None, logger=None, db=None):
+        self.name = name
         self.sessions = []
         self.collections = {}
         self.systems = systems
         self.llm = llm or MockLLM()
         self.ef = ef or (lambda x: [0] * len(x))
         self.db = db or ChromaVectorDB
-        self.logger = logger or NotebookLogger(self.__class__.__name__)
+        self.logger = logger or logging.getLogger(self.name)
     
-    def create_session(self, name=None, db=None, llm=None, ef=None, logger=None, use_cache=False):
+    def create_session(self, name=None, db=None, llm=None, ef=None, logger=None, silent=False, debug=False, use_cache=False, log_format='notebook'):
         llm = llm or self.llm
         ef = ef or self.ef
         db = db or self.db()
+        logger = logger or self.logger.getChild(f'session.{name}')
+        ch = logging.StreamHandler()
+        formatter = JSONLogFormatter() if log_format == 'json' else NotebookFormatter()
+        ch.setFormatter(formatter)
+        self.logger.addHandler(ch)
+        level = logging.INFO
+        if debug: level = logging.DEBUG
+        elif silent: level = logging.ERROR
+        logger.setLevel(level)
         session = Session(name=name, db=db, llm=llm, ef=ef, logger=logger,
                           collections=self.collections, use_cache=use_cache)
         self.sessions = self.sessions.append(session)
         return session
     
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         session = self.create_session(
@@ -1147,17 +1124,17 @@
     return DEFAULT_SESSION.chain(*steps, **kwargs)
 
 
 def store(*items, collection=None, **kwargs) -> Collection:
     return DEFAULT_SESSION.store(*items, collection=collection, **kwargs)
 
 
-def query(query=None, field=None, where=None, collection=None, **kwargs) -> Collection:
+def query(*texts, field=None, where=None, collection=None, **kwargs) -> Collection:
     return DEFAULT_SESSION.query(
-        query, field=field, where=where, collection=collection, **kwargs)
+        *texts, field=field, where=where, collection=collection, **kwargs)
 
 
 def collection(name=None) -> Collection:
     return DEFAULT_SESSION.collection(name)
 
 
 def evaluate(*testcases, **kwargs) -> Collection:
@@ -1193,12 +1170,12 @@
     DEFAULT_SESSION = session
 
 
 Embedding = List[float]
 EmbedFunction = Callable[[List[str]], List[Embedding]]
 
 
-def init(llm=None, ef=None, logger=None, use_cache=False, **kwargs):
-    w = World(llm=llm, ef=ef, logger=logger, **kwargs)
-    session = w.create_session(use_cache=use_cache)
+def init(llm=None, ef=None, logger=None, use_cache=False, log_format='notebook', **kwargs):
+    w = World('test', llm=llm, ef=ef, logger=logger, **kwargs)
+    session = w.create_session(use_cache=use_cache, log_format=log_format)
     set_default_world(w)
     set_default_session(session)
```

### Comparing `promptz-0.0.7/promptz.egg-info/requires.txt` & `promptz-0.0.8/promptz.egg-info/requires.txt`

 * *Files identical despite different names*

