# Comparing `tmp/wom_py-0.5.0.tar.gz` & `tmp/wom_py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.5.0.tar", max compression
+gzip compressed data, was "wom_py-0.6.0.tar", max compression
```

## Comparing `wom_py-0.5.0.tar` & `wom_py-0.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-07-01 18:21:28.398859 wom_py-0.5.0/LICENSE
--rw-r--r--   0        0        0     2712 2023-07-01 18:21:28.398859 wom_py-0.5.0/README.md
--rw-r--r--   0        0        0     2157 2023-07-01 18:21:28.398859 wom_py-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4438 2023-07-01 18:21:28.486856 wom_py-0.5.0/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/_cli.py
--rw-r--r--   0        0        0     8648 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/client.py
--rw-r--r--   0        0        0     1447 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/constants.py
--rw-r--r--   0        0        0     7388 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/errors.py
--rw-r--r--   0        0        0     3281 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/__init__.py
--rw-r--r--   0        0        0     1557 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7413 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-07-01 18:21:28.398859 wom_py-0.5.0/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1740 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9738 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/http.py
--rw-r--r--   0        0        0     1471 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1793 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/names/enums.py
--rw-r--r--   0        0        0     4894 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/names/models.py
--rw-r--r--   0        0        0     1783 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5686 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/players/enums.py
--rw-r--r--   0        0        0    12222 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/py.typed
--rw-r--r--   0        0        0     5561 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/result.py
--rw-r--r--   0        0        0     6596 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/routes.py
--rw-r--r--   0        0        0    35491 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/__init__.py
--rw-r--r--   0        0        0     2050 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/base.py
--rw-r--r--   0        0        0    21170 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/competitions.py
--rw-r--r--   0        0        0     3528 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/deltas.py
--rw-r--r--   0        0        0     3688 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/efficiency.py
--rw-r--r--   0        0        0    24089 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/groups.py
--rw-r--r--   0        0        0     5772 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/http.py
--rw-r--r--   0        0        0     4031 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/names.py
--rw-r--r--   0        0        0    20107 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/players.py
--rw-r--r--   0        0        0     3506 2023-07-01 18:21:28.402859 wom_py-0.5.0/wom/services/records.py
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 wom_py-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-27 03:34:30.525718 wom_py-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2765 2023-07-27 03:34:30.525718 wom_py-0.6.0/README.md
+-rw-r--r--   0        0        0     2157 2023-07-27 03:34:30.529718 wom_py-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4438 2023-07-27 03:34:30.633730 wom_py-0.6.0/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/_cli.py
+-rw-r--r--   0        0        0     8648 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/constants.py
+-rw-r--r--   0        0        0     7521 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/errors.py
+-rw-r--r--   0        0        0     3281 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7413 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1740 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9738 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/http.py
+-rw-r--r--   0        0        0     1471 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1793 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/names/enums.py
+-rw-r--r--   0        0        0     4894 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/names/models.py
+-rw-r--r--   0        0        0     1783 2023-07-27 03:34:30.529718 wom_py-0.6.0/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5686 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/models/players/enums.py
+-rw-r--r--   0        0        0    12222 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/py.typed
+-rw-r--r--   0        0        0     5561 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/result.py
+-rw-r--r--   0        0        0     6596 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/routes.py
+-rw-r--r--   0        0        0    35491 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/__init__.py
+-rw-r--r--   0        0        0     2050 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/base.py
+-rw-r--r--   0        0        0    21170 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/competitions.py
+-rw-r--r--   0        0        0     3528 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/deltas.py
+-rw-r--r--   0        0        0     3688 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/efficiency.py
+-rw-r--r--   0        0        0    24089 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/groups.py
+-rw-r--r--   0        0        0     5772 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/http.py
+-rw-r--r--   0        0        0     4031 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/names.py
+-rw-r--r--   0        0        0    20107 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/players.py
+-rw-r--r--   0        0        0     3506 2023-07-27 03:34:30.533719 wom_py-0.6.0/wom/services/records.py
+-rw-r--r--   0        0        0     3881 1970-01-01 00:00:00.000000 wom_py-0.6.0/PKG-INFO
```

### Comparing `wom_py-0.5.0/LICENSE` & `wom_py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/README.md` & `wom_py-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 - Player achievements
 - Group competitions
 - Global leaderboards
 - A discord bot for interacting with the API
 
 ## Contributing
 
-wom.py is open to contributions.
-
-Come back soon™ once I've written the contributing guide.
+wom.py is open to contributions. Check out the
+[contributing guide](https://github.com/Jonxslays/wom.py/blob/master/CONTRIBUTING.md) to learn how.
 
 ## License
 
 wom.py is licensed under the
 [MIT License](https://github.com/Jonxslays/wom.py/blob/master/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -16,11 +16,11 @@
 you're interested in learning more about the Wise Old Man project, consider
 checking out any of these links: - [Website](https://wiseoldman.net/) - [API
 documentation](https://docs.wiseoldman.net/) - [Github repository](https://
 wiseoldman.net/github) - [Discord community](https://wiseoldman.net/discord) -
 [Support the developers on Patreon](https://wiseoldman.net/patreon) Some of the
 popular features include: - Experience tracking - Boss killcounts - Player
 achievements - Group competitions - Global leaderboards - A discord bot for
-interacting with the API ## Contributing wom.py is open to contributions. Come
-back soonâ¢ once I've written the contributing guide. ## License wom.py is
-licensed under the [MIT License](https://github.com/Jonxslays/wom.py/blob/
-master/LICENSE).
+interacting with the API ## Contributing wom.py is open to contributions. Check
+out the [contributing guide](https://github.com/Jonxslays/wom.py/blob/master/
+CONTRIBUTING.md) to learn how. ## License wom.py is licensed under the [MIT
+License](https://github.com/Jonxslays/wom.py/blob/master/LICENSE).
```

### Comparing `wom_py-0.5.0/pyproject.toml` & `wom_py-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.5.0"
+version = "0.6.0"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
```

### Comparing `wom_py-0.5.0/wom/__init__.py` & `wom_py-0.6.0/wom/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 """
 
 from __future__ import annotations
 
 from typing import Final
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.5.0"
+__version__: Final[str] = "0.6.0"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[c4955d3]"
+__git_sha__: Final[str] = "[e41a723]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
```

### Comparing `wom_py-0.5.0/wom/__main__.py` & `wom_py-0.6.0/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/_cli.py` & `wom_py-0.6.0/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/client.py` & `wom_py-0.6.0/wom/client.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/constants.py` & `wom_py-0.6.0/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/enums.py` & `wom_py-0.6.0/wom/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     CommanderZilyana = "commander_zilyana"
     CorporealBeast = "corporeal_beast"
     CrazyArchaeologist = "crazy_archaeologist"
     DagannothPrime = "dagannoth_prime"
     DagannothRex = "dagannoth_rex"
     DagannothSupreme = "dagannoth_supreme"
     DerangedArchaeologist = "deranged_archaeologist"
+    DukeSucellus = "duke_sucellus"
     GeneralGraardor = "general_graardor"
     GiantMole = "giant_mole"
     GrotesqueGuardians = "grotesque_guardians"
     Hespori = "hespori"
     KalphiteQueen = "kalphite_queen"
     KingBlackDragon = "king_black_dragon"
     Kraken = "kraken"
@@ -222,21 +223,24 @@
     Sarachnis = "sarachnis"
     Scorpia = "scorpia"
     Skotizo = "skotizo"
     Spindel = "spindel"
     Tempoross = "tempoross"
     TheGauntlet = "the_gauntlet"
     TheCorruptedGauntlet = "the_corrupted_gauntlet"
+    TheLeviathan = "the_leviathan"
+    TheWhisperer = "the_whisperer"
     TheatreOfBlood = "theatre_of_blood"
     TheatreOfBloodHard = "theatre_of_blood_hard_mode"
     ThermonuclearSmokeDevil = "thermonuclear_smoke_devil"
     TombsOfAmascut = "tombs_of_amascut"
     TombsOfAmascutExpert = "tombs_of_amascut_expert"
     TzKalZuk = "tzkal_zuk"
     TzTokJad = "tztok_jad"
+    Vardorvis = "vardorvis"
     Venenatis = "venenatis"
     Vetion = "vetion"
     Vorkath = "vorkath"
     Wintertodt = "wintertodt"
     Zalcano = "zalcano"
     Zulrah = "zulrah"
```

### Comparing `wom_py-0.5.0/wom/errors.py` & `wom_py-0.6.0/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/__init__.py` & `wom_py-0.6.0/wom/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/base.py` & `wom_py-0.6.0/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/competitions/__init__.py` & `wom_py-0.6.0/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/competitions/enums.py` & `wom_py-0.6.0/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/competitions/models.py` & `wom_py-0.6.0/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/deltas/__init__.py` & `wom_py-0.6.0/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/deltas/models.py` & `wom_py-0.6.0/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/groups/__init__.py` & `wom_py-0.6.0/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/groups/enums.py` & `wom_py-0.6.0/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/groups/models.py` & `wom_py-0.6.0/wom/models/groups/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/http.py` & `wom_py-0.6.0/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/names/__init__.py` & `wom_py-0.6.0/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/names/enums.py` & `wom_py-0.6.0/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/names/models.py` & `wom_py-0.6.0/wom/models/names/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/players/__init__.py` & `wom_py-0.6.0/wom/models/players/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/players/enums.py` & `wom_py-0.6.0/wom/models/players/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/players/models.py` & `wom_py-0.6.0/wom/models/players/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/records/__init__.py` & `wom_py-0.6.0/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/models/records/models.py` & `wom_py-0.6.0/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/result.py` & `wom_py-0.6.0/wom/result.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/routes.py` & `wom_py-0.6.0/wom/routes.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/serializer.py` & `wom_py-0.6.0/wom/serializer.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/__init__.py` & `wom_py-0.6.0/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/base.py` & `wom_py-0.6.0/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/competitions.py` & `wom_py-0.6.0/wom/services/competitions.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/deltas.py` & `wom_py-0.6.0/wom/services/deltas.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/efficiency.py` & `wom_py-0.6.0/wom/services/efficiency.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/groups.py` & `wom_py-0.6.0/wom/services/groups.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/http.py` & `wom_py-0.6.0/wom/services/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/names.py` & `wom_py-0.6.0/wom/services/names.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/players.py` & `wom_py-0.6.0/wom/services/players.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/wom/services/records.py` & `wom_py-0.6.0/wom/services/records.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.5.0/PKG-INFO` & `wom_py-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.5.0
+Version: 0.6.0
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -89,16 +89,15 @@
 - Player achievements
 - Group competitions
 - Global leaderboards
 - A discord bot for interacting with the API
 
 ## Contributing
 
-wom.py is open to contributions.
-
-Come back soon™ once I've written the contributing guide.
+wom.py is open to contributions. Check out the
+[contributing guide](https://github.com/Jonxslays/wom.py/blob/master/CONTRIBUTING.md) to learn how.
 
 ## License
 
 wom.py is licensed under the
 [MIT License](https://github.com/Jonxslays/wom.py/blob/master/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wom-py Version: 0.5.0 Summary: An asynchronous
+Metadata-Version: 2.1 Name: wom-py Version: 0.6.0 Summary: An asynchronous
 wrapper for the Wise Old Man API. Home-page: https://github.com/Jonxslays/
 wom.py License: MIT Author: Jonxslays Requires-Python: >=3.8 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -31,11 +31,11 @@
 you're interested in learning more about the Wise Old Man project, consider
 checking out any of these links: - [Website](https://wiseoldman.net/) - [API
 documentation](https://docs.wiseoldman.net/) - [Github repository](https://
 wiseoldman.net/github) - [Discord community](https://wiseoldman.net/discord) -
 [Support the developers on Patreon](https://wiseoldman.net/patreon) Some of the
 popular features include: - Experience tracking - Boss killcounts - Player
 achievements - Group competitions - Global leaderboards - A discord bot for
-interacting with the API ## Contributing wom.py is open to contributions. Come
-back soonâ¢ once I've written the contributing guide. ## License wom.py is
-licensed under the [MIT License](https://github.com/Jonxslays/wom.py/blob/
-master/LICENSE).
+interacting with the API ## Contributing wom.py is open to contributions. Check
+out the [contributing guide](https://github.com/Jonxslays/wom.py/blob/master/
+CONTRIBUTING.md) to learn how. ## License wom.py is licensed under the [MIT
+License](https://github.com/Jonxslays/wom.py/blob/master/LICENSE).
```

