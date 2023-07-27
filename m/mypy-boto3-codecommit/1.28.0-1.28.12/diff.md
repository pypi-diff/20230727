# Comparing `tmp/mypy-boto3-codecommit-1.28.0.tar.gz` & `tmp/mypy-boto3-codecommit-1.28.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codecommit-1.28.0.tar", last modified: Thu Jul  6 20:59:12 2023, max compression
+gzip compressed data, was "mypy-boto3-codecommit-1.28.12.tar", last modified: Thu Jul 27 05:34:27 2023, max compression
```

## Comparing `mypy-boto3-codecommit-1.28.0.tar` & `mypy-boto3-codecommit-1.28.12.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.718251 mypy-boto3-codecommit-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22911 2023-07-06 20:59:12.718251 mypy-boto3-codecommit-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21414 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.718251 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71776 2023-07-06 20:35:54.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    71685 2023-07-06 20:35:54.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-07-06 20:35:54.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-07-06 20:35:54.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-06 20:35:54.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-06 20:35:54.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    78905 2023-07-06 20:35:58.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    78810 2023-07-06 20:35:55.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:12.718251 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22911 2023-07-06 20:59:12.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 20:59:12.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:12.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:12.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 20:59:12.000000 mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:12.718251 mypy-boto3-codecommit-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 20:35:53.000000 mypy-boto3-codecommit-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21462 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71776 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71685 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10990 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79773 2023-07-27 05:19:03.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79676 2023-07-27 05:19:03.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:01.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:27.000000 mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:27.328555 mypy-boto3-codecommit-1.28.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:19:00.000000 mypy-boto3-codecommit-1.28.12/setup.py
```

### Comparing `mypy-boto3-codecommit-1.28.0/LICENSE` & `mypy-boto3-codecommit-1.28.12/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/PKG-INFO` & `mypy-boto3-codecommit-1.28.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeCommit 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeCommit 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecommit"></a>
 
 # mypy-boto3-codecommit
 
 [![PyPI - mypy-boto3-codecommit](https://img.shields.io/pypi/v/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecommit?color=blue)](https://pypistats.org/packages/mypy-boto3-codecommit)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -379,15 +379,15 @@
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
-    LocationTypeDef,
+    LocationOutputTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
@@ -444,15 +444,15 @@
     GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
     GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
     ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
     ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
     ListBranchesOutputTypeDef,
@@ -462,14 +462,15 @@
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
     ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    LocationTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
     MergeBranchesByFastForwardOutputTypeDef,
     MergeBranchesBySquashOutputTypeDef,
     MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
@@ -479,14 +480,15 @@
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
     PutFileOutputTypeDef,
+    RepositoryTriggerTypeDef,
     PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
@@ -518,33 +520,33 @@
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
-    PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
-    PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
+    PostCommentForComparedCommitInputRequestTypeDef,
+    PostCommentForPullRequestInputRequestTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
```

### Comparing `mypy-boto3-codecommit-1.28.0/README.md` & `mypy-boto3-codecommit-1.28.12/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-codecommit"></a>
 
 # mypy-boto3-codecommit
 
 [![PyPI - mypy-boto3-codecommit](https://img.shields.io/pypi/v/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecommit?color=blue)](https://pypistats.org/packages/mypy-boto3-codecommit)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -347,15 +347,15 @@
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
-    LocationTypeDef,
+    LocationOutputTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
@@ -412,15 +412,15 @@
     GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
     GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
     ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
     ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
     ListBranchesOutputTypeDef,
@@ -430,14 +430,15 @@
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
     ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    LocationTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
     MergeBranchesByFastForwardOutputTypeDef,
     MergeBranchesBySquashOutputTypeDef,
     MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
@@ -447,14 +448,15 @@
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
     PutFileOutputTypeDef,
+    RepositoryTriggerTypeDef,
     PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
@@ -486,33 +488,33 @@
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
-    PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
-    PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
+    PostCommentForComparedCommitInputRequestTypeDef,
+    PostCommentForPullRequestInputRequestTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
```

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/__init__.py` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/__init__.pyi` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/__main__.py` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeCommit 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.CodeCommit 1.28.12\nVersion:         1.28.12\nBuilder version:"
+        " 7.15.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit\nOther"
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

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/client.py` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/client.pyi` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/literals.py` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApprovalStateType",
     "ChangeTypeEnumType",
     "ConflictDetailLevelTypeEnumType",
     "ConflictResolutionStrategyTypeEnumType",
     "DescribePullRequestEventsPaginatorName",
     "FileModeTypeEnumType",
@@ -45,15 +44,14 @@
     "CodeCommitServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApprovalStateType = Literal["APPROVE", "REVOKE"]
 ChangeTypeEnumType = Literal["A", "D", "M"]
 ConflictDetailLevelTypeEnumType = Literal["FILE_LEVEL", "LINE_LEVEL"]
 ConflictResolutionStrategyTypeEnumType = Literal[
     "ACCEPT_DESTINATION", "ACCEPT_SOURCE", "AUTOMERGE", "NONE"
 ]
 DescribePullRequestEventsPaginatorName = Literal["describe_pull_request_events"]
@@ -202,14 +200,15 @@
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
@@ -288,26 +287,28 @@
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

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/literals.pyi` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ApprovalStateType",
     "ChangeTypeEnumType",
     "ConflictDetailLevelTypeEnumType",
     "ConflictResolutionStrategyTypeEnumType",
     "DescribePullRequestEventsPaginatorName",
     "FileModeTypeEnumType",
@@ -44,14 +45,15 @@
     "CodeCommitServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ApprovalStateType = Literal["APPROVE", "REVOKE"]
 ChangeTypeEnumType = Literal["A", "D", "M"]
 ConflictDetailLevelTypeEnumType = Literal["FILE_LEVEL", "LINE_LEVEL"]
 ConflictResolutionStrategyTypeEnumType = Literal[
     "ACCEPT_DESTINATION", "ACCEPT_SOURCE", "AUTOMERGE", "NONE"
 ]
 DescribePullRequestEventsPaginatorName = Literal["describe_pull_request_events"]
@@ -200,14 +202,15 @@
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
@@ -286,26 +289,28 @@
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

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/paginator.py` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/paginator.pyi` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/type_defs.py` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
-    "LocationTypeDef",
+    "LocationOutputTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
@@ -123,15 +123,15 @@
     "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
     "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
-    "RepositoryTriggerTypeDef",
+    "RepositoryTriggerOutputTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
     "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
     "ListBranchesOutputTypeDef",
@@ -141,14 +141,15 @@
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "LocationTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
     "MergeBranchesByFastForwardOutputTypeDef",
     "MergeBranchesBySquashOutputTypeDef",
     "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
@@ -158,14 +159,15 @@
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "PutFileInputRequestTypeDef",
     "PutFileOutputTypeDef",
+    "RepositoryTriggerTypeDef",
     "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
@@ -197,33 +199,33 @@
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
-    "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
-    "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
     "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
+    "PostCommentForComparedCommitInputRequestTypeDef",
+    "PostCommentForPullRequestInputRequestTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
@@ -471,16 +473,16 @@
         "clientRequestToken": str,
         "callerReactions": List[str],
         "reactionCounts": Dict[str, int],
     },
     total=False,
 )
 
-LocationTypeDef = TypedDict(
-    "LocationTypeDef",
+LocationOutputTypeDef = TypedDict(
+    "LocationOutputTypeDef",
     {
         "filePath": str,
         "filePosition": int,
         "relativeFileVersion": RelativeFileVersionEnumType,
     },
     total=False,
 )
@@ -1355,34 +1357,34 @@
 GetRepositoryTriggersInputRequestTypeDef = TypedDict(
     "GetRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-_RequiredRepositoryTriggerTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerTypeDef",
+_RequiredRepositoryTriggerOutputTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerOutputTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": List[RepositoryTriggerEventEnumType],
     },
 )
-_OptionalRepositoryTriggerTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerTypeDef",
+_OptionalRepositoryTriggerOutputTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerOutputTypeDef",
     {
         "customData": str,
         "branches": List[str],
     },
     total=False,
 )
 
 
-class RepositoryTriggerTypeDef(
-    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+class RepositoryTriggerOutputTypeDef(
+    _RequiredRepositoryTriggerOutputTypeDef, _OptionalRepositoryTriggerOutputTypeDef
 ):
     pass
 
 
 ListApprovalRuleTemplatesInputRequestTypeDef = TypedDict(
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     {
@@ -1629,14 +1631,24 @@
     {
         "tags": Dict[str, str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LocationTypeDef = TypedDict(
+    "LocationTypeDef",
+    {
+        "filePath": str,
+        "filePosition": int,
+        "relativeFileVersion": RelativeFileVersionEnumType,
+    },
+    total=False,
+)
+
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1862,14 +1874,38 @@
         "commitId": str,
         "blobId": str,
         "treeId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRepositoryTriggerTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerTypeDef",
+    {
+        "name": str,
+        "destinationArn": str,
+        "events": Sequence[RepositoryTriggerEventEnumType],
+    },
+)
+_OptionalRepositoryTriggerTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerTypeDef",
+    {
+        "customData": str,
+        "branches": Sequence[str],
+    },
+    total=False,
+)
+
+
+class RepositoryTriggerTypeDef(
+    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+):
+    pass
+
+
 PutRepositoryTriggersOutputTypeDef = TypedDict(
     "PutRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2230,112 +2266,59 @@
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
 CommentsForPullRequestTypeDef = TypedDict(
     "CommentsForPullRequestTypeDef",
     {
         "pullRequestId": str,
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
-_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-        "content": str,
-    },
-)
-_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
-    {
-        "beforeCommitId": str,
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
-    },
-    total=False,
-)
-
-
-class PostCommentForComparedCommitInputRequestTypeDef(
-    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
-    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
-):
-    pass
-
-
 PostCommentForComparedCommitOutputTypeDef = TypedDict(
     "PostCommentForComparedCommitOutputTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comment": CommentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
-    {
-        "pullRequestId": str,
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "content": str,
-    },
-)
-_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
-    {
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
-    },
-    total=False,
-)
-
-
-class PostCommentForPullRequestInputRequestTypeDef(
-    _RequiredPostCommentForPullRequestInputRequestTypeDef,
-    _OptionalPostCommentForPullRequestInputRequestTypeDef,
-):
-    pass
-
-
 PostCommentForPullRequestOutputTypeDef = TypedDict(
     "PostCommentForPullRequestOutputTypeDef",
     {
         "repositoryName": str,
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comment": CommentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
@@ -2435,43 +2418,80 @@
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
-        "triggers": List[RepositoryTriggerTypeDef],
+        "triggers": List[RepositoryTriggerOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
+ListRepositoriesOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputTypeDef",
     {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
+        "repositories": List[RepositoryNameIdPairTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
+_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
+        "afterCommitId": str,
+        "content": str,
     },
 )
+_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
+    {
+        "beforeCommitId": str,
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
+    },
+    total=False,
+)
 
-ListRepositoriesOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputTypeDef",
+
+class PostCommentForComparedCommitInputRequestTypeDef(
+    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
+    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
     {
-        "repositories": List[RepositoryNameIdPairTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pullRequestId": str,
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "content": str,
     },
 )
+_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
+    {
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+
+class PostCommentForPullRequestInputRequestTypeDef(
+    _RequiredPostCommentForPullRequestInputRequestTypeDef,
+    _OptionalPostCommentForPullRequestInputRequestTypeDef,
+):
+    pass
+
 
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
         "source": MergeHunkDetailTypeDef,
         "destination": MergeHunkDetailTypeDef,
@@ -2521,14 +2541,30 @@
 )
 
 
 class PutFileEntryTypeDef(_RequiredPutFileEntryTypeDef, _OptionalPutFileEntryTypeDef):
     pass
 
 
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
 ReactionForCommentTypeDef = TypedDict(
     "ReactionForCommentTypeDef",
     {
         "reaction": ReactionValueFormatsTypeDef,
         "reactionUsers": List[str],
         "reactionsFromDeletedUsersCount": int,
     },
```

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit/type_defs.pyi` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     "BatchGetCommitsErrorTypeDef",
     "BatchGetCommitsInputRequestTypeDef",
     "BatchGetRepositoriesInputRequestTypeDef",
     "RepositoryMetadataTypeDef",
     "BlobMetadataTypeDef",
     "BranchInfoTypeDef",
     "CommentTypeDef",
-    "LocationTypeDef",
+    "LocationOutputTypeDef",
     "UserInfoTypeDef",
     "FileModesTypeDef",
     "FileSizesTypeDef",
     "IsBinaryFileTypeDef",
     "MergeOperationsTypeDef",
     "ObjectTypesTypeDef",
     "DeleteFileEntryTypeDef",
@@ -122,15 +122,15 @@
     "GetMergeOptionsOutputTypeDef",
     "GetPullRequestApprovalStatesInputRequestTypeDef",
     "GetPullRequestInputRequestTypeDef",
     "GetPullRequestOverrideStateInputRequestTypeDef",
     "GetPullRequestOverrideStateOutputTypeDef",
     "GetRepositoryInputRequestTypeDef",
     "GetRepositoryTriggersInputRequestTypeDef",
-    "RepositoryTriggerTypeDef",
+    "RepositoryTriggerOutputTypeDef",
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     "ListApprovalRuleTemplatesOutputTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef",
     "ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef",
     "ListBranchesInputListBranchesPaginateTypeDef",
     "ListBranchesInputRequestTypeDef",
     "ListBranchesOutputTypeDef",
@@ -140,14 +140,15 @@
     "ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef",
     "ListRepositoriesForApprovalRuleTemplateOutputTypeDef",
     "ListRepositoriesInputListRepositoriesPaginateTypeDef",
     "ListRepositoriesInputRequestTypeDef",
     "RepositoryNameIdPairTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "LocationTypeDef",
     "MergeBranchesByFastForwardInputRequestTypeDef",
     "MergeBranchesByFastForwardOutputTypeDef",
     "MergeBranchesBySquashOutputTypeDef",
     "MergeBranchesByThreeWayOutputTypeDef",
     "MergeHunkDetailTypeDef",
     "MergeMetadataTypeDef",
     "MergePullRequestByFastForwardInputRequestTypeDef",
@@ -157,14 +158,15 @@
     "PullRequestCreatedEventMetadataTypeDef",
     "PullRequestSourceReferenceUpdatedEventMetadataTypeDef",
     "PullRequestStatusChangedEventMetadataTypeDef",
     "PutCommentReactionInputRequestTypeDef",
     "SourceFileSpecifierTypeDef",
     "PutFileInputRequestTypeDef",
     "PutFileOutputTypeDef",
+    "RepositoryTriggerTypeDef",
     "PutRepositoryTriggersOutputTypeDef",
     "ReactionValueFormatsTypeDef",
     "RepositoryTriggerExecutionFailureTypeDef",
     "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApprovalRuleTemplateContentInputRequestTypeDef",
@@ -196,33 +198,33 @@
     "GetBranchOutputTypeDef",
     "DeleteCommentContentOutputTypeDef",
     "GetCommentOutputTypeDef",
     "PostCommentReplyOutputTypeDef",
     "UpdateCommentOutputTypeDef",
     "CommentsForComparedCommitTypeDef",
     "CommentsForPullRequestTypeDef",
-    "PostCommentForComparedCommitInputRequestTypeDef",
     "PostCommentForComparedCommitOutputTypeDef",
-    "PostCommentForPullRequestInputRequestTypeDef",
     "PostCommentForPullRequestOutputTypeDef",
     "CommitTypeDef",
     "ConflictMetadataTypeDef",
     "ConflictResolutionTypeDef",
     "CreateCommitOutputTypeDef",
     "CreatePullRequestInputRequestTypeDef",
     "EvaluatePullRequestApprovalRulesOutputTypeDef",
     "GetFolderOutputTypeDef",
     "GetRepositoryTriggersOutputTypeDef",
-    "PutRepositoryTriggersInputRequestTypeDef",
-    "TestRepositoryTriggersInputRequestTypeDef",
     "ListRepositoriesOutputTypeDef",
+    "PostCommentForComparedCommitInputRequestTypeDef",
+    "PostCommentForPullRequestInputRequestTypeDef",
     "MergeHunkTypeDef",
     "PullRequestMergedStateChangedEventMetadataTypeDef",
     "PullRequestTargetTypeDef",
     "PutFileEntryTypeDef",
+    "PutRepositoryTriggersInputRequestTypeDef",
+    "TestRepositoryTriggersInputRequestTypeDef",
     "ReactionForCommentTypeDef",
     "TestRepositoryTriggersOutputTypeDef",
     "CreatePullRequestApprovalRuleOutputTypeDef",
     "UpdatePullRequestApprovalRuleContentOutputTypeDef",
     "GetDifferencesOutputTypeDef",
     "GetCommentsForComparedCommitOutputTypeDef",
     "GetCommentsForPullRequestOutputTypeDef",
@@ -468,16 +470,16 @@
         "clientRequestToken": str,
         "callerReactions": List[str],
         "reactionCounts": Dict[str, int],
     },
     total=False,
 )
 
-LocationTypeDef = TypedDict(
-    "LocationTypeDef",
+LocationOutputTypeDef = TypedDict(
+    "LocationOutputTypeDef",
     {
         "filePath": str,
         "filePosition": int,
         "relativeFileVersion": RelativeFileVersionEnumType,
     },
     total=False,
 )
@@ -1312,33 +1314,33 @@
 GetRepositoryTriggersInputRequestTypeDef = TypedDict(
     "GetRepositoryTriggersInputRequestTypeDef",
     {
         "repositoryName": str,
     },
 )
 
-_RequiredRepositoryTriggerTypeDef = TypedDict(
-    "_RequiredRepositoryTriggerTypeDef",
+_RequiredRepositoryTriggerOutputTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerOutputTypeDef",
     {
         "name": str,
         "destinationArn": str,
         "events": List[RepositoryTriggerEventEnumType],
     },
 )
-_OptionalRepositoryTriggerTypeDef = TypedDict(
-    "_OptionalRepositoryTriggerTypeDef",
+_OptionalRepositoryTriggerOutputTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerOutputTypeDef",
     {
         "customData": str,
         "branches": List[str],
     },
     total=False,
 )
 
-class RepositoryTriggerTypeDef(
-    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+class RepositoryTriggerOutputTypeDef(
+    _RequiredRepositoryTriggerOutputTypeDef, _OptionalRepositoryTriggerOutputTypeDef
 ):
     pass
 
 ListApprovalRuleTemplatesInputRequestTypeDef = TypedDict(
     "ListApprovalRuleTemplatesInputRequestTypeDef",
     {
         "nextToken": str,
@@ -1570,14 +1572,24 @@
     {
         "tags": Dict[str, str],
         "nextToken": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+LocationTypeDef = TypedDict(
+    "LocationTypeDef",
+    {
+        "filePath": str,
+        "filePosition": int,
+        "relativeFileVersion": RelativeFileVersionEnumType,
+    },
+    total=False,
+)
+
 _RequiredMergeBranchesByFastForwardInputRequestTypeDef = TypedDict(
     "_RequiredMergeBranchesByFastForwardInputRequestTypeDef",
     {
         "repositoryName": str,
         "sourceCommitSpecifier": str,
         "destinationCommitSpecifier": str,
     },
@@ -1793,14 +1805,36 @@
         "commitId": str,
         "blobId": str,
         "treeId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
+_RequiredRepositoryTriggerTypeDef = TypedDict(
+    "_RequiredRepositoryTriggerTypeDef",
+    {
+        "name": str,
+        "destinationArn": str,
+        "events": Sequence[RepositoryTriggerEventEnumType],
+    },
+)
+_OptionalRepositoryTriggerTypeDef = TypedDict(
+    "_OptionalRepositoryTriggerTypeDef",
+    {
+        "customData": str,
+        "branches": Sequence[str],
+    },
+    total=False,
+)
+
+class RepositoryTriggerTypeDef(
+    _RequiredRepositoryTriggerTypeDef, _OptionalRepositoryTriggerTypeDef
+):
+    pass
+
 PutRepositoryTriggersOutputTypeDef = TypedDict(
     "PutRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2155,108 +2189,59 @@
     "CommentsForComparedCommitTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
 CommentsForPullRequestTypeDef = TypedDict(
     "CommentsForPullRequestTypeDef",
     {
         "pullRequestId": str,
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comments": List[CommentTypeDef],
     },
     total=False,
 )
 
-_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
-    {
-        "repositoryName": str,
-        "afterCommitId": str,
-        "content": str,
-    },
-)
-_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
-    {
-        "beforeCommitId": str,
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
-    },
-    total=False,
-)
-
-class PostCommentForComparedCommitInputRequestTypeDef(
-    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
-    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
-):
-    pass
-
 PostCommentForComparedCommitOutputTypeDef = TypedDict(
     "PostCommentForComparedCommitOutputTypeDef",
     {
         "repositoryName": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comment": CommentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
-    {
-        "pullRequestId": str,
-        "repositoryName": str,
-        "beforeCommitId": str,
-        "afterCommitId": str,
-        "content": str,
-    },
-)
-_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
-    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
-    {
-        "location": LocationTypeDef,
-        "clientRequestToken": str,
-    },
-    total=False,
-)
-
-class PostCommentForPullRequestInputRequestTypeDef(
-    _RequiredPostCommentForPullRequestInputRequestTypeDef,
-    _OptionalPostCommentForPullRequestInputRequestTypeDef,
-):
-    pass
-
 PostCommentForPullRequestOutputTypeDef = TypedDict(
     "PostCommentForPullRequestOutputTypeDef",
     {
         "repositoryName": str,
         "pullRequestId": str,
         "beforeCommitId": str,
         "afterCommitId": str,
         "beforeBlobId": str,
         "afterBlobId": str,
-        "location": LocationTypeDef,
+        "location": LocationOutputTypeDef,
         "comment": CommentTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CommitTypeDef = TypedDict(
     "CommitTypeDef",
@@ -2354,43 +2339,76 @@
     },
 )
 
 GetRepositoryTriggersOutputTypeDef = TypedDict(
     "GetRepositoryTriggersOutputTypeDef",
     {
         "configurationId": str,
-        "triggers": List[RepositoryTriggerTypeDef],
+        "triggers": List[RepositoryTriggerOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PutRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "PutRepositoryTriggersInputRequestTypeDef",
+ListRepositoriesOutputTypeDef = TypedDict(
+    "ListRepositoriesOutputTypeDef",
     {
-        "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
+        "repositories": List[RepositoryNameIdPairTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TestRepositoryTriggersInputRequestTypeDef = TypedDict(
-    "TestRepositoryTriggersInputRequestTypeDef",
+_RequiredPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForComparedCommitInputRequestTypeDef",
     {
         "repositoryName": str,
-        "triggers": Sequence[RepositoryTriggerTypeDef],
+        "afterCommitId": str,
+        "content": str,
+    },
+)
+_OptionalPostCommentForComparedCommitInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForComparedCommitInputRequestTypeDef",
+    {
+        "beforeCommitId": str,
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
     },
+    total=False,
 )
 
-ListRepositoriesOutputTypeDef = TypedDict(
-    "ListRepositoriesOutputTypeDef",
+class PostCommentForComparedCommitInputRequestTypeDef(
+    _RequiredPostCommentForComparedCommitInputRequestTypeDef,
+    _OptionalPostCommentForComparedCommitInputRequestTypeDef,
+):
+    pass
+
+_RequiredPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_RequiredPostCommentForPullRequestInputRequestTypeDef",
     {
-        "repositories": List[RepositoryNameIdPairTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "pullRequestId": str,
+        "repositoryName": str,
+        "beforeCommitId": str,
+        "afterCommitId": str,
+        "content": str,
     },
 )
+_OptionalPostCommentForPullRequestInputRequestTypeDef = TypedDict(
+    "_OptionalPostCommentForPullRequestInputRequestTypeDef",
+    {
+        "location": LocationTypeDef,
+        "clientRequestToken": str,
+    },
+    total=False,
+)
+
+class PostCommentForPullRequestInputRequestTypeDef(
+    _RequiredPostCommentForPullRequestInputRequestTypeDef,
+    _OptionalPostCommentForPullRequestInputRequestTypeDef,
+):
+    pass
 
 MergeHunkTypeDef = TypedDict(
     "MergeHunkTypeDef",
     {
         "isConflict": bool,
         "source": MergeHunkDetailTypeDef,
         "destination": MergeHunkDetailTypeDef,
@@ -2438,14 +2456,30 @@
     },
     total=False,
 )
 
 class PutFileEntryTypeDef(_RequiredPutFileEntryTypeDef, _OptionalPutFileEntryTypeDef):
     pass
 
+PutRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "PutRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
+TestRepositoryTriggersInputRequestTypeDef = TypedDict(
+    "TestRepositoryTriggersInputRequestTypeDef",
+    {
+        "repositoryName": str,
+        "triggers": Sequence[RepositoryTriggerTypeDef],
+    },
+)
+
 ReactionForCommentTypeDef = TypedDict(
     "ReactionForCommentTypeDef",
     {
         "reaction": ReactionValueFormatsTypeDef,
         "reactionUsers": List[str],
         "reactionsFromDeletedUsersCount": int,
     },
```

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/PKG-INFO` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codecommit
-Version: 1.28.0
-Summary: Type annotations for boto3.CodeCommit 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.12
+Summary: Type annotations for boto3.CodeCommit 1.28.12 service generated with mypy-boto3-builder 7.15.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -33,29 +33,29 @@
 <a id="mypy-boto3-codecommit"></a>
 
 # mypy-boto3-codecommit
 
 [![PyPI - mypy-boto3-codecommit](https://img.shields.io/pypi/v/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codecommit.svg?color=blue)](https://pypi.org/project/mypy-boto3-codecommit)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-codecommit?color=blue)](https://pypistats.org/packages/mypy-boto3-codecommit)
+[![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codecommit)](https://pepy.tech/project/mypy-boto3-codecommit)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeCommit 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
+[boto3.CodeCommit 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#CodeCommit)
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
 [mypy-boto3-codecommit docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codecommit/).
 
 See how it helps to find and fix potential bugs:
 
@@ -379,15 +379,15 @@
     BatchGetCommitsErrorTypeDef,
     BatchGetCommitsInputRequestTypeDef,
     BatchGetRepositoriesInputRequestTypeDef,
     RepositoryMetadataTypeDef,
     BlobMetadataTypeDef,
     BranchInfoTypeDef,
     CommentTypeDef,
-    LocationTypeDef,
+    LocationOutputTypeDef,
     UserInfoTypeDef,
     FileModesTypeDef,
     FileSizesTypeDef,
     IsBinaryFileTypeDef,
     MergeOperationsTypeDef,
     ObjectTypesTypeDef,
     DeleteFileEntryTypeDef,
@@ -444,15 +444,15 @@
     GetMergeOptionsOutputTypeDef,
     GetPullRequestApprovalStatesInputRequestTypeDef,
     GetPullRequestInputRequestTypeDef,
     GetPullRequestOverrideStateInputRequestTypeDef,
     GetPullRequestOverrideStateOutputTypeDef,
     GetRepositoryInputRequestTypeDef,
     GetRepositoryTriggersInputRequestTypeDef,
-    RepositoryTriggerTypeDef,
+    RepositoryTriggerOutputTypeDef,
     ListApprovalRuleTemplatesInputRequestTypeDef,
     ListApprovalRuleTemplatesOutputTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef,
     ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef,
     ListBranchesInputListBranchesPaginateTypeDef,
     ListBranchesInputRequestTypeDef,
     ListBranchesOutputTypeDef,
@@ -462,14 +462,15 @@
     ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef,
     ListRepositoriesForApprovalRuleTemplateOutputTypeDef,
     ListRepositoriesInputListRepositoriesPaginateTypeDef,
     ListRepositoriesInputRequestTypeDef,
     RepositoryNameIdPairTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
+    LocationTypeDef,
     MergeBranchesByFastForwardInputRequestTypeDef,
     MergeBranchesByFastForwardOutputTypeDef,
     MergeBranchesBySquashOutputTypeDef,
     MergeBranchesByThreeWayOutputTypeDef,
     MergeHunkDetailTypeDef,
     MergeMetadataTypeDef,
     MergePullRequestByFastForwardInputRequestTypeDef,
@@ -479,14 +480,15 @@
     PullRequestCreatedEventMetadataTypeDef,
     PullRequestSourceReferenceUpdatedEventMetadataTypeDef,
     PullRequestStatusChangedEventMetadataTypeDef,
     PutCommentReactionInputRequestTypeDef,
     SourceFileSpecifierTypeDef,
     PutFileInputRequestTypeDef,
     PutFileOutputTypeDef,
+    RepositoryTriggerTypeDef,
     PutRepositoryTriggersOutputTypeDef,
     ReactionValueFormatsTypeDef,
     RepositoryTriggerExecutionFailureTypeDef,
     ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateApprovalRuleTemplateContentInputRequestTypeDef,
@@ -518,33 +520,33 @@
     GetBranchOutputTypeDef,
     DeleteCommentContentOutputTypeDef,
     GetCommentOutputTypeDef,
     PostCommentReplyOutputTypeDef,
     UpdateCommentOutputTypeDef,
     CommentsForComparedCommitTypeDef,
     CommentsForPullRequestTypeDef,
-    PostCommentForComparedCommitInputRequestTypeDef,
     PostCommentForComparedCommitOutputTypeDef,
-    PostCommentForPullRequestInputRequestTypeDef,
     PostCommentForPullRequestOutputTypeDef,
     CommitTypeDef,
     ConflictMetadataTypeDef,
     ConflictResolutionTypeDef,
     CreateCommitOutputTypeDef,
     CreatePullRequestInputRequestTypeDef,
     EvaluatePullRequestApprovalRulesOutputTypeDef,
     GetFolderOutputTypeDef,
     GetRepositoryTriggersOutputTypeDef,
-    PutRepositoryTriggersInputRequestTypeDef,
-    TestRepositoryTriggersInputRequestTypeDef,
     ListRepositoriesOutputTypeDef,
+    PostCommentForComparedCommitInputRequestTypeDef,
+    PostCommentForPullRequestInputRequestTypeDef,
     MergeHunkTypeDef,
     PullRequestMergedStateChangedEventMetadataTypeDef,
     PullRequestTargetTypeDef,
     PutFileEntryTypeDef,
+    PutRepositoryTriggersInputRequestTypeDef,
+    TestRepositoryTriggersInputRequestTypeDef,
     ReactionForCommentTypeDef,
     TestRepositoryTriggersOutputTypeDef,
     CreatePullRequestApprovalRuleOutputTypeDef,
     UpdatePullRequestApprovalRuleContentOutputTypeDef,
     GetDifferencesOutputTypeDef,
     GetCommentsForComparedCommitOutputTypeDef,
     GetCommentsForPullRequestOutputTypeDef,
```

### Comparing `mypy-boto3-codecommit-1.28.0/mypy_boto3_codecommit.egg-info/SOURCES.txt` & `mypy-boto3-codecommit-1.28.12/mypy_boto3_codecommit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codecommit-1.28.0/setup.py` & `mypy-boto3-codecommit-1.28.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codecommit",
-    version="1.28.0",
+    version="1.28.12",
     packages=["mypy_boto3_codecommit"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeCommit 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.CodeCommit 1.28.12 service generated with mypy-boto3-builder"
+        " 7.15.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

