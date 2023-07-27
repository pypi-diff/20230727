# Comparing `tmp/mrchef-0.6.0.tar.gz` & `tmp/mrchef-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrchef-0.6.0.tar", max compression
+gzip compressed data, was "mrchef-0.7.0.tar", max compression
```

## Comparing `mrchef-0.6.0.tar` & `mrchef-0.7.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-07-07 05:52:08.782651 mrchef-0.6.0/LICENSE
--rw-r--r--   0        0        0     5291 2023-07-07 05:52:08.783651 mrchef-0.6.0/README.md
--rw-r--r--   0        0        0       55 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/__init__.py
--rw-r--r--   0        0        0      177 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/__main__.py
--rw-r--r--   0        0        0     4857 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/cli.py
--rw-r--r--   0        0        0    25292 2023-07-07 05:52:08.783651 mrchef-0.6.0/mrchef/lib.py
--rw-r--r--   0        0        0      985 2023-07-07 05:52:08.784651 mrchef-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6351 1970-01-01 00:00:00.000000 mrchef-0.6.0/setup.py
--rw-r--r--   0        0        0     6320 1970-01-01 00:00:00.000000 mrchef-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-27 10:35:56.228882 mrchef-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5349 2023-07-27 10:35:56.228882 mrchef-0.7.0/README.md
+-rw-r--r--   0        0        0       55 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/__init__.py
+-rw-r--r--   0        0        0      177 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/__main__.py
+-rw-r--r--   0        0        0     4857 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/cli.py
+-rw-r--r--   0        0        0    27881 2023-07-27 10:35:56.229882 mrchef-0.7.0/mrchef/lib.py
+-rw-r--r--   0        0        0      985 2023-07-27 10:35:56.229882 mrchef-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6409 1970-01-01 00:00:00.000000 mrchef-0.7.0/setup.py
+-rw-r--r--   0        0        0     6378 1970-01-01 00:00:00.000000 mrchef-0.7.0/PKG-INFO
```

### Comparing `mrchef-0.6.0/LICENSE` & `mrchef-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mrchef-0.6.0/README.md` & `mrchef-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 ```sh
 mrchef --help-all
 ```
 
 ### Using Python
 
-Install it:
+For speed, it's highly recommended to use Python >= 3.11. Install it:
 
 ```sh
 pip install mrchef
 ```
 
 Use it:
```

### Comparing `mrchef-0.6.0/mrchef/cli.py` & `mrchef-0.7.0/mrchef/cli.py`

 * *Files identical despite different names*

### Comparing `mrchef-0.6.0/mrchef/lib.py` & `mrchef-0.7.0/mrchef/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,80 @@
 """Mr. Chef's core functionality."""
 
 import re
 import warnings
 from contextlib import suppress
 from dataclasses import dataclass, field
 from datetime import datetime
+from functools import lru_cache
 from logging import DEBUG, ERROR, captureWarnings, getLogger
 from pathlib import Path
 from shutil import rmtree
 from textwrap import dedent
-from typing import Optional
+from typing import Generator, Optional
 
 import coloredlogs
 import requests
 import tomlkit
 from git_find_repos import find_repos
 from plumbum import local
 from plumbum.commands.processes import ProcessExecutionError
+from tomlkit._utils import Collection, _basic_escapes, decode, escape_string
 
 CONFIG_FILE = "mrchef.toml"
 FREEZER_FILE = ".mrchef.freezer.toml"
 
 logger = getLogger("mrchef")
 coloredlogs.install(logger=logger)
 
 # Combine with warnings
 warnings_logger = getLogger("py.warnings")
 coloredlogs.install(logger=warnings_logger)
 captureWarnings(True)
 
 
+# HACK https://github.com/sdispater/tomlkit/pull/304
+def _patched_escape_string(
+    s: str, escape_sequences: Collection[str] = _basic_escapes
+) -> str:
+    ds = decode(s)
+    found_sequences = {seq for seq in escape_sequences if seq in ds}
+    return escape_string(s, found_sequences)
+
+
+tomlkit._utils.escape_string = _patched_escape_string
+tomlkit.items.escape_string = _patched_escape_string
+
+
+def _toml_load(fd):
+    """Load TOML without any interest in preserving style.
+
+    This is a HACK because the problem it tries to solve is that tomlkit is
+    extremely slow. Just [see the report][1].
+
+    The best fix would be that tomlkit itself gets faster. But until then, this
+    works if you run Mr. Chef with Python 3.11 (which has tomllib built-in).
+
+    We only use this helper for the freezer file, because it doesn't need to
+    preserve style. Since it can contain patches, those are really slow to
+    parse and dump for tomlkit. The user config file is usually just fine with
+    it, because it's smaller.
+
+    [1]:
+    https://github.com/pwwang/toml-bench/blob/master/reports/with_python3.11.md#running-speed-with-data-provided-by-rtoml
+    """
+    try:
+        import tomllib
+
+        return tomllib.load(fd)
+    except ImportError:
+        # Not on python 3.11 yet? Well, this is gonna be slow...
+        return tomlkit.load(fd).unwrap()
+
+
 class MrChefError(Exception):
     """Core MrChef exception.
 
     It will be handled and pretty-printed when raised to CLI.
     """
 
     def __init__(self, msg: str, trace_level=DEBUG):
@@ -87,16 +128,17 @@
             self.config_user = tomlkit.load(fd)
             break
         else:
             raise MrChefError(f"No {CONFIG_FILE} file found here or in parent folders.")
         # Attempt to merge normal config with frozen one
         self.freezer_file = self.path / FREEZER_FILE
         try:
-            with self.freezer_file.open("r") as fd:
-                self.config_frozen = tomlkit.load(fd)
+            with self.freezer_file.open("rb") as fd:
+                # Style in the freezer isn't preserved, so we unwrap it to be faster
+                self.config_frozen = _toml_load(fd)
         except FileNotFoundError:
             warnings.warn("Freezer file not found.", stacklevel=2)
             self.config_frozen = {}
         # Setup self and do some checks
         assert self.config_user["version"] == 1
         self.kitchen = self.path / self.config_user["kitchen"]
         self.config_frozen.setdefault("meals", {})
@@ -148,14 +190,40 @@
             # Get cached content
             return self.config_frozen["spices"][spice_url]
         except KeyError:
             # Cached content not found, get it from the Internet
             logger.info(f"Spice was not frozen, downloading: {spice_url}")
             return self._get_spice_content(spice_url, True)
 
+    def _patches_generator(self) -> Generator[Path, None, None]:
+        """A generator that creates new patch file names in the kitchen."""
+        num = 0
+        while True:
+            patch_path = self.kitchen / f"mrchef-{num:03d}.patch"
+            if not patch_path.exists():
+                yield patch_path
+            num += 1
+
+    def _new_patch(self) -> Path:
+        """Generate a new patch file name in the kitchen."""
+        try:
+            generator = self._cached_patch_generator
+        except AttributeError:
+            self._cached_patch_generator = self._patches_generator()
+            generator = self._cached_patch_generator
+        return next(generator)
+
+    def _is_auto_patch(self, patch_path: Path) -> bool:
+        """Check if the patch was generated by MrChef."""
+        return (
+            patch_path.name.startswith("mrchef-")
+            and patch_path.suffix == ".patch"
+            and patch_path.parent == self.kitchen
+        )
+
     @classmethod
     def init(cls, where: Path):
         """Initialize a new kitchen."""
         where.joinpath(CONFIG_FILE).write_text(
             dedent(
                 """\
                 version = 1
@@ -234,15 +302,15 @@
             for hot_commit in git_commits_diff(meal_path, meal.rev, "HEAD"):
                 hot_patch_id = git_commit_patch_id(meal_path, hot_commit)
                 try:
                     # Get patch URL from freezer
                     hot_spice_url = self.config_frozen["patch2spice"][hot_patch_id]
                 except KeyError:
                     # The patch is local; store it locally
-                    local_path = self.kitchen / f"mrchef-{hot_patch_id}.patch"
+                    local_path = self._new_patch()
                     local_contents = git_get_commit_patch(meal_path, hot_commit)
                     hot_spice_url = str(local_path.relative_to(self.path))
                     local_path.write_text(local_contents)
                     # Cache patch contents in the freezer
                     self.config_frozen["spices"][hot_spice_url] = local_contents
                     self.config_frozen["patch2spice"][hot_patch_id] = hot_spice_url
                     # Store patch in user configuration
@@ -476,14 +544,19 @@
         logger.info("Removing spice from %s: %s", key, url)
         try:
             self.config_user["meals"][key]["spices"].remove(url)
         except ValueError as error:
             raise MrChefError(
                 f"Cannot remove spice, not found in meal {key}: {url}"
             ) from error
+        # If it was an autogenerated patch file, remove it
+        patch_file = self.path / url
+        if self._is_auto_patch(patch_file):
+            patch_file.unlink(missing_ok=True)
+        # Clean the kitchen
         self.warmup(meal_path)
         self.update_user_config()
         self.freeze()
 
     def spice_export(self, url: str) -> str:
         """Export spice contents from the freezer.
 
@@ -639,30 +712,26 @@
         folder: Path to git repo.
         rev1: First commit to compare.
         rev2: Second commit to compare.
     """
     return git(folder)("merge-base", rev1, rev2).strip()
 
 
+@lru_cache
 def git_remote_head(folder: Path, remote_url: str, remote_ref: str) -> str:
     """Get latest commit sha from remote url and ref combination.
 
     Args:
         folder: Path to git repo.
         remote_url: Absolute URL to remote.
         remote_ref: Branch or revision to fetch from remote.
     """
     _git = git(folder)
-    try:
-        _git("remote", "add", "_mrchef", remote_url)
-        _git("fetch", "--write-fetch-head", "_mrchef", remote_ref)
-        result = _git("rev-parse", "FETCH_HEAD").strip()
-    finally:
-        _git("remote", "rm", "_mrchef")
-    return result
+    _git("fetch", "--write-fetch-head", remote_url, remote_ref)
+    return _git("rev-parse", "FETCH_HEAD").strip()
 
 
 def git_rev(folder: Path) -> str:
     """Know the commit where a git repository is currently checked out."""
     return git(folder)("rev-parse", "--verify", "HEAD").strip()
```

### Comparing `mrchef-0.6.0/pyproject.toml` & `mrchef-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mrchef"
-version = "0.6.0"
+version = "0.7.0"
 description = "Metarepo Chef"
 authors = ["Moduon <info@moduon.team>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://gitlab.com/moduon/mrchef"
 
 [tool.poetry.scripts]
```

### Comparing `mrchef-0.6.0/setup.py` & `mrchef-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  'xdg>=5.1.1']
 
 entry_points = \
 {'console_scripts': ['mrchef = mrchef.__main__:run']}
 
 setup_kwargs = {
     'name': 'mrchef',
-    'version': '0.6.0',
+    'version': '0.7.0',
     'description': 'Metarepo Chef',
-    'long_description': "# Mr. Chef\n\n👨\u200d🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.\n\n## Why\n\nIt has features that no other meta-repo manager has:\n\n-   Code is 100% reproducible.\n-   Full freeze-warmup-freeze coding cycle.\n-   Upstream patching supported.\n-   Downstream patching supported.\n-   Mixed and multi-patching repo supported.\n-   Automated updates.\n-   Automatic disk space economization with [git-autoshare][].\n-   Food! 🥘\n\nLet's dive in. Imagine you need to create an app that requires many unrelated modules to\nbe properly glued together. How would you organize your source code?\n\nThere are multiple answers to that question:\n\n-   Use separate repos and glue them together through packaging. But what if some code\n    you need isn't properly packaged? What if some dependencies need more than 1 patch\n    to work?\n-   Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if\n    some parts are open source and you need to upstream or review changes?\n-   Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,\n    that requires that every time you do a `git checkout`... or almost any git\n    command..., you need to use some `--recurse-submodules` flag. Also it gives _a lot_\n    of headaches when you move files around and perform basically any operation. And\n    what if you need to merge 2 upstream patches?\n-   Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then,\n    you need even more deep knowledge than with submodules to be able to review or\n    publish patches. And again, how to merge more than one patch?\n-   Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't\n    ready for it yet. Still we need Git.\n\nThe solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are\nmany meta-repo managers out there, but none of them has all the features that I already\ntold you about Mr. Chef.\n\n## Glossary\n\nMr. Chef introduces a new code management concept based on the metaphor of a buffet. Use\nthis glossary to understand the rest of the recipe... readme! Sorry...\n\n-   _Buffet_ is the main git repository that contains all the instructions to build it.\n-   The _config file_ is a file named `mrchef.toml` that stands in the root of your\n    _buffet_ and configures what Mr. Chef should do.\n-   The _kitchen_ is the root folder, inside the _buffet_, where you can find the\n    _meals_. It's configured inside the _config file_.\n-   A _meal_ is like a git submodule: another git repo inside your _kitchen_.\n-   A _spice_ is a patch that is added to a _meal_.\n-   The _freezer_ is where we store the gory details needed to make the kitchen 100%\n    reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.\n-   _Warming up_ means getting meals outside of the _freezer_ and putting them in the\n    _kitchen_, ready to cook!\n-   _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed\n    up_ in the _kitchen_.\n\n## How\n\n### Using CLI\n\nInstall it:\n\n```sh\npipx install mrchef\n```\n\nUsually you start by creating a new configuration file:\n\n```sh\nmrchef init\n```\n\nIt will create a new `mrchef.toml` file with some comments about how to use it. You can\ndelete them once you know how to do it.\n\nNow, you will need to add a meal:\n\n```sh\nmrchef meal-add kitchen/hello https://github.com/octocat/Hello-World master\n```\n\n💡 Mr. Chef uses [git-autoshare][] automatically. It will help you if you need to clone\nhuge repos! But you have to configure it before adding the meals.\n\nYou can add more meals just like that.\n\nMaybe you need to apply a couple of spices to the meal? OK:\n\n```sh\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/2256\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/34\n```\n\nDid `master` get new commits? Or did those PRs get updated? Update everything:\n\n```sh\nmrchef update\n```\n\nCool, huh? 😏 Mr. Chef can do more things! To see all commands and what they do:\n\n```sh\nmrchef --help-all\n```\n\n### Using Python\n\nInstall it:\n\n```sh\npip install mrchef\n```\n\nUse it:\n\n```python\nimport mrchef\n```\n\n### Using Nix\n\nInstall it:\n\n```sh\nnix profile install gitlab:moduon/mrchef\n```\n\nDid I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)\nfor that job.\n\nGo read [the flake](./flake.nix). You'll find helpers ready to convert a buffet into\naggregated source code. Read [the minimal test](./tests/nix/testMinimal.nix) to\nunderstand how to use them. Ready to replace git submodules?\n\nKeep in mind this if using nix:\n\n-   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541\n    or https://github.com/NixOS/nix/issues/5119 are fixed.\n\n-   Most mrchef-based derivations will benefit a lot from pre-filtering the sources\n    before the build. Typically, by just including `./mrchef.toml`,\n    `./.mrchef.freezer.toml` and `./kitchen/` (if it exists and the kitchen is named\n    like that), you will have all you need to build.\n\n## Who\n\nCreated and maintained by [Moduon Team](https://www.moduon.team/).\n\nOriginal idea by [Jairo Llopis](https://www.recallstack.icu/).\n\n## Where\n\nAnywhere you want! 🎁 It's [GPL 3.0+](./LICENSE).\n\n[git-autoshare]: https://github.com/acsone/git-autoshare\n",
+    'long_description': "# Mr. Chef\n\n👨\u200d🍳 Meta-Repo Chef. Culinary git helper to work with code buffets.\n\n## Why\n\nIt has features that no other meta-repo manager has:\n\n-   Code is 100% reproducible.\n-   Full freeze-warmup-freeze coding cycle.\n-   Upstream patching supported.\n-   Downstream patching supported.\n-   Mixed and multi-patching repo supported.\n-   Automated updates.\n-   Automatic disk space economization with [git-autoshare][].\n-   Food! 🥘\n\nLet's dive in. Imagine you need to create an app that requires many unrelated modules to\nbe properly glued together. How would you organize your source code?\n\nThere are multiple answers to that question:\n\n-   Use separate repos and glue them together through packaging. But what if some code\n    you need isn't properly packaged? What if some dependencies need more than 1 patch\n    to work?\n-   Use [a monorepo](https://en.wikipedia.org/wiki/Monorepo). However, what happens if\n    some parts are open source and you need to upstream or review changes?\n-   Use [git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules). However,\n    that requires that every time you do a `git checkout`... or almost any git\n    command..., you need to use some `--recurse-submodules` flag. Also it gives _a lot_\n    of headaches when you move files around and perform basically any operation. And\n    what if you need to merge 2 upstream patches?\n-   Use [git subtrees](https://www.atlassian.com/git/tutorials/git-subtree). But then,\n    you need even more deep knowledge than with submodules to be able to review or\n    publish patches. And again, how to merge more than one patch?\n-   Use [Pijul](https://pijul.org/posts/2022-01-07-monorepos/). But the world isn't\n    ready for it yet. Still we need Git.\n\nThe solution is to [use a meta-repo](https://notes.burke.libbey.me/metarepo/). There are\nmany meta-repo managers out there, but none of them has all the features that I already\ntold you about Mr. Chef.\n\n## Glossary\n\nMr. Chef introduces a new code management concept based on the metaphor of a buffet. Use\nthis glossary to understand the rest of the recipe... readme! Sorry...\n\n-   _Buffet_ is the main git repository that contains all the instructions to build it.\n-   The _config file_ is a file named `mrchef.toml` that stands in the root of your\n    _buffet_ and configures what Mr. Chef should do.\n-   The _kitchen_ is the root folder, inside the _buffet_, where you can find the\n    _meals_. It's configured inside the _config file_.\n-   A _meal_ is like a git submodule: another git repo inside your _kitchen_.\n-   A _spice_ is a patch that is added to a _meal_.\n-   The _freezer_ is where we store the gory details needed to make the kitchen 100%\n    reproducible. Mr. Chef saves it in a file called `.mrchef.freezer.toml`.\n-   _Warming up_ means getting meals outside of the _freezer_ and putting them in the\n    _kitchen_, ready to cook!\n-   _Freezing_ means writing a new _freezer_ that can reproduce what's currently _warmed\n    up_ in the _kitchen_.\n\n## How\n\n### Using CLI\n\nInstall it:\n\n```sh\npipx install mrchef\n```\n\nUsually you start by creating a new configuration file:\n\n```sh\nmrchef init\n```\n\nIt will create a new `mrchef.toml` file with some comments about how to use it. You can\ndelete them once you know how to do it.\n\nNow, you will need to add a meal:\n\n```sh\nmrchef meal-add kitchen/hello https://github.com/octocat/Hello-World master\n```\n\n💡 Mr. Chef uses [git-autoshare][] automatically. It will help you if you need to clone\nhuge repos! But you have to configure it before adding the meals.\n\nYou can add more meals just like that.\n\nMaybe you need to apply a couple of spices to the meal? OK:\n\n```sh\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/2256\nmrchef spice-add kitchen/hello https://github.com/octocat/Hello-World/pull/34\n```\n\nDid `master` get new commits? Or did those PRs get updated? Update everything:\n\n```sh\nmrchef update\n```\n\nCool, huh? 😏 Mr. Chef can do more things! To see all commands and what they do:\n\n```sh\nmrchef --help-all\n```\n\n### Using Python\n\nFor speed, it's highly recommended to use Python >= 3.11. Install it:\n\n```sh\npip install mrchef\n```\n\nUse it:\n\n```python\nimport mrchef\n```\n\n### Using Nix\n\nInstall it:\n\n```sh\nnix profile install gitlab:moduon/mrchef\n```\n\nDid I say buffets are 100% reproducible? Nothing better than [Nix](https://nixos.org/)\nfor that job.\n\nGo read [the flake](./flake.nix). You'll find helpers ready to convert a buffet into\naggregated source code. Read [the minimal test](./tests/nix/testMinimal.nix) to\nunderstand how to use them. Ready to replace git submodules?\n\nKeep in mind this if using nix:\n\n-   You should enable flakes. At least, until https://github.com/NixOS/nix/issues/5541\n    or https://github.com/NixOS/nix/issues/5119 are fixed.\n\n-   Most mrchef-based derivations will benefit a lot from pre-filtering the sources\n    before the build. Typically, by just including `./mrchef.toml`,\n    `./.mrchef.freezer.toml` and `./kitchen/` (if it exists and the kitchen is named\n    like that), you will have all you need to build.\n\n## Who\n\nCreated and maintained by [Moduon Team](https://www.moduon.team/).\n\nOriginal idea by [Jairo Llopis](https://www.recallstack.icu/).\n\n## Where\n\nAnywhere you want! 🎁 It's [GPL 3.0+](./LICENSE).\n\n[git-autoshare]: https://github.com/acsone/git-autoshare\n",
     'author': 'Moduon',
     'author_email': 'info@moduon.team',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/moduon/mrchef',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mrchef-0.6.0/PKG-INFO` & `mrchef-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrchef
-Version: 0.6.0
+Version: 0.7.0
 Summary: Metarepo Chef
 Home-page: https://gitlab.com/moduon/mrchef
 License: GPL-3.0-or-later
 Author: Moduon
 Author-email: info@moduon.team
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -134,15 +134,15 @@
 
 ```sh
 mrchef --help-all
 ```
 
 ### Using Python
 
-Install it:
+For speed, it's highly recommended to use Python >= 3.11. Install it:
 
 ```sh
 pip install mrchef
 ```
 
 Use it:
```

