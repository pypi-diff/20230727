# Comparing `tmp/paper-qa-3.4.1.tar.gz` & `tmp/paper-qa-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.4.1.tar", last modified: Mon Jul 24 19:21:56 2023, max compression
+gzip compressed data, was "paper-qa-3.5.0.tar", last modified: Thu Jul 27 13:02:25 2023, max compression
```

## Comparing `paper-qa-3.4.1.tar` & `paper-qa-3.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 19:21:09.000000 paper-qa-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-24 19:21:56.796503 paper-qa-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-24 19:21:09.000000 paper-qa-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.792503 paper-qa-3.4.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 19:21:56.000000 paper-qa-3.4.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    23961 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-24 19:21:09.000000 paper-qa-3.4.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:21:56.796503 paper-qa-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-24 19:21:09.000000 paper-qa-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:21:56.796503 paper-qa-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    28522 2023-07-24 19:21:09.000000 paper-qa-3.4.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.765984 paper-qa-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-27 13:01:37.000000 paper-qa-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-27 13:02:25.765984 paper-qa-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-27 13:01:37.000000 paper-qa-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 13:02:25.000000 paper-qa-3.5.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24198 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 13:01:37.000000 paper-qa-3.5.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 13:02:25.765984 paper-qa-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-27 13:01:37.000000 paper-qa-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:02:25.761983 paper-qa-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    28728 2023-07-27 13:01:37.000000 paper-qa-3.5.0/tests/test_paperqa.py
```

### Comparing `paper-qa-3.4.1/LICENSE` & `paper-qa-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.1/PKG-INFO` & `paper-qa-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.4.1
+Version: 3.5.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.4.1/README.md` & `paper-qa-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.5.0/paper_qa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.4.1
+Version: 3.5.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.4.1/paperqa/chains.py` & `paper-qa-3.5.0/paperqa/chains.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.memory.chat_memory import BaseChatMemory
 from langchain.prompts import BasePromptTemplate, PromptTemplate, StringPromptTemplate
 from langchain.prompts.chat import ChatPromptTemplate, HumanMessagePromptTemplate
 from langchain.schema import LLMResult, SystemMessage
 
+from .prompts import default_system_prompt
 from .types import CBManager
 
 memory_prompt = PromptTemplate(
     input_variables=["memory", "start"],
-    template="Previous answers that may be helpful:\n\n{memory}\n\n"
+    template="Here are previous questions and answers, which may be referenced in subsequent questions:\n\n{memory}\n\n"
     "----------------------------------------\n\n"
     "{start}",
 )
 
 
 class FallbackLLMChain(LLMChain):
     """Chain that falls back to synchronous generation if the async generation fails."""
@@ -48,14 +49,15 @@
 
 
 def make_chain(
     prompt: StringPromptTemplate,
     llm: BaseLanguageModel,
     skip_system: bool = False,
     memory: Optional[BaseChatMemory] = None,
+    system_prompt: str = default_system_prompt,
 ) -> FallbackLLMChain:
     if memory and len(memory.load_memory_variables({})["memory"]) > 0:
         # we copy the prompt so we don't modify the original
         # TODO: Figure out pipeline prompts to avoid this
         # the problem with pipeline prompts is that
         # the memory is a constant (or partial), not  a prompt
         # and I cannot seem to make an empty prompt (or str)
@@ -68,19 +70,15 @@
             input_variables=prompt.input_variables,
             template=memory_prompt.format(
                 start=prompt.template, **memory.load_memory_variables({})
             ),
         )
         prompt = new_prompt
     if type(llm) == ChatOpenAI:
-        system_message_prompt = SystemMessage(
-            content="Answer in an unbiased, concise, scholarly tone. "
-            "You may refuse to answer if there is insufficient information. "
-            "If there are ambiguous terms or acronyms, first define them. ",
-        )
+        system_message_prompt = SystemMessage(content=system_prompt)
         human_message_prompt = ExtendedHumanMessagePromptTemplate(prompt=prompt)
         if skip_system:
             chat_prompt = ChatPromptTemplate.from_messages([human_message_prompt])
         else:
             chat_prompt = ChatPromptTemplate.from_messages(
                 [system_message_prompt, human_message_prompt]
             )
```

### Comparing `paper-qa-3.4.1/paperqa/contrib/zotero.py` & `paper-qa-3.5.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.1/paperqa/docs.py` & `paper-qa-3.5.0/paperqa/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,15 +438,18 @@
 
         # now finally cut down
         matches = matches[:k]
 
         async def process(match):
             callbacks = get_callbacks("evidence:" + match.metadata["name"])
             summary_chain = make_chain(
-                self.prompts.summary, self.summary_llm, memory=self.memory_model
+                self.prompts.summary,
+                self.summary_llm,
+                memory=self.memory_model,
+                system_prompt=self.prompts.system,
             )
             # This is dangerous because it
             # could mask errors that are important- like auth errors
             # I also cannot know what the exception
             # type is because any model could be used
             # my best idea is see if there is a 4XX
             # http code in the exception
@@ -568,14 +571,15 @@
                 get_callbacks=get_callbacks,
             )
         if self.prompts.pre is not None:
             chain = make_chain(
                 self.prompts.pre,
                 cast(BaseLanguageModel, self.llm),
                 memory=self.memory_model,
+                system_prompt=self.prompts.system,
             )
             pre = await chain.arun(
                 question=answer.question, callbacks=get_callbacks("pre")
             )
             answer.context = pre + "\n\n" + answer.context
         bib = dict()
         if len(answer.context) < 10 and not self.memory:
@@ -584,14 +588,15 @@
             )
         else:
             callbacks = get_callbacks("answer")
             qa_chain = make_chain(
                 self.prompts.qa,
                 cast(BaseLanguageModel, self.llm),
                 memory=self.memory_model,
+                system_prompt=self.prompts.system,
             )
             answer_text = await qa_chain.arun(
                 context=answer.context,
                 answer_length=answer.answer_length,
                 question=answer.question,
                 callbacks=callbacks,
             )
@@ -615,14 +620,15 @@
         answer.references = bib_str
 
         if self.prompts.post is not None:
             chain = make_chain(
                 self.prompts.post,
                 cast(BaseLanguageModel, self.llm),
                 memory=self.memory_model,
+                system_prompt=self.prompts.system,
             )
             post = await chain.arun(**answer.dict(), callbacks=get_callbacks("post"))
             answer.answer = post
             answer.formatted_answer = f"Question: {answer.question}\n\n{post}\n"
             if len(bib) > 0:
                 answer.formatted_answer += f"\nReferences\n\n{bib_str}\n"
         if self.memory_model is not None:
```

### Comparing `paper-qa-3.4.1/paperqa/prompts.py` & `paper-qa-3.5.0/paperqa/prompts.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "for the question below based on the provided context. "
     "If the context provides insufficient information, "
     'reply "I cannot answer". '
     "For each part of your answer, indicate which sources most support it "
     "via valid citation markers at the end of sentences, like (Example2012). "
     "Answer in an unbiased, comprehensive, and scholarly tone. "
     "If the question is subjective, provide an opinionated answer in the concluding 1-2 sentences. \n\n"
-    "{context}\n"
+    "Context (with relevance scores):\n {context}\n"
     "Question: {question}\n"
     "Answer: ",
 )
 
 select_paper_prompt = PromptTemplate(
     input_variables=["question", "papers"],
     template="Select papers that may help answer the question below. "
@@ -47,7 +47,13 @@
 # so TODO: update year next year
 citation_prompt = PromptTemplate(
     input_variables=["text"],
     template="Provide the citation for the following text in MLA Format. The year is 2023\n"
     "{text}\n\n"
     "Citation:",
 )
+
+default_system_prompt = (
+    "Answer in an unbiased, concise, scholarly tone. "
+    "You may refuse to answer if there is insufficient information. "
+    "If there are ambiguous terms or acronyms, first define them. "
+)
```

### Comparing `paper-qa-3.4.1/paperqa/readers.py` & `paper-qa-3.5.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.1/paperqa/types.py` & `paper-qa-3.5.0/paperqa/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain.prompts import PromptTemplate
 from pydantic import BaseModel, validator
 
-from .prompts import citation_prompt, qa_prompt, select_paper_prompt, summary_prompt
+from .prompts import (
+    citation_prompt,
+    default_system_prompt,
+    qa_prompt,
+    select_paper_prompt,
+    summary_prompt,
+)
 
 StrPath = Union[str, Path]
 DocKey = Any
 CBManager = Union[AsyncCallbackManagerForChainRun, CallbackManagerForChainRun]
 CallbackFactory = Callable[[str], Union[None, List[BaseCallbackHandler]]]
 
 
@@ -33,14 +39,15 @@
 class PromptCollection(BaseModel):
     summary: PromptTemplate = summary_prompt
     qa: PromptTemplate = qa_prompt
     select: PromptTemplate = select_paper_prompt
     cite: PromptTemplate = citation_prompt
     pre: Optional[PromptTemplate] = None
     post: Optional[PromptTemplate] = None
+    system: str = default_system_prompt
 
     @validator("summary")
     def check_summary(cls, v: PromptTemplate) -> PromptTemplate:
         if not set(v.input_variables).issubset(set(summary_prompt.input_variables)):
             raise ValueError(
                 f"Summary prompt can only have variables: {summary_prompt.input_variables}"
             )
```

### Comparing `paper-qa-3.4.1/paperqa/utils.py` & `paper-qa-3.5.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.1/setup.py` & `paper-qa-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.4.1/tests/test_paperqa.py` & `paper-qa-3.5.0/tests/test_paperqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -660,36 +660,43 @@
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.query("What country is Bates from?")
 
+    docs = Docs(
+        prompts=PromptCollection(
+            system="Answer all questions with as few words as possible"
+        )
+    )
+    docs.query("What country is Bates from?")
+
 
 def test_memory():
     # Not sure why, but gpt-3.5 cannot do this anymore.
     docs = Docs(memory=True, k=3, max_sources=1, llm="gpt-4", key_filter=False)
     docs.add_url(
         "https://en.wikipedia.org/wiki/Red_Army",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
     answer1 = docs.query("When did the Soviet Union and Japan agree to a cease-fire?")
     assert answer1.memory is not None
     assert "1939" in answer1.answer
     assert "Answer" in docs.memory_model.load_memory_variables({})["memory"]
-    answer2 = docs.query("When was it resolved?")
+    answer2 = docs.query("When was the conflict resolved?")
     assert "1941" in answer2.answer or "1945" in answer2.answer
     assert answer2.memory is not None
     assert "Answer" in docs.memory_model.load_memory_variables({})["memory"]
     print(answer2.answer)
 
     docs.clear_memory()
 
-    answer3 = docs.query("When was it resolved?")
+    answer3 = docs.query("When was the conflict resolved?")
     assert answer3.memory is not None
     assert (
         "I cannot answer" in answer3.answer
         or "insufficient" in answer3.answer
         or "does not provide" in answer3.answer
     )
```

