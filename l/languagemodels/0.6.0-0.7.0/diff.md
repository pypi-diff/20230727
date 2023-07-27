# Comparing `tmp/languagemodels-0.6.0.tar.gz` & `tmp/languagemodels-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "languagemodels-0.6.0.tar", last modified: Fri Jun 30 03:21:39 2023, max compression
+gzip compressed data, was "languagemodels-0.7.0.tar", last modified: Thu Jul 27 14:47:18 2023, max compression
```

## Comparing `languagemodels-0.6.0.tar` & `languagemodels-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-30 03:21:39.589745 languagemodels-0.6.0/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9369 2023-06-30 03:21:39.585744 languagemodels-0.6.0/PKG-INFO
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-30 03:21:39.585744 languagemodels-0.6.0/languagemodels/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10679 2023-06-30 03:08:32.000000 languagemodels-0.6.0/languagemodels/__init__.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     5811 2023-06-28 20:37:56.000000 languagemodels-0.6.0/languagemodels/embeddings.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     7919 2023-06-30 03:08:32.000000 languagemodels-0.6.0/languagemodels/inference.py
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8340 2023-06-30 03:08:32.000000 languagemodels-0.6.0/languagemodels/models.py
-drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-06-30 03:21:39.585744 languagemodels-0.6.0/languagemodels.egg-info/
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9369 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/PKG-INFO
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      306 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/SOURCES.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/dependency_links.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       61 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/requires.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-06-30 03:21:39.000000 languagemodels-0.6.0/languagemodels.egg-info/top_level.txt
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-06-30 03:21:39.589745 languagemodels-0.6.0/setup.cfg
--rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      800 2023-06-30 03:19:50.000000 languagemodels-0.6.0/setup.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-07-27 14:47:18.560143 languagemodels-0.7.0/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9974 2023-07-27 14:47:18.560143 languagemodels-0.7.0/PKG-INFO
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-07-27 14:47:18.556142 languagemodels-0.7.0/languagemodels/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    12249 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/__init__.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9502 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/config.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     8157 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/embeddings.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)    10112 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/inference.py
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     3526 2023-07-27 14:43:00.000000 languagemodels-0.7.0/languagemodels/models.py
+drwxrwxr-x   0 jncraton  (1000) jncraton  (1000)        0 2023-07-27 14:47:18.560143 languagemodels-0.7.0/languagemodels.egg-info/
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)     9974 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/PKG-INFO
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      331 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/SOURCES.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)        1 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/dependency_links.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       47 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/requires.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       15 2023-07-27 14:47:18.000000 languagemodels-0.7.0/languagemodels.egg-info/top_level.txt
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)       38 2023-07-27 14:47:18.560143 languagemodels-0.7.0/setup.cfg
+-rw-rw-r--   0 jncraton  (1000) jncraton  (1000)      775 2023-07-27 14:43:00.000000 languagemodels-0.7.0/setup.py
```

### Comparing `languagemodels-0.6.0/PKG-INFO` & `languagemodels-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.6.0
+Version: 0.7.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![x64 Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
-        [![ARM64 Build](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml)[![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
+        [![ARM64 Build](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jncraton/languagemodels/blob/master/examples/translate.ipynb)
         
         Python building blocks to explore large language models on any computer with 512MB of RAM
         
         [![Try with Replit Badge](https://replit.com/badge?caption=Try%20with%20Replit&variant=small)](https://replit.com/@jncraton/langaugemodels#main.py)
         
         ![Translation hello world example](media/hello.gif)
         
-        Target Audience
-        ---------------
-        
-        This package is designed to be as simple as possible for **learners** and **educators** exploring how large language models intersect with modern software development. The interfaces to this package are all simple functions using standard types. The complexity of large language models is hidden from view while providing free local inference using light-weight, open models. All included models are free for educational use, no API keys are required, and all inference is performed locally by default.
+        This package makes using large language models in software as simple as possible. All inference is performed locally to keep your data private by default.
         
         Installation and Getting Started
         --------------------------------
         
         This package can be installed using the following command:
         
         ```sh
@@ -46,33 +43,47 @@
         This will require downloading a significant amount of data (~250MB) on the first run. Models will be cached for later use and subsequent calls should be quick.
         
         Example Usage
         -------------
         
         Here are some usage examples as Python REPL sessions. This should work in the REPL, notebooks, or in traditional scripts and applications.
         
-        ### Text Completions
+        ### Instruction Following
         
         ```python
         >>> import languagemodels as lm
         
-        >>> lm.complete("She hid in her room until")
-        'she was sure she was safe'
+        >>> lm.do("Translate to English: Hola, mundo!")
+        'Hello, world!'
+        
+        >>> lm.do("What is the capital of France?")
+        'Paris.'
         ```
         
-        ### Instruction Following
+        ### Adjusting Model Performance
+        
+        The base model should run quickly on any system with 512MB of memory, but this memory limit can be increased to select more powerful models that will consume more resources. Here's an example:
         
         ```python
         >>> import languagemodels as lm
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'You have 8 apples.'
+        >>> lm.set_max_ram('4gb')
+        4.0
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'I have 2 apples left.'
+        ```
         
-        >>> lm.do("Translate to English: Hola, mundo!")
-        'Hello, world!'
+        ### Text Completions
         
-        >>> lm.do("What is the capital of France?")
-        'Paris.'
+        ```python
+        >>> import languagemodels as lm
+        
+        >>> lm.complete("She hid in her room until")
+        'she was sure she was safe'
         ```
         
         ### Chat
         
         ```python
         >>> lm.chat('''
         ...      System: Respond as a helpful assistant.
@@ -80,14 +91,29 @@
         ...      User: What time is it?
         ...
         ...      Assistant:
         ...      ''')
         'I'm sorry, but as an AI language model, I don't have access to real-time information. Please provide me with the specific time you are asking for so that I can assist you better.'
         ```
         
+        ### Code
+        
+        A model tuned on Python code is included. It can be used to complete code snippets.
+        
+        ```python
+        >>> import languagemodels as lm
+        >>> lm.code("""
+        ... a = 2
+        ... b = 5
+        ...
+        ... # Swap a and b
+        ... """)
+        'a, b = b, a'
+        ```
+        
         ### External Retrieval
         
         Helper functions are provided to retrieve text from external sources that can be used to augment prompt context.
         
         ```python
         >>> import languagemodels as lm
         
@@ -116,93 +142,78 @@
         
         ### Semantic Search
         
         Semantic search is provided to retrieve documents that may provide helpful context from a document store.
         
         ```python
         >>> import languagemodels as lm
-        
-        >>> lm.store_doc("Mars is a planet")
-        >>> lm.store_doc("The sun is hot")
-        >>> lm.load_doc("What is Mars?")
-        'Mars is a planet'
-        ```
-        
-        This can also be used to get a blend of context from stored documents:
-        
-        ```python
-        >>> import languagemodels as lm
         >>> lm.store_doc(lm.get_wiki("Python"), "Python")
         >>> lm.store_doc(lm.get_wiki("C language"), "C")
         >>> lm.store_doc(lm.get_wiki("Javascript"), "Javascript")
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
-        'Python: It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.
-        
-        C: It was designed to be compiled to provide low-level access to memory and language constructs that map efficiently to machine instructions, all with minimal runtime support.
+        'From Python document: It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.
         
-        C: The book The C Programming Language, co-authored by the original language designer, served for many years as the de facto standard for the language.'
+        From C document: It was designed to be compiled to provide low-level access to memory and language constructs that map efficiently to machine instructions, all with minimal runtime support.'
         ```
         
-        ### Performance
+        [Full documentation](https://languagemodels.netlify.app/)
         
-        The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
+        ### Speed
         
-        The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
+        This package currently outperforms Hugging Face `transformers` for CPU inference thanks to int8 quantization and the [CTranslate2](https://github.com/OpenNMT/CTranslate2) backend. The following table compares CPU inference performance on identical models using the best available quantization on a 20 question test set.
         
-        ```python
-        >>> import languagemodels as lm
-        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
-        'You have 8 apples.'
-        >>> lm.set_max_ram('4gb')
-        4.0
-        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
-        'I have 2 apples left.'
-        ```
+        | Backend                   | Inference Time | Memory Used |
+        |---------------------------|----------------|-------------|
+        | Hugging Face transformers | 22s            | 1.77GB      |
+        | This package              | 11s            | 0.34GB      |
         
-        [Full documentation](https://languagemodels.netlify.app/)
+        Note that quantization does technically harm output quality slightly, but it should be negligible at this level.
+        
+        ### Models
+        
+        This package does allow direct model selection, but sensible defaults are preferred to allow the package to improve over time as stronger models become available. The models used are 1000x smaller than the largest models in use today. They are useful as learning tools, but perform far below the current state of the art.
+        
+        This package currently uses [LaMini-Flan-T5-base](https://huggingface.co/MBZUAI/LaMini-Flan-T5-248M) as its default model. This is a fine-tuning of the T5 base model on top of the [FLAN](https://huggingface.co/google/flan-t5-base) fine-tuning. The model is tuned to respond to instructions in a human-like manner. The following human evaluations were reported in the [paper](https://github.com/mbzuai-nlp/LaMini-LM) associated with this model family:
+        
+        ![Human-rated model comparison](media/model-comparison.png)
+        
+        For code completions, the [CodeT5+](https://arxiv.org/abs/2305.07922) series of models are used.
         
         Commercial Use
         --------------
         
-        This package itself is licensed for commerical use, but the models used may not be compatible with commercial use. In order to use this package commercially, you may want to filter models by their license type using the `require_model_license` function.
+        This package itself is licensed for commercial use, but the models used may not be compatible with commercial use. In order to use this package commercially, you can filter models by license type using the `require_model_license` function.
         
         ```python
         >>> import languagemodels as lm
-        >>> lm.do("What is your favorite animal.")
-        >>> "As an AI language model, I don't have preferences or emotions."
-        >>> lm.require_model_license("apache.*|mit")
-        >>> lm.do("What is your favorite animal.")
-        'Lion.'
+        >>> lm.config['instruct_model']
+        'LaMini-Flan-T5-248M-ct2-int8'
+        >>> lm.require_model_license("apache|bsd|mit")
+        >>> lm.config['instruct_model']
+        'flan-t5-base-ct2-int8'
         ```
         
-        The commercially-licensed models may not perform as well as the default models. It is recommended to confirm that the models used do meet the licensing requirements for your software.
+        It is recommended to confirm that the models used meet the licensing requirements for your software.
         
         Projects Ideas
         --------------
         
-        This package can be used to do the heavy lifting for a number of learning projects:
+        One of the goals for this package is to be a straightforward tool for learners and educators exploring how large language models intersect with modern software development. It can be used to do the heavy lifting for a number of learning projects:
         
         - CLI Chatbot (see [examples/chat.py](examples/chat.py))
         - Streamlit chatbot (see [examples/streamlitchat.py](examples/streamlitchat.py))
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search over documents
         - Document question answering
         
         Several example programs and notebooks are included in the `examples` directory.
         
-        Attribution
-        -----------
-        
-        - [CTranslate2](https://github.com/OpenNMT/CTranslate2)
-        - [LaMini-Flan-T5](https://huggingface.co/MBZUAI/LaMini-Flan-T5-783M)
-        - [Flan-T5](https://huggingface.co/google/flan-t5-large)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `languagemodels-0.6.0/languagemodels/__init__.py` & `languagemodels-0.7.0/languagemodels/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import requests
 import datetime
 import json
+import re
 
-from languagemodels.models import set_max_ram, require_model_license
+from languagemodels.config import config
 from languagemodels.inference import (
     generate_instruct,
+    generate_code,
     rank_instruct,
     parse_chat,
     list_tokens,
 )
 from languagemodels.embeddings import RetrievalContext
 
 docs = RetrievalContext()
@@ -29,15 +31,15 @@
     'are able to fly'
 
     >>> complete("She hid in her room until") #doctest: +SKIP
     'she was sure she was safe'
     """
 
     result = generate_instruct(
-        "Write a sentence", max_tokens=200, temperature=0.7, prefix=prompt
+        "Write a sentence", max_tokens=200, temperature=0.7, topk=40, prefix=prompt
     )
 
     if result.startswith(prompt):
         prefix_length = len(prompt)
         return result[prefix_length:]
     else:
         return result
@@ -102,21 +104,21 @@
 
     :param message: Prompt using formatting described above
     :return: Completion returned from the language model
 
     Examples:
 
     >>> chat('''
-    ...      System: Respond as a helpful assistant. It is 5:15pm.
+    ...      System: Respond as a helpful assistant. It is 5:00pm.
     ...
     ...      User: What time is it?
     ...
     ...      Assistant:
     ...      ''')
-    '...5:15pm...'
+    '...5:00pm...'
     """
 
     messages = parse_chat(prompt)
 
     # Suppress starts of all assistant messages to avoid repeat generation
     suppress = [
         "Assistant: " + m["content"].split(" ")[0]
@@ -141,53 +143,77 @@
         "system": "System",
         "user": "Question",
         "assistant": "Assistant",
     }
 
     messages = [f"{rolemap[m['role']]}: {m['content']}" for m in messages]
 
-    prompt = "\n\n".join(messages)
+    prompt = "\n\n".join(messages) + "\n\n" + "Assistant:"
 
     if prompt.startswith("System:"):
         prompt = prompt[7:].strip()
 
     response = generate_instruct(
         prompt,
         max_tokens=200,
         repetition_penalty=1.3,
         temperature=0.3,
-        prefix="Assistant: ",
+        topk=40,
+        prefix="Assistant:",
         suppress=suppress,
     )
 
     # Remove duplicate assistant being generated
     if response.startswith("Assistant:"):
         response = response[10:]
 
     return response.strip()
 
 
+def code(prompt: str) -> str:
+    """Complete a code prompt
+
+    This assumes that users are expecting Python completions. Default models
+    are fine-tuned on Python where applicable.
+
+    :param prompt: Code context to complete
+    :return: Completion returned from the language model
+
+    Examples:
+
+    >>> code("# Print Hello, world!\\n")
+    'print("Hello, world!")\\n'
+
+    >>> code("def return_4():")
+    '...return 4...'
+    """
+    result = generate_code(prompt, max_tokens=200, topk=1)
+
+    return result
+
+
 def extract_answer(question: str, context: str) -> str:
     """Extract an answer to a `question` from a provided `context`
 
     The returned answer will always be a substring extracted from `context`.
     It may not always be a correct or meaningful answer, but it will never be
     an arbitrary hallucination.
 
     :param question: A question to answer using knowledge from context
     :param context: Knowledge used to answer the question
     :return: Answer to the question.
 
     Examples:
 
     >>> context = "There is a green ball and a red box"
-    >>> extract_answer("What color is the ball?", context) #doctest: +SKIP
-    'green'
+    >>> extract_answer("What color is the ball?", context).lower()
+    '...green...'
+
     >>> extract_answer("Who created Python?", get_wiki('Python')) #doctest: +SKIP
-    'Guido van Rossum'
+    '...Guido van Rossum...'
     """
 
     return generate_instruct(f"{context}\n\n{question}")
 
 
 def classify(doc: str, label1: str, label2: str) -> str:
     """Performs binary classification on an input
@@ -290,22 +316,38 @@
     url = "https://api.wikimedia.org/core/v1/wikipedia/en/search/title"
     response = requests.get(url, params={"q": topic, "limit": 5})
     response = json.loads(response.text)
 
     for page in response["pages"]:
         wiki_result = requests.get(
             f"https://en.wikipedia.org/w/api.php?action=query&prop=extracts|pageprops&"
-            f"exintro&explaintext&redirects=1&titles={page['title']}&format=json"
+            f"exintro&redirects=1&titles={page['title']}&format=json"
         ).json()
 
         first = wiki_result["query"]["pages"].popitem()[1]
         if "disambiguation" in first["pageprops"]:
             continue
 
         summary = first["extract"]
+
+        cutoffs = [
+            "See_also",
+            "Notes",
+            "References",
+            "Further_reading",
+            "External_links",
+        ]
+
+        for cutoff in cutoffs:
+            summary = summary.split(f'<span id="{cutoff}">', 1)[0]
+
+        summary = re.sub(r"<p>", "\n\n", summary, flags=re.I)
+        summary = re.sub(r"\s*[\n\r]+\s*", "\n\n", summary, flags=re.I)
+        summary = re.sub(r"<.*?>", "", summary, flags=re.I)
+        summary = summary.strip()
         return summary
     else:
         return "No matching wiki page found."
 
 
 def get_weather(latitude, longitude):
     """Fetch the current weather for a supplied longitude and latitude
@@ -384,7 +426,35 @@
     2
 
     >>> count_tokens("Hola mundo")
     5
     """
 
     return len(list_tokens(prompt))
+
+
+def set_max_ram(value):
+    """Sets max allowed RAM
+
+    This value takes priority over environment variables
+
+    Returns the numeric value set in GB
+
+    >>> set_max_ram(16)
+    16.0
+
+    >>> set_max_ram('512mb')
+    0.5
+    """
+
+    config["max_ram"] = value
+
+    return config["max_ram"]
+
+
+def require_model_license(match_re):
+    """Require models to match supplied regex
+
+    This can be used to enforce certain licensing constraints when using this
+    package.
+    """
+    config["model_license"] = match_re
```

### Comparing `languagemodels-0.6.0/languagemodels/embeddings.py` & `languagemodels-0.7.0/languagemodels/embeddings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,164 @@
 import numpy as np
 
 from languagemodels.models import get_model
 
 
-def cosine_similarity(a, b):
-    dot_product = np.dot(a, b)
-    magnitude_a = np.linalg.norm(a)
-    magnitude_b = np.linalg.norm(b)
-    return dot_product / (magnitude_a * magnitude_b)
+def embed(doc):
+    """Gets embeddings for a document
+
+    >>> embed("I love Python!")[-3:]
+    array([0.1..., 0.1..., 0.0...], dtype=float32)
+    """
+    tokenizer, model = get_model("embedding")
+
+    tokens = tokenizer.encode(doc).ids
+    output = model.forward_batch([tokens[:512]])
+    embedding = np.mean(np.array(output.last_hidden_state), axis=1)[0]
+    embedding = embedding / np.linalg.norm(embedding)
+    return embedding
+
+
+def search(query, docs):
+    """Return docs sorted by match against query
+
+    :param query: Input to match in search
+    :param docs: List of docs to search against
+    :return: List of (doc_num, score) tuples sorted by score descending
+    """
+
+    query_embedding = embed(query)
+
+    scores = [np.dot(query_embedding, d.embedding) for d in docs]
+
+    return sorted(enumerate(scores), key=lambda x: x[1], reverse=True)
+
+
+def get_token_ids(doc):
+    """Return list of token ids for a document
+
+    Note that the tokenzier used here is from the generative model.
+
+    This is used for token counting for the context, not for tokenization
+    before embedding.
+    """
+
+    generative_tokenizer, _ = get_model("instruct", tokenizer_only=True)
+
+    # We need to disable and re-enable truncation here
+    # This allows us to tokenize very large documents
+    # We won't be feeding the tokens themselves to a model, so this
+    # shouldn't cause any problems.
+    trunk = generative_tokenizer.truncation
+    if trunk:
+        generative_tokenizer.no_truncation()
+    ids = generative_tokenizer.encode(doc, add_special_tokens=False).ids
+    if trunk:
+        generative_tokenizer.enable_truncation(
+            trunk["max_length"], stride=trunk["stride"], strategy=trunk["strategy"]
+        )
+
+    return ids
+
+
+def chunk_doc(doc, name="", chunk_size=64, chunk_overlap=8):
+    """Break a document into chunks
+
+    :param doc: Document to chunk
+    :param name: Optional document name
+    :param chunk_size: Length of individual chunks in tokens
+    :param chunk_overlap: Number of tokens to overlap when breaking chunks
+    :return: List of strings representing the chunks
+
+    >>> chunk_doc("")
+    []
+
+    >>> chunk_doc("Hello")
+    ['Hello']
+
+    >>> chunk_doc("Hello " * 65)
+    ['Hello Hello...', 'Hello...']
+
+    >>> chunk_doc("Hello world. " * 24)[0]
+    'Hello world. ...Hello world.'
+
+    >>> len(chunk_doc("Hello world. " * 20))
+    1
+
+    >>> len(chunk_doc("Hello world. " * 24))
+    2
+
+    # Check to make sure sentences aren't broken on decimal points
+    >>> chunk_doc(('z. ' + ' 37.468 ' * 5) * 3)[0]
+    'z. 37.468 ...z.'
+    """
+    generative_tokenizer, _ = get_model("instruct", tokenizer_only=True)
+
+    tokens = get_token_ids(doc)
+    separators = [get_token_ids(t)[-1] for t in [".", "!", "?", ")."]]
+
+    name_tokens = []
+
+    label = f"From {name} document:" if name else ""
+
+    if name:
+        name_tokens = get_token_ids(label)
+
+    i = 0
+    chunks = []
+    chunk = name_tokens.copy()
+    while i < len(tokens):
+        token = tokens[i]
+        chunk.append(token)
+        i += 1
+
+        # Save the last chunk if we're done
+        if i == len(tokens):
+            chunks.append(generative_tokenizer.decode(chunk))
+            break
+
+        if len(chunk) == chunk_size:
+            # Backtrack to find a reasonable cut point
+            for j in range(1, chunk_size - chunk_overlap * 2):
+                if chunk[chunk_size - j] in separators:
+                    ctx = generative_tokenizer.decode(
+                        chunk[chunk_size - j : chunk_size - j + 2]
+                    )
+                    if " " in ctx:
+                        # Found a good separator
+                        text = generative_tokenizer.decode(chunk[: chunk_size - j + 1])
+                        chunks.append(text)
+                        chunk = name_tokens + chunk[chunk_size - j + 1 :]
+                        break
+            else:
+                # No semantically meaningful cutpoint found
+                # Default to a hard cut
+                text = generative_tokenizer.decode(chunk)
+                chunks.append(text)
+                # Share some overlap with next chunk
+                overlap = max(
+                    chunk_overlap, chunk_size - len(name_tokens) - (len(tokens) - i)
+                )
+                chunk = name_tokens + chunk[-overlap:]
+
+    return chunks
+
+
+class Document:
+    """
+    A document used for semantic search
+
+    Documents have content and an embedding that is used to match the content
+    against other semantically similar documents.
+    """
+
+    def __init__(self, content, name=""):
+        self.content = content
+        self.embedding = embed(content)
+        self.name = name
 
 
 class RetrievalContext:
     """
     Provides a context for document retrieval
 
     Documents are embedded and cached for later search.
@@ -27,174 +174,119 @@
 
     >>> rc.get_match("Where is Paris?")
     'Paris is in France.'
 
     >>> rc.clear()
     >>> rc.get_match("Where is Paris?")
 
-    >>> rc.get_embedding("I love Python!")[-3:]
-    array([0.1..., 0.1..., 0.0...], dtype=float32)
+    >>> rc.clear()
+    >>> rc.store(' '.join(['Python'] * 4096))
+    >>> len(rc.chunks)
+    73
 
     >>> rc.clear()
-    >>> rc.store('Python ' * 232)
+    >>> rc.store(' '.join(['Python'] * 232))
     >>> len(rc.chunks)
     4
 
     >>> rc.get_context("What is Python?")
     'Python Python Python...'
 
+    >>> [len(c.content.split()) for c in rc.chunks]
+    [64, 64, 64, 64]
+
     >>> len(rc.get_context("What is Python?").split())
     128
     """
 
     def __init__(self, chunk_size=64, chunk_overlap=8):
         self.chunk_size = chunk_size
         self.chunk_overlap = chunk_overlap
         self.clear()
 
     def clear(self):
         self.docs = []
-        self.embeddings = []
         self.chunks = []
-        self.chunk_embeddings = []
-
-    def get_embedding(self, doc):
-        """Gets embeddings for a document"""
-        tokenizer, model = get_model("embedding")
-
-        tokens = tokenizer.encode(doc).ids
-        output = model.forward_batch([tokens[:512]])
-        embedding = np.mean(np.array(output.last_hidden_state), axis=1)[0]
-        embedding = embedding / np.linalg.norm(embedding)
-        return embedding
 
     def store(self, doc, name=""):
         """Stores a document along with embeddings
 
         This stores both the document as well as document chunks
 
         >>> rc = RetrievalContext()
         >>> rc.clear()
-        >>> rc.store('Python ' * 233)
+        >>> rc.store(' '.join(['Python'] * 233))
         >>> len(rc.chunks)
         5
 
         >>> rc.clear()
-        >>> rc.store('Python ' * 232)
+        >>> rc.store(' '.join(['Python'] * 232))
         >>> len(rc.chunks)
         4
 
         >>> rc.clear()
         >>> rc.store('Python')
         >>> len(rc.chunks)
         1
 
         >>> rc.clear()
         >>> rc.store('It is a language.', 'Python')
         >>> len(rc.chunks)
         1
-        >>> rc.chunks
-        ['Python: It is a language.']
+        >>> [c.content for c in rc.chunks]
+        ['From Python document: It is a language.']
 
         >>> rc = RetrievalContext()
         >>> rc.clear()
-        >>> rc.store('details ' * 225, 'Python')
+        >>> rc.store(' '.join(['details'] * 217), 'Python')
         >>> len(rc.chunks)
         5
 
         >>> rc.clear()
-        >>> rc.store('details ' * 224, 'Python')
+        >>> rc.store(' '.join(['details'] * 216), 'Python')
         >>> len(rc.chunks)
         4
-        >>> rc.chunks
-        ['Python: details details details...']
+        >>> [c.content for c in rc.chunks]
+        ['From Python document: details details details...']
         """
 
         if doc not in self.docs:
-            embedding = self.get_embedding(doc)
-            self.embeddings.append(embedding)
-            self.docs.append(doc)
+            self.docs.append(Document(doc))
             self.store_chunks(doc, name)
 
     def store_chunks(self, doc, name=""):
-        # Note that the tokenzier used here is from the generative model
-        # This is used for token counting for the context, not for tokenization
-        # before embedding
-        generative_tokenizer, _ = get_model("instruct")
-
-        tokens = generative_tokenizer.EncodeAsPieces(doc)
-
-        name_tokens = []
-
-        if name:
-            name_tokens = generative_tokenizer.EncodeAsPieces(f"{name}:")
-
-        i = 0
-        chunk = name_tokens.copy()
-        while i < len(tokens):
-            token = tokens[i]
-            chunk.append(token)
-            i += 1
-
-            # Begin looking for probable sentence when half of target size
-
-            full = len(chunk) == self.chunk_size
-            half_full = len(chunk) > self.chunk_size / 2
-            eof = i == len(tokens)
-            sep = token in [".", "!", "?", ")."]
-
-            if eof or full or (half_full and sep):
-                # Store tokens and start next chunk
-                text = generative_tokenizer.Decode(chunk)
-                embedding = self.get_embedding(text)
-                self.chunk_embeddings.append(embedding)
-                self.chunks.append(text)
-                chunk = name_tokens.copy()
-                if full and not eof:
-                    # If the heuristic didn't get a semantic boundary, overlap
-                    # next chunk to provide some context
-                    i -= self.chunk_overlap
-                    i = max(0, i)
+        chunks = chunk_doc(doc, name, self.chunk_size, self.chunk_overlap)
+
+        for chunk in chunks:
+            self.chunks.append(Document(chunk))
 
     def get_context(self, query, max_tokens=128):
         """Gets context matching a query
 
         Context is capped by token length and is retrieved from stored
         document chunks
         """
 
         if len(self.chunks) == 0:
             return None
 
-        query_embedding = self.get_embedding(query)
-
-        scores = [cosine_similarity(query_embedding, e) for e in self.chunk_embeddings]
-        doc_score_pairs = list(zip(self.chunks, scores))
-
-        doc_score_pairs = sorted(doc_score_pairs, key=lambda x: x[1], reverse=True)
+        results = search(query, self.chunks)
 
         chunks = []
         tokens = 0
 
-        generative_tokenizer, _ = get_model("instruct")
-
-        for chunk, score in doc_score_pairs:
-            chunk_tokens = len(generative_tokenizer.EncodeAsPieces(chunk))
+        for chunk_id, score in results:
+            chunk = self.chunks[chunk_id].content
+            chunk_tokens = len(get_token_ids(chunk))
             if tokens + chunk_tokens <= max_tokens and score > 0.1:
                 chunks.append(chunk)
                 tokens += chunk_tokens
 
         context = "\n\n".join(chunks)
 
         return context
 
     def get_match(self, query):
         if len(self.docs) == 0:
             return None
 
-        query_embedding = self.get_embedding(query)
-
-        scores = [cosine_similarity(query_embedding, e) for e in self.embeddings]
-        doc_score_pairs = list(zip(self.docs, scores))
-
-        doc_score_pairs = sorted(doc_score_pairs, key=lambda x: x[1], reverse=True)
-        return doc_score_pairs[0][0]
+        return self.docs[search(query, self.docs)[0][0]].content
```

### Comparing `languagemodels-0.6.0/languagemodels/inference.py` & `languagemodels-0.7.0/languagemodels/inference.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 class InferenceException(Exception):
     pass
 
 
 def list_tokens(prompt):
     """Generates a list of tokens for a supplied prompt
 
-    >>> list_tokens("Hello, world!")
+    >>> list_tokens("Hello, world!") # doctest: +SKIP
     [('▁Hello', 8774), (',', 6), ('▁world', 296), ('!', 55)]
+
+    >>> list_tokens("Hello, world!")
+    [('...Hello', ...), ... ('...world', ...), ...]
     """
     tokenizer, _ = get_model("instruct")
 
-    tokens = tokenizer.EncodeAsPieces(prompt)
-    ids = tokenizer.EncodeAsIds(prompt)
+    output = tokenizer.encode(prompt, add_special_tokens=False)
+    tokens = output.tokens
+    ids = output.ids
 
     return list(zip(tokens, ids))
 
 
 def generate_ts(engine, prompt, max_tokens=200):
     """Generates a single text response for a prompt from a textsynth server
 
@@ -126,31 +130,81 @@
         return generate_ts("flan_t5_xxl_q4", prompt, max_tokens).strip()
 
     if os.environ.get("LANGUAGEMODELS_OA_KEY"):
         return chat_oa("gpt-3.5-turbo", prompt, max_tokens).strip()
 
     tokenizer, model = get_model("instruct")
 
-    suppress = [tokenizer.EncodeAsPieces(s) for s in suppress]
+    suppress = [tokenizer.encode(s, add_special_tokens=False).tokens for s in suppress]
+
+    if hasattr(model, "translate_batch"):
+        results = model.translate_batch(
+            [tokenizer.encode(prompt).tokens],
+            target_prefix=[tokenizer.encode(prefix, add_special_tokens=False).tokens],
+            repetition_penalty=repetition_penalty,
+            max_decoding_length=max_tokens,
+            sampling_temperature=temperature,
+            sampling_topk=topk,
+            suppress_sequences=suppress,
+            beam_size=1,
+        )
+        output_tokens = results[0].hypotheses[0]
+        output_ids = [tokenizer.token_to_id(t) for t in output_tokens]
+        text = tokenizer.decode(output_ids, skip_special_tokens=True)
+    else:
+        prompt = (
+            "Below is an instruction that describes a task.\n"
+            "Write a response that appropriately completes the request.\n\n"
+            f"### Instruction:{prompt}\n\n### Response:"
+        )
+        results = model.generate_batch(
+            [tokenizer.encode(prompt).tokens],
+            repetition_penalty=repetition_penalty,
+            max_length=max_tokens,
+            sampling_temperature=temperature,
+            sampling_topk=topk,
+            beam_size=1,
+        )
+        output_ids = results[0].sequences_ids[0]
+        text = tokenizer.decode(output_ids, skip_special_tokens=True)
+        text = text[len(prompt) :]
+
+    return text
+
+
+def generate_code(
+    prompt,
+    max_tokens=200,
+    temperature=0.1,
+    topk=1,
+    repetition_penalty=1.2,
+    prefix="",
+):
+    """Generates one completion for a prompt using a code-tuned model
+
+    >>> generate_code("# Print Hello, World!\\n")
+    'print("Hello, World!")\\n'
+    """
+
+    tokenizer, model = get_model("code")
 
-    input_tokens = tokenizer.EncodeAsPieces(prompt) + ["</s>"]
     results = model.translate_batch(
-        [input_tokens],
-        target_prefix=[tokenizer.EncodeAsPieces(prefix)],
+        [tokenizer.encode(prompt).tokens],
+        target_prefix=[tokenizer.encode(prefix, add_special_tokens=False).tokens],
         repetition_penalty=repetition_penalty,
         max_decoding_length=max_tokens,
         sampling_temperature=temperature,
         sampling_topk=topk,
-        suppress_sequences=suppress,
         beam_size=1,
     )
-
     output_tokens = results[0].hypotheses[0]
+    output_ids = [tokenizer.token_to_id(t) for t in output_tokens]
+    text = tokenizer.decode(output_ids, skip_special_tokens=True)
 
-    return tokenizer.DecodePieces(output_tokens)
+    return text
 
 
 def rank_instruct(input, targets):
     """Sorts a list of targets by their probabilities
 
     >>> rank_instruct("I love python", ['positive', 'negative'])
     ['positive', 'negative']
@@ -159,20 +213,28 @@
     'negative'
 
     >>> rank_instruct("The wizard raised their wand", ['fantasy', 'documentary'])
     ['fantasy', 'documentary']
     """
     tokenizer, model = get_model("instruct")
 
-    input_tokens = tokenizer.EncodeAsPieces(input) + ["</s>"]
+    input_tokens = tokenizer.encode(input).tokens
 
-    scores = model.score_batch(
-        [input_tokens] * len(targets),
-        target=[tokenizer.EncodeAsPieces(t) for t in targets],
-    )
+    if "Generator" in str(type(model)):
+        prompt = f'Classify as {", ".join(targets)}: {input} Classification:'
+        input_tokens = tokenizer.encode(prompt).tokens
+
+        scores = model.score_batch(
+            [input_tokens + tokenizer.encode(t).tokens for t in targets],
+        )
+    else:
+        scores = model.score_batch(
+            [input_tokens] * len(targets),
+            target=[tokenizer.encode(t).tokens for t in targets],
+        )
 
     logprobs = [sum(r.log_probs) for r in scores]
 
     results = sorted(zip(targets, logprobs), key=lambda r: -r[1])
 
     return [r[0] for r in results]
```

### Comparing `languagemodels-0.6.0/languagemodels.egg-info/PKG-INFO` & `languagemodels-0.7.0/languagemodels.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: languagemodels
-Version: 0.6.0
+Version: 0.7.0
 Summary: Simple inference for large language models
 Home-page: https://github.com/jncraton/languagemodels
 Author: Jon Craton
 Author-email: jon@joncraton.com
 License: UNKNOWN
 Description: Language Models
         ===============
         
         [![PyPI version](https://badge.fury.io/py/languagemodels.svg)](https://badge.fury.io/py/languagemodels)
         [![docs](https://img.shields.io/badge/docs-online-brightgreen)](https://languagemodels.netlify.app/)
         [![x64 Build](https://github.com/jncraton/languagemodels/actions/workflows/build.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/build.yml)
-        [![ARM64 Build](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml)[![Netlify Status](https://api.netlify.com/api/v1/badges/722e625a-c6bc-4373-bd88-c017adc58c00/deploy-status)](https://app.netlify.com/sites/languagemodels/deploys)
+        [![ARM64 Build](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml/badge.svg)](https://github.com/jncraton/languagemodels/actions/workflows/pi.yml)
         [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jncraton/languagemodels/blob/master/examples/translate.ipynb)
         
         Python building blocks to explore large language models on any computer with 512MB of RAM
         
         [![Try with Replit Badge](https://replit.com/badge?caption=Try%20with%20Replit&variant=small)](https://replit.com/@jncraton/langaugemodels#main.py)
         
         ![Translation hello world example](media/hello.gif)
         
-        Target Audience
-        ---------------
-        
-        This package is designed to be as simple as possible for **learners** and **educators** exploring how large language models intersect with modern software development. The interfaces to this package are all simple functions using standard types. The complexity of large language models is hidden from view while providing free local inference using light-weight, open models. All included models are free for educational use, no API keys are required, and all inference is performed locally by default.
+        This package makes using large language models in software as simple as possible. All inference is performed locally to keep your data private by default.
         
         Installation and Getting Started
         --------------------------------
         
         This package can be installed using the following command:
         
         ```sh
@@ -46,33 +43,47 @@
         This will require downloading a significant amount of data (~250MB) on the first run. Models will be cached for later use and subsequent calls should be quick.
         
         Example Usage
         -------------
         
         Here are some usage examples as Python REPL sessions. This should work in the REPL, notebooks, or in traditional scripts and applications.
         
-        ### Text Completions
+        ### Instruction Following
         
         ```python
         >>> import languagemodels as lm
         
-        >>> lm.complete("She hid in her room until")
-        'she was sure she was safe'
+        >>> lm.do("Translate to English: Hola, mundo!")
+        'Hello, world!'
+        
+        >>> lm.do("What is the capital of France?")
+        'Paris.'
         ```
         
-        ### Instruction Following
+        ### Adjusting Model Performance
+        
+        The base model should run quickly on any system with 512MB of memory, but this memory limit can be increased to select more powerful models that will consume more resources. Here's an example:
         
         ```python
         >>> import languagemodels as lm
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'You have 8 apples.'
+        >>> lm.set_max_ram('4gb')
+        4.0
+        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
+        'I have 2 apples left.'
+        ```
         
-        >>> lm.do("Translate to English: Hola, mundo!")
-        'Hello, world!'
+        ### Text Completions
         
-        >>> lm.do("What is the capital of France?")
-        'Paris.'
+        ```python
+        >>> import languagemodels as lm
+        
+        >>> lm.complete("She hid in her room until")
+        'she was sure she was safe'
         ```
         
         ### Chat
         
         ```python
         >>> lm.chat('''
         ...      System: Respond as a helpful assistant.
@@ -80,14 +91,29 @@
         ...      User: What time is it?
         ...
         ...      Assistant:
         ...      ''')
         'I'm sorry, but as an AI language model, I don't have access to real-time information. Please provide me with the specific time you are asking for so that I can assist you better.'
         ```
         
+        ### Code
+        
+        A model tuned on Python code is included. It can be used to complete code snippets.
+        
+        ```python
+        >>> import languagemodels as lm
+        >>> lm.code("""
+        ... a = 2
+        ... b = 5
+        ...
+        ... # Swap a and b
+        ... """)
+        'a, b = b, a'
+        ```
+        
         ### External Retrieval
         
         Helper functions are provided to retrieve text from external sources that can be used to augment prompt context.
         
         ```python
         >>> import languagemodels as lm
         
@@ -116,93 +142,78 @@
         
         ### Semantic Search
         
         Semantic search is provided to retrieve documents that may provide helpful context from a document store.
         
         ```python
         >>> import languagemodels as lm
-        
-        >>> lm.store_doc("Mars is a planet")
-        >>> lm.store_doc("The sun is hot")
-        >>> lm.load_doc("What is Mars?")
-        'Mars is a planet'
-        ```
-        
-        This can also be used to get a blend of context from stored documents:
-        
-        ```python
-        >>> import languagemodels as lm
         >>> lm.store_doc(lm.get_wiki("Python"), "Python")
         >>> lm.store_doc(lm.get_wiki("C language"), "C")
         >>> lm.store_doc(lm.get_wiki("Javascript"), "Javascript")
         >>> lm.get_doc_context("What does it mean for batteries to be included in a language?")
-        'Python: It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.
-        
-        C: It was designed to be compiled to provide low-level access to memory and language constructs that map efficiently to machine instructions, all with minimal runtime support.
+        'From Python document: It is often described as a "batteries included" language due to its comprehensive standard library.Guido van Rossum began working on Python in the late 1980s as a successor to the ABC programming language and first released it in 1991 as Python 0.9.
         
-        C: The book The C Programming Language, co-authored by the original language designer, served for many years as the de facto standard for the language.'
+        From C document: It was designed to be compiled to provide low-level access to memory and language constructs that map efficiently to machine instructions, all with minimal runtime support.'
         ```
         
-        ### Performance
+        [Full documentation](https://languagemodels.netlify.app/)
         
-        The models used by this package are 1000x smaller than the largest models in use today. They are useful as learning tools, but if you are expecting ChatGPT or similar performance, you will be very disappointed.
+        ### Speed
         
-        The base model should work on any system with 512MB of memory, but this memory limit can be increased. Setting this value higher will require more memory and generate results more slowly, but the results should be superior. Here's an example:
+        This package currently outperforms Hugging Face `transformers` for CPU inference thanks to int8 quantization and the [CTranslate2](https://github.com/OpenNMT/CTranslate2) backend. The following table compares CPU inference performance on identical models using the best available quantization on a 20 question test set.
         
-        ```python
-        >>> import languagemodels as lm
-        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
-        'You have 8 apples.'
-        >>> lm.set_max_ram('4gb')
-        4.0
-        >>> lm.do("If I have 7 apples then eat 5, how many apples do I have?")
-        'I have 2 apples left.'
-        ```
+        | Backend                   | Inference Time | Memory Used |
+        |---------------------------|----------------|-------------|
+        | Hugging Face transformers | 22s            | 1.77GB      |
+        | This package              | 11s            | 0.34GB      |
         
-        [Full documentation](https://languagemodels.netlify.app/)
+        Note that quantization does technically harm output quality slightly, but it should be negligible at this level.
+        
+        ### Models
+        
+        This package does allow direct model selection, but sensible defaults are preferred to allow the package to improve over time as stronger models become available. The models used are 1000x smaller than the largest models in use today. They are useful as learning tools, but perform far below the current state of the art.
+        
+        This package currently uses [LaMini-Flan-T5-base](https://huggingface.co/MBZUAI/LaMini-Flan-T5-248M) as its default model. This is a fine-tuning of the T5 base model on top of the [FLAN](https://huggingface.co/google/flan-t5-base) fine-tuning. The model is tuned to respond to instructions in a human-like manner. The following human evaluations were reported in the [paper](https://github.com/mbzuai-nlp/LaMini-LM) associated with this model family:
+        
+        ![Human-rated model comparison](media/model-comparison.png)
+        
+        For code completions, the [CodeT5+](https://arxiv.org/abs/2305.07922) series of models are used.
         
         Commercial Use
         --------------
         
-        This package itself is licensed for commerical use, but the models used may not be compatible with commercial use. In order to use this package commercially, you may want to filter models by their license type using the `require_model_license` function.
+        This package itself is licensed for commercial use, but the models used may not be compatible with commercial use. In order to use this package commercially, you can filter models by license type using the `require_model_license` function.
         
         ```python
         >>> import languagemodels as lm
-        >>> lm.do("What is your favorite animal.")
-        >>> "As an AI language model, I don't have preferences or emotions."
-        >>> lm.require_model_license("apache.*|mit")
-        >>> lm.do("What is your favorite animal.")
-        'Lion.'
+        >>> lm.config['instruct_model']
+        'LaMini-Flan-T5-248M-ct2-int8'
+        >>> lm.require_model_license("apache|bsd|mit")
+        >>> lm.config['instruct_model']
+        'flan-t5-base-ct2-int8'
         ```
         
-        The commercially-licensed models may not perform as well as the default models. It is recommended to confirm that the models used do meet the licensing requirements for your software.
+        It is recommended to confirm that the models used meet the licensing requirements for your software.
         
         Projects Ideas
         --------------
         
-        This package can be used to do the heavy lifting for a number of learning projects:
+        One of the goals for this package is to be a straightforward tool for learners and educators exploring how large language models intersect with modern software development. It can be used to do the heavy lifting for a number of learning projects:
         
         - CLI Chatbot (see [examples/chat.py](examples/chat.py))
         - Streamlit chatbot (see [examples/streamlitchat.py](examples/streamlitchat.py))
         - Chatbot with information retrieval
         - Chatbot with access to real-time information
         - Tool use
         - Text classification
         - Extractive question answering
         - Semantic search over documents
         - Document question answering
         
         Several example programs and notebooks are included in the `examples` directory.
         
-        Attribution
-        -----------
-        
-        - [CTranslate2](https://github.com/OpenNMT/CTranslate2)
-        - [LaMini-Flan-T5](https://huggingface.co/MBZUAI/LaMini-Flan-T5-783M)
-        - [Flan-T5](https://huggingface.co/google/flan-t5-large)
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `languagemodels-0.6.0/setup.py` & `languagemodels-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import setuptools
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="languagemodels",
-    version="0.6.0",
+    version="0.7.0",
     author="Jon Craton",
     author_email="jon@joncraton.com",
     description="Simple inference for large language models",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jncraton/languagemodels",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8',
     install_requires=[
-        "sentencepiece",
         "huggingface_hub",
         "ctranslate2>=3.15.0",
         "tokenizers",
        ],
 )
```

