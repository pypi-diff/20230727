# Comparing `tmp/zyte-common-items-0.7.0.tar.gz` & `tmp/zyte-common-items-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zyte-common-items-0.7.0.tar", last modified: Tue Jul 11 14:16:42 2023, max compression
+gzip compressed data, was "zyte-common-items-0.8.0.tar", last modified: Thu Jul 27 12:13:01 2023, max compression
```

## Comparing `zyte-common-items-0.7.0.tar` & `zyte-common-items-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/zyte_common_items/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    34865 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-11 14:16:31.000000 zyte-common-items-0.7.0/zyte_common_items/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:16:42.717479 zyte-common-items-0.7.0/zyte_common_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 14:16:42.000000 zyte-common-items-0.7.0/zyte_common_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:13:01.701554 zyte-common-items-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 12:13:01.701554 zyte-common-items-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 12:13:01.701554 zyte-common-items-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:13:01.697554 zyte-common-items-0.8.0/zyte_common_items/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38188 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-27 12:12:49.000000 zyte-common-items-0.8.0/zyte_common_items/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 12:13:01.697554 zyte-common-items-0.8.0/zyte_common_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 12:13:01.000000 zyte-common-items-0.8.0/zyte_common_items.egg-info/top_level.txt
```

### Comparing `zyte-common-items-0.7.0/LICENSE` & `zyte-common-items-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.7.0/PKG-INFO` & `zyte-common-items-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.7.0
+Version: 0.8.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-common-items-0.7.0/README.rst` & `zyte-common-items-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.7.0/setup.py` & `zyte-common-items-0.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,18 +19,18 @@
             "tests",
         ]
     ),
     package_data={
         "zyte_common_items": ["py.typed", "VERSION"],
     },
     install_requires=[
-        "attrs>=21.3.0",
+        "attrs>=22.1.0",
         "itemadapter>=0.8.0",
-        "web-poet>=0.7.0",
-        "zyte-parsers",
+        "web-poet>=0.9.0",
+        "zyte-parsers>=0.2.0",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `zyte-common-items-0.7.0/zyte_common_items/__init__.py` & `zyte-common-items-0.8.0/zyte_common_items/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,20 +7,24 @@
     AggregateRating,
     Amenity,
     ArticleListMetadata,
     ArticleMetadata,
     ArticleNavigationMetadata,
     Audio,
     Author,
+    BaseSalary,
     Brand,
     Breadcrumb,
     BusinessPlaceMetadata,
     Gtin,
     Header,
+    HiringOrganization,
     Image,
+    JobLocation,
+    JobPostingMetadata,
     Link,
     Metadata,
     NamedLink,
     OpeningHoursItem,
     ParentPlace,
     ProbabilityMetadata,
     ProbabilityRequest,
@@ -35,14 +39,15 @@
 )
 from .items import (
     Article,
     ArticleFromList,
     ArticleList,
     ArticleNavigation,
     BusinessPlace,
+    JobPosting,
     Product,
     ProductFromList,
     ProductList,
     ProductNavigation,
     ProductVariant,
     RealEstate,
 )
@@ -50,21 +55,23 @@
     ArticleListPage,
     ArticleNavigationPage,
     ArticlePage,
     BaseArticleListPage,
     BaseArticleNavigationPage,
     BaseArticlePage,
     BaseBusinessPlacePage,
+    BaseJobPostingPage,
     BasePage,
     BaseProductListPage,
     BaseProductNavigationPage,
     BaseProductPage,
     BaseRealEstatePage,
     BusinessPlacePage,
     HasMetadata,
+    JobPostingPage,
     MetadataT,
     Page,
     ProductListPage,
     ProductNavigationPage,
     ProductPage,
     RealEstatePage,
 )
```

### Comparing `zyte-common-items-0.7.0/zyte_common_items/adapter.py` & `zyte-common-items-0.8.0/zyte_common_items/adapter.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.7.0/zyte_common_items/base.py` & `zyte-common-items-0.8.0/zyte_common_items/base.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.7.0/zyte_common_items/components.py` & `zyte-common-items-0.8.0/zyte_common_items/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes for data nested within items."""
+import base64
 from typing import List, Optional, Type
 
 import attrs
 
 from zyte_common_items.base import Item
 from zyte_common_items.util import convert_to_class, url_to_str
 
@@ -85,14 +86,21 @@
 
 @attrs.define(kw_only=True)
 class BusinessPlaceMetadata(Metadata):
     pass
 
 
 @attrs.define(kw_only=True)
+class JobPostingMetadata(Metadata):
+    """Metadata associated with a job posting."""
+
+    pass
+
+
+@attrs.define(kw_only=True)
 class ProductMetadata(_DetailsMetadata):
     pass
 
 
 @attrs.define(kw_only=True)
 class ProductListMetadata(_ListMetadata):
     pass
@@ -398,33 +406,62 @@
     #: Name of the header
     name: str
 
     #: Value of the header
     value: str
 
 
-@attrs.define(kw_only=True)
+@attrs.define(slots=False)
 class Request(Item):
     """Describe a web request to load a page"""
 
-    #: Name of the page being requested.
-    name: Optional[str] = None
-
     #: HTTP URL
     url: str = attrs.field(converter=url_to_str)
 
     #: HTTP method
     method: str = "GET"
 
     #: HTTP request body, Base64-encoded
     body: Optional[str] = None
 
     #: HTTP headers
     headers: Optional[List[Header]] = None
 
+    #: Name of the page being requested.
+    name: Optional[str] = None
+
+    _body_bytes = None
+
+    @property
+    def body_bytes(self) -> Optional[bytes]:
+        """Request.body as bytes"""
+        # todo: allow to set body bytes in __init__, to avoid encoding/decoding.
+        if self._body_bytes is None:
+            if self.body is not None:
+                self._body_bytes = base64.b64decode(self.body)
+        return self._body_bytes
+
+    def to_scrapy(self, callback, **kwargs):
+        """
+        Convert a request to scrapy.Request.
+        All kwargs are passed to scrapy.Request as-is.
+        """
+        import scrapy
+
+        header_list = [(header.name, header.value) for header in self.headers or []]
+
+        return scrapy.Request(
+            url=self.url,
+            callback=callback,
+            method=self.method or "GET",
+            headers=header_list,
+            body=self.body_bytes,
+            **kwargs
+        )
+
 
 @attrs.define
 class Video(_Media):
     """Video.
 
     See :class:`Article.videos <zyte_common_items.Article.videos>`.
     """
@@ -443,7 +480,52 @@
 
 @attrs.define(kw_only=True)
 class ProbabilityRequest(Request):
     """A :class:`Request` that includes a probability value."""
 
     #: Data extraction process metadata.
     metadata: Optional[ProbabilityMetadata] = None
+
+
+@attrs.define(kw_only=True)
+class JobLocation(Item):
+    """Location of a job offer."""
+
+    #: Job location, as it appears on the website.
+    raw: Optional[str] = None
+
+
+@attrs.define(kw_only=True)
+class BaseSalary(Item):
+    """Base salary of a job offer."""
+
+    #: Salary amount as it appears on the website.
+    raw: Optional[str] = None
+
+    #: The minimum value of the base salary as a number string.
+    valueMin: Optional[str] = None
+
+    #: The maximum value of the base salary as a number string.
+    valueMax: Optional[str] = None
+
+    #: The type of rate associated with the salary, e.g. monthly, annual, daily.
+    rateType: Optional[str] = None
+
+    #: Currency associated with the salary amount.
+    currency: Optional[str] = None
+
+    #: Currency associated with the salary amount, without normalization.
+    currencyRaw: Optional[str] = None
+
+
+@attrs.define(kw_only=True)
+class HiringOrganization(Item):
+    """Organization that is hiring for a job offer."""
+
+    #: Name of the hiring organization.
+    name: Optional[str] = None
+
+    #: Organization information as available on the website.
+    nameRaw: Optional[str] = None
+
+    #: Identifier of the organization used by job posting website.
+    id: Optional[str] = None
```

### Comparing `zyte-common-items-0.7.0/zyte_common_items/items.py` & `zyte-common-items-0.8.0/zyte_common_items/items.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,23 @@
     AggregateRating,
     Amenity,
     ArticleListMetadata,
     ArticleMetadata,
     ArticleNavigationMetadata,
     Audio,
     Author,
+    BaseSalary,
     Brand,
     Breadcrumb,
     BusinessPlaceMetadata,
     Gtin,
+    HiringOrganization,
     Image,
+    JobLocation,
+    JobPostingMetadata,
     Link,
     NamedLink,
     OpeningHoursItem,
     ParentPlace,
     ProbabilityMetadata,
     ProbabilityRequest,
     ProductListMetadata,
@@ -1034,7 +1038,101 @@
     #: numbered as 0 on the website, it should be extracted as `1` nonetheless.
     pageNumber: Optional[int] = None
 
     #: Data extraction process metadata.
     metadata: Optional[ArticleNavigationMetadata] = attrs.field(
         default=None, converter=attrs.converters.optional(MetadataCaster(ArticleNavigationMetadata)), kw_only=True  # type: ignore
     )
+
+
+@attrs.define(kw_only=True)
+class JobPosting(Item):
+    #: The url of the final response, after any redirects.
+    url: str = attrs.field(converter=url_to_str)
+
+    #: The identifier of the job posting.
+    jobPostingId: Optional[str] = None
+
+    #: Publication date of the job posting.
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ"
+    #:
+    #: With timezone, if available.
+    datePublished: Optional[str] = None
+
+    #: Same date as datePublished, but before parsing/normalization, i.e. as it appears on the website.
+    datePublishedRaw: Optional[str] = None
+
+    #: The date when the job posting was most recently modified.
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ"
+    #:
+    #: With timezone, if available.
+    dateModified: Optional[str] = None
+
+    #: Same date as dateModified, but before parsing/normalization, i.e. as it appears on the website.
+    dateModifiedRaw: Optional[str] = None
+
+    #: The date after which the job posting is not valid, e.g. the end of an offer.
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ"
+    #:
+    #: With timezone, if available.
+    validThrough: Optional[str] = None
+
+    #: Same date as validThrough, but before parsing/normalization, i.e. as it appears on the website.
+    validThroughRaw: Optional[str] = None
+
+    #: The title of the job posting.
+    jobTitle: Optional[str] = None
+
+    #: The headline of the job posting.
+    headline: Optional[str] = None
+
+    #: A (typically single) geographic location associated with the job position.
+    jobLocation: Optional[JobLocation] = None
+
+    #: A description of the job posting including sub-headings, with newline separators.
+    #:
+    #: Format:
+    #:
+    #: - trimmed (no whitespace at the beginning or the end of the description string),
+    #:
+    #: - line breaks included,
+    #:
+    #: - no length limit,
+    #:
+    #: - no normalization of Unicode characters.
+    description: Optional[str] = None
+
+    #: Simplified HTML of the description, including sub-headings, image captions and embedded content.
+    descriptionHtml: Optional[str] = None
+
+    #: Type of employment (e.g. full-time, part-time, contract, temporary, seasonal, internship).
+    employmentType: Optional[str] = None
+
+    #: The base salary of the job or of an employee in the proposed role.
+    baseSalary: Optional[BaseSalary] = None
+
+    #: Candidate requirements for the job.
+    requirements: Optional[List[str]] = None
+
+    #: Information about the organization offering the job position.
+    hiringOrganization: Optional[HiringOrganization] = None
+
+    #: Job start date
+    #:
+    #: Format: ISO 8601 format: "YYYY-MM-DDThh:mm:ssZ"
+    #:
+    #: With timezone, if available.
+    jobStartDate: Optional[str] = None
+
+    #: Same date as jobStartDate, but before parsing/normalization, i.e. as it appears on the website.
+    jobStartDateRaw: Optional[str] = None
+
+    #: Specifies the remote status of the position.
+    remoteStatus: Optional[str] = None
+
+    #: Contains metadata about the data extraction process.
+    metadata: Optional[JobPostingMetadata] = attrs.field(
+        default=None, converter=attrs.converters.optional(MetadataCaster(JobPostingMetadata)), kw_only=True  # type: ignore
+    )
```

### Comparing `zyte-common-items-0.7.0/zyte_common_items/pages.py` & `zyte-common-items-0.8.0/zyte_common_items/pages.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,33 @@
 from web_poet.pages import ItemT
 
 from .components import (
     ArticleListMetadata,
     ArticleMetadata,
     ArticleNavigationMetadata,
     BusinessPlaceMetadata,
+    JobPostingMetadata,
     ProductListMetadata,
     ProductMetadata,
     ProductNavigationMetadata,
     RealEstateMetadata,
     request_list_processor,
 )
 from .items import (
     Article,
     ArticleList,
     ArticleNavigation,
     BusinessPlace,
+    JobPosting,
     Product,
     ProductList,
     ProductNavigation,
     RealEstate,
 )
-from .processors import breadcrumbs_processor
+from .processors import brand_processor, breadcrumbs_processor
 from .util import format_datetime, metadata_processor
 
 #: Generic type for metadata classes for specific item types.
 MetadataT = TypeVar("MetadataT")
 
 
 def _date_downloaded_now():
@@ -122,16 +124,23 @@
 
 class BaseBusinessPlacePage(
     BasePage, Returns[BusinessPlace], HasMetadata[BusinessPlaceMetadata]
 ):
     pass
 
 
+class BaseJobPostingPage(
+    BasePage, Returns[JobPosting], HasMetadata[JobPostingMetadata]
+):
+    pass
+
+
 class BaseProductPage(BasePage, Returns[Product], HasMetadata[ProductMetadata]):
     class Processors(BasePage.Processors):
+        brand = [brand_processor]
         breadcrumbs = [breadcrumbs_processor]
 
 
 class BaseProductListPage(
     BasePage, Returns[ProductList], HasMetadata[ProductListMetadata]
 ):
     class Processors(BasePage.Processors):
@@ -181,16 +190,21 @@
 
 class BusinessPlacePage(
     Page, Returns[BusinessPlace], HasMetadata[BusinessPlaceMetadata]
 ):
     pass
 
 
+class JobPostingPage(Page, Returns[JobPosting], HasMetadata[JobPostingMetadata]):
+    pass
+
+
 class ProductPage(Page, Returns[Product], HasMetadata[ProductMetadata]):
     class Processors(Page.Processors):
+        brand = [brand_processor]
         breadcrumbs = [breadcrumbs_processor]
 
 
 class ProductListPage(Page, Returns[ProductList], HasMetadata[ProductListMetadata]):
     class Processors(Page.Processors):
         breadcrumbs = [breadcrumbs_processor]
```

### Comparing `zyte-common-items-0.7.0/zyte_common_items/processors.py` & `zyte-common-items-0.8.0/zyte_common_items/processors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Iterable
 from typing import Any, List, Optional
 
 from lxml.html import HtmlElement
 from parsel import Selector, SelectorList
 from web_poet.mixins import ResponseShortcutsMixin
 from zyte_parsers import Breadcrumb as zp_Breadcrumb
-from zyte_parsers import extract_breadcrumbs
+from zyte_parsers import extract_brand_name, extract_breadcrumbs
 
 from .items import Breadcrumb
 
 
 def _get_base_url(page: Any) -> Optional[str]:
     if isinstance(page, ResponseShortcutsMixin):
         return page.base_url
@@ -45,7 +45,26 @@
     results: List[Any] = []
     for item in value:
         if isinstance(item, zp_Breadcrumb):
             results.append(_from_zp_breadcrumb(item))
         else:
             results.append(item)
     return results
+
+
+def brand_processor(value: Any) -> Any:
+    """Convert the data into a brand name if possible.
+
+    Supported inputs are :class:`~parsel.selector.Selector`,
+    :class:`~parsel.selector.SelectorList` and :class:`~lxml.html.HtmlElement`.
+    Other inputs are returned as is.
+    """
+
+    if isinstance(value, SelectorList):
+        if len(value) == 0:
+            return None
+        value = value[0]
+
+    if isinstance(value, (Selector, HtmlElement)):
+        return extract_brand_name(value, search_depth=2)
+
+    return value
```

### Comparing `zyte-common-items-0.7.0/zyte_common_items/util.py` & `zyte-common-items-0.8.0/zyte_common_items/util.py`

 * *Files identical despite different names*

### Comparing `zyte-common-items-0.7.0/zyte_common_items.egg-info/PKG-INFO` & `zyte-common-items-0.8.0/zyte_common_items.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zyte-common-items
-Version: 0.7.0
+Version: 0.8.0
 Summary: Item definitions for Zyte API schema
 Home-page: https://github.com/zytedata/zyte-common-items
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `zyte-common-items-0.7.0/zyte_common_items.egg-info/SOURCES.txt` & `zyte-common-items-0.8.0/zyte_common_items.egg-info/SOURCES.txt`

 * *Files identical despite different names*

