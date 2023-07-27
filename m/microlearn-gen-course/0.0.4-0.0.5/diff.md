# Comparing `tmp/microlearn_gen_course-0.0.4.tar.gz` & `tmp/microlearn_gen_course-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microlearn_gen_course-0.0.4.tar", last modified: Tue Jul 25 07:14:29 2023, max compression
+gzip compressed data, was "microlearn_gen_course-0.0.5.tar", last modified: Thu Jul 27 11:03:32 2023, max compression
```

## Comparing `microlearn_gen_course-0.0.4.tar` & `microlearn_gen_course-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/gen_course/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_answer_to_article_ques.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_course_article_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_course_articles_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/gen_course/gen_course_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 07:14:29.000000 microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:14:29.315779 microlearn_gen_course-0.0.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_answer_to_article_ques.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_gen_course_article_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_gen_course_articles_titles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-25 07:14:17.000000 microlearn_gen_course-0.0.4/src/tests/test_gen_course_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:32.003998 microlearn_gen_course-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:31.999998 microlearn_gen_course-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:31.999998 microlearn_gen_course-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 11:03:32.003998 microlearn_gen_course-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-27 11:03:32.003998 microlearn_gen_course-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:31.999998 microlearn_gen_course-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:32.003998 microlearn_gen_course-0.0.5/src/gen_course/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/gen_course/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/gen_course/gen_answer_to_article_ques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/gen_course/gen_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/gen_course/gen_course_article_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/gen_course/gen_course_articles_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/gen_course/gen_course_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:32.003998 microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 11:03:31.000000 microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-27 11:03:31.000000 microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:03:31.000000 microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-27 11:03:31.000000 microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 11:03:31.000000 microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:03:32.003998 microlearn_gen_course-0.0.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/tests/test_answer_to_article_ques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/tests/test_gen_course_article_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/tests/test_gen_course_articles_titles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-27 11:03:21.000000 microlearn_gen_course-0.0.5/src/tests/test_gen_course_metadata.py
```

### Comparing `microlearn_gen_course-0.0.4/.github/workflows/publish.yml` & `microlearn_gen_course-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/PKG-INFO` & `microlearn_gen_course-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn_gen_course
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for generating microlearn course content
 Home-page: https://github.com/AIprojectflow/gen_course
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/gen_course/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/gen_course/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_gen_course-0.0.4/setup.cfg` & `microlearn_gen_course-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/src/gen_course/gen_answer_to_article_ques.py` & `microlearn_gen_course-0.0.5/src/gen_course/gen_answer_to_article_ques.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/src/gen_course/gen_base.py` & `microlearn_gen_course-0.0.5/src/gen_course/gen_base.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/src/gen_course/gen_course_article_content.py` & `microlearn_gen_course-0.0.5/src/gen_course/gen_course_articles_titles.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,44 @@
 """
-Generator for course's article's content.
+Generator for course's articles titles.
 """
 from typing import List
 from langchain.output_parsers import PydanticOutputParser
 from pydantic import BaseModel, Field
 
 from .gen_base import GenBase
 
 
-class CourseArticleModel(BaseModel):
-    content: str = Field(description="Article content")
-    questions: List[str] = Field(
-        description="List of questions related to the article")
+class CourseArticlesTitlesModel(BaseModel):
+    titles: List[str] = Field(
+        description="List of course's articles titles. All the titles are unique and sequential for the course.")
 
-    def get_article_content(self) -> str:
-        return f"""{self.content}
 
-Questions the reader may be interested in making after reading the article:
-1. {self.questions[0]}
-2. {self.questions[1]}
-3. {self.questions[2]}"""
-
-
-class GenCourseArticleContent(GenBase):
+class GenCourseArticleTitles(GenBase):
     """
-    Generator class for course's article's content'.
+    Generator class for course's articles titles.
     """
     HUMAN_PROMPT = """I'm developing a micro learning course about the following:
 ---
 Title: {course_title}
 Description: {course_description}
 ---
-Write a short article of maximum {content_length_words} for this title: "{article_title}". Do not repeat the title in the article content. Write 3 questions about the article that the reader might be interested in asking after reading the article."""
+Write {articles_count} titles for the articles of the course. Each title should be maximum of {title_length_words} words."""
 
     def __init__(self, llm, verbose: bool = False):
         super().__init__(llm, verbose)
 
     def get_output_parser(self):
-        return PydanticOutputParser(pydantic_object=CourseArticleModel)
+        return PydanticOutputParser(pydantic_object=CourseArticlesTitlesModel)
 
     def generate(self,
                  course_title: str,
                  course_description: str,
-                 article_title: str,
-                 content_length_words: int = 150,
-                 ) -> CourseArticleModel:
+                 articles_count: int,
+                 title_length_words: int = 8,
+                 ) -> CourseArticlesTitlesModel:
         return self.generate_output(
             course_title=course_title,
             course_description=course_description,
-            article_title=article_title,
-            content_length_words=content_length_words,
+            articles_count=articles_count,
+            title_length_words=title_length_words,
         )
```

### Comparing `microlearn_gen_course-0.0.4/src/gen_course/gen_course_metadata.py` & `microlearn_gen_course-0.0.5/src/gen_course/gen_course_metadata.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/PKG-INFO` & `microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microlearn-gen-course
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package for generating microlearn course content
 Home-page: https://github.com/AIprojectflow/gen_course
 Project-URL: Bug Tracker, https://github.com/AIprojectflow/gen_course/issues
 Project-URL: Changelog, https://github.com/AIprojectflow/gen_course/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `microlearn_gen_course-0.0.4/src/microlearn_gen_course.egg-info/SOURCES.txt` & `microlearn_gen_course-0.0.5/src/microlearn_gen_course.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/src/tests/test_answer_to_article_ques.py` & `microlearn_gen_course-0.0.5/src/tests/test_answer_to_article_ques.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/src/tests/test_gen_course_articles_titles.py` & `microlearn_gen_course-0.0.5/src/tests/test_gen_course_articles_titles.py`

 * *Files identical despite different names*

### Comparing `microlearn_gen_course-0.0.4/src/tests/test_gen_course_metadata.py` & `microlearn_gen_course-0.0.5/src/tests/test_gen_course_metadata.py`

 * *Files identical despite different names*

