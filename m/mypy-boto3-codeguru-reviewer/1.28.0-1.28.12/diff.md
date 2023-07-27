# Comparing `tmp/mypy-boto3-codeguru-reviewer-1.28.0.tar.gz` & `tmp/mypy-boto3-codeguru-reviewer-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.28.0.tar", last modified: Thu Jul  6 20:59:14 2023, max compression
+gzip compressed data, was "mypy-boto3-codeguru-reviewer-1.28.12.tar", last modified: Thu Jul 27 05:34:28 2023, max compression
```

## Comparing `mypy-boto3-codeguru-reviewer-1.28.0.tar` & `mypy-boto3-codeguru-reviewer-1.28.12.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:14.014254 mypy-boto3-codeguru-reviewer-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-06 20:59:14.010254 mypy-boto3-codeguru-reviewer-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:14.002254 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21005 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20983 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-06 20:36:04.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:14.010254 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 20:59:13.000000 mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:14.014254 mypy-boto3-codeguru-reviewer-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 20:36:03.000000 mypy-boto3-codeguru-reviewer-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.168553 mypy-boto3-codeguru-reviewer-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-07-27 05:34:28.164553 mypy-boto3-codeguru-reviewer-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.160553 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24069 2023-07-27 05:19:08.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24043 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:28.164553 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16877 2023-07-27 05:34:27.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:28.000000 mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:28.168553 mypy-boto3-codeguru-reviewer-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:19:07.000000 mypy-boto3-codeguru-reviewer-1.28.12/setup.py
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/LICENSE` & `mypy-boto3-codeguru-reviewer-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeGuruReviewer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-reviewer"></a>
 
 # mypy-boto3-codeguru-reviewer
 
 [![PyPI - mypy-boto3-codeguru-reviewer](https://img.shields.io/pypi/v/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,61 +364,71 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
+    BranchDiffSourceCodeTypeOutputTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
+    CodeArtifactsOutputTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
+    CommitDiffSourceCodeTypeOutputTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeReviewRequestRequestTypeDef,
     DescribeRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackTypeDef,
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
+    EventInfoOutputTypeDef,
     EventInfoTypeDef,
+    KMSKeyDetailsOutputTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
+    RepositoryHeadSourceCodeTypeOutputTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    S3RepositoryDetailsOutputTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
+    RequestMetadataOutputTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
+    S3BucketRepositoryOutputTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
     AssociateRepositoryResponseTypeDef,
     DescribeRepositoryAssociationResponseTypeDef,
     DisassociateRepositoryResponseTypeDef,
+    SourceCodeTypeOutputTypeDef,
     SourceCodeTypeTypeDef,
     CodeReviewSummaryTypeDef,
     CodeReviewTypeDef,
     RepositoryAnalysisTypeDef,
     ListCodeReviewsResponseTypeDef,
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/README.md` & `mypy-boto3-codeguru-reviewer-1.28.12/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codeguru-reviewer"></a>
 
 # mypy-boto3-codeguru-reviewer
 
 [![PyPI - mypy-boto3-codeguru-reviewer](https://img.shields.io/pypi/v/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -332,61 +332,71 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
+    BranchDiffSourceCodeTypeOutputTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
+    CodeArtifactsOutputTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
+    CommitDiffSourceCodeTypeOutputTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeReviewRequestRequestTypeDef,
     DescribeRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackTypeDef,
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
+    EventInfoOutputTypeDef,
     EventInfoTypeDef,
+    KMSKeyDetailsOutputTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
+    RepositoryHeadSourceCodeTypeOutputTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    S3RepositoryDetailsOutputTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
+    RequestMetadataOutputTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
+    S3BucketRepositoryOutputTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
     AssociateRepositoryResponseTypeDef,
     DescribeRepositoryAssociationResponseTypeDef,
     DisassociateRepositoryResponseTypeDef,
+    SourceCodeTypeOutputTypeDef,
     SourceCodeTypeTypeDef,
     CodeReviewSummaryTypeDef,
     CodeReviewTypeDef,
     RepositoryAnalysisTypeDef,
     ListCodeReviewsResponseTypeDef,
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.py` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__init__.pyi` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/__main__.py` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeGuruReviewer 1.28.0\nVersion:         1.28.0\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeGuruReviewer 1.28.12\nVersion:         1.28.12\nBuilder"
+        " version: 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.12")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.py` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/client.pyi` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.py` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -275,26 +276,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/literals.pyi` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -273,26 +274,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.py` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/paginator.pyi` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.py` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,61 +33,71 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "KMSKeyDetailsTypeDef",
+    "BranchDiffSourceCodeTypeOutputTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
+    "CodeArtifactsOutputTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
+    "CommitDiffSourceCodeTypeOutputTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeReviewRequestRequestTypeDef",
     "DescribeRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackTypeDef",
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
+    "EventInfoOutputTypeDef",
     "EventInfoTypeDef",
+    "KMSKeyDetailsOutputTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
+    "RepositoryHeadSourceCodeTypeOutputTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "S3RepositoryDetailsOutputTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
+    "RequestMetadataOutputTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
+    "S3BucketRepositoryOutputTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
     "AssociateRepositoryResponseTypeDef",
     "DescribeRepositoryAssociationResponseTypeDef",
     "DisassociateRepositoryResponseTypeDef",
+    "SourceCodeTypeOutputTypeDef",
     "SourceCodeTypeTypeDef",
     "CodeReviewSummaryTypeDef",
     "CodeReviewTypeDef",
     "RepositoryAnalysisTypeDef",
     "ListCodeReviewsResponseTypeDef",
     "CreateCodeReviewResponseTypeDef",
     "DescribeCodeReviewResponseTypeDef",
@@ -100,22 +110,51 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
     },
     total=False,
 )
 
+BranchDiffSourceCodeTypeOutputTypeDef = TypedDict(
+    "BranchDiffSourceCodeTypeOutputTypeDef",
+    {
+        "SourceBranchName": str,
+        "DestinationBranchName": str,
+    },
+)
+
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
 
+_RequiredCodeArtifactsOutputTypeDef = TypedDict(
+    "_RequiredCodeArtifactsOutputTypeDef",
+    {
+        "SourceCodeArtifactsObjectKey": str,
+    },
+)
+_OptionalCodeArtifactsOutputTypeDef = TypedDict(
+    "_OptionalCodeArtifactsOutputTypeDef",
+    {
+        "BuildArtifactsObjectKey": str,
+    },
+    total=False,
+)
+
+
+class CodeArtifactsOutputTypeDef(
+    _RequiredCodeArtifactsOutputTypeDef, _OptionalCodeArtifactsOutputTypeDef
+):
+    pass
+
+
 _RequiredCodeArtifactsTypeDef = TypedDict(
     "_RequiredCodeArtifactsTypeDef",
     {
         "SourceCodeArtifactsObjectKey": str,
     },
 )
 _OptionalCodeArtifactsTypeDef = TypedDict(
@@ -154,14 +193,24 @@
         "MeteredLinesOfCodeCount": int,
         "SuppressedLinesOfCodeCount": int,
         "FindingsCount": int,
     },
     total=False,
 )
 
+CommitDiffSourceCodeTypeOutputTypeDef = TypedDict(
+    "CommitDiffSourceCodeTypeOutputTypeDef",
+    {
+        "SourceCommit": str,
+        "DestinationCommit": str,
+        "MergeBaseCommit": str,
+    },
+    total=False,
+)
+
 CommitDiffSourceCodeTypeTypeDef = TypedDict(
     "CommitDiffSourceCodeTypeTypeDef",
     {
         "SourceCommit": str,
         "DestinationCommit": str,
         "MergeBaseCommit": str,
     },
@@ -230,23 +279,41 @@
 DisassociateRepositoryRequestRequestTypeDef = TypedDict(
     "DisassociateRepositoryRequestRequestTypeDef",
     {
         "AssociationArn": str,
     },
 )
 
+EventInfoOutputTypeDef = TypedDict(
+    "EventInfoOutputTypeDef",
+    {
+        "Name": str,
+        "State": str,
+    },
+    total=False,
+)
+
 EventInfoTypeDef = TypedDict(
     "EventInfoTypeDef",
     {
         "Name": str,
         "State": str,
     },
     total=False,
 )
 
+KMSKeyDetailsOutputTypeDef = TypedDict(
+    "KMSKeyDetailsOutputTypeDef",
+    {
+        "KMSKeyId": str,
+        "EncryptionOption": EncryptionOptionType,
+    },
+    total=False,
+)
+
 _RequiredListCodeReviewsRequestRequestTypeDef = TypedDict(
     "_RequiredListCodeReviewsRequestRequestTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalListCodeReviewsRequestRequestTypeDef = TypedDict(
@@ -415,14 +482,21 @@
 RepositoryHeadSourceCodeTypeTypeDef = TypedDict(
     "RepositoryHeadSourceCodeTypeTypeDef",
     {
         "BranchName": str,
     },
 )
 
+RepositoryHeadSourceCodeTypeOutputTypeDef = TypedDict(
+    "RepositoryHeadSourceCodeTypeOutputTypeDef",
+    {
+        "BranchName": str,
+    },
+)
+
 S3RepositoryTypeDef = TypedDict(
     "S3RepositoryTypeDef",
     {
         "Name": str,
         "BucketName": str,
     },
 )
@@ -459,14 +533,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+S3RepositoryDetailsOutputTypeDef = TypedDict(
+    "S3RepositoryDetailsOutputTypeDef",
+    {
+        "BucketName": str,
+        "CodeArtifacts": CodeArtifactsOutputTypeDef,
+    },
+    total=False,
+)
+
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
     },
     total=False,
@@ -520,14 +603,25 @@
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RequestMetadataOutputTypeDef = TypedDict(
+    "RequestMetadataOutputTypeDef",
+    {
+        "RequestId": str,
+        "Requester": str,
+        "EventInfo": EventInfoOutputTypeDef,
+        "VendorName": VendorNameType,
+    },
+    total=False,
+)
+
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
         "Requester": str,
         "EventInfo": EventInfoTypeDef,
         "VendorName": VendorNameType,
@@ -588,20 +682,41 @@
         "Name": str,
         "Owner": str,
         "ProviderType": ProviderTypeType,
         "State": RepositoryAssociationStateType,
         "StateReason": str,
         "LastUpdatedTimeStamp": datetime,
         "CreatedTimeStamp": datetime,
-        "KMSKeyDetails": KMSKeyDetailsTypeDef,
-        "S3RepositoryDetails": S3RepositoryDetailsTypeDef,
+        "KMSKeyDetails": KMSKeyDetailsOutputTypeDef,
+        "S3RepositoryDetails": S3RepositoryDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredS3BucketRepositoryOutputTypeDef = TypedDict(
+    "_RequiredS3BucketRepositoryOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalS3BucketRepositoryOutputTypeDef = TypedDict(
+    "_OptionalS3BucketRepositoryOutputTypeDef",
+    {
+        "Details": S3RepositoryDetailsOutputTypeDef,
     },
     total=False,
 )
 
+
+class S3BucketRepositoryOutputTypeDef(
+    _RequiredS3BucketRepositoryOutputTypeDef, _OptionalS3BucketRepositoryOutputTypeDef
+):
+    pass
+
+
 _RequiredS3BucketRepositoryTypeDef = TypedDict(
     "_RequiredS3BucketRepositoryTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalS3BucketRepositoryTypeDef = TypedDict(
@@ -675,14 +790,26 @@
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SourceCodeTypeOutputTypeDef = TypedDict(
+    "SourceCodeTypeOutputTypeDef",
+    {
+        "CommitDiff": CommitDiffSourceCodeTypeOutputTypeDef,
+        "RepositoryHead": RepositoryHeadSourceCodeTypeOutputTypeDef,
+        "BranchDiff": BranchDiffSourceCodeTypeOutputTypeDef,
+        "S3BucketRepository": S3BucketRepositoryOutputTypeDef,
+        "RequestMetadata": RequestMetadataOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
         "RepositoryHead": RepositoryHeadSourceCodeTypeTypeDef,
         "BranchDiff": BranchDiffSourceCodeTypeTypeDef,
         "S3BucketRepository": S3BucketRepositoryTypeDef,
@@ -701,15 +828,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
         "MetricsSummary": MetricsSummaryTypeDef,
-        "SourceCodeType": SourceCodeTypeTypeDef,
+        "SourceCodeType": SourceCodeTypeOutputTypeDef,
     },
     total=False,
 )
 
 CodeReviewTypeDef = TypedDict(
     "CodeReviewTypeDef",
     {
@@ -720,15 +847,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "StateReason": str,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
-        "SourceCodeType": SourceCodeTypeTypeDef,
+        "SourceCodeType": SourceCodeTypeOutputTypeDef,
         "AssociationArn": str,
         "Metrics": MetricsTypeDef,
         "AnalysisTypes": List[AnalysisTypeType],
         "ConfigFileState": ConfigFileStateType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/type_defs.pyi` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -32,61 +32,71 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "KMSKeyDetailsTypeDef",
+    "BranchDiffSourceCodeTypeOutputTypeDef",
     "BranchDiffSourceCodeTypeTypeDef",
+    "CodeArtifactsOutputTypeDef",
     "CodeArtifactsTypeDef",
     "CodeCommitRepositoryTypeDef",
     "MetricsSummaryTypeDef",
     "MetricsTypeDef",
+    "CommitDiffSourceCodeTypeOutputTypeDef",
     "CommitDiffSourceCodeTypeTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeReviewRequestRequestTypeDef",
     "DescribeRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackTypeDef",
     "DescribeRepositoryAssociationRequestRequestTypeDef",
     "DisassociateRepositoryRequestRequestTypeDef",
+    "EventInfoOutputTypeDef",
     "EventInfoTypeDef",
+    "KMSKeyDetailsOutputTypeDef",
     "ListCodeReviewsRequestRequestTypeDef",
     "ListRecommendationFeedbackRequestRequestTypeDef",
     "RecommendationFeedbackSummaryTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef",
     "ListRepositoryAssociationsRequestRequestTypeDef",
     "RepositoryAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "PutRecommendationFeedbackRequestRequestTypeDef",
     "RuleMetadataTypeDef",
     "RepositoryHeadSourceCodeTypeTypeDef",
+    "RepositoryHeadSourceCodeTypeOutputTypeDef",
     "S3RepositoryTypeDef",
     "ThirdPartySourceRepositoryTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "S3RepositoryDetailsOutputTypeDef",
     "S3RepositoryDetailsTypeDef",
     "DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef",
     "DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef",
     "DescribeRecommendationFeedbackResponseTypeDef",
+    "RequestMetadataOutputTypeDef",
     "RequestMetadataTypeDef",
     "ListRecommendationFeedbackResponseTypeDef",
     "ListRepositoryAssociationsResponseTypeDef",
     "RecommendationSummaryTypeDef",
     "RepositoryTypeDef",
     "RepositoryAssociationTypeDef",
+    "S3BucketRepositoryOutputTypeDef",
     "S3BucketRepositoryTypeDef",
     "ListRecommendationsResponseTypeDef",
     "AssociateRepositoryRequestRequestTypeDef",
     "AssociateRepositoryResponseTypeDef",
     "DescribeRepositoryAssociationResponseTypeDef",
     "DisassociateRepositoryResponseTypeDef",
+    "SourceCodeTypeOutputTypeDef",
     "SourceCodeTypeTypeDef",
     "CodeReviewSummaryTypeDef",
     "CodeReviewTypeDef",
     "RepositoryAnalysisTypeDef",
     "ListCodeReviewsResponseTypeDef",
     "CreateCodeReviewResponseTypeDef",
     "DescribeCodeReviewResponseTypeDef",
@@ -99,22 +109,49 @@
     {
         "KMSKeyId": str,
         "EncryptionOption": EncryptionOptionType,
     },
     total=False,
 )
 
+BranchDiffSourceCodeTypeOutputTypeDef = TypedDict(
+    "BranchDiffSourceCodeTypeOutputTypeDef",
+    {
+        "SourceBranchName": str,
+        "DestinationBranchName": str,
+    },
+)
+
 BranchDiffSourceCodeTypeTypeDef = TypedDict(
     "BranchDiffSourceCodeTypeTypeDef",
     {
         "SourceBranchName": str,
         "DestinationBranchName": str,
     },
 )
 
+_RequiredCodeArtifactsOutputTypeDef = TypedDict(
+    "_RequiredCodeArtifactsOutputTypeDef",
+    {
+        "SourceCodeArtifactsObjectKey": str,
+    },
+)
+_OptionalCodeArtifactsOutputTypeDef = TypedDict(
+    "_OptionalCodeArtifactsOutputTypeDef",
+    {
+        "BuildArtifactsObjectKey": str,
+    },
+    total=False,
+)
+
+class CodeArtifactsOutputTypeDef(
+    _RequiredCodeArtifactsOutputTypeDef, _OptionalCodeArtifactsOutputTypeDef
+):
+    pass
+
 _RequiredCodeArtifactsTypeDef = TypedDict(
     "_RequiredCodeArtifactsTypeDef",
     {
         "SourceCodeArtifactsObjectKey": str,
     },
 )
 _OptionalCodeArtifactsTypeDef = TypedDict(
@@ -151,14 +188,24 @@
         "MeteredLinesOfCodeCount": int,
         "SuppressedLinesOfCodeCount": int,
         "FindingsCount": int,
     },
     total=False,
 )
 
+CommitDiffSourceCodeTypeOutputTypeDef = TypedDict(
+    "CommitDiffSourceCodeTypeOutputTypeDef",
+    {
+        "SourceCommit": str,
+        "DestinationCommit": str,
+        "MergeBaseCommit": str,
+    },
+    total=False,
+)
+
 CommitDiffSourceCodeTypeTypeDef = TypedDict(
     "CommitDiffSourceCodeTypeTypeDef",
     {
         "SourceCommit": str,
         "DestinationCommit": str,
         "MergeBaseCommit": str,
     },
@@ -225,23 +272,41 @@
 DisassociateRepositoryRequestRequestTypeDef = TypedDict(
     "DisassociateRepositoryRequestRequestTypeDef",
     {
         "AssociationArn": str,
     },
 )
 
+EventInfoOutputTypeDef = TypedDict(
+    "EventInfoOutputTypeDef",
+    {
+        "Name": str,
+        "State": str,
+    },
+    total=False,
+)
+
 EventInfoTypeDef = TypedDict(
     "EventInfoTypeDef",
     {
         "Name": str,
         "State": str,
     },
     total=False,
 )
 
+KMSKeyDetailsOutputTypeDef = TypedDict(
+    "KMSKeyDetailsOutputTypeDef",
+    {
+        "KMSKeyId": str,
+        "EncryptionOption": EncryptionOptionType,
+    },
+    total=False,
+)
+
 _RequiredListCodeReviewsRequestRequestTypeDef = TypedDict(
     "_RequiredListCodeReviewsRequestRequestTypeDef",
     {
         "Type": TypeType,
     },
 )
 _OptionalListCodeReviewsRequestRequestTypeDef = TypedDict(
@@ -404,14 +469,21 @@
 RepositoryHeadSourceCodeTypeTypeDef = TypedDict(
     "RepositoryHeadSourceCodeTypeTypeDef",
     {
         "BranchName": str,
     },
 )
 
+RepositoryHeadSourceCodeTypeOutputTypeDef = TypedDict(
+    "RepositoryHeadSourceCodeTypeOutputTypeDef",
+    {
+        "BranchName": str,
+    },
+)
+
 S3RepositoryTypeDef = TypedDict(
     "S3RepositoryTypeDef",
     {
         "Name": str,
         "BucketName": str,
     },
 )
@@ -448,14 +520,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+S3RepositoryDetailsOutputTypeDef = TypedDict(
+    "S3RepositoryDetailsOutputTypeDef",
+    {
+        "BucketName": str,
+        "CodeArtifacts": CodeArtifactsOutputTypeDef,
+    },
+    total=False,
+)
+
 S3RepositoryDetailsTypeDef = TypedDict(
     "S3RepositoryDetailsTypeDef",
     {
         "BucketName": str,
         "CodeArtifacts": CodeArtifactsTypeDef,
     },
     total=False,
@@ -505,14 +586,25 @@
     "DescribeRecommendationFeedbackResponseTypeDef",
     {
         "RecommendationFeedback": RecommendationFeedbackTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+RequestMetadataOutputTypeDef = TypedDict(
+    "RequestMetadataOutputTypeDef",
+    {
+        "RequestId": str,
+        "Requester": str,
+        "EventInfo": EventInfoOutputTypeDef,
+        "VendorName": VendorNameType,
+    },
+    total=False,
+)
+
 RequestMetadataTypeDef = TypedDict(
     "RequestMetadataTypeDef",
     {
         "RequestId": str,
         "Requester": str,
         "EventInfo": EventInfoTypeDef,
         "VendorName": VendorNameType,
@@ -573,20 +665,39 @@
         "Name": str,
         "Owner": str,
         "ProviderType": ProviderTypeType,
         "State": RepositoryAssociationStateType,
         "StateReason": str,
         "LastUpdatedTimeStamp": datetime,
         "CreatedTimeStamp": datetime,
-        "KMSKeyDetails": KMSKeyDetailsTypeDef,
-        "S3RepositoryDetails": S3RepositoryDetailsTypeDef,
+        "KMSKeyDetails": KMSKeyDetailsOutputTypeDef,
+        "S3RepositoryDetails": S3RepositoryDetailsOutputTypeDef,
     },
     total=False,
 )
 
+_RequiredS3BucketRepositoryOutputTypeDef = TypedDict(
+    "_RequiredS3BucketRepositoryOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalS3BucketRepositoryOutputTypeDef = TypedDict(
+    "_OptionalS3BucketRepositoryOutputTypeDef",
+    {
+        "Details": S3RepositoryDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
+class S3BucketRepositoryOutputTypeDef(
+    _RequiredS3BucketRepositoryOutputTypeDef, _OptionalS3BucketRepositoryOutputTypeDef
+):
+    pass
+
 _RequiredS3BucketRepositoryTypeDef = TypedDict(
     "_RequiredS3BucketRepositoryTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalS3BucketRepositoryTypeDef = TypedDict(
@@ -656,14 +767,26 @@
     {
         "RepositoryAssociation": RepositoryAssociationTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+SourceCodeTypeOutputTypeDef = TypedDict(
+    "SourceCodeTypeOutputTypeDef",
+    {
+        "CommitDiff": CommitDiffSourceCodeTypeOutputTypeDef,
+        "RepositoryHead": RepositoryHeadSourceCodeTypeOutputTypeDef,
+        "BranchDiff": BranchDiffSourceCodeTypeOutputTypeDef,
+        "S3BucketRepository": S3BucketRepositoryOutputTypeDef,
+        "RequestMetadata": RequestMetadataOutputTypeDef,
+    },
+    total=False,
+)
+
 SourceCodeTypeTypeDef = TypedDict(
     "SourceCodeTypeTypeDef",
     {
         "CommitDiff": CommitDiffSourceCodeTypeTypeDef,
         "RepositoryHead": RepositoryHeadSourceCodeTypeTypeDef,
         "BranchDiff": BranchDiffSourceCodeTypeTypeDef,
         "S3BucketRepository": S3BucketRepositoryTypeDef,
@@ -682,15 +805,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
         "MetricsSummary": MetricsSummaryTypeDef,
-        "SourceCodeType": SourceCodeTypeTypeDef,
+        "SourceCodeType": SourceCodeTypeOutputTypeDef,
     },
     total=False,
 )
 
 CodeReviewTypeDef = TypedDict(
     "CodeReviewTypeDef",
     {
@@ -701,15 +824,15 @@
         "ProviderType": ProviderTypeType,
         "State": JobStateType,
         "StateReason": str,
         "CreatedTimeStamp": datetime,
         "LastUpdatedTimeStamp": datetime,
         "Type": TypeType,
         "PullRequestId": str,
-        "SourceCodeType": SourceCodeTypeTypeDef,
+        "SourceCodeType": SourceCodeTypeOutputTypeDef,
         "AssociationArn": str,
         "Metrics": MetricsTypeDef,
         "AnalysisTypes": List[AnalysisTypeType],
         "ConfigFileState": ConfigFileStateType,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.py` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer/waiter.pyi` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codeguru-reviewer
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeGuruReviewer 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeGuruReviewer 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codeguru-reviewer"></a>
 
 # mypy-boto3-codeguru-reviewer
 
 [![PyPI - mypy-boto3-codeguru-reviewer](https://img.shields.io/pypi/v/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/mypy-boto3-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codeguru-reviewer?color=blue)](https://pypistats.org/packages/mypy-boto3-codeguru-reviewer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codeguru-reviewer)](https://pepy.tech/project/mypy-boto3-codeguru-reviewer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeGuruReviewer 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
+[boto3.CodeGuruReviewer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-codeguru-reviewer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,61 +364,71 @@
 
 `mypy_boto3_codeguru_reviewer.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_codeguru_reviewer.type_defs import (
     KMSKeyDetailsTypeDef,
+    BranchDiffSourceCodeTypeOutputTypeDef,
     BranchDiffSourceCodeTypeTypeDef,
+    CodeArtifactsOutputTypeDef,
     CodeArtifactsTypeDef,
     CodeCommitRepositoryTypeDef,
     MetricsSummaryTypeDef,
     MetricsTypeDef,
+    CommitDiffSourceCodeTypeOutputTypeDef,
     CommitDiffSourceCodeTypeTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeReviewRequestRequestTypeDef,
     DescribeRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackTypeDef,
     DescribeRepositoryAssociationRequestRequestTypeDef,
     DisassociateRepositoryRequestRequestTypeDef,
+    EventInfoOutputTypeDef,
     EventInfoTypeDef,
+    KMSKeyDetailsOutputTypeDef,
     ListCodeReviewsRequestRequestTypeDef,
     ListRecommendationFeedbackRequestRequestTypeDef,
     RecommendationFeedbackSummaryTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
     ListRepositoryAssociationsRequestRequestTypeDef,
     RepositoryAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     PutRecommendationFeedbackRequestRequestTypeDef,
     RuleMetadataTypeDef,
     RepositoryHeadSourceCodeTypeTypeDef,
+    RepositoryHeadSourceCodeTypeOutputTypeDef,
     S3RepositoryTypeDef,
     ThirdPartySourceRepositoryTypeDef,
     ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    S3RepositoryDetailsOutputTypeDef,
     S3RepositoryDetailsTypeDef,
     DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
     DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
     DescribeRecommendationFeedbackResponseTypeDef,
+    RequestMetadataOutputTypeDef,
     RequestMetadataTypeDef,
     ListRecommendationFeedbackResponseTypeDef,
     ListRepositoryAssociationsResponseTypeDef,
     RecommendationSummaryTypeDef,
     RepositoryTypeDef,
     RepositoryAssociationTypeDef,
+    S3BucketRepositoryOutputTypeDef,
     S3BucketRepositoryTypeDef,
     ListRecommendationsResponseTypeDef,
     AssociateRepositoryRequestRequestTypeDef,
     AssociateRepositoryResponseTypeDef,
     DescribeRepositoryAssociationResponseTypeDef,
     DisassociateRepositoryResponseTypeDef,
+    SourceCodeTypeOutputTypeDef,
     SourceCodeTypeTypeDef,
     CodeReviewSummaryTypeDef,
     CodeReviewTypeDef,
     RepositoryAnalysisTypeDef,
     ListCodeReviewsResponseTypeDef,
     CreateCodeReviewResponseTypeDef,
     DescribeCodeReviewResponseTypeDef,
```

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt` & `mypy-boto3-codeguru-reviewer-1.28.12/mypy_boto3_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codeguru-reviewer-1.28.0/setup.py` & `mypy-boto3-codeguru-reviewer-1.28.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codeguru-reviewer",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeGuruReviewer 1.28.0 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.CodeGuruReviewer 1.28.12 service generated with"
+        " mypy-boto3-builder 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

