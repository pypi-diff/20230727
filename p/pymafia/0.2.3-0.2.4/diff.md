# Comparing `tmp/pymafia-0.2.3.tar.gz` & `tmp/pymafia-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymafia-0.2.3.tar", max compression
+gzip compressed data, was "pymafia-0.2.4.tar", max compression
```

## Comparing `pymafia-0.2.3.tar` & `pymafia-0.2.4.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0     1068 2023-07-19 00:19:44.272158 pymafia-0.2.3/LICENSE
--rw-r--r--   0        0        0     5694 2023-07-19 00:19:44.276158 pymafia-0.2.3/README.md
--rw-r--r--   0        0        0     1283 2023-07-19 00:20:21.588134 pymafia-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      390 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/__init__.py
--rw-r--r--   0        0        0      283 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/ash/__init__.py
--rw-r--r--   0        0        0     3251 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/ash/conversion.py
--rw-r--r--   0        0        0     1421 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/ash/library.py
--rw-r--r--   0        0        0     3315 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/combat.py
--rw-r--r--   0        0        0     1527 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/__init__.py
--rw-r--r--   0        0        0     2442 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/bounty.py
--rw-r--r--   0        0        0     1836 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/class_.py
--rw-r--r--   0        0        0     2464 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/coinmaster.py
--rw-r--r--   0        0        0     2526 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/effect.py
--rw-r--r--   0        0        0     2653 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/element.py
--rw-r--r--   0        0        0     6826 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/familiar.py
--rw-r--r--   0        0        0    11495 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/item.py
--rw-r--r--   0        0        0     5338 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/location.py
--rw-r--r--   0        0        0     1813 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/modifier.py
--rw-r--r--   0        0        0     6712 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/monster.py
--rw-r--r--   0        0        0     1976 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/path.py
--rw-r--r--   0        0        0     2772 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/phylum.py
--rw-r--r--   0        0        0     2765 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/servant.py
--rw-r--r--   0        0        0     3160 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/skill.py
--rw-r--r--   0        0        0     2542 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/slot.py
--rw-r--r--   0        0        0     1314 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/stat.py
--rw-r--r--   0        0        0     2610 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/thrall.py
--rw-r--r--   0        0        0     2889 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/datatypes/vykea.py
--rw-r--r--   0        0        0      545 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/__init__.py
--rw-r--r--   0        0        0      583 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/barrel_god.py
--rw-r--r--   0        0        0      890 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/boxing_daycare.py
--rw-r--r--   0        0        0     1350 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/cartography.py
--rw-r--r--   0        0        0     1030 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/cosplay_saber.py
--rw-r--r--   0        0        0     1784 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/crimbo_shrub.py
--rw-r--r--   0        0        0     1286 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/god_lobster.py
--rw-r--r--   0        0        0     1569 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/love_tunnel.py
--rw-r--r--   0        0        0     1044 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/mumming_trunk.py
--rw-r--r--   0        0        0     3518 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/pantogram.py
--rw-r--r--   0        0        0     1597 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/protonic_pack.py
--rw-r--r--   0        0        0     1139 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/snojo.py
--rw-r--r--   0        0        0     1299 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/songboom.py
--rw-r--r--   0        0        0      670 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/stomping_boots.py
--rw-r--r--   0        0        0     1408 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/iotms/witchess.py
--rw-r--r--   0        0        0      125 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/kolmafia/__init__.py
--rw-r--r--   0        0        0     1875 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/kolmafia/kolmafia.py
--rw-r--r--   0        0        0     1504 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/kolmafia/patch.py
--rw-r--r--   0        0        0     1682 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/player.py
--rw-r--r--   0        0        0     1148 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/preference.py
--rw-r--r--   0        0        0     1277 2023-07-19 00:19:44.276158 pymafia-0.2.3/src/pymafia/utils.py
--rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 pymafia-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-27 19:11:31.203307 pymafia-0.2.4/LICENSE
+-rw-r--r--   0        0        0     5694 2023-07-27 19:11:31.203307 pymafia-0.2.4/README.md
+-rw-r--r--   0        0        0     1597 2023-07-27 19:12:08.967238 pymafia-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      327 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/ash/__init__.py
+-rw-r--r--   0        0        0     3794 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/ash/conversion.py
+-rw-r--r--   0        0        0      551 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/ash/function.py
+-rw-r--r--   0        0        0    87892 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/ash/library.py
+-rw-r--r--   0        0        0     3315 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/combat.py
+-rw-r--r--   0        0        0     1527 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/bounty.py
+-rw-r--r--   0        0        0     1847 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/class_.py
+-rw-r--r--   0        0        0     2475 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/coinmaster.py
+-rw-r--r--   0        0        0     2537 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/effect.py
+-rw-r--r--   0        0        0     2664 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/element.py
+-rw-r--r--   0        0        0     6837 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/familiar.py
+-rw-r--r--   0        0        0    11506 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/item.py
+-rw-r--r--   0        0        0     5349 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/location.py
+-rw-r--r--   0        0        0     1824 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/modifier.py
+-rw-r--r--   0        0        0     6723 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/monster.py
+-rw-r--r--   0        0        0     1987 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/path.py
+-rw-r--r--   0        0        0     2783 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/phylum.py
+-rw-r--r--   0        0        0     2776 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/servant.py
+-rw-r--r--   0        0        0     3171 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/skill.py
+-rw-r--r--   0        0        0     2553 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/slot.py
+-rw-r--r--   0        0        0     1325 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/stat.py
+-rw-r--r--   0        0        0     2621 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/thrall.py
+-rw-r--r--   0        0        0     2900 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/datatypes/vykea.py
+-rw-r--r--   0        0        0      545 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/barrel_god.py
+-rw-r--r--   0        0        0      890 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/boxing_daycare.py
+-rw-r--r--   0        0        0     1355 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/cartography.py
+-rw-r--r--   0        0        0     1030 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/cosplay_saber.py
+-rw-r--r--   0        0        0     1784 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/crimbo_shrub.py
+-rw-r--r--   0        0        0     1291 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/god_lobster.py
+-rw-r--r--   0        0        0     1574 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/love_tunnel.py
+-rw-r--r--   0        0        0     1044 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/mumming_trunk.py
+-rw-r--r--   0        0        0     3518 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/pantogram.py
+-rw-r--r--   0        0        0     1597 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/protonic_pack.py
+-rw-r--r--   0        0        0     1139 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/snojo.py
+-rw-r--r--   0        0        0     1299 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/songboom.py
+-rw-r--r--   0        0        0      670 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/stomping_boots.py
+-rw-r--r--   0        0        0     1413 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/iotms/witchess.py
+-rw-r--r--   0        0        0      125 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/kolmafia/__init__.py
+-rw-r--r--   0        0        0     1875 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/kolmafia/kolmafia.py
+-rw-r--r--   0        0        0     1504 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/kolmafia/patch.py
+-rw-r--r--   0        0        0     1682 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/player.py
+-rw-r--r--   0        0        0     1148 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/preference.py
+-rw-r--r--   0        0        0     1872 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia/utils.py
+-rw-r--r--   0        0        0     1264 2023-07-27 19:11:31.203307 pymafia-0.2.4/src/pymafia_config.py
+-rw-r--r--   0        0        0     6366 1970-01-01 00:00:00.000000 pymafia-0.2.4/PKG-INFO
```

### Comparing `pymafia-0.2.3/LICENSE` & `pymafia-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/README.md` & `pymafia-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/pyproject.toml` & `pymafia-0.2.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [tool.poetry]
 name = "pymafia"
-version = "0.2.3"  # This is the standard placeholder for poetry-dynamic-versioning
+version = "0.2.4" # This is the standard placeholder for poetry-dynamic-versioning
 description = "A Python module and bridge for reflecting KoLmafia's Java environment"
 license = "MIT"
 authors = ["MrFizzyBubbs <MrFizzyBubbs@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MrFizzyBubbs/pymafia"
+packages = [
+  { include = "pymafia", from = "src" },
+  { include = "pymafia_config.py", from = "src" },
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 JPype1 = "^1.4.1"
 wrapt = "^1.15.0"
 
 [tool.poetry.group.dev.dependencies]
@@ -25,29 +29,34 @@
 pre-commit = "^3.2.2"
 
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 ignore = [
-  "E501",  # Line too long, handled by black
+  "E501", # Line too long, handled by black
 ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = [
-  "F401",  # Unused import
-  "F403",  # Wildcard import
+  "F401", # Unused import
+  "F403", # Wildcard import
 ]
 "tests/__init__.py" = [
-  "E722",  # Bare except
+  "E722", # Bare except
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
 
+[[tool.mypy.overrides]]
+# Disable error: Overloaded function signature 2 will never be matched: signature 1's parameter type(s) are the same or broader [misc]
+module = "pymafia.ash.library"
+ignore_errors = true
+
 [tool.yamlfix]
 explicit_start = false
 
 [tool.poetry-dynamic-versioning]
 enable = false
 format = "{base}"
 style = "pep440"
```

### Comparing `pymafia-0.2.3/src/pymafia/combat.py` & `pymafia-0.2.4/src/pymafia/combat.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/__init__.py` & `pymafia-0.2.4/src/pymafia/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/bounty.py` & `pymafia-0.2.4/src/pymafia/datatypes/bounty.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Bounty]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.BOUNTY_TYPE.allValues()
         return from_java(values)
 
     @property
     def plural(self) -> str:
         return km.BountyDatabase.getPlural(self.name) or ""
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/class_.py` & `pymafia-0.2.4/src/pymafia/datatypes/class_.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Class]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.CLASS_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def primestat(self) -> Stat:
         from pymafia.datatypes.stat import Stat
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/coinmaster.py` & `pymafia-0.2.4/src/pymafia/datatypes/coinmaster.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Coinmaster]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.COINMASTER_TYPE.allValues()
         return from_java(values)
 
     @property
     def token(self) -> str:
         return self.coinmaster.getToken() if self.coinmaster else ""
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/effect.py` & `pymafia-0.2.4/src/pymafia/datatypes/effect.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Effect]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.EFFECT_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def default(self) -> str:
         return km.EffectDatabase.getDefaultAction(self.id) or ""
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/element.py` & `pymafia-0.2.4/src/pymafia/datatypes/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Element]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.ELEMENT_TYPE.allValues()
         return from_java(values)
 
     @property
     def image(self) -> str:
         # No image for Slime or Supercold in Manuel
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/familiar.py` & `pymafia-0.2.4/src/pymafia/datatypes/familiar.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Familiar]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.FAMILIAR_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def hatchling(self) -> Item:
         from pymafia.datatypes.item import Item
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/item.py` & `pymafia-0.2.4/src/pymafia/datatypes/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Item]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.ITEM_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def tcrs_name(self) -> str:
         """Return the name of the Item as it appears in your current Two Crazy Random Summer run. If you are not in a TCRS run, the regular Item name is returned."""
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/location.py` & `pymafia-0.2.4/src/pymafia/datatypes/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Location]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.LOCATION_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def url(self) -> str:
         return f"adventure.php?snarfblat={self.id}"
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/modifier.py` & `pymafia-0.2.4/src/pymafia/datatypes/modifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Modifier]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.MODIFIER_TYPE.allValues()
         return from_java(values)
 
     @property
     def type_(self) -> ModifierValueType:
         modifier_value_type = (
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/monster.py` & `pymafia-0.2.4/src/pymafia/datatypes/monster.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Monster]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.MONSTER_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def article(self) -> str:
         return self.monster.getArticle() if self.monster is not None else ""
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/path.py` & `pymafia-0.2.4/src/pymafia/datatypes/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Path]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.PATH_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def avatar(self) -> bool:
         return self.ascension_path.isAvatar()
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/phylum.py` & `pymafia-0.2.4/src/pymafia/datatypes/phylum.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Phylum]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.PHYLUM_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def image(self) -> str:
         if self.phylum == km.MonsterDatabase.Phylum.NONE:
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/servant.py` & `pymafia-0.2.4/src/pymafia/datatypes/servant.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Servant]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.SERVANT_TYPE.allValues()
         return from_java(values)
 
     @property
     def servant(self) -> Any:
         return km.EdServantData.findEdServant(self.name)
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/skill.py` & `pymafia-0.2.4/src/pymafia/datatypes/skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Skill]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.SKILL_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def type(self) -> str:
         return km.SkillDatabase.getSkillTypeName(self.id)
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/slot.py` & `pymafia-0.2.4/src/pymafia/datatypes/slot.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Slot]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.SLOT_TYPE.allValues()
         return from_java(values)
 
 
 Slot.NONE = Slot()
 Slot.HAT = Slot("hat")
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/stat.py` & `pymafia-0.2.4/src/pymafia/datatypes/stat.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Stat]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.STAT_TYPE.allValues()
         return from_java(values)
 
 
 Stat.NONE = Stat()
 Stat.MUSCLE = Stat("Muscle")
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/thrall.py` & `pymafia-0.2.4/src/pymafia/datatypes/thrall.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Thrall]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.THRALL_TYPE.allValues()
         return sorted(from_java(values))
 
     @property
     def thrall(self) -> Any:
         return km.KoLCharacter.findPastaThrall(self.type)
```

### Comparing `pymafia-0.2.3/src/pymafia/datatypes/vykea.py` & `pymafia-0.2.4/src/pymafia/datatypes/vykea.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         return f"{type(self).__name__}({str(self)!r})"
 
     def __bool__(self) -> bool:
         return self != type(self)()
 
     @classmethod
     def all(cls) -> list[Vykea]:
-        from pymafia.ash import from_java
+        from pymafia.ash.conversion import from_java
 
         values = km.DataTypes.VYKEA_TYPE.allValues()
         return from_java(values)
 
     @property
     def name(self) -> str:
         return self.companion.getName()
```

### Comparing `pymafia-0.2.3/src/pymafia/iotms/__init__.py` & `pymafia-0.2.4/src/pymafia/iotms/__init__.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/barrel_god.py` & `pymafia-0.2.4/src/pymafia/iotms/barrel_god.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/boxing_daycare.py` & `pymafia-0.2.4/src/pymafia/iotms/boxing_daycare.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/cartography.py` & `pymafia-0.2.4/src/pymafia/iotms/cartography.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,12 @@
     turns = ash.my_turncount()
     while not player.in_combat():
         if ash.my_turncount() > turns:
             raise RuntimeError("Map the Monsters unsuccessful?")
         ash.visit_url(location.url)
         if player.in_choice(1435):
             ash.run_choice(1, False, f"heyscriptswhatsupwinkwink={monster.id}")
-            ash.run_combat(macro)
+            ash.run_combat(str(macro))
             return True
         else:
             ash.run_choice(-1, False)
     return False
```

### Comparing `pymafia-0.2.3/src/pymafia/iotms/cosplay_saber.py` & `pymafia-0.2.4/src/pymafia/iotms/cosplay_saber.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/crimbo_shrub.py` & `pymafia-0.2.4/src/pymafia/iotms/crimbo_shrub.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/god_lobster.py` & `pymafia-0.2.4/src/pymafia/iotms/god_lobster.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     if not have():
         return False
     if fights_left() < 1:
         return False
 
     ash.use_familiar(FAMILIAR)
     ash.visit_url("main.php?fightgodlobster=1")
-    ash.run_combat(macro)
+    ash.run_combat(str(macro))
     ash.run_choice(int(reward))
     return True
```

### Comparing `pymafia-0.2.3/src/pymafia/iotms/love_tunnel.py` & `pymafia-0.2.4/src/pymafia/iotms/love_tunnel.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
     set_property("choiceAdventure1222", 1)  # Entrance
     set_property("choiceAdventure1223", 1)  # Fight LOV Enforcer
     set_property("choiceAdventure1224", int(equipment))
     set_property("choiceAdventure1225", 1)  # Fight LOV Engineer
     set_property("choiceAdventure1226", int(effect))
     set_property("choiceAdventure1227", 1)  # Fight LOV Equivocator
     set_property("choiceAdventure1228", int(item))
-    return ash.adv1(LOCATION, -1, macro)
+    return ash.adv1(LOCATION, -1, str(macro))
```

### Comparing `pymafia-0.2.3/src/pymafia/iotms/mumming_trunk.py` & `pymafia-0.2.4/src/pymafia/iotms/mumming_trunk.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/pantogram.py` & `pymafia-0.2.4/src/pymafia/iotms/pantogram.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/protonic_pack.py` & `pymafia-0.2.4/src/pymafia/iotms/protonic_pack.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/snojo.py` & `pymafia-0.2.4/src/pymafia/iotms/snojo.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/songboom.py` & `pymafia-0.2.4/src/pymafia/iotms/songboom.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/stomping_boots.py` & `pymafia-0.2.4/src/pymafia/iotms/stomping_boots.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/iotms/witchess.py` & `pymafia-0.2.4/src/pymafia/iotms/witchess.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,9 +45,9 @@
     ash.run_choice(1)
     ash.visit_url(
         f"choice.php?option=1&pwd&whichchoice=1182&piece={piece.value.id}",
         False,
     )
     if not player.in_combat(piece.value):
         return False
-    ash.run_combat(macro)
+    ash.run_combat(str(macro))
     return True
```

### Comparing `pymafia-0.2.3/src/pymafia/kolmafia/kolmafia.py` & `pymafia-0.2.4/src/pymafia/kolmafia/kolmafia.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/kolmafia/patch.py` & `pymafia-0.2.4/src/pymafia/kolmafia/patch.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/player.py` & `pymafia-0.2.4/src/pymafia/player.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/preference.py` & `pymafia-0.2.4/src/pymafia/preference.py`

 * *Files identical despite different names*

### Comparing `pymafia-0.2.3/src/pymafia/utils.py` & `pymafia-0.2.4/src/pymafia/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+__all__ = ["launch_gui", "login", "abort", "log", "execute", "script"]
+
 from html import escape
+from typing import Any
 
 from jpype import JClass
 
+from pymafia.ash.conversion import from_java
 from pymafia.kolmafia import km
 
 ByteArrayOutputStream = JClass("java.io.ByteArrayOutputStream")
 PrintStream = JClass("java.io.PrintStream")
 OutputStream = JClass("java.io.OutputStream")
+String = JClass("java.lang.String")
+ByteArrayInputStream = JClass("java.io.ByteArrayInputStream")
 
 
 def launch_gui():
     """Launch the KoLmafia GUI."""
     km.KoLmafia.main(["--GUI"])
 
 
@@ -41,7 +47,16 @@
 def execute(command: str) -> str:
     """Execute a command in the KoLmafia CLI and return the output."""
     ostream = OutputStream @ ByteArrayOutputStream()
     out = PrintStream(ostream)
     km.RequestLogger.openCustom(out)
     km.KoLmafiaCLI.DEFAULT_SHELL.executeLine(command)
     return ostream.toString()
+
+
+def script(lines: str, convert=True) -> Any:
+    """Execute an ash script and return the result, optionally converting it."""
+    stream = ByteArrayInputStream(String(lines).getBytes())
+    interpreter = km.AshRuntime()
+    interpreter.validate(None, stream)
+    value = interpreter.execute("main", None)
+    return from_java(value) if convert else value
```

### Comparing `pymafia-0.2.3/PKG-INFO` & `pymafia-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymafia
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python module and bridge for reflecting KoLmafia's Java environment
 Home-page: https://github.com/MrFizzyBubbs/pymafia
 License: MIT
 Author: MrFizzyBubbs
 Author-email: MrFizzyBubbs@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

