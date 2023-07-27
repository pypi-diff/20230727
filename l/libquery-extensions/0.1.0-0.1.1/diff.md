# Comparing `tmp/libquery_extensions-0.1.0.tar.gz` & `tmp/libquery_extensions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquery_extensions-0.1.0.tar", max compression
+gzip compressed data, was "libquery_extensions-0.1.1.tar", max compression
```

## Comparing `libquery_extensions-0.1.0.tar` & `libquery_extensions-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    34523 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/LICENSE
--rw-r--r--   0        0        0      729 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/README.md
--rw-r--r--   0        0        0      458 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/__init__.py
--rw-r--r--   0        0        0       75 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/alabama_maps/__init__.py
--rw-r--r--   0        0        0     6070 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/alabama_maps/_fetch_metadata.py
--rw-r--r--   0        0        0      971 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/alabama_maps/_querier.py
--rw-r--r--   0        0        0      587 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/alabama_maps/_typing.py
--rw-r--r--   0        0        0     3601 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/_utils/fetch_metadata.py
--rw-r--r--   0        0        0     1863 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/_utils/fetch_queries.py
--rw-r--r--   0        0        0      111 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/__init__.py
--rw-r--r--   0        0        0      911 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_fetch_image.py
--rw-r--r--   0        0        0     6902 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_fetch_metadata.py
--rw-r--r--   0        0        0     3546 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_fetch_queries.py
--rw-r--r--   0        0        0      864 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_querier.py
--rw-r--r--   0        0        0     1284 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_typing.py
--rw-r--r--   0        0        0      310 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_utils.py
--rw-r--r--   0        0        0      105 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/__init__.py
--rw-r--r--   0        0        0      650 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_fetch_image.py
--rw-r--r--   0        0        0     3172 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_fetch_metadata.py
--rw-r--r--   0        0        0     2807 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_fetch_queries.py
--rw-r--r--   0        0        0      861 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_querier.py
--rw-r--r--   0        0        0      807 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_typing.py
--rw-r--r--   0        0        0      107 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/__init__.py
--rw-r--r--   0        0        0      650 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_fetch_image.py
--rw-r--r--   0        0        0     3617 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_fetch_metadata.py
--rw-r--r--   0        0        0     3511 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_fetch_queries.py
--rw-r--r--   0        0        0      862 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_querier.py
--rw-r--r--   0        0        0      715 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_typing.py
--rw-r--r--   0        0        0      970 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_utils.py
--rw-r--r--   0        0        0     1027 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/get_chrome_driver.py
--rw-r--r--   0        0        0       69 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/telefact/__init__.py
--rw-r--r--   0        0        0     5765 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/telefact/_fetch_metadata.py
--rw-r--r--   0        0        0     1081 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/telefact/_querier.py
--rw-r--r--   0        0        0      732 2023-07-23 00:56:39.199967 libquery_extensions-0.1.0/libquery_extensions/telefact/_typing.py
--rw-r--r--   0        0        0      582 2023-07-23 00:56:39.203966 libquery_extensions-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1397 1970-01-01 00:00:00.000000 libquery_extensions-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/LICENSE
+-rw-r--r--   0        0        0      729 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/README.md
+-rw-r--r--   0        0        0      456 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/alabama_maps/__init__.py
+-rw-r--r--   0        0        0     6070 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/alabama_maps/_fetch_metadata.py
+-rw-r--r--   0        0        0      971 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/alabama_maps/_querier.py
+-rw-r--r--   0        0        0      581 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/alabama_maps/_typing.py
+-rw-r--r--   0        0        0     3601 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/british_library/_utils/fetch_metadata.py
+-rw-r--r--   0        0        0     1863 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/british_library/_utils/fetch_queries.py
+-rw-r--r--   0        0        0      111 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/__init__.py
+-rw-r--r--   0        0        0      903 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_fetch_image.py
+-rw-r--r--   0        0        0     6878 2023-07-27 01:32:21.001964 libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_fetch_metadata.py
+-rw-r--r--   0        0        0     3538 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_fetch_queries.py
+-rw-r--r--   0        0        0      864 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_querier.py
+-rw-r--r--   0        0        0     1278 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_typing.py
+-rw-r--r--   0        0        0      310 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_utils.py
+-rw-r--r--   0        0        0      105 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_fetch_image.py
+-rw-r--r--   0        0        0     3148 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_fetch_metadata.py
+-rw-r--r--   0        0        0     2799 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_fetch_queries.py
+-rw-r--r--   0        0        0      861 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_querier.py
+-rw-r--r--   0        0        0      801 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_typing.py
+-rw-r--r--   0        0        0      107 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_fetch_image.py
+-rw-r--r--   0        0        0     3593 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_fetch_metadata.py
+-rw-r--r--   0        0        0     3569 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_fetch_queries.py
+-rw-r--r--   0        0        0      862 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_querier.py
+-rw-r--r--   0        0        0      709 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_typing.py
+-rw-r--r--   0        0        0      970 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_utils.py
+-rw-r--r--   0        0        0     1027 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/get_chrome_driver.py
+-rw-r--r--   0        0        0       69 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/telefact/__init__.py
+-rw-r--r--   0        0        0     5763 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/telefact/_fetch_metadata.py
+-rw-r--r--   0        0        0     1081 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/telefact/_querier.py
+-rw-r--r--   0        0        0      726 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/libquery_extensions/telefact/_typing.py
+-rw-r--r--   0        0        0      582 2023-07-27 01:32:21.005964 libquery_extensions-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1397 1970-01-01 00:00:00.000000 libquery_extensions-0.1.1/PKG-INFO
```

### Comparing `libquery_extensions-0.1.0/LICENSE` & `libquery_extensions-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/README.md` & `libquery_extensions-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/alabama_maps/_fetch_metadata.py` & `libquery_extensions-0.1.1/libquery_extensions/alabama_maps/_fetch_metadata.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/alabama_maps/_querier.py` & `libquery_extensions-0.1.1/libquery_extensions/alabama_maps/_querier.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/alabama_maps/_typing.py` & `libquery_extensions-0.1.1/libquery_extensions/alabama_maps/_typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The type declarations specific to the `Alabama Maps` data source.
 """
 
 from typing import TypedDict, Union
 
-from libquery.typing import MetadataEntry as BaseMetadataEntry
+from libquery.typing import MetadataEntry as _MetadataEntry
 
 
 class SourceData(TypedDict):
     """The data directly returned from the url."""
 
     mainAuthor: Union[str, None]
     titleDescription: str
@@ -16,11 +16,11 @@
     date: str
     scale: str
     originalSource: str
     viewUrl: str
     downloadUrl: str
 
 
-class MetadataEntry(BaseMetadataEntry):
+class MetadataEntry(_MetadataEntry):
     """The data structure of an entry in the metadata."""
 
     sourceData: SourceData
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/_utils/fetch_metadata.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/_utils/fetch_metadata.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/_utils/fetch_queries.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/_utils/fetch_queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Utility functions for extracting query URLs from a webpage URL.
 """
 
 import json
 import os
-from typing import Any, Callable, List, TypedDict, Set
+from typing import Any, Callable, List, Set, TypedDict
 
 import backoff
 from libquery.utils.jsonl import load_jl
 from selenium import webdriver
 from selenium.common.exceptions import WebDriverException
 from tqdm import tqdm
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_fetch_image.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_fetch_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Fetch images from the urls stored in metadata.
 """
 
 from typing import List
 
 from libquery.typing import ImageQuery
-from libquery.utils.image import fetch as base_fetch_image
+from libquery.utils.image import fetch as _fetch_image
 from ._typing import MetadataEntry
 from ._utils import get_image_uuid
 
 
 def _build_image_queries(metadata: List[MetadataEntry]) -> List[ImageQuery]:
     """Build a list of image urls to query."""
 
@@ -25,8 +25,8 @@
             }
             for image_url in source_data["images"]
         ]
     return img_queries
 
 
 def fetch_image(metadata_path: str, img_dir: str) -> None:
-    return base_fetch_image(metadata_path, img_dir, _build_image_queries)
+    return _fetch_image(metadata_path, img_dir, _build_image_queries)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_fetch_metadata.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_fetch_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import cssutils
 from selenium import webdriver
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
-from .._utils.fetch_metadata import fetch_metadata as base_fetch_metadata
+from .._utils.fetch_metadata import fetch_metadata as _fetch_metadata
 from ._typing import SourceData
 
 
 def _cleansing_text(text: str) -> str:
     text = codecs.getdecoder("unicode_escape")(text)[0]
     text = re.sub(
         r"[\xc2-\xf4][\x80-\xbf]+",
@@ -179,10 +179,8 @@
     if short_description is not None:
         source_data["item"]["shortDescription"] = short_description
     source_data["images"] = _get_image_urls(driver)
     return source_data
 
 
 def fetch_metadata(query_path: str, metadata_path: str, html_dir: str = None) -> None:
-    return base_fetch_metadata(
-        query_path, metadata_path, _extract_source_data, html_dir
-    )
+    return _fetch_metadata(query_path, metadata_path, _extract_source_data, html_dir)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_fetch_queries.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_fetch_queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 from .._utils.fetch_queries import (
-    fetch_queries as base_fetch_queries,
+    fetch_queries as _fetch_queries,
     Query,
 )
 
 
 def _get_next_page_url(driver: webdriver.Chrome) -> Union[str, None]:
     """
     The extract the URL of the next page from the next page button.
@@ -100,8 +100,8 @@
     if next_page_url is not None:
         sleep(3)
         queries += _extract_queries(driver, next_page_url)
     return queries
 
 
 def fetch_queries(base_urls: List[str], query_path: str) -> None:
-    base_fetch_queries(base_urls, query_path, _extract_queries)
+    _fetch_queries(base_urls, query_path, _extract_queries)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_querier.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_querier.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/collection_items/_typing.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/collection_items/_typing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The type declarations specific to the `British Library Collection Items` data source.
 """
 
 from typing import List, TypedDict
 
-from libquery.typing import MetadataEntry as BaseMetadataEntry
+from libquery.typing import MetadataEntry as _MetadataEntry
 from typing_extensions import NotRequired
 
 
 Item = TypedDict(
     "Item",
     {
         "Full title": NotRequired[str],
@@ -36,11 +36,11 @@
 class SourceData(TypedDict):
     """The data directly returned from the url."""
 
     item: Item
     images: NotRequired[List[str]]
 
 
-class MetadataEntry(BaseMetadataEntry):
+class MetadataEntry(_MetadataEntry):
     """The data structure of an entry in the metadata."""
 
     sourceData: SourceData
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_fetch_image.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_fetch_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Fetch images from the urls stored in metadata.
 """
 
 from typing import List
 
 from libquery.typing import ImageQuery
-from libquery.utils.image import fetch as base_fetch_image
+from libquery.utils.image import fetch as _fetch_image
 
 from ._typing import MetadataEntry
 
 
 def _build_image_queries(metadata: List[MetadataEntry]) -> List[ImageQuery]:
     """Build a list of image urls to query."""
 
@@ -19,8 +19,8 @@
             "uuid": d["uuid"],
         }
         for d in metadata
     ]
 
 
 def fetch_image(metadata_path: str, img_dir: str) -> None:
-    return base_fetch_image(metadata_path, img_dir, _build_image_queries)
+    return _fetch_image(metadata_path, img_dir, _build_image_queries)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_fetch_metadata.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_fetch_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     NoSuchElementException,
     TimeoutException,
 )
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
-from .._utils.fetch_metadata import fetch_metadata as base_fetch_metadata
+from .._utils.fetch_metadata import fetch_metadata as _fetch_metadata
 
 
 def _get_image_url(driver: webdriver.Chrome) -> str:
     """
     Extract image download URL from the webpage.
     The webpage is expected to have one image.
     """
@@ -87,10 +87,8 @@
         "assetName": _get_asset_name(driver),
         **_get_additional_attributes(driver),
         "downloadUrl": _get_image_url(driver),
     }
 
 
 def fetch_metadata(query_path: str, metadata_path: str, html_dir: str = None) -> None:
-    return base_fetch_metadata(
-        query_path, metadata_path, _extract_source_data, html_dir
-    )
+    return _fetch_metadata(query_path, metadata_path, _extract_source_data, html_dir)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_fetch_queries.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_fetch_queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from selenium.common.exceptions import TimeoutException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 from .._utils.fetch_queries import (
-    fetch_queries as base_fetch_queries,
+    fetch_queries as _fetch_queries,
     Query,
 )
 
 
 def _scroll2bottom(driver: webdriver.Chrome) -> None:
     """
     Scroll to the bottom of the page to
@@ -81,8 +81,8 @@
             "queryUrl": _parse_query_url(d),
         }
         for d in preview_article_elements
     ]
 
 
 def fetch_queries(base_urls: List[str], query_path: str) -> None:
-    base_fetch_queries(base_urls, query_path, _extract_queries)
+    _fetch_queries(base_urls, query_path, _extract_queries)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_querier.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_querier.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/images_online/_typing.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/images_online/_typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The type declarations specific to the `Telefact` data source.
 """
 
 from typing import TypedDict
 
-from libquery.typing import MetadataEntry as BaseMetadataEntry
+from libquery.typing import MetadataEntry as _MetadataEntry
 from typing_extensions import NotRequired
 
 
 SourceData = TypedDict(
     "SourceData",
     {
         "assetName": str,
@@ -21,11 +21,11 @@
         "Credit": NotRequired[str],
         "Artist/creator": NotRequired[str],
         "Author": NotRequired[str],
     },
 )
 
 
-class MetadataEntry(BaseMetadataEntry):
+class MetadataEntry(_MetadataEntry):
     """The data structure of an entry in the metadata."""
 
     sourceData: SourceData
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_fetch_image.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_fetch_image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Fetch images from the urls stored in metadata.
 """
 
 from typing import List
 
 from libquery.typing import ImageQuery
-from libquery.utils.image import fetch as base_fetch_image
+from libquery.utils.image import fetch as _fetch_image
 
 from ._typing import MetadataEntry
 
 
 def _build_image_queries(metadata: List[MetadataEntry]) -> List[ImageQuery]:
     """Build a list of image urls to query."""
 
@@ -19,8 +19,8 @@
             "uuid": d["uuid"],
         }
         for d in metadata
     ]
 
 
 def fetch_image(metadata_path: str, img_dir: str) -> None:
-    return base_fetch_image(metadata_path, img_dir, _build_image_queries)
+    return _fetch_image(metadata_path, img_dir, _build_image_queries)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_fetch_metadata.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_fetch_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeoutException,
 )
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
-from .._utils.fetch_metadata import fetch_metadata as base_fetch_metadata
+from .._utils.fetch_metadata import fetch_metadata as _fetch_metadata
 from ._utils import try_switch_to_replay_iframe
 
 
 def _get_image_url(driver: webdriver.Chrome) -> str:
     try:
         image_link_wrapper: WebElement = WebDriverWait(driver, 20).until(
             EC.presence_of_element_located((By.ID, "imagelinkwrapper"))
@@ -98,10 +98,8 @@
         "title": _get_title(driver),
         **_get_attributes_from_table(driver),
         "downloadUrl": _get_image_url(driver),
     }
 
 
 def fetch_metadata(query_path: str, metadata_path: str, html_dir: str = None) -> None:
-    return base_fetch_metadata(
-        query_path, metadata_path, _extract_source_data, html_dir
-    )
+    return _fetch_metadata(query_path, metadata_path, _extract_source_data, html_dir)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_fetch_queries.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_fetch_queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,36 @@
 )
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 
 from .._utils.fetch_queries import (
-    fetch_queries as base_fetch_queries,
+    fetch_queries as _fetch_queries,
     Query,
 )
 from ._utils import try_switch_to_replay_iframe
 
 
 def _prefix_href(href: Union[str, None], driver: webdriver.Chrome) -> Union[str, None]:
     """
     If the drive is currently on a webarchive page,
     add webarchive URL to the href.
     """
 
+    webarchive_url = "https://www.webarchive.org.uk/wayback/archive"
     if href is None:
         return None
+    if href.startswith(webarchive_url):
+        return href
 
-    webarchive_prefix = ""
-    if "https://www.webarchive.org.uk/wayback/archive" in driver.current_url:
-        webarchive_prefix = driver.current_url.split("http:")[0]
-    return f"{webarchive_prefix}{href}"
+    prefix = ""
+    if webarchive_url in driver.current_url:
+        prefix = driver.current_url.split("http:")[0]
+    return f"{prefix}{href}"
 
 
 def _get_next_page_url(driver: webdriver.Chrome) -> Union[str, None]:
     try:
         pagination_element: WebElement = WebDriverWait(driver, 20).until(
             EC.presence_of_element_located((By.ID, "paginationtop"))
         )
@@ -101,8 +104,8 @@
     if next_page_url is not None and next_page_url != "":
         sleep(3)
         queries += _extract_queries(driver, next_page_url)
     return queries
 
 
 def fetch_queries(base_urls: List[str], query_path: str) -> None:
-    base_fetch_queries(base_urls, query_path, _extract_queries)
+    _fetch_queries(base_urls, query_path, _extract_queries)
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_querier.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_querier.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_typing.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The type declarations specific to the `Telefact` data source.
 """
 
 from typing import TypedDict
 
-from libquery.typing import MetadataEntry as BaseMetadataEntry
+from libquery.typing import MetadataEntry as _MetadataEntry
 from typing_extensions import NotRequired
 
 SourceData = TypedDict(
     "SourceData",
     {
         "title": str,
         "Medium": str,
@@ -20,11 +20,11 @@
         "Width": NotRequired[str],
         "Length": NotRequired[str],
         "Map scale ratio": NotRequired[str],
     },
 )
 
 
-class MetadataEntry(BaseMetadataEntry):
+class MetadataEntry(_MetadataEntry):
     """The data structure of an entry in the metadata."""
 
     sourceData: SourceData
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/british_library/online_gallery/_utils.py` & `libquery_extensions-0.1.1/libquery_extensions/british_library/online_gallery/_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from selenium import webdriver
-from selenium.webdriver.common.by import By
 from selenium.common.exceptions import TimeoutException
+from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
 
 def try_switch_to_replay_iframe(driver: webdriver.Chrome) -> None:
     """
     Get into the replay iframe that present when the webpage is
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/get_chrome_driver.py` & `libquery_extensions-0.1.1/libquery_extensions/get_chrome_driver.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/telefact/_fetch_metadata.py` & `libquery_extensions-0.1.1/libquery_extensions/telefact/_fetch_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     return {
         "year": year,
         "month": month,
         "day": day,
     }
 
 
-def __get_id_in_source(query: str) -> str:
+def _get_id_in_source(query: str) -> str:
     """Extract idInSource from the query."""
     return query.split("/")[-2]
 
 
 def _parse(response: Response) -> MetadataEntry:
     """
     Parse metadata of entries in Telefact.
@@ -117,15 +117,15 @@
     try:
         image_url = _get_image_url(html_text)
         publish_date = _get_publish_date(html_text)
     except Exception as e:
         raise ValueError(f"Fail to parse url: {response.url}") from e
 
     source = "Telefact"
-    id_in_source = __get_id_in_source(response.url)
+    id_in_source = _get_id_in_source(response.url)
 
     return {
         "uuid": str(uuid5(UUID(int=0), f"{source}/{id_in_source}")),
         "url": response.url,
         "source": source,
         "idInSource": id_in_source,
         "accessDate": datetime.now(timezone.utc).isoformat(),
```

### Comparing `libquery_extensions-0.1.0/libquery_extensions/telefact/_querier.py` & `libquery_extensions-0.1.1/libquery_extensions/telefact/_querier.py`

 * *Files identical despite different names*

### Comparing `libquery_extensions-0.1.0/libquery_extensions/telefact/_typing.py` & `libquery_extensions-0.1.1/libquery_extensions/telefact/_typing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 The type declarations specific to the `Telefact` data source.
 """
 
 from typing import List, Literal, TypedDict
 
 from typing_extensions import NotRequired
-from libquery.typing import MetadataEntry as BaseMetadataEntry
+from libquery.typing import MetadataEntry as _MetadataEntry
 
 
 class TimePoint(TypedDict):
     """The time point data structure."""
 
     year: int
     month: NotRequired[int]
@@ -21,11 +21,11 @@
 
     authors: List[Literal["Modley, Rudolf"]]
     publishDate: TimePoint
     downloadUrl: str
     languages: List[Literal["eng"]]
 
 
-class MetadataEntry(BaseMetadataEntry):
+class MetadataEntry(_MetadataEntry):
     """The data structure of an entry in the metadata."""
 
     sourceData: SourceData
```

### Comparing `libquery_extensions-0.1.0/pyproject.toml` & `libquery_extensions-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "libquery-extensions"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Yu Zhang <yuzhang94@outlook.com>"]
 readme = "README.md"
 packages = [{include = "libquery_extensions"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 backoff = "^2.2.1"
 tqdm = "^4.65.0"
 webdriver-manager = "^3.8.6"
 typing-extensions = "^4.7.1"
 cssutils = "^2.7.1"
-libquery = "^0.1.0"
 selenium = "^4.10.0"
+libquery = "^0.1.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `libquery_extensions-0.1.0/PKG-INFO` & `libquery_extensions-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: libquery-extensions
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Yu Zhang
 Author-email: yuzhang94@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cssutils (>=2.7.1,<3.0.0)
-Requires-Dist: libquery (>=0.1.0,<0.2.0)
+Requires-Dist: libquery (>=0.1.1,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: selenium (>=4.10.0,<5.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: libquery-extensions Version: 0.1.0 Summary: Author:
+Metadata-Version: 2.1 Name: libquery-extensions Version: 0.1.1 Summary: Author:
 Yu Zhang Author-email: yuzhang94@outlook.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backoff (>=2.2.1,<3.0.0) Requires-Dist: cssutils
-(>=2.7.1,<3.0.0) Requires-Dist: libquery (>=0.1.0,<0.2.0) Requires-Dist:
+(>=2.7.1,<3.0.0) Requires-Dist: libquery (>=0.1.1,<0.2.0) Requires-Dist:
 requests (>=2.31.0,<3.0.0) Requires-Dist: selenium (>=4.10.0,<5.0.0) Requires-
 Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Requires-Dist: webdriver-manager (>=3.8.6,<4.0.0) Description-Content-Type:
 text/markdown [Newest_PyPI_version] [Code_style:_black] [Commitizen_friendly] #
 libquery_extensions Extensions to [libquery](https://github.com/oldvis/
 libquery). ## Installation ```sh pip install libquery_extensions ``` ##
 Documentation See our [documentation website](https://oldvis.github.io/
```

