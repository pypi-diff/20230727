# Comparing `tmp/ols_py-0.3.0.tar.gz` & `tmp/ols_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ols_py-0.3.0.tar", max compression
+gzip compressed data, was "ols_py-0.5.0.tar", max compression
```

## Comparing `ols_py-0.3.0.tar` & `ols_py-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3549 2023-06-05 03:08:16.163353 ols_py-0.3.0/README.md
--rw-r--r--   0        0        0     2286 2023-06-05 03:08:16.167353 ols_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       55 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/__init__.py
--rw-r--r--   0        0        0    10705 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/client.py
--rw-r--r--   0        0        0     1641 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/instances.py
--rw-r--r--   0        0        0     2975 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/ols4_client.py
--rw-r--r--   0        0        0       49 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/ols4_schemas/__init__.py
--rw-r--r--   0        0        0     1118 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/ols4_schemas/responses.py
--rw-r--r--   0        0        0        0 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/py.typed
--rw-r--r--   0        0        0       89 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/__init__.py
--rw-r--r--   0        0        0      408 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/common.py
--rw-r--r--   0        0        0     4219 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/requests.py
--rw-r--r--   0        0        0     3752 2023-06-05 03:08:16.167353 ols_py-0.3.0/src/ols_py/schemas/responses.py
--rw-r--r--   0        0        0     4556 1970-01-01 00:00:00.000000 ols_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3549 2023-07-27 06:33:02.495271 ols_py-0.5.0/README.md
+-rw-r--r--   0        0        0     2329 2023-07-27 06:33:02.499271 ols_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/__init__.py
+-rw-r--r--   0        0        0    10711 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/client.py
+-rw-r--r--   0        0        0     1641 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/instances.py
+-rw-r--r--   0        0        0     2975 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/ols4_client.py
+-rw-r--r--   0        0        0       49 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/ols4_schemas/__init__.py
+-rw-r--r--   0        0        0     1454 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/ols4_schemas/responses.py
+-rw-r--r--   0        0        0        0 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/py.typed
+-rw-r--r--   0        0        0       89 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/schemas/__init__.py
+-rw-r--r--   0        0        0      488 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/schemas/common.py
+-rw-r--r--   0        0        0     4471 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/schemas/requests.py
+-rw-r--r--   0        0        0     3876 2023-07-27 06:33:02.499271 ols_py-0.5.0/src/ols_py/schemas/responses.py
+-rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 ols_py-0.5.0/PKG-INFO
```

### Comparing `ols_py-0.3.0/README.md` & `ols_py-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ols_py-0.3.0/pyproject.toml` & `ols_py-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ols-py"
-version = "0.3.0"
+version = "0.5.0"
 description = "Python client for the Ontology Lookup Service"
 authors = [
     "Marius Mather <marius.mather@sydney.edu.au>",
 ]
 license = "MIT"
 readme = "README.md"
 
@@ -15,26 +15,27 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed",
 ]
 
 packages = [
     { include = "ols_py", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10.1, <4.0"
 requests = ">=2.0, <3.0"
-pydantic = "^1.10.2"
+pydantic = "^2.1.1"
 
 [tool.poetry.group.jupyterlab]
 optional = true
 
 [tool.poetry.group.jupyterlab.dependencies]
 jupyterlab = "^3.6"
```

### Comparing `ols_py-0.3.0/src/ols_py/client.py` & `ols_py-0.5.0/src/ols_py/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     ) -> schemas.responses.OntologyList:
         """
         Get the list of ontologies the OLS instance has.
 
         :param page: Page number of results (starting at 0)
         :param size: Number of results per page (API default is 20)
         """
-        params = schemas.requests.PageParams(page=page, size=size).dict(
+        params = schemas.requests.PageParams(page=page, size=size).model_dump(
             exclude_none=True
         )
         ontology_list = self.get_with_schema(
             schemas.responses.OntologyList, "/ontologies", params=params
         )
         return ontology_list
```

### Comparing `ols_py-0.3.0/src/ols_py/instances.py` & `ols_py-0.5.0/src/ols_py/instances.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.3.0/src/ols_py/ols4_client.py` & `ols_py-0.5.0/src/ols_py/ols4_client.py`

 * *Files identical despite different names*

### Comparing `ols_py-0.3.0/src/ols_py/schemas/requests.py` & `ols_py-0.5.0/src/ols_py/schemas/requests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 from typing import Literal, Optional, TypedDict
 
-from pydantic import BaseModel, NonNegativeInt, PositiveInt, validator
+from pydantic import BaseModel, NonNegativeInt, PositiveInt, field_validator
 
 from .common import AnnotationFieldName, EntityType
 
 
 class PageParams(BaseModel):
     """
     Pagination params accepted by endpoints that return multiple
     resources
     """
 
-    size: Optional[PositiveInt]
+    size: Optional[PositiveInt] = None
     """Number of results per page"""
-    page: Optional[NonNegativeInt]
+    page: Optional[NonNegativeInt] = None
     """Which page to fetch (starting at 0)"""
 
 
 # TODO: unclear whether the API accepts the same set of fields
 #   for query/return. Defining them separately for now
 # NOTE: fields seem to be badly documented. The best canonical source I've
 #   been able to find seems to be going directly to the SOLR config for OLS
@@ -31,15 +31,18 @@
     "iri",
     "label",
     "obo_id",
     "ontology_name",
     "ontology_prefix",
     "short_form",
     "subset",
+    # TODO: OLS3 uses synonym, OLS4 uses synonyms. Best option for now
+    #   is to allow both.
     "synonym",
+    "synonyms",
     "type",
 ]
 SearchQueryFields = Literal[
     "annotations",
     "description",
     "iri",
     "label",
@@ -58,55 +61,56 @@
     you can use in the request - we want to convert any
     lists of options to comma-separated strings, which
     we can't do with the default dict() method
     """
 
     q: str
     """Query to search for"""
-    ontology: Optional[list[str]]
+    ontology: Optional[list[str]] = None
     """Ontologies to search, e.g. `["mondo", "upheno"]`"""
-    type: Optional[EntityType]
+    type: Optional[EntityType] = None
     """Type of term to search for, e.g. "class", "property" """
-    slim: Optional[list[str]]
-    fieldList: Optional[list[SearchReturnFields | AnnotationFieldName]]
+    slim: Optional[list[str]] = None
+    fieldList: Optional[list[SearchReturnFields | AnnotationFieldName]] = None
     """Which fields to return in the results"""
-    queryFields: Optional[list[SearchQueryFields | AnnotationFieldName]]
+    queryFields: Optional[list[SearchQueryFields | AnnotationFieldName]] = None
     """Which fields to search over"""
-    exact: Optional[bool]
-    groupField: Optional[bool]
+    exact: Optional[bool] = None
+    groupField: Optional[bool] = None
     """Group results by unique ID"""
-    obsoletes: Optional[bool]
+    obsoletes: Optional[bool] = None
     """Include obsoleted terms in the results"""
-    local: Optional[bool]
+    local: Optional[bool] = None
     """Only return terms in a defining ontology"""
-    childrenOf: Optional[list[str]]
+    childrenOf: Optional[list[str]] = None
     """Restrict results to children of these terms"""
-    allChildrenOf: Optional[list[str]]
+    allChildrenOf: Optional[list[str]] = None
     """
     Restrict results to children of these terms, plus other
     child-like relations e.g. "part of", "develops from"
     """
-    rows: Optional[int]
+    rows: Optional[int] = None
     """
     Number of results per page
     """
-    start: Optional[int]
+    start: Optional[int] = None
     """
     Index of first result
     """
 
-    @validator(
+    @field_validator(
         "ontology",
         "slim",
         "childrenOf",
         "allChildrenOf",
         "fieldList",
         "queryFields",
-        pre=True,
+        mode="before",
     )
+    @classmethod
     def _single_to_list(cls, v):
         """
         If a single string is passed but we expect
         list[str], convert to a 1-item list automatically.
         Called at the pre-validation step.
         """
         if isinstance(v, str):
```

### Comparing `ols_py-0.3.0/src/ols_py/schemas/responses.py` & `ols_py-0.5.0/src/ols_py/schemas/responses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 import pydantic
-from pydantic import BaseModel, Extra, Field, HttpUrl
+from pydantic import BaseModel, ConfigDict, Field, HttpUrl
 
 from ols_py.schemas.common import EntityType
 
 
 class PageInfo(BaseModel):
     """
     Page information returned in paginated responses
@@ -34,31 +34,29 @@
 
     iri: pydantic.AnyUrl
     label: str
     description: list[str]
     # Not specifying annotations for now, not sure if these
     #   are fixed
     annotation: dict[str, list[str]]
-    synonyms: Optional[list[str]]
+    synonyms: Optional[list[str]] = None
     ontology_name: str
     ontology_prefix: str
     ontology_iri: pydantic.AnyUrl
     is_obsolete: bool
-    term_replaced_by: Optional[Any]
+    term_replaced_by: Optional[Any] = None
     has_children: bool
     is_root: bool
     short_form: str
     # Higher level terms may not have an obo ID, e.g.
     # terms will be descendants of http://www.w3.org/2002/07/owl#Thing
-    obo_id: Optional[str]
-    in_subset: Optional[Any]
+    obo_id: Optional[str] = None
+    in_subset: Optional[Any] = None
     links: dict[str, Link] = Field(..., alias="_links")
-
-    class Config:
-        extra = "allow"
+    model_config = ConfigDict(extra="allow")
 
 
 class ApiInfoLinks(BaseModel):
     """
     Set of links returned in the root endpoint/
     API ifno
     """
@@ -80,17 +78,15 @@
 
 
 class OntologyItem(BaseModel):
     ontologyId: str
     status: str
     numberOfProperties: int
     numberOfTerms: int
-
-    class Config:
-        extra = "allow"
+    model_config = ConfigDict(extra="allow")
 
 
 class OntologyListEmbedded(BaseModel):
     ontologies: list[OntologyItem]
 
 
 class OntologyList(BaseModel):
@@ -133,28 +129,28 @@
     """
 
     embedded: EmbeddedTerms = Field(..., alias="_embedded")
     links: TermInDefiningOntologyLinks = Field(..., alias="_links")
     page: PageInfo
 
 
-class SearchResultItem(BaseModel, extra=Extra.allow):
-    id: Optional[str]
-    annotations: Optional[list[str]]
-    annotations_trimmed: Optional[list[str]]
-    description: Optional[list[str]]
-    iri: Optional[str]
-    label: Optional[str]
-    obo_id: Optional[str]
-    ontology_name: Optional[str]
-    ontology_prefix: Optional[str]
-    subset: Optional[list[str]]
-    short_form: Optional[str]
-    synonym: Optional[list[str]]
-    type: Optional[EntityType]
+class SearchResultItem(BaseModel, extra="allow"):
+    id: Optional[str] = None
+    annotations: Optional[list[str]] = None
+    annotations_trimmed: Optional[list[str]] = None
+    description: Optional[list[str]] = None
+    iri: Optional[str] = None
+    label: Optional[str] = None
+    obo_id: Optional[str] = None
+    ontology_name: Optional[str] = None
+    ontology_prefix: Optional[str] = None
+    subset: Optional[list[str]] = None
+    short_form: Optional[str] = None
+    synonym: Optional[list[str]] = None
+    type: Optional[EntityType] = None
 
 
 class SearchResponseResponse(BaseModel):
     numFound: int
     start: int
     docs: list[SearchResultItem]
```

### Comparing `ols_py-0.3.0/PKG-INFO` & `ols_py-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ols-py
-Version: 0.3.0
+Version: 0.5.0
 Summary: Python client for the Ontology Lookup Service
 Home-page: https://ahida-development.github.io/ols-py
 License: MIT
 Author: Marius Mather
 Author-email: marius.mather@sydney.edu.au
 Requires-Python: >=3.10.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
 Requires-Dist: requests (>=2.0,<3.0)
 Project-URL: Documentation, https://ahida-development.github.io/ols-py
 Project-URL: Repository, https://github.com/ahida-development/ols-py
 Description-Content-Type: text/markdown
 
 # ols-py
```

