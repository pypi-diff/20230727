# Comparing `tmp/harrier-0.8.tar.gz` & `tmp/harrier-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/harrier-0.8.tar", last modified: Thu Mar 14 14:47:53 2019, max compression
+gzip compressed data, was "dist/harrier-0.9.tar", last modified: Fri May 24 16:28:17 2019, max compression
```

## Comparing `harrier-0.8.tar` & `harrier-0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-14 14:47:53.000000 harrier-0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      573 2019-03-14 14:46:55.000000 harrier-0.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1883 2019-03-14 14:46:55.000000 harrier-0.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      194 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      478 2019-03-14 14:47:53.000000 harrier-0.8/harrier.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2019-03-14 14:47:53.000000 harrier-0.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2019-03-14 14:47:53.000000 harrier-0.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-14 14:47:53.000000 harrier-0.8/harrier/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2935 2019-03-14 14:46:55.000000 harrier-0.8/harrier/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6722 2019-03-14 14:46:55.000000 harrier-0.8/harrier/build.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1946 2019-03-14 14:46:55.000000 harrier-0.8/harrier/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2328 2019-03-14 14:46:55.000000 harrier-0.8/harrier/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10746 2019-03-14 14:46:55.000000 harrier-0.8/harrier/render.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-03-14 14:46:55.000000 harrier-0.8/harrier/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6111 2019-03-14 14:46:55.000000 harrier-0.8/harrier/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-03-14 14:46:55.000000 harrier-0.8/harrier/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7930 2019-03-14 14:46:55.000000 harrier-0.8/harrier/extensions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7725 2019-03-14 14:46:55.000000 harrier-0.8/harrier/assets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4200 2019-03-14 14:46:55.000000 harrier-0.8/harrier/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9477 2019-03-14 14:46:55.000000 harrier-0.8/harrier/dev.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2068 2019-03-14 14:46:55.000000 harrier-0.8/harrier/frontmatter.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 16:28:17.000000 harrier-0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      573 2019-05-24 16:27:23.000000 harrier-0.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1883 2019-05-24 16:27:23.000000 harrier-0.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      194 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       63 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      478 2019-05-24 16:28:17.000000 harrier-0.9/harrier.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      250 2019-05-24 16:28:17.000000 harrier-0.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1438 2019-05-24 16:28:17.000000 harrier-0.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-05-24 16:28:17.000000 harrier-0.9/harrier/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2935 2019-05-24 16:27:23.000000 harrier-0.9/harrier/main.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6728 2019-05-24 16:27:23.000000 harrier-0.9/harrier/build.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1946 2019-05-24 16:27:23.000000 harrier-0.9/harrier/data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2328 2019-05-24 16:27:23.000000 harrier-0.9/harrier/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10763 2019-05-24 16:27:23.000000 harrier-0.9/harrier/render.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2019-05-24 16:27:23.000000 harrier-0.9/harrier/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6111 2019-05-24 16:27:23.000000 harrier-0.9/harrier/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-05-24 16:27:23.000000 harrier-0.9/harrier/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7930 2019-05-24 16:27:23.000000 harrier-0.9/harrier/extensions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7725 2019-05-24 16:27:23.000000 harrier-0.9/harrier/assets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4456 2019-05-24 16:27:23.000000 harrier-0.9/harrier/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9477 2019-05-24 16:27:23.000000 harrier-0.9/harrier/dev.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2068 2019-05-24 16:27:23.000000 harrier-0.9/harrier/frontmatter.py
```

### Comparing `harrier-0.8/README.rst` & `harrier-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `harrier-0.8/setup.py` & `harrier-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier.egg-info/PKG-INFO` & `harrier-0.9/harrier.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: harrier
-Version: 0.8
+Version: 0.9
 Summary: Static site generator
 Home-page: https://github.com/samuelcolvin/harrier
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Description: harrier
         =======
```

### Comparing `harrier-0.8/PKG-INFO` & `harrier-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: harrier
-Version: 0.8
+Version: 0.9
 Summary: Static site generator
 Home-page: https://github.com/samuelcolvin/harrier
 Author: Samuel Colvin
 Author-email: s@muelcolvin.com
 License: MIT
 Description: harrier
         =======
```

### Comparing `harrier-0.8/harrier/main.py` & `harrier-0.9/harrier/main.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier/build.py` & `harrier-0.9/harrier/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime
 from pathlib import Path
 from time import time
 from typing import Optional
 
 from pydantic import BaseModel, validator
 
-from .common import URI_NOT_ALLOWED, HarrierProblem, clean_uri, log_complete, norm_path_ref, slugify
+from .common import RE_URI_NOT_ALLOWED, HarrierProblem, clean_uri, log_complete, norm_path_ref, slugify
 from .config import Config
 from .extensions import ExtensionError
 from .frontmatter import parse_front_matter, parse_yaml
 
 # extensions where we want to do anything except just copy the file to the output dir
 OUTPUT_HTML = {'.html', '.md', '.yml', '.yaml'}
 YAML_FILE = {'.yml', '.yaml'}
@@ -183,15 +183,15 @@
     uri: str
     template: Optional[str]
 
     @validator('uri')
     def validate_uri(cls, v):
         if not v.startswith('/'):
             raise ValueError(f'uri must start with a slash: "{v}')
-        invalid = URI_NOT_ALLOWED.findall(v)
+        invalid = RE_URI_NOT_ALLOWED.findall(v)
         if invalid:
             invalid = ', '.join(f'"{inv}"' for inv in invalid)
             raise ValueError(f'uri contains invalid characters: {invalid}')
         return v
 
     class Config:
         allow_extra = True
```

### Comparing `harrier-0.8/harrier/data.py` & `harrier-0.9/harrier/data.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier/cli.py` & `harrier-0.9/harrier/cli.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier/render.py` & `harrier-0.9/harrier/render.py`

 * *Files identical despite different names*

```diff
@@ -191,15 +191,15 @@
         elif is_ordered:
             return f'<ol>\n{content}</ol>'
         else:
             return f'<ul>\n{content}</ul>'
 
     @staticmethod
     def header(content, level):
-        return f'<h{level} id="{level}-{slugify(content)}">{content}</h{level}>\n'
+        return f'<h{level} id="{level}-{slugify(content, path_like=False)}">{content}</h{level}>\n'
 
     @staticmethod
     def triple_emphasis(content):
         return f'<u>{content}</u>'
 
 
 def get_outfile(data: dict, config: Config):
```

### Comparing `harrier-0.8/harrier/config.py` & `harrier-0.9/harrier/config.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier/extensions.py` & `harrier-0.9/harrier/extensions.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier/assets.py` & `harrier-0.9/harrier/assets.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier/common.py` & `harrier-0.9/harrier/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from time import time
 
 import click
 from pydantic.validators import str_validator
 from ruamel.yaml import YAML
 
 yaml = YAML(typ='safe')
-URI_NOT_ALLOWED = re.compile(r'[^a-zA-Z0-9_\-/.]')
 completed_logger = logging.getLogger('harrier.completed')
 
 
 class HarrierProblem(RuntimeError):
     pass
 
 
@@ -48,19 +47,28 @@
         return cls(value)
 
 
 def norm_path_ref(p: Path, rel: Path):
     return '/' + normcase(str(p.relative_to(rel)))
 
 
-def slugify(title):
-    name = title.replace(' ', '-').lower()
-    name = URI_NOT_ALLOWED.sub('', name)
-    name = re.sub('-{2,}', '-', name)
-    return name.strip('_-')
+RE_URI_NOT_ALLOWED = re.compile(r'[^a-zA-Z0-9_\-/.]')
+RE_HTML_SYMBOL = re.compile(r'&(?:#\d{2,}|[a-z0-9]{2,});')
+RE_TITLE_NOT_ALLOWED = re.compile(r'[^a-z0-9_\-]')
+RE_REPEAT_DASH = re.compile(r'-{2,}')
+
+
+def slugify(v, *, path_like=True):
+    v = v.replace(' ', '-').lower()
+    if path_like:
+        v = RE_URI_NOT_ALLOWED.sub('', v)
+    else:
+        v = RE_HTML_SYMBOL.sub('', v)
+        v = RE_TITLE_NOT_ALLOWED.sub('', v)
+    return RE_REPEAT_DASH.sub('-', v).strip('_-')
 
 
 def clean_uri(uri, config):
     if uri == '':
         return '/'
     uri = uri.strip('/')
     if config.apply_trailing_slash and '.' not in uri.rsplit('/', 1)[-1]:
```

### Comparing `harrier-0.8/harrier/dev.py` & `harrier-0.9/harrier/dev.py`

 * *Files identical despite different names*

### Comparing `harrier-0.8/harrier/frontmatter.py` & `harrier-0.9/harrier/frontmatter.py`

 * *Files identical despite different names*

