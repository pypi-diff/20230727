# Comparing `tmp/pachyderm_sdk-2.7.0a5.tar.gz` & `tmp/pachyderm_sdk-2.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pachyderm_sdk-2.7.0a5.tar", max compression
+gzip compressed data, was "pachyderm_sdk-2.7.0rc1.tar", max compression
```

## Comparing `pachyderm_sdk-2.7.0a5.tar` & `pachyderm_sdk-2.7.0rc1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     2830 2023-07-11 20:49:13.653865 pachyderm_sdk-2.7.0a5/README.md
--rw-r--r--   0        0        0      357 2023-07-11 20:49:13.654306 pachyderm_sdk-2.7.0a5/pachyderm_sdk/__init__.py
--rw-r--r--   0        0        0      645 2023-07-11 20:49:13.654665 pachyderm_sdk-2.7.0a5/pachyderm_sdk/__main__.py
--rw-r--r--   0        0        0        8 2023-05-24 21:54:17.401075 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/.gitignore
--rw-r--r--   0        0        0        0 2023-07-07 17:16:28.113268 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/__init__.py
--rw-r--r--   0        0        0     2292 2023-07-07 17:16:28.113923 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/admin/__init__.py
--rw-r--r--   0        0        0      903 2023-07-11 20:49:13.654915 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/admin/extension.py
--rw-r--r--   0        0        0    45738 2023-07-07 17:19:41.391727 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/auth/__init__.py
--rw-r--r--   0        0        0    12532 2023-07-12 22:57:38.373119 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/debug/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-11 20:49:13.655053 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/debug/extension.py
--rw-r--r--   0        0        0    12463 2023-06-30 22:07:22.000000 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/enterprise/__init__.py
--rw-r--r--   0        0        0    19931 2023-07-07 17:19:41.392327 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/identity/__init__.py
--rw-r--r--   0        0        0    15874 2023-07-03 21:33:32.186628 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/license/__init__.py
--rw-r--r--   0        0        0    83954 2023-07-12 22:57:38.374254 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/__init__.py
--rw-r--r--   0        0        0     4127 2023-07-12 16:48:09.915620 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/_additions.py
--rw-r--r--   0        0        0    23950 2023-07-12 16:48:09.916294 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/extension.py
--rw-r--r--   0        0        0     4018 2023-05-30 21:36:31.919242 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/file.py
--rw-r--r--   0        0        0    86311 2023-07-07 17:19:41.393463 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pps/__init__.py
--rw-r--r--   0        0        0     4153 2023-07-11 20:49:13.655977 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pps/extension.py
--rw-r--r--   0        0        0     1113 2023-07-07 17:15:46.279138 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/taskapi/__init__.py
--rw-r--r--   0        0        0    10917 2023-07-03 21:33:32.188398 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/transaction/__init__.py
--rw-r--r--   0        0        0     3265 2023-07-11 20:49:13.656272 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/transaction/extension.py
--rw-r--r--   0        0        0     2041 2023-06-30 22:07:22.000000 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/version/__init__.py
--rw-r--r--   0        0        0     4638 2023-07-07 17:16:28.116245 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/worker/__init__.py
--rw-r--r--   0        0        0     1950 2023-07-12 16:48:09.916829 pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/worker/extension.py
--rw-r--r--   0        0        0    11683 2023-07-12 22:57:38.375640 pachyderm_sdk-2.7.0a5/pachyderm_sdk/client.py
--rw-r--r--   0        0        0     3521 2023-07-11 20:49:13.657192 pachyderm_sdk-2.7.0a5/pachyderm_sdk/config.py
--rw-r--r--   0        0        0      953 2023-07-11 20:48:30.951263 pachyderm_sdk-2.7.0a5/pachyderm_sdk/constants.py
--rw-r--r--   0        0        0     1485 2023-07-11 20:48:30.951823 pachyderm_sdk-2.7.0a5/pachyderm_sdk/datum_batching.py
--rw-r--r--   0        0        0     1613 2023-07-11 20:49:13.657513 pachyderm_sdk-2.7.0a5/pachyderm_sdk/errors.py
--rw-r--r--   0        0        0     1754 2023-07-11 20:49:13.657777 pachyderm_sdk-2.7.0a5/pachyderm_sdk/interceptor.py
--rw-r--r--   0        0        0     1479 2023-07-12 22:59:05.388769 pachyderm_sdk-2.7.0a5/pyproject.toml
--rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 pachyderm_sdk-2.7.0a5/PKG-INFO
+-rw-r--r--   0        0        0     2830 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/README.md
+-rw-r--r--   0        0        0      357 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/__init__.py
+-rw-r--r--   0        0        0      645 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/__main__.py
+-rw-r--r--   0        0        0        8 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/__init__.py
+-rw-r--r--   0        0        0     2731 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/__init__.py
+-rw-r--r--   0        0        0     1036 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/extension.py
+-rw-r--r--   0        0        0    45738 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/auth/__init__.py
+-rw-r--r--   0        0        0    12532 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/__init__.py
+-rw-r--r--   0        0        0     1572 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/extension.py
+-rw-r--r--   0        0        0    12463 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/enterprise/__init__.py
+-rw-r--r--   0        0        0    19931 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/identity/__init__.py
+-rw-r--r--   0        0        0    15874 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/license/__init__.py
+-rw-r--r--   0        0        0    83954 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/__init__.py
+-rw-r--r--   0        0        0     5398 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/_additions.py
+-rw-r--r--   0        0        0    25802 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/extension.py
+-rw-r--r--   0        0        0     4018 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/file.py
+-rw-r--r--   0        0        0    86768 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/__init__.py
+-rw-r--r--   0        0        0      677 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/_additions.py
+-rw-r--r--   0        0        0     4222 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/extension.py
+-rw-r--r--   0        0        0     1113 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/taskapi/__init__.py
+-rw-r--r--   0        0        0    10917 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/__init__.py
+-rw-r--r--   0        0        0     3614 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/extension.py
+-rw-r--r--   0        0        0     2041 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/version/__init__.py
+-rw-r--r--   0        0        0     4638 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/__init__.py
+-rw-r--r--   0        0        0     1872 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/extension.py
+-rw-r--r--   0        0        0    12044 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/client.py
+-rw-r--r--   0        0        0     4077 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/config.py
+-rw-r--r--   0        0        0      994 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/constants.py
+-rw-r--r--   0        0        0     1570 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/datum_batching.py
+-rw-r--r--   0        0        0     1613 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/errors.py
+-rw-r--r--   0        0        0     1858 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/interceptor.py
+-rw-r--r--   0        0        0     1503 2023-07-27 16:44:39.426643 pachyderm_sdk-2.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 pachyderm_sdk-2.7.0rc1/PKG-INFO
```

### Comparing `pachyderm_sdk-2.7.0a5/README.md` & `pachyderm_sdk-2.7.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/__main__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/admin/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,18 @@
     Optional,
 )
 
 import betterproto
 import betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 import grpc
 
-from .. import version as _version__
+from .. import (
+    pfs as _pfs__,
+    version as _version__,
+)
 
 
 if TYPE_CHECKING:
     import grpc
 
 
 @dataclass(eq=False, repr=False)
@@ -30,37 +33,50 @@
     proxy_host: str = betterproto.string_field(5)
     proxy_tls: bool = betterproto.bool_field(6)
 
 
 @dataclass(eq=False, repr=False)
 class InspectClusterRequest(betterproto.Message):
     client_version: "_version__.Version" = betterproto.message_field(1)
+    current_project: "_pfs__.Project" = betterproto.message_field(2)
+    """
+    If CurrentProject is set, then InspectCluster will return an error if the
+    project does not exist.
+    """
 
 
 class ApiStub:
     def __init__(self, channel: "grpc.Channel"):
         self.__rpc_inspect_cluster = channel.unary_unary(
             "/admin_v2.API/InspectCluster",
             request_serializer=InspectClusterRequest.SerializeToString,
             response_deserializer=ClusterInfo.FromString,
         )
 
     def inspect_cluster(
-        self, *, client_version: "_version__.Version" = None
+        self,
+        *,
+        client_version: "_version__.Version" = None,
+        current_project: "_pfs__.Project" = None
     ) -> "ClusterInfo":
         request = InspectClusterRequest()
         if client_version is not None:
             request.client_version = client_version
+        if current_project is not None:
+            request.current_project = current_project
 
         return self.__rpc_inspect_cluster(request)
 
 
 class ApiBase:
     def inspect_cluster(
-        self, client_version: "_version__.Version", context: "grpc.ServicerContext"
+        self,
+        client_version: "_version__.Version",
+        current_project: "_pfs__.Project",
+        context: "grpc.ServicerContext",
     ) -> "ClusterInfo":
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     __proto_path__ = "admin_v2.API"
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/admin/extension.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/extension.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+"""Handwritten classes/methods that augment the existing Admin API."""
 import pachyderm_sdk
 
 from . import ApiStub as _GeneratedApiStub
 from ..version import Version
 from . import ClusterInfo
 
 
 class ApiStub(_GeneratedApiStub):
     # noinspection PyMethodOverriding
     def inspect_cluster(self) -> "ClusterInfo":
+        """Inspect the cluster and check version mismatch."""
         try:
             version = _extract_version(pachyderm_sdk.__version__)
         except ValueError:
             return super().inspect_cluster()
         return super().inspect_cluster(client_version=version)
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/auth/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/debug/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/debug/extension.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Handwritten classes/methods that augment the existing Debug API."""
 from typing import Iterator, List, Optional, TYPE_CHECKING
 
 from . import DebugStub
 from . import DumpChunk, System
 
 if TYPE_CHECKING:
     from ..pps import Pipeline
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/enterprise/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/enterprise/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/identity/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/license/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/license/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/_additions.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/_additions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,65 @@
+""" This file patches methods onto the PFS Noun objects.
+
+This is done, as opposed to subclassing them, for these methods
+  to automatically be accessible on any objects included in the
+  response from the API.
+
+Note: These are internally patched and this file should
+  not be imported directly by users.
+"""
 import re
 
 from . import Branch, Commit, File, Project, Repo
 
 branch_re = re.compile(r"^[a-zA-Z\d_-]+$")
 uuid_re = re.compile(r"^[\da-f]{12}4[\da-f]{19}$")
 
 
 def _Repo_from_uri(uri: str) -> Repo:
     """
     Parses the following format:
-        [project/]<repo>
+        [project/]repo
 
     If no project is specified it defaults to "default".
     """
     if "/" in uri:
         project, repo = uri.split("/", 1)
     else:
         project, repo = "default", uri
     return Repo(name=repo, type="user", project=Project(name=project))
 
 
 def _Repo_as_uri(self: "Repo") -> str:
+    """Returns the URI for the Repo object in the following format:
+      project/repo
+
+    If no project is specified it defaults to "default"
+    """
     project = "default"
     if self.project and self.project.name:
         project = self.project.name
     return f"{project}/{self.name}"
 
 
+def _Repo___post_init__(self: "Repo") -> None:
+    if not self.project or not self.project.name:
+        self.project = Project(name="default")
+    super(self.__class__, self).__post_init__()
+
+
 Repo.from_uri = _Repo_from_uri
 Repo.as_uri = Repo.__str__ = _Repo_as_uri
+Repo.__post_init__ = _Repo___post_init__
 
 
 def _Branch_from_uri(uri: str) -> Branch:
     """
     Parses the following format:
-        [project/]<repo>@branch
+        [project/]repo@branch
 
     If no project is specified it defaults to "default".
 
     Raises:
         ValueError: If no branch is specified.
     """
     if "@" not in uri:
@@ -49,36 +70,40 @@
     project_repo, branch = uri.split("@", 1)
     if not branch_re.match(branch):
         raise ValueError(f"Invalid branch name: {branch}")
     return Branch(name=branch, repo=Repo.from_uri(project_repo))
 
 
 def _Branch_as_uri(self: "Branch") -> str:
+    """Returns the URI for the Branch object in the following format:
+      project/repo@branch
+
+    If no project is specified it defaults to "default"
+    """
     return f"{self.repo.as_uri()}@{self.name}"
 
 
 Branch.from_uri = _Branch_from_uri
 Branch.as_uri = Branch.__str__ = _Branch_as_uri
 
 
 def _Commit_from_uri(uri: str) -> Commit:
     """
     Parses the following format:
-        [project/]<repo>@<branch-or-commit>
-    where @<branch-or-commit> can take the form:
+        [project/]repo@branch-or-commit
+    where @branch-or-commit can take the form:
         @branch
         @branch=commit
         @commit
-    Additionally @<branch-or-commit> can be augmented with caret notation:
+    Additionally @branch-or-commit can be augmented with caret notation:
         @branch^2
 
     All unspecified components will default to None, except for an unspecified
       project which defaults to "default".
     """
-    # TODO: Can we do more error checking here?
     if "@" not in uri:
         raise ValueError(
             "Could not parse branch/commit. URI must have the form: "
             "[project/]<repo>@(branch|branch=commit|commit)"
         )
     project_repo, branch_or_commit = uri.split("@", 1)
     repo = Repo.from_uri(project_repo)
@@ -94,14 +119,21 @@
         branch=Branch(name=branch, repo=repo),
         id=commit,
         repo=repo,
     )
 
 
 def _Commit_as_uri(self: "Commit") -> str:
+    """Returns the URI for the Commit object in one of the following formats:
+        project/repo@branch
+        project/repo@branch=commit
+        project/repo@commit
+
+    If no project is specified it defaults to "default"
+    """
     project_repo = self.branch.repo.as_uri()
     if self.branch.name and self.id:
         return f"{project_repo}@{self.branch.name}={self.id}"
     elif self.branch.name:
         return f"{project_repo}@{self.branch.name}"
     else:
         return f"{project_repo}@{self.id}"
@@ -110,20 +142,20 @@
 Commit.from_uri = _Commit_from_uri
 Commit.as_uri = Commit.__str__ = _Commit_as_uri
 
 
 def _File_from_uri(uri: str) -> File:
     """
     Parses the following format:
-        [project/]<repo>@<branch-or-commit>[:<path/in/pfs>]
-    where @<branch-or-commit> can take the form:
+        [project/]repo@branch-or-commit[:path/in/pfs]
+    where @branch-or-commit can take the form:
         @branch
         @branch=commit
         @commit
-    Additionally @<branch-or-commit> can be augmented with caret notation:
+    Additionally @branch-or-commit can be augmented with caret notation:
         @branch^2
 
     All unspecified components will default to None, except for an unspecified
       project which defaults to "default".
     """
     if ":" in uri:
         project_repo_branch, path = uri.split(":", 1)
@@ -133,12 +165,19 @@
     return File(
         commit=Commit.from_uri(project_repo_branch),
         path=path,
     )
 
 
 def _File_as_uri(self: "File") -> str:
+    """Returns the URI for the File object in one of the following formats:
+        project/repo@branch:/path
+        project/repo@branch=commit:/path
+        project/repo@commit:/path
+
+    If no project is specified it defaults to "default"
+    """
     return f"{self.commit.as_uri()}:{self.path}"
 
 
 File.from_uri = _File_from_uri
 File.as_uri = File.__str__ = _File_as_uri
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/extension.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Handwritten classes/methods that augment the existing PFS API."""
 import io
 import os
 from contextlib import contextmanager
 from dataclasses import fields
 from functools import wraps
 from pathlib import Path
 from typing import Callable, ContextManager, Iterable, List, Union, TYPE_CHECKING
@@ -72,27 +73,21 @@
         super().__init__(
             **{field.name: getattr(commit, field.name) for field in fields(commit)}
         )
 
     def wait(self) -> "CommitInfo":
         """Waits until the commit is finished being created.
 
-        This method is intended to be called on a closed commit, but provided
-        with this class to be used following the commit context.
-        (See example in class docstring)
+        See OpenCommit docstring for an example.
         """
         return self._stub.wait_commit(self)
 
-    def wait_set(self) -> List["CommitInfo"]:  # TODO: Better name?
+    def wait_all(self) -> List["CommitInfo"]:
         """Similar to Commit.wait but streams back the pfs.CommitInfo
         from all the downstream jobs that were initiated by this commit.
-
-        This method is intended to be called on a closed commit, but provided
-        with this class to be used following the commit context.
-        (See example in class docstring)
         """
         return self._stub.wait_commit_set(CommitSet(id=self._commit.id))
 
 
 class OpenCommit(ClosedCommit):
     """An OpenCommit is an extension of the pfs.Commit message with some
     helpful methods that provide a more intuitive UX when writing to a commit.
@@ -122,14 +117,38 @@
         self._stub = stub
         super().__init__(commit, stub)
 
     def _close(self):
         """Transform an OpenCommit into a ClosedCommit."""
         self.__class__ = ClosedCommit
 
+    def put_files(self, *, source: Union[Path, str], path: str) -> None:
+        """Recursively insert the contents of source into the open commit under path,
+        matching the directory structure of source.
+
+        This is roughly equivalent to ``pachctl put file -r``
+
+        Parameters
+        ----------
+        source : Union[Path, str]
+            The directory to recursively insert content from.
+        path : str
+            The destination path in PFS.
+
+        Examples
+        --------
+        >>> from pachyderm_sdk import Client
+        >>> from pachyderm_sdk.api import pfs
+        >>> client: Client
+        >>> branch = pfs.Branch.from_uri("images@master")
+        >>> with client.pfs.commit(branch=branch) as commit:
+        >>>     commit.put_files(source="path/to/local/files", path="/")
+        """
+        self._stub.put_files(commit=self._commit, source=source, path=path)
+
     def put_file_from_bytes(self, path: str, data: bytes, append: bool = False) -> "File":
         """Uploads a PFS file from a bytestring.
 
         Parameters
         ----------
         path : str
             The path in the repo the data will be written to.
@@ -139,14 +158,19 @@
             If true, appends the data to the file specified at `path`, if
             they already exist. Otherwise, overwrites them.
 
         Raises
         ------
         ValueError: If the commit is closed.
 
+        Returns
+        -------
+        A pfs.File object that that points to the uploaded file.
+        NOTE: The commit must be closed before you can read this file.
+
         Examples
         --------
         >>> from pachyderm_sdk import Client
         >>> from pachyderm_sdk.api import pfs
         >>> client: Client
         >>> with client.pfs.commit(branch=pfs.Branch.from_uri("images@master")) as commit:
         >>>     commit.put_file_from_bytes(path="/file.txt", data=b"SOME BYTES")
@@ -173,14 +197,19 @@
             If true, allows for recursive scraping on some types URLs, for
             example on s3:// URLs
 
         Raises
         ------
         ValueError: If the commit is closed.
 
+        Returns
+        -------
+        A pfs.File object that that points to the uploaded file.
+        NOTE: The commit must be closed before you can read this file.
+
         Examples
         --------
         >>> from pachyderm_sdk import Client
         >>> from pachyderm_sdk.api import pfs
         >>> client: Client
         >>> with client.pfs.commit(branch=pfs.Branch.from_uri("images@master")) as commit:
         >>>     commit.put_file_from_url(
@@ -205,27 +234,32 @@
             If true, appends the data to the file specified at `path`, if
             they already exist. Otherwise, overwrites them.
 
         Raises
         ------
         ValueError: If the commit is closed.
 
+        Returns
+        -------
+        A pfs.File object that that points to the uploaded file.
+        NOTE: The commit must be closed before you can read this file.
+
         Examples
         --------
         >>> from pachyderm_sdk import Client
         >>> from pachyderm_sdk.api import pfs
         >>> client: Client
         >>> with client.pfs.commit(branch=pfs.Branch.from_uri("images@master")) as commit:
         >>>     with open("local_file.dat", "rb") as source:
         >>>         commit.put_file_from_file(path="/index.html", file=source)
         """
         self._stub.put_file_from_file(commit=self, path=path, file=file, append=append)
         return File(commit=self._commit, path=path)
 
-    def copy_file(self, *, src: "File", dst: str, append: bool = True) -> "File":
+    def copy_file(self, *, src: "File", dst: str, append: bool = False) -> "File":
         """Copies a file within PFS
 
         Parameters
         ----------
         src : pfs.File
             This file to be copied.
         dst : str
@@ -234,38 +268,47 @@
             If true, appends the contents of src to dst if it exists.
             Otherwise, overwrites the file.
 
         Raises
         ------
         ValueError: If the commit is closed.
 
+        Returns
+        -------
+        A pfs.File object that that points to the new file.
+        NOTE: The commit must be closed before you can read this file.
+
         Examples
         --------
         >>> from pachyderm_sdk import Client
         >>> from pachyderm_sdk.api import pfs
         >>> client: Client
         >>> source = pfs.File.from_uri("images@master:/file.dat")
         >>> with client.pfs.commit(branch=pfs.Branch.from_uri("images@master")) as commit:
         >>>     commit.copy_file(src=source, dst="/copy.dat")
         """
         self._stub.copy_file(commit=self, src=src, dst=dst, append=append)
         return File(commit=self._commit, path=dst)
 
-    def delete_file(self, *, path: str) -> "File":  # TODO: Should we return anything?
+    def delete_file(self, *, path: str) -> "File":
         """Copies a file within PFS
 
         Parameters
         ----------
         path : str
             The path of the file to be deleted.
 
         Raises
         ------
         ValueError: If the commit is closed.
 
+        Returns
+        -------
+        A pfs.File object that that points to the deleted file.
+
         Examples
         --------
         >>> from pachyderm_sdk import Client
         >>> from pachyderm_sdk.api import pfs
         >>> client: Client
         >>> with client.pfs.commit(branch=pfs.Branch.from_uri("images@master")) as commit:
         >>>     commit.delete_file(path="/file.dat")
@@ -298,26 +341,25 @@
     def commit(
         self, *, parent: "Commit" = None, description: str = "", branch: "Branch" = None
     ) -> ContextManager["OpenCommit"]:
         """A context manager for running operations within a commit.
 
         When inside this context, the returned object is an OpenCommit which accepts
           write-operations. Upon exiting the context, the commit is closed and the
-          OpenCommit becomes a ClosedCommit, no longer allowing write-operations
-          to the commit.
+          OpenCommit becomes a ClosedCommit and no longer allowing write-operations.
 
         Parameters
         ----------
-        parent : pfs.Commit
+        parent : pfs.Commit, optional
             The parent commit of the new commit. parent may be empty in which case
             the commit that Branch points to will be used as the parent.
             If the branch does not exist, the commit will have no parent.
         description : str, optional
             A description of the commit.
-        branch : pfs.Branch
+        branch : pfs.Branch, optional
             The branch where the commit is created.
 
         Yields
         -------
         pfs.Commit
             A protobuf object that represents a commit.
 
@@ -351,14 +393,18 @@
     @transaction_incompatible
     def put_files(self, *, commit: "Commit", source: Union[Path, str], path: str) -> None:
         """Recursively insert the contents of source into the open commit under path,
         matching the directory structure of source.
 
         This is roughly equivalent to ``pachctl put file -r``
 
+        Note: This method opens multiple gRPC streams and this appears to break in
+          some REPL environment (such as those based in IDEs). If you encounter this
+          problem, please try a different REPL environment or run as a script.
+
         Parameters
         ----------
         commit : pfs.Commit
             The open commit to add files to.
         source : Union[Path, str]
             The directory to recursively insert content from.
         path : str
@@ -490,32 +536,42 @@
         >>> client: Client
         >>> with client.pfs.commit(branch=pfs.Branch.from_uri("images@master")) as c:
         >>>     with open("local_file.dat", "rb") as source:
         >>>         client.pfs.put_file_from_file(
         >>>             commit=c, path="/index.html", file=source
         >>>         )
         """
+        check = file.read(BUFFER_SIZE)
+        if len(check) > 0:
+            if not isinstance(check, bytes):
+                raise TypeError("File must output bytes")
+
+        def file_iterator():
+            if not check:
+                return
+            yield check
+            while True:
+                data = file.read(BUFFER_SIZE)
+                if len(data) == 0:
+                    return
+                yield data
 
-        # TODO: Can we verify that the file is outputting bytes?
         def operations() -> Iterable[ModifyFileRequest]:
             yield ModifyFileRequest(set_commit=commit)
             if not append:
                 yield ModifyFileRequest(delete_file=DeleteFile(path=path))
             yield ModifyFileRequest(add_file=AddFile(path=path, raw=b""))
-            while True:
-                data = file.read(BUFFER_SIZE)
-                if len(data) == 0:
-                    return
+            for data in file_iterator():
                 yield ModifyFileRequest(add_file=AddFile(path=path, raw=data))
 
         return self.modify_file(operations())
 
     @transaction_incompatible
     def copy_file(
-        self, *, commit: "Commit", src: "File", dst: str, append: bool = True
+        self, *, commit: "Commit", src: "File", dst: str, append: bool = False
     ) -> Empty:
         """Copies a file within PFS
 
         Parameters
         ----------
         commit : pfs.Commit
             An open commit to modify.
@@ -683,15 +739,15 @@
             return True
         except grpc.RpcError as err:
             err: grpc.Call
             if err.code() == grpc.StatusCode.NOT_FOUND:
                 return False
             raise err
 
-    def pfs_file(self, file: "File") -> "PFSFile":  # TODO: Naming?
+    def pfs_file(self, file: "File") -> "PFSFile":
         """Wraps the response stream of a client.pfs.get_file() call with a
         PFSFile object. This wrapper class allows you to interact with the
         file stream as a normal file object.
 
         Parameters
         ----------
         file : pfs.File
@@ -706,15 +762,15 @@
         >>> with client.pfs.pfs_file(file=source) as pfs_file:
         >>>     for line in pfs_file:
         >>>         print(line)
         """
         stream = self.get_file(file=file)
         return PFSFile(stream)
 
-    def pfs_tar_file(self, file: "File") -> "PFSTarFile":  # TODO: Naming?
+    def pfs_tar_file(self, file: "File") -> "PFSTarFile":
         """Wraps the response stream of a client.pfs.get_tar_file() call with a
         PFSTarFile object. This wrapper class allows you to interact with the
         file stream as a standard tarfile.TarFile object.
 
         Parameters
         ----------
         file : pfs.File
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pfs/file.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/file.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pps/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,19 @@
     )
     sql_database: "_pfs__.SqlDatabaseEgress" = betterproto.message_field(
         3, group="target"
     )
 
 
 @dataclass(eq=False, repr=False)
+class Determined(betterproto.Message):
+    workspaces: List[str] = betterproto.string_field(1)
+
+
+@dataclass(eq=False, repr=False)
 class Job(betterproto.Message):
     pipeline: "Pipeline" = betterproto.message_field(1)
     id: str = betterproto.string_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class Metadata(betterproto.Message):
@@ -442,14 +447,15 @@
 
     state: "JobState" = betterproto.enum_field(11)
     reason: str = betterproto.string_field(12)
     created: datetime = betterproto.message_field(13)
     started: datetime = betterproto.message_field(14)
     finished: datetime = betterproto.message_field(15)
     details: "JobInfoDetails" = betterproto.message_field(16)
+    auth_token: str = betterproto.string_field(17)
 
 
 @dataclass(eq=False, repr=False)
 class JobInfoDetails(betterproto.Message):
     transform: "Transform" = betterproto.message_field(1)
     parallelism_spec: "ParallelismSpec" = betterproto.message_field(2)
     egress: "Egress" = betterproto.message_field(3)
@@ -588,14 +594,15 @@
     metadata: "Metadata" = betterproto.message_field(29)
     reprocess_spec: str = betterproto.string_field(30)
     unclaimed_tasks: int = betterproto.int64_field(31)
     worker_rc: str = betterproto.string_field(32)
     autoscaling: bool = betterproto.bool_field(33)
     tolerations: List["Toleration"] = betterproto.message_field(34)
     sidecar_resource_requests: "ResourceSpec" = betterproto.message_field(35)
+    determined: "Determined" = betterproto.message_field(36)
 
 
 @dataclass(eq=False, repr=False)
 class PipelineInfos(betterproto.Message):
     pipeline_info: List["PipelineInfo"] = betterproto.message_field(1)
 
 
@@ -922,14 +929,15 @@
     metadata: "Metadata" = betterproto.message_field(28)
     reprocess_spec: str = betterproto.string_field(29)
     autoscaling: bool = betterproto.bool_field(30)
     tolerations: List["Toleration"] = betterproto.message_field(34)
     sidecar_resource_requests: "ResourceSpec" = betterproto.message_field(35)
     details_json: str = betterproto.string_field(36)
     dry_run: bool = betterproto.bool_field(37)
+    determined: "Determined" = betterproto.message_field(38)
 
 
 @dataclass(eq=False, repr=False)
 class CreatePipelineResponse(betterproto.Message):
     details_json: str = betterproto.string_field(1)
 
 
@@ -1506,15 +1514,16 @@
         spec_commit: "_pfs__.Commit" = None,
         metadata: "Metadata" = None,
         reprocess_spec: str = "",
         autoscaling: bool = False,
         tolerations: Optional[List["Toleration"]] = None,
         sidecar_resource_requests: "ResourceSpec" = None,
         details_json: str = "",
-        dry_run: bool = False
+        dry_run: bool = False,
+        determined: "Determined" = None
     ) -> "betterproto_lib_google_protobuf.Empty":
         tolerations = tolerations or []
 
         request = CreatePipelineRequest()
         if pipeline is not None:
             request.pipeline = pipeline
         if tf_job is not None:
@@ -1562,14 +1571,16 @@
         request.autoscaling = autoscaling
         if tolerations is not None:
             request.tolerations = tolerations
         if sidecar_resource_requests is not None:
             request.sidecar_resource_requests = sidecar_resource_requests
         request.details_json = details_json
         request.dry_run = dry_run
+        if determined is not None:
+            request.determined = determined
 
         return self.__rpc_create_pipeline(request)
 
     def inspect_pipeline(
         self, *, pipeline: "Pipeline" = None, details: bool = False
     ) -> "PipelineInfo":
         request = InspectPipelineRequest()
@@ -1985,14 +1996,15 @@
         metadata: "Metadata",
         reprocess_spec: str,
         autoscaling: bool,
         tolerations: Optional[List["Toleration"]],
         sidecar_resource_requests: "ResourceSpec",
         details_json: str,
         dry_run: bool,
+        determined: "Determined",
         context: "grpc.ServicerContext",
     ) -> "betterproto_lib_google_protobuf.Empty":
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
     def inspect_pipeline(
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/pps/extension.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Handwritten classes/methods that augment the existing PPS API."""
 import base64
 import json
 from typing import Dict
 
 import grpc
 from betterproto.lib.google.protobuf import Empty
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/taskapi/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/taskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/transaction/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/transaction/extension.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Handwritten classes/methods that augment the existing Transaction API."""
 from contextlib import contextmanager
 from typing import Callable, ContextManager
 
 import grpc
 
 from . import ApiStub as _GeneratedApiStub
 from . import (
@@ -19,21 +20,24 @@
         set_transaction_id: Callable[[str], None],
     ):
         self._get_transaction_id = get_transaction_id
         self._set_transaction_id = set_transaction_id
         super().__init__(channel=channel)
 
     def start_transaction(self) -> "Transaction":
-        # TODO: Should we do this?
+        """Starts a transaction and sets the transaction ID within the client.
+        This will make all subsequent resource operations performed by the client
+        occur within the returned transaction, until the transaction is finished.
+        """
         response = super().start_transaction()
         self._set_transaction_id(response.id)
         return response
 
     def finish_transaction(self, *, transaction: "Transaction" = None) -> "TransactionInfo":
-        # TODO: Should we do this?
+        """Finishes a transaction and removes the transaction ID within the client."""
         response = super().finish_transaction(transaction=transaction)
         self._set_transaction_id("")
         return response
 
     @contextmanager
     def transaction(self) -> ContextManager[Transaction]:
         """A context manager for running operations within a transaction. When
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/version/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/worker/__init__.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/api/worker/extension.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/extension.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,9 +45,8 @@
         load_dotenv(DOTENV_PATH_WORKER, override=True)
 
         self.__error = None
         try:
             yield
         except Exception as error:
             self.__error = repr(error)
-            # TODO: Probably want better logging here than a print statement.
             print(f"{self.__error}\nReporting above error to worker.")
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/client.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The Client used to interact with a Pachyderm instance."""
 import contextlib
 import os
 from pathlib import Path
 from typing import Optional, Union
 from urllib.parse import urlparse
 
 import grpc
@@ -33,33 +34,38 @@
 from .errors import AuthServiceNotActivated, BadClusterDeploymentID
 from .interceptor import MetadataClientInterceptor, MetadataType
 
 __all__ = ("Client",)
 
 
 class Client:
-    """The :class:`.Client` class that users will primarily interact with.
-    Initialize an instance with ``python_pachyderm.Client()``.
+    """The Client used to interact with a Pachyderm instance.
 
-    To see documentation on the methods :class:`.Client` can call, refer to the
-    `mixins` module.
+    Examples
+    --------
+    Connect to a pachyderm instance using your local config file:
+    >>> from pachyderm_sdk import Client
+    >>> client = Client.from_config()
+
+    Connect to a pachyderm instance using a URL/address:
+    >>> from pachyderm_sdk import Client
+    >>> client = Client.from_pachd_address("test.work.com:30080")
     """
 
     def __init__(
         self,
         host: str = DEFAULT_HOST,
         port: int = DEFAULT_PORT,
         auth_token: Optional[str] = None,
         root_certs: Optional[bytes] = None,
         transaction_id: str = None,
         tls: bool = False,
     ):
         """
-        Creates a Pachyderm client. If both files don't exist, a client
-        with default settings is created.
+        Creates a Pachyderm client.
 
         Parameters
         ----------
         host : str, optional
             The pachd host. Default is 'localhost', which is used with
             ``pachctl port-forward``.
         port : int, optional
@@ -250,14 +256,15 @@
                     expected_deployment_id, cluster_info.deployment_id
                 )
 
         return client
 
     @property
     def auth_token(self):
+        """The authentication token. Used if authentication is enabled on the cluster."""
         return self._auth_token
 
     @auth_token.setter
     def auth_token(self, value):
         self._auth_token = value
         self._metadata = self._build_metadata()
         self._channel = _apply_metadata_interceptor(
@@ -266,14 +273,15 @@
             ),
             metadata=self._metadata,
         )
         self._init_api()
 
     @property
     def transaction_id(self):
+        """The ID of the transaction to run operations on."""
         return self._transaction_id
 
     @transaction_id.setter
     def transaction_id(self, value):
         self._transaction_id = value
         self._metadata = self._build_metadata()
         self._channel = _apply_metadata_interceptor(
@@ -310,14 +318,15 @@
         if self._auth_token is not None:
             metadata.append(("authn-token", self._auth_token))
         if self._transaction_id is not None:
             metadata.append(("pach-transaction", self._transaction_id))
         return metadata
 
     def get_version(self) -> Version:
+        """Requests version information from the pachd cluster."""
         return self._version_api.get_version()
 
 
 def _apply_metadata_interceptor(
     channel: grpc.Channel, metadata: MetadataType
 ) -> grpc.Channel:
     metadata_interceptor = MetadataClientInterceptor(metadata)
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/config.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,61 @@
+"""Functionality for parsing Pachyderm config files."""
 import json
 import os
 from base64 import b64decode
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 from .errors import ConfigError
 
 
 class ConfigFile:
+    """A parsed Pachyderm config file."""
     def __init__(self, config_file: Union[Path, str]):
+        """
+        Parameters
+        ----------
+        config_file : str
+            The path to the config file.
+        """
         config_file = Path(os.path.expanduser(config_file)).resolve()
         self._config_file_data = json.loads(config_file.read_bytes())
 
     @property
     def user_id(self) -> str:
+        """The user ID of the config file."""
         return self._config_file_data["user_id"]
 
     @property
     def active_context(self) -> "Context":
+        """The currently-active context."""
         active_context_name = self._config_file_data["v2"]["active_context"]
         contexts = self._config_file_data["v2"]["contexts"]
         if active_context_name not in contexts:
             raise ConfigError(f"active context not found: {active_context_name}")
         return Context(**contexts[active_context_name])
 
     @property
     def active_enterprise_context(self) -> "Context":
+        """The currently-active context that is enterprise-enabled."""
         context_name = self._config_file_data["v2"].get("active_enterprise_context")
         if context_name is None:
             raise ConfigError("active enterprise context is not specified")
         contexts = self._config_file_data["v2"]["contexts"]
         if context_name not in contexts:
             raise ConfigError(f"active enterprise context not found: {context_name}")
         return Context(**contexts[context_name])
 
 
 @dataclass
 class Context:
+    """A context contains all the information needed to connect to a pachyderm
+    instance. Not all fields need to be present for the context to be valid."""
+
     source: Optional[int] = None
     """An integer that specifies where the config came from. 
     This parameter is for internal use only and should not be modified."""
 
     pachd_address: Optional[str] = None
     """A host:port specification for connecting to pachd."""
 
@@ -76,15 +90,15 @@
     """Whether the context represents an enterprise server."""
 
     port_forwarders: Dict[str, int] = None
     """A mapping of service name -> local port."""
 
     @property
     def active_pachd_address(self) -> str:
-        """This pachd factors in port-forwarding."""
+        """This pachd address factors in port-forwarding."""
         if self.pachd_address is None:
             port = 30650
             if self.port_forwarders:
                 port = self.port_forwarders.get("pachd", 30650)
             return f"grpc://localhost:{port}"
         return self.pachd_address
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/constants.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 OIDC_TOKEN_ENV = "PACH_PYTHON_OIDC_TOKEN"
 ENTERPRISE_CODE_ENV = "PACH_PYTHON_ENTERPRISE_CODE"
 PACH_CONFIG_ENV = "PACH_CONFIG"
 PACHD_SERVICE_HOST_ENV = "PACHD_PEER_SERVICE_HOST"
 PACHD_SERVICE_PORT_ENV = "PACHD_PEER_SERVICE_PORT"
 WORKER_PORT_ENV = "PPS_WORKER_GRPC_PORT"
 
+# `~` used below to make docs look better.
+CONFIG_PATH_LOCAL = Path("~").joinpath(".pachyderm", "config.json")
 CONFIG_PATH_SPOUT = Path("/").joinpath("pachctl", "config.json")
-CONFIG_PATH_LOCAL = Path.home().joinpath(".pachyderm", "config.json")
 DOTENV_PATH_WORKER = Path("/pfs/.env")
 
 MAX_RECEIVE_MESSAGE_SIZE = 20 * 1024**2  # 20MB
 PRIMARY_USER_AGENT = "pachyderm-sdk"
 SECONDARY_USER_AGENT = f"v{__version__}" if __version__ else "unspecified"
 GRPC_CHANNEL_OPTIONS = [
     ("grpc.max_receive_message_length", MAX_RECEIVE_MESSAGE_SIZE),
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/datum_batching.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/datum_batching.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""A high-level decorator for pipeline code that uses the datum-batching feature."""
 from functools import wraps
 from typing import Callable
 
 from . import Client
 
 PIPELINE_FUNC = Callable[..., None]
```

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/errors.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0a5/pachyderm_sdk/interceptor.py` & `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/interceptor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+Implementation of a gRPC interceptor used to set request metadata
+and catch connection errors.
+"""
+
 from os import environ
 from typing import Any, Callable, Sequence, Optional, Tuple, Union
 
 import grpc
 from grpc_interceptor import ClientCallDetails, ClientInterceptor
 
 from .errors import AuthServiceNotActivated
```

### Comparing `pachyderm_sdk-2.7.0a5/pyproject.toml` & `pachyderm_sdk-2.7.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "pachyderm_sdk"
-version = "v2.7.0-alpha.5"
+version = "2.7.0-rc.1"
 description = "Python Pachyderm Client"
 authors = ["Pachyderm Integrations <integrations@pachyderm.io>"]
 license = "Apache 2.0"
-documentation = "https://python-pachyderm.readthedocs.io/en/stable/"
+documentation = "https://docs.pachyderm.com/latest/sdk/python/"
 readme = 'README.md'
-repository = "https://github.com/pachyderm/python-pachyderm"
+repository = "https://github.com/pachyderm/pachyderm/tree/master/python-sdk"
 keywords = ["pachyderm"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -25,14 +25,15 @@
 certifi = ">=2022.9"
 grpcio = ">=1.50.0,<1.52.0"
 grpc-interceptor = "^0.14.2"
 python-dotenv = "1.0"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
+pdoc3 = "0.10.0"
 pandas = "2.0.3"
 pytest = "^7.2.1"
 pytest-black-ng = "^0.4.1"
 
 [tool.poetry.scripts]
 pachyderm-sdk-check-connection = 'pachyderm_sdk.__main__:check_connection'
```

### Comparing `pachyderm_sdk-2.7.0a5/PKG-INFO` & `pachyderm_sdk-2.7.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pachyderm-sdk
-Version: 2.7.0a5
+Version: 2.7.0rc1
 Summary: Python Pachyderm Client
-Home-page: https://github.com/pachyderm/python-pachyderm
+Home-page: https://github.com/pachyderm/pachyderm/tree/master/python-sdk
 License: Apache 2.0
 Keywords: pachyderm
 Author: Pachyderm Integrations
 Author-email: integrations@pachyderm.io
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,16 +22,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: betterproto (==2.0.0b5)
 Requires-Dist: certifi (>=2022.9)
 Requires-Dist: grpc-interceptor (>=0.14.2,<0.15.0)
 Requires-Dist: grpcio (>=1.50.0,<1.52.0)
 Requires-Dist: python-dotenv (==1.0)
-Project-URL: Documentation, https://python-pachyderm.readthedocs.io/en/stable/
-Project-URL: Repository, https://github.com/pachyderm/python-pachyderm
+Project-URL: Documentation, https://docs.pachyderm.com/latest/sdk/python/
+Project-URL: Repository, https://github.com/pachyderm/pachyderm/tree/master/python-sdk
 Description-Content-Type: text/markdown
 
 # Pachyderm's Python SDK
 
 Official Python client/SDK for Pachyderm.
 The successor to https://github.com/pachyderm/python-pachyderm.
```

