# Comparing `tmp/pyjlyric-1.0.0.tar.gz` & `tmp/pyjlyric-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjlyric-1.0.0.tar", max compression
+gzip compressed data, was "pyjlyric-1.1.0.tar", max compression
```

## Comparing `pyjlyric-1.0.0.tar` & `pyjlyric-1.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1076 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/LICENSE
--rw-r--r--   0        0        0     2676 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/README.md
--rw-r--r--   0        0        0      156 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/__init__.py
--rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/animap/__init__.py
--rw-r--r--   0        0        0      144 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/animap/model.py
--rw-r--r--   0        0        0     2201 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/animap/parser.py
--rw-r--r--   0        0        0      817 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/base.py
--rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/evesta/__init__.py
--rw-r--r--   0        0        0      203 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/evesta/model.py
--rw-r--r--   0        0        0     2466 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/evesta/parser.py
--rw-r--r--   0        0        0      133 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/gakki/__init__.py
--rw-r--r--   0        0        0      164 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/gakki/model.py
--rw-r--r--   0        0        0     2589 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/gakki/parser.py
--rw-r--r--   0        0        0      133 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/hoick/__init__.py
--rw-r--r--   0        0        0      648 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/hoick/model.py
--rw-r--r--   0        0        0     2557 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/hoick/parser.py
--rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jlyric/__init__.py
--rw-r--r--   0        0        0      203 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jlyric/model.py
--rw-r--r--   0        0        0     3107 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jlyric/parser.py
--rw-r--r--   0        0        0      145 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/joysound/__init__.py
--rw-r--r--   0        0        0     4363 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/joysound/model.py
--rw-r--r--   0        0        0     2426 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/joysound/parser.py
--rw-r--r--   0        0        0      137 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jtotal/__init__.py
--rw-r--r--   0        0        0      165 2023-07-17 12:54:28.659412 pyjlyric-1.0.0/pyjlyric/jtotal/model.py
--rw-r--r--   0        0        0     2717 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/jtotal/parser.py
--rw-r--r--   0        0        0      149 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/kashinavi/__init__.py
--rw-r--r--   0        0        0      890 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/kashinavi/model.py
--rw-r--r--   0        0        0     2599 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/kashinavi/parser.py
--rw-r--r--   0        0        0     1606 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/main.py
--rw-r--r--   0        0        0      681 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/model.py
--rw-r--r--   0        0        0      149 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/musicbook/__init__.py
--rw-r--r--   0        0        0      529 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/musicbook/model.py
--rw-r--r--   0        0        0     3063 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/musicbook/parser.py
--rw-r--r--   0        0        0     2713 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/parse.py
--rw-r--r--   0        0        0      157 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/petitlyrics/__init__.py
--rw-r--r--   0        0        0      985 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/petitlyrics/model.py
--rw-r--r--   0        0        0     3538 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/petitlyrics/parser.py
--rw-r--r--   0        0        0        0 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/py.typed
--rw-r--r--   0        0        0      137 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utamap/__init__.py
--rw-r--r--   0        0        0      144 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utamap/model.py
--rw-r--r--   0        0        0     2084 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utamap/parser.py
--rw-r--r--   0        0        0      137 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utanet/__init__.py
--rw-r--r--   0        0        0      275 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utanet/model.py
--rw-r--r--   0        0        0     3274 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utanet/parser.py
--rw-r--r--   0        0        0      137 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utaten/__init__.py
--rw-r--r--   0        0        0      275 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utaten/model.py
--rw-r--r--   0        0        0     4173 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/utaten/parser.py
--rw-r--r--   0        0        0     2943 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyjlyric/util.py
--rw-r--r--   0        0        0     2120 2023-07-17 12:54:28.663412 pyjlyric-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3652 1970-01-01 00:00:00.000000 pyjlyric-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-27 16:56:00.644005 pyjlyric-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2676 2023-07-27 16:56:00.644005 pyjlyric-1.1.0/README.md
+-rw-r--r--   0        0        0      156 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/__init__.py
+-rw-r--r--   0        0        0      137 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/animap/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/animap/model.py
+-rw-r--r--   0        0        0     2201 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/animap/parser.py
+-rw-r--r--   0        0        0      817 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/base.py
+-rw-r--r--   0        0        0      137 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/evesta/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/evesta/model.py
+-rw-r--r--   0        0        0     2466 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/evesta/parser.py
+-rw-r--r--   0        0        0      133 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/gakki/__init__.py
+-rw-r--r--   0        0        0      164 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/gakki/model.py
+-rw-r--r--   0        0        0     2589 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/gakki/parser.py
+-rw-r--r--   0        0        0      133 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/hoick/__init__.py
+-rw-r--r--   0        0        0      648 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/hoick/model.py
+-rw-r--r--   0        0        0     2557 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/hoick/parser.py
+-rw-r--r--   0        0        0      137 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/jlyric/__init__.py
+-rw-r--r--   0        0        0      203 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/jlyric/model.py
+-rw-r--r--   0        0        0     3107 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/jlyric/parser.py
+-rw-r--r--   0        0        0      145 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/joysound/__init__.py
+-rw-r--r--   0        0        0     4363 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/joysound/model.py
+-rw-r--r--   0        0        0     2426 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/joysound/parser.py
+-rw-r--r--   0        0        0      137 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/jtotal/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/jtotal/model.py
+-rw-r--r--   0        0        0     2717 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/jtotal/parser.py
+-rw-r--r--   0        0        0      149 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/kashinavi/__init__.py
+-rw-r--r--   0        0        0      891 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/kashinavi/model.py
+-rw-r--r--   0        0        0     2599 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/kashinavi/parser.py
+-rw-r--r--   0        0        0     1606 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/main.py
+-rw-r--r--   0        0        0      681 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/model.py
+-rw-r--r--   0        0        0      149 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/musicbook/__init__.py
+-rw-r--r--   0        0        0      529 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/musicbook/model.py
+-rw-r--r--   0        0        0     3063 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/musicbook/parser.py
+-rw-r--r--   0        0        0     2713 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/parse.py
+-rw-r--r--   0        0        0      157 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/petitlyrics/__init__.py
+-rw-r--r--   0        0        0      985 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/petitlyrics/model.py
+-rw-r--r--   0        0        0     3538 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/petitlyrics/parser.py
+-rw-r--r--   0        0        0        0 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/py.typed
+-rw-r--r--   0        0        0      137 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utamap/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utamap/model.py
+-rw-r--r--   0        0        0     2084 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utamap/parser.py
+-rw-r--r--   0        0        0      137 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utanet/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utanet/model.py
+-rw-r--r--   0        0        0     3274 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utanet/parser.py
+-rw-r--r--   0        0        0      137 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utaten/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utaten/model.py
+-rw-r--r--   0        0        0     4173 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/utaten/parser.py
+-rw-r--r--   0        0        0     2943 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyjlyric/util.py
+-rw-r--r--   0        0        0     2111 2023-07-27 16:56:00.648006 pyjlyric-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 pyjlyric-1.1.0/PKG-INFO
```

### Comparing `pyjlyric-1.0.0/LICENSE` & `pyjlyric-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/README.md` & `pyjlyric-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/animap/parser.py` & `pyjlyric-1.1.0/pyjlyric/animap/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/base.py` & `pyjlyric-1.1.0/pyjlyric/base.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/evesta/parser.py` & `pyjlyric-1.1.0/pyjlyric/evesta/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/gakki/parser.py` & `pyjlyric-1.1.0/pyjlyric/gakki/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/hoick/model.py` & `pyjlyric-1.1.0/pyjlyric/hoick/model.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/hoick/parser.py` & `pyjlyric-1.1.0/pyjlyric/hoick/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/jlyric/parser.py` & `pyjlyric-1.1.0/pyjlyric/jlyric/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/joysound/model.py` & `pyjlyric-1.1.0/pyjlyric/joysound/model.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/joysound/parser.py` & `pyjlyric-1.1.0/pyjlyric/joysound/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/jtotal/parser.py` & `pyjlyric-1.1.0/pyjlyric/jtotal/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/kashinavi/model.py` & `pyjlyric-1.1.0/pyjlyric/kashinavi/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from pydantic import BaseModel, Field, HttpUrl
 
 from pyjlyric.model import LyricPage, WithUrlText
 
 
 class _ByArtist(BaseModel):
-    _type: str = Field(..., alias="@type")
-    name: str
+    type_: str = Field(..., alias="@type")
+    name_: str
     url: HttpUrl
 
 
 class _RecordedAs(BaseModel):
-    _type: str = Field(..., alias="@type")
+    type_: str = Field(..., alias="@type")
     by_artist: _ByArtist = Field(..., alias="byArtist")
 
 
 class _Lyricist(BaseModel):
-    _type: str = Field(..., alias="@type")
+    type_: str = Field(..., alias="@type")
     name: str
 
 
 class _Composer(BaseModel):
-    _type: str = Field(..., alias="@type")
+    type_: str = Field(..., alias="@type")
     name: str
 
 
 class _MainEntityOfPage(BaseModel):
-    _type: str = Field(..., alias="@type")
+    type_: str = Field(..., alias="@type")
     url: HttpUrl
 
 
 class _Lyrics(BaseModel):
-    _type: str = Field(..., alias="@type")
+    type_: str = Field(..., alias="@type")
     main_entity_of_page: _MainEntityOfPage = Field(..., alias="mainEntityOfPage")
     text: str
 
 
 class KashinaviLyricPage(LyricPage):
     artist: WithUrlText
     composer: str
```

### Comparing `pyjlyric-1.0.0/pyjlyric/kashinavi/parser.py` & `pyjlyric-1.1.0/pyjlyric/kashinavi/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/main.py` & `pyjlyric-1.1.0/pyjlyric/main.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/model.py` & `pyjlyric-1.1.0/pyjlyric/model.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/musicbook/model.py` & `pyjlyric-1.1.0/pyjlyric/musicbook/model.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/musicbook/parser.py` & `pyjlyric-1.1.0/pyjlyric/musicbook/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/parse.py` & `pyjlyric-1.1.0/pyjlyric/parse.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/petitlyrics/model.py` & `pyjlyric-1.1.0/pyjlyric/petitlyrics/model.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/petitlyrics/parser.py` & `pyjlyric-1.1.0/pyjlyric/petitlyrics/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/utamap/parser.py` & `pyjlyric-1.1.0/pyjlyric/utamap/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/utanet/parser.py` & `pyjlyric-1.1.0/pyjlyric/utanet/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/utaten/parser.py` & `pyjlyric-1.1.0/pyjlyric/utaten/parser.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyjlyric/util.py` & `pyjlyric-1.1.0/pyjlyric/util.py`

 * *Files identical despite different names*

### Comparing `pyjlyric-1.0.0/pyproject.toml` & `pyjlyric-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -67,19 +67,19 @@
   "japanese-songs",
 ]
 name = "pyjlyric"
 packages = [{include = "pyjlyric"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/pyjlyric"
-version = "1.0.0"
+version = "1.1.0"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-pydantic = ">=1.10.5,<3.0.0"
+pydantic = "^2.0.2"
 typing-extensions = "^4.5.0"
 requests = "^2.28.2"
 beautifulsoup4 = "^4.11.2"
 lxml = "^4.9.2"
 chardet = "^5.1.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `pyjlyric-1.0.0/PKG-INFO` & `pyjlyric-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjlyric
-Version: 1.0.0
+Version: 1.1.0
 Summary: Japanese Lyric Aggregator
 Home-page: https://github.com/eggplants/pyjlyric
 License: MIT
 Keywords: japanese,lyrics,download-lyrics,lyrics-scraping,japanese-songs
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.9,<3.12
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: lxml (>=4.9.2,<5.0.0)
-Requires-Dist: pydantic (>=1.10.5,<3.0.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/eggplants/pyjlyric
 Description-Content-Type: text/markdown
 
 # pyjlyric: Japanese Lyric Aggregator
```

