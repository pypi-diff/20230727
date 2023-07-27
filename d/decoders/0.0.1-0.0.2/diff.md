# Comparing `tmp/decoders-0.0.1.tar.gz` & `tmp/decoders-0.0.2.tar.gz`

## Comparing `decoders-0.0.1.tar` & `decoders-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,29 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 decoders-0.0.1/__init__.py
--rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 decoders-0.0.1/LICENSE
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 decoders-0.0.1/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 decoders-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 decoders-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 decoders-0.0.2/build_upload.sh
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 decoders-0.0.2/example.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 decoders-0.0.2/.idea/.gitignore
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 decoders-0.0.2/.idea/decoders.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 decoders-0.0.2/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 decoders-0.0.2/.idea/modules.xml
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 decoders-0.0.2/.idea/workspace.xml
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 decoders-0.0.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 decoders-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/__init__.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/fake_transformer.py
+-rw-r--r--   0        0        0    73618 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/utils.py
+-rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/assisted_decoder.py
+-rw-r--r--   0        0        0    64452 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/beam_constrained_decoder.py
+-rw-r--r--   0        0        0    20487 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/beam_sampling_decoder.py
+-rw-r--r--   0        0        0    20749 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/beam_search_decoder.py
+-rw-r--r--   0        0        0    22318 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/beam_utils.py
+-rw-r--r--   0        0        0    28222 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/contrastive_decoder.py
+-rw-r--r--   0        0        0    24000 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/diverse_group_beam_decoder.py
+-rw-r--r--   0        0        0    16092 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/greedy_decoder.py
+-rw-r--r--   0        0        0    17351 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/sampling_decoder.py
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/stochastic_beam_search.py
+-rw-r--r--   0        0        0    33026 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/utils.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/sbs_helpers/gumbel.py
+-rw-r--r--   0        0        0    56757 2020-02-02 00:00:00.000000 decoders-0.0.2/src/decoders/strategies/sbs_helpers/logits_process.py
+-rw-r--r--   0        0        0    11418 2020-02-02 00:00:00.000000 decoders-0.0.2/LICENSE
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 decoders-0.0.2/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 decoders-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 decoders-0.0.2/PKG-INFO
```

### Comparing `decoders-0.0.1/LICENSE` & `decoders-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decoders-0.0.1/pyproject.toml` & `decoders-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "decoders"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Manuel de Prada Corral", email="manueldeprada@gmail.com" },
 ]
 description = "Diverse and extensible generation decoding libraries for transformers."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `decoders-0.0.1/PKG-INFO` & `decoders-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoders
-Version: 0.0.1
+Version: 0.0.2
 Summary: Diverse and extensible generation decoding libraries for transformers.
 Project-URL: Homepage, https://github.com/manueldeprada/decoders
 Author-email: Manuel de Prada Corral <manueldeprada@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

