# Comparing `tmp/e-models-1.5.1.tar.gz` & `tmp/e-models-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.5.1.tar", last modified: Fri Jul 21 18:31:03 2023, max compression
+gzip compressed data, was "e-models-1.5.2.tar", last modified: Thu Jul 27 16:16:57 2023, max compression
```

## Comparing `e-models-1.5.1.tar` & `e-models-1.5.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.335693 e-models-1.5.1/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.1/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-21 18:31:03.335693 e-models-1.5.1/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-06-01 14:06:43.000000 e-models-1.5.1/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-07-21 18:31:03.000000 e-models-1.5.1/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-07-21 18:28:43.000000 e-models-1.5.1/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/datasets/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.1/emodels/datasets/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12161 2023-07-05 14:16:27.000000 e-models-1.5.1/emodels/datasets/models.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.1/emodels/datasets/tokenizers.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4716 2023-06-23 22:38:40.000000 e-models-1.5.1/emodels/datasets/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.1/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/html2text/utils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.1/emodels/py.typed
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.331693 e-models-1.5.1/emodels/scrapyutils/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.1/emodels/scrapyutils/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-21 17:45:38.000000 e-models-1.5.1/emodels/scrapyutils/loader.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 18:26:42.000000 e-models-1.5.1/emodels/scrapyutils/response.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.1/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-07-21 18:31:03.335693 e-models-1.5.1/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      907 2023-07-21 18:28:27.000000 e-models-1.5.1/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-21 18:31:03.335693 e-models-1.5.1/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.1/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8260 2023-07-21 18:10:59.000000 e-models-1.5.1/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.718224 e-models-1.5.2/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.5.2/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-27 16:16:57.718224 e-models-1.5.2/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2928 2023-07-25 17:58:30.000000 e-models-1.5.2/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3468 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      655 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       62 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-07-27 16:16:57.000000 e-models-1.5.2/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       22 2023-07-27 16:16:25.000000 e-models-1.5.2/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-07-26 22:24:33.000000 e-models-1.5.2/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/datasets/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-06-23 18:11:59.000000 e-models-1.5.2/emodels/datasets/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    12135 2023-07-27 14:36:45.000000 e-models-1.5.2/emodels/datasets/models.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1929 2023-07-05 14:16:56.000000 e-models-1.5.2/emodels/datasets/tokenizers.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6935 2023-07-27 13:48:16.000000 e-models-1.5.2/emodels/datasets/utils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    35479 2023-07-21 16:26:32.000000 e-models-1.5.2/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.5.2/emodels/py.typed
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.714224 e-models-1.5.2/emodels/scrapyutils/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      137 2023-06-23 22:04:28.000000 e-models-1.5.2/emodels/scrapyutils/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2575 2023-07-26 22:24:33.000000 e-models-1.5.2/emodels/scrapyutils/loader.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6000 2023-07-21 19:40:03.000000 e-models-1.5.2/emodels/scrapyutils/response.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.5.2/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-07-27 16:16:57.718224 e-models-1.5.2/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1017 2023-07-27 16:16:20.000000 e-models-1.5.2/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-07-27 16:16:57.718224 e-models-1.5.2/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6346 2023-07-21 17:31:24.000000 e-models-1.5.2/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8234 2023-07-26 22:27:27.000000 e-models-1.5.2/tests/test_scrapyutils.py
```

### Comparing `e-models-1.5.1/LICENSE` & `e-models-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/PKG-INFO` & `e-models-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.1
+Version: 1.5.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.1/README.md` & `e-models-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/e_models.egg-info/PKG-INFO` & `e-models-1.5.2/e_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.5.1
+Version: 1.5.2
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.5.1/e_models.egg-info/SOURCES.txt` & `e-models-1.5.2/e_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/emodels/datasets/models.py` & `e-models-1.5.2/emodels/datasets/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 """
 import logging
 from abc import abstractmethod
-from typing import get_args, Generator, List, TypedDict, NewType, Any, Protocol
+from typing import Generator, List, TypedDict, Any, Protocol, Tuple
 
 import joblib
 from scrapy.http import HtmlResponse
 import pandas as pd
 from sklearn.metrics import (
     accuracy_score,
     recall_score,
@@ -34,16 +34,14 @@
 )
 from emodels.datasets.utils import WebsiteSampleData
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
-TargetLabel = NewType("TargetLabel", str)
-
 
 class ModelFilename(Filename):
     pass
 
 
 class VectorizerFilename(Filename):
     pass
@@ -57,41 +55,45 @@
 
 
 class ModelWithDataset(Protocol):
     FSHELPER: FSHelper = None
     datasets: DatasetsDict | None = None
 
     dataset_repository: DatasetFilename
-    target_label: TargetLabel
+    features: Tuple[str, ...]
+    target_label: str
     project: str
 
+    def __init__(self):
+        raise ValueError("Class must not be instantiated.")
+
     @classmethod
     @abstractmethod
     def build_fshelper(cls, settings) -> FSHelper:
         ...
 
     @classmethod
     def _fshelper(cls) -> FSHelper:
         if cls.FSHELPER is None:
             settings = get_project_settings()
             cls.FSHELPER = cls.build_fshelper(settings)
         return cls.FSHELPER
 
     @classmethod
     def get_dataset_from_filename(cls, filename: DatasetFilename) -> DatasetsDict:
-        df = pd.read_json(filename, lines=True, compression="gzip").drop("manually_labelled", axis=1)
+        df = pd.read_json(filename, lines=True, compression="gzip")
         df = df[~df[cls.target_label].isnull()]
 
         df_train = df[df.dataset_bucket == "train"].drop("dataset_bucket", axis=1)
         df_test = df[df.dataset_bucket == "test"].drop("dataset_bucket", axis=1)
 
-        df_X_train = df_train.drop(list(get_args(TargetLabel)), axis=1)
+        df_X_train = df_train[list(cls.features)]
         df_Y_train = df_train[cls.target_label]
 
-        df_X_test = df_test.drop(list(get_args(TargetLabel)), axis=1)
+        df_X_test = df_test[list(cls.features)]
         df_Y_test = df_test[cls.target_label]
 
         return {
             "X_train": df_X_train,
             "X_test": df_X_test,
             "Y_train": df_Y_train,
             "Y_test": df_Y_test,
```

### Comparing `e-models-1.5.1/emodels/datasets/tokenizers.py` & `e-models-1.5.2/emodels/datasets/tokenizers.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/emodels/datasets/utils.py` & `e-models-1.5.2/emodels/datasets/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,29 +2,31 @@
 """
 import os
 import abc
 import gzip
 import json
 import logging
 from random import random
-from typing import List, Literal, Tuple, Protocol, cast, Dict, Any, IO
+from typing import List, Literal, Tuple, Protocol, cast, Dict, Any, IO, Optional
 
-from typing_extensions import TypedDict
+from typing_extensions import Self, TypedDict
+from shub_workflow.deliver.futils import exists
 from scrapy.http import TextResponse
 import lxml.html
 
-from emodels.config import EMODELS_DIR
+from emodels.config import EMODELS_DIR, EMODELS_ITEMS_DIR
 
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
 NO_TEXT_TAGS = ["script", "style", "noscript"]
 
 DatasetBucket = Literal["train", "validation", "test"]
+DEFAULT_DATASET_RATIO = (0.67, 0.33)
 
 
 class Filename(str):
     """
     A class that represents a filename.
 
     This class provides a number of methods for working with filenames,
@@ -39,14 +41,15 @@
     >>> filename.basename
     'file.txt'
     >>> filename.local("myproject")
     '/home/myuser/.datasets/myproject/file.txt'
     >>> with filename.open() as f:
     ...     contents = f.read()
     """
+
     @property
     def basename(self):
         return self.__class__(os.path.basename(self))
 
     def local(self, project_name: str):
         """
         Creates a local standard path to find a copy of the source file.
@@ -54,20 +57,32 @@
         basedir = os.path.join(EMODELS_DIR, project_name)
         os.makedirs(basedir, exist_ok=True)
         return self.__class__(os.path.join(basedir, self.basename))
 
     def open(self, mode="rt"):
         return open(self, mode)
 
+    @classmethod
+    def local_by_name(cls, name: str, project_name: str) -> Self:
+        """
+        Returns a Filename object by name and project.
+        """
+        return cls(os.path.join(EMODELS_DIR, project_name, f"{name}.jl.gz"))
+
+    def delete_local(self, project_name: str):
+        os.remove(self.local(project_name))
+
 
 class DatasetFilename(Filename):
     """
     A class that represents a dataset filename. Datasets are gzipped
-    and have json lines format
+    and have json lines format, They are iterable and has a method
+    append() in order to add new samples.
     """
+
     _file: None | IO
 
     def __new__(cls, text):
         obj = super().__new__(cls, text)
         obj._file = None
         return obj
 
@@ -84,30 +99,67 @@
         return json.loads(line)
 
     def append(self, data: Dict[str, Any]):
         assert not self._file, "Already opened."
         with self.open("at") as fz:
             print(json.dumps(data), file=fz)
 
+    @classmethod
+    def build_from_items(
+        cls,
+        name: str,
+        project: str,
+        classes: Optional[Tuple[str]] = None,
+        dataset_ratio: Tuple[float, ...] = DEFAULT_DATASET_RATIO,
+    ) -> Self:
+        """
+        Build a dataset dict from extracted items in user dataset folder.
+        - name is a name for the dataset. It will determine the storing filename.
+        - project is the name of the project the dataset belongs to. It will determine the storing filename.
+        - If classes is a tuple of strings, select only the specified
+        item subfolders.
+        - dataset_ratio is the same for get_random_dataset() and determines how samples are distributed
+          among train, test and validation buckets.
+        """
+        result = cls.local_by_name(name, project)
+        if exists(result):
+            raise ValueError(
+                "Output file already exists. "
+                f'open with {cls.__name__}.local_by_name("{name}", "{project}") or remove it for rebuilding'
+            )
+        for sf in os.listdir(EMODELS_ITEMS_DIR):
+            for f in os.listdir(os.path.join(EMODELS_ITEMS_DIR, sf)):
+                df = DatasetFilename(os.path.join(EMODELS_ITEMS_DIR, sf, f))
+                for sample in df:
+                    sample["dataset_bucket"] = get_random_dataset(dataset_ratio)
+                    result.append(sample)
+        return result
+
 
 class WebsiteSampleData(TypedDict):
     url: str
     body: str
     status: int
 
 
 class WebsiteDatasetFilename(DatasetFilename):
     """
     Website Datasets contain a collection of WebsiteSampleData
     """
+
     def __next__(self) -> WebsiteSampleData:
         return cast(WebsiteSampleData, super().__next__())
 
 
-def get_random_dataset(dataset_ratio: Tuple[float, ...] = (0.6, 0.4)) -> DatasetBucket:
+def get_random_dataset(dataset_ratio: Tuple[float, ...] = DEFAULT_DATASET_RATIO) -> DatasetBucket:
+    """
+    - dataset_ratio: a 2-tuple of floats. The first element is the probability to yield "train",
+      and the second element the probability to yield "test". If they sum below 1, the remaining
+      is the probability to yield "validation".
+    """
     assert len(dataset_ratio) == 2, "Invalid dataset_ratio len: must be 2."
     r = random()
     if r < dataset_ratio[0]:
         return "train"
     if r < sum(dataset_ratio):
         return "test"
     return "validation"
```

### Comparing `e-models-1.5.1/emodels/html2text/__init__.py` & `e-models-1.5.2/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/emodels/html2text/config.py` & `e-models-1.5.2/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/emodels/html2text/utils.py` & `e-models-1.5.2/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/emodels/scrapyutils/loader.py` & `e-models-1.5.2/emodels/scrapyutils/loader.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/emodels/scrapyutils/response.py` & `e-models-1.5.2/emodels/scrapyutils/response.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/setup.py` & `e-models-1.5.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.5.1',
+    version      = '1.5.2',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
     packages     = find_packages(),
     install_requires=(
+        "datasets",
+        "scikit-learn",
         "scrapy",
+        "sentencepiece",
+        "torch",
+        "transformers",
     ),
     scripts = [],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
```

### Comparing `e-models-1.5.1/tests/test_html2text.py` & `e-models-1.5.2/tests/test_html2text.py`

 * *Files identical despite different names*

### Comparing `e-models-1.5.1/tests/test_scrapyutils.py` & `e-models-1.5.2/tests/test_scrapyutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 from unittest import TestCase
 from typing import Dict
 
 from itemloaders.processors import TakeFirst
 from scrapy import Item, Field
 from scrapy.http import TextResponse
 
-os.environ["EMODELS_SAVE_EXTRACT_ITEMS"] = "1"
-os.environ["EMODELS_DIR"] = os.path.dirname(__file__)
+from emodels import config
+from emodels.scrapyutils.loader import ExtractItemLoader
+from emodels.scrapyutils.response import COMMENT_RE, ExtractTextResponse
+from emodels.datasets.utils import DatasetFilename, build_response_from_sample_data
 
-from emodels import config  # noqa
-from emodels.scrapyutils.loader import ExtractItemLoader  # noqa
-from emodels.scrapyutils.response import COMMENT_RE, ExtractTextResponse  # noqa
-from emodels.datasets.utils import DatasetFilename, build_response_from_sample_data  # noqa
 
-
-class JobItem(Item):
+class JobItemTest(Item):
     job_title = Field()
     description = Field()
     url = Field()
     employment_type = Field()
     apply_url = Field()
     job_id = Field()
     publication_date = Field()
@@ -32,52 +29,55 @@
     state = Field()
     country = Field()
     response = Field()
     locality = Field()
 
 
 class JobItemLoader(ExtractItemLoader):
-    default_item_class = JobItem
+    default_item_class = JobItemTest
     default_output_processor = TakeFirst()
 
 
-class BusinessSearchItem(Item):
+class BusinessSearchItemTest(Item):
     name = Field()
     phone = Field()
     website = Field()
     address = Field()
     profile_url = Field()
     category = Field()
     locality = Field()
     street = Field()
     postal_code = Field()
     address_alt = Field()
 
 
 class BusinessSearchItemLoader(ExtractItemLoader):
-    default_item_class = BusinessSearchItem
+    default_item_class = BusinessSearchItemTest
     default_output_processor = TakeFirst()
 
 
 class ScrapyUtilsTests(TestCase):
-    jobs_result_file = DatasetFilename(os.path.join(config.EMODELS_DIR, "items/JobItem/0.jl.gz"))
-    business_result_file = DatasetFilename(os.path.join(config.EMODELS_DIR, "items/BusinessSearchItem/0.jl.gz"))
+    jobs_result_file = DatasetFilename(os.path.join(config.EMODELS_DIR, "items/JobItemTest/0.jl.gz"))
+    business_result_file = DatasetFilename(os.path.join(config.EMODELS_DIR, "items/BusinessSearchItemTest/0.jl.gz"))
     samples_file = DatasetFilename(os.path.join(os.path.dirname(__file__), "samples.jl.gz"))
     samples: Dict[str, TextResponse]
 
     @classmethod
     def setUpClass(cls):
         cls.samples = {d["url"]: build_response_from_sample_data(d) for d in cls.samples_file}
 
     def tearDown(self):
         for col in "jobs", "business":
             fname = getattr(self, f"{col}_result_file")
             dname = os.path.dirname(fname)
-            for f in os.listdir(dname):
-                os.remove(os.path.join(dname, f))
+            try:
+                for f in os.listdir(dname):
+                    os.remove(os.path.join(dname, f))
+            except FileNotFoundError:
+                pass
 
     def test_case_one(self):
         tresponse = self.samples["https://careers.und.edu/jobs/job21.html"]
         loader = JobItemLoader(response=tresponse)
         loader.add_text_re("job_title", tid="#job_title_2_2")
         loader.add_text_re("employment_type", tid="#employment_type_2_2_0_0")
         loader.add_text_re("job_id", tid="#requisition_identifier_2_2_0")
```

