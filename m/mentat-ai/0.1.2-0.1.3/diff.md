# Comparing `tmp/mentat-ai-0.1.2.tar.gz` & `tmp/mentat-ai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentat-ai-0.1.2.tar", last modified: Wed Jul 26 04:00:56 2023, max compression
+gzip compressed data, was "mentat-ai-0.1.3.tar", last modified: Thu Jul 27 13:53:07 2023, max compression
```

## Comparing `mentat-ai-0.1.2.tar` & `mentat-ai-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.298325 mentat-ai-0.1.2/
--rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.2/LICENSE
--rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-26 04:00:56.298210 mentat-ai-0.1.2/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)     2722 2023-07-26 03:56:30.000000 mentat-ai-0.1.2/README.md
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.295221 mentat-ai-0.1.2/mentat/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.2/mentat/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      166 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/__main__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     6013 2023-07-25 13:33:37.000000 mentat-ai-0.1.2/mentat/app.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/change_conflict_resolution.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/code_change.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/code_change_display.py
--rw-r--r--   0 biobootloader   (501) staff       (20)    13118 2023-07-26 03:57:32.000000 mentat-ai-0.1.2/mentat/code_file_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1536 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/config_manager.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2340 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/conversation.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      325 2023-07-25 13:34:36.000000 mentat-ai-0.1.2/mentat/default_config.json
--rw-r--r--   0 biobootloader   (501) staff       (20)     3798 2023-07-25 13:33:37.000000 mentat-ai-0.1.2/mentat/llm_api.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/logging_config.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/mentat/parsing.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.2/mentat/prompts.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/streaming_printer.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/mentat/user_input_manager.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.295902 mentat-ai-0.1.2/mentat_ai.egg-info/
--rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/PKG-INFO
--rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/SOURCES.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/dependency_links.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/entry_points.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/requires.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-26 04:00:56.000000 mentat-ai-0.1.2/mentat_ai.egg-info/top_level.txt
--rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/pyproject.toml
--rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-26 04:00:56.298356 mentat-ai-0.1.2/setup.cfg
--rw-r--r--   0 biobootloader   (501) staff       (20)      463 2023-07-26 04:00:19.000000 mentat-ai-0.1.2/setup.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.296009 mentat-ai-0.1.2/testbed/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.2/testbed/__init__.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.296393 mentat-ai-0.1.2/testbed/multifile_calculator/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.2/testbed/multifile_calculator/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.2/testbed/multifile_calculator/calculator.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.2/testbed/multifile_calculator/operations.py
-drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-26 04:00:56.298045 mentat-ai-0.1.2/tests/
--rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.2/tests/__init__.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/benchmark_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2580 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/code_file_manager_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/tests/codechange_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      148 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/config_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     3689 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/conftest.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.2/tests/measure_api_speed.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.2/tests/record_benchmark.py
--rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-22 22:55:34.000000 mentat-ai-0.1.2/tests/system_test.py
--rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.2/tests/ui_test.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.749173 mentat-ai-0.1.3/
+-rw-r--r--   0 biobootloader   (501) staff       (20)    11357 2023-07-08 00:24:17.000000 mentat-ai-0.1.3/LICENSE
+-rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-27 13:53:07.749057 mentat-ai-0.1.3/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2961 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/README.md
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.745394 mentat-ai-0.1.3/mentat/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 23:06:24.000000 mentat-ai-0.1.3/mentat/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      166 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/__main__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     6025 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/mentat/app.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4175 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/change_conflict_resolution.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     5095 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/code_change.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4283 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/code_change_display.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)    13189 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/mentat/code_file_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1536 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/config_manager.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2340 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/conversation.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      325 2023-07-25 13:34:36.000000 mentat-ai-0.1.3/mentat/default_config.json
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3798 2023-07-25 13:33:37.000000 mentat-ai-0.1.3/mentat/llm_api.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1696 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/logging_config.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     8169 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/mentat/parsing.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3559 2023-07-15 05:21:35.000000 mentat-ai-0.1.3/mentat/prompts.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1452 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/streaming_printer.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3193 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/mentat/user_input_manager.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.746084 mentat-ai-0.1.3/mentat_ai.egg-info/
+-rw-r--r--   0 biobootloader   (501) staff       (20)       75 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/PKG-INFO
+-rw-r--r--   0 biobootloader   (501) staff       (20)      997 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)        1 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       46 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/entry_points.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)      765 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/requires.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       21 2023-07-27 13:53:07.000000 mentat-ai-0.1.3/mentat_ai.egg-info/top_level.txt
+-rw-r--r--   0 biobootloader   (501) staff       (20)       91 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/pyproject.toml
+-rw-r--r--   0 biobootloader   (501) staff       (20)       38 2023-07-27 13:53:07.749204 mentat-ai-0.1.3/setup.cfg
+-rw-r--r--   0 biobootloader   (501) staff       (20)      463 2023-07-27 13:52:38.000000 mentat-ai-0.1.3/setup.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.746187 mentat-ai-0.1.3/testbed/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:08:09.000000 mentat-ai-0.1.3/testbed/__init__.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.746772 mentat-ai-0.1.3/testbed/multifile_calculator/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-05-31 00:07:36.000000 mentat-ai-0.1.3/testbed/multifile_calculator/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      580 2023-07-18 20:17:52.000000 mentat-ai-0.1.3/testbed/multifile_calculator/calculator.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      179 2023-07-18 20:17:50.000000 mentat-ai-0.1.3/testbed/multifile_calculator/operations.py
+drwxr-xr-x   0 biobootloader   (501) staff       (20)        0 2023-07-27 13:53:07.748889 mentat-ai-0.1.3/tests/
+-rw-r--r--   0 biobootloader   (501) staff       (20)        0 2023-07-12 22:56:07.000000 mentat-ai-0.1.3/tests/__init__.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     4010 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/benchmark_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2700 2023-07-27 13:51:20.000000 mentat-ai-0.1.3/tests/code_file_manager_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     7507 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/tests/codechange_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      148 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/config_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     3689 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/conftest.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     1467 2023-07-12 22:02:48.000000 mentat-ai-0.1.3/tests/measure_api_speed.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2605 2023-07-25 13:33:37.000000 mentat-ai-0.1.3/tests/record_benchmark.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)     2924 2023-07-22 22:55:34.000000 mentat-ai-0.1.3/tests/system_test.py
+-rw-r--r--   0 biobootloader   (501) staff       (20)      825 2023-07-21 00:32:22.000000 mentat-ai-0.1.3/tests/ui_test.py
```

### Comparing `mentat-ai-0.1.2/LICENSE` & `mentat-ai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/README.md` & `mentat-ai-0.1.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 [![Twitter Follow](https://img.shields.io/twitter/follow/bio_bootloader?style=social)](https://twitter.com/bio_bootloader)
 [![Discord Follow](https://dcbadge.vercel.app/api/server/XbPdxAMJte?style=flat)](https://discord.gg/zbvd9qx9Pb)
+[![Stable Version](https://img.shields.io/pypi/v/mentat-ai?color=blue)](https://pypi.org/project/mentat-ai/)
+
 # 🧙‍♂️ Mentat ⚡
 
 > _It is by will alone I set my mind in motion_
 > 
 > The Mentat Mantra
 
 The Mentats of Dune combine human creativity with computer-like processing - and now you can too.
@@ -12,18 +14,20 @@
 
 Mentat is the AI tool that assists you with any coding task, right from your command line.
 
 Unlike Copilot, Mentat coordinates edits across multiple locations and files. And unlike ChatGPT, Mentat already has the context of your project - no copy and pasting required!
 
 Want help understanding a new codebase? Need to add a new feature? Refactor existing code? Mentat can do it!
 
-# 🍿 Example Videos
+# 🍿 Example Videos (🔊 on!)
+
+https://github.com/biobootloader/mentat/assets/128252497/35b027a9-d639-452c-a53c-ef019a645719
 
-See the videos on [Twitter](https://twitter.com/bio_bootloader/status/1683906735248125955) or YouTube:
-- [Intro (2 min)](https://www.youtube.com/watch?v=lODjaWclwpY)
+See more videos on [Twitter](https://twitter.com/bio_bootloader/status/1683906735248125955) or YouTube:
+- [Intro (2 min - same video as above)](https://www.youtube.com/watch?v=lODjaWclwpY)
 - [Explaining and editing Llama2.c (3 min)](https://www.youtube.com/watch?v=qSyTWMFOjPs)
 - [More Mentat features (4 min)](https://www.youtube.com/watch?v=YJLDIqq8k2A)
 
 # ⚙️ Setup
 
 ## Install
```

### Comparing `mentat-ai-0.1.2/mentat/app.py` & `mentat-ai-0.1.3/mentat/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     setup_logging()
     setup_api_key()
     logging.debug(f"Paths: {paths}")
 
     cost_tracker = CostTracker()
     try:
         loop(paths, cost_tracker)
-    except KeyboardInterrupt as e:
+    except (EOFError, KeyboardInterrupt) as e:
         print(e)
     finally:
         cost_tracker.display_total_cost()
 
 
 def loop(paths: Iterable[str], cost_tracker: CostTracker) -> None:
     config = ConfigManager()
```

### Comparing `mentat-ai-0.1.2/mentat/change_conflict_resolution.py` & `mentat-ai-0.1.3/mentat/change_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/code_change.py` & `mentat-ai-0.1.3/mentat/code_change.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/code_change_display.py` & `mentat-ai-0.1.3/mentat/code_change_display.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/code_file_manager.py` & `mentat-ai-0.1.3/mentat/code_file_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import mimetypes
 import os
 import subprocess
 from collections import defaultdict
 from pathlib import Path
 from typing import Iterable
 
-import git
-import pathspec
 from termcolor import cprint
 
 from .change_conflict_resolution import (
     resolve_insertion_conflicts,
     resolve_non_insertion_conflicts,
 )
 from .code_change import CodeChange, CodeChangeAction
@@ -211,22 +209,25 @@
         self.file_paths = []
 
         for path in paths:
             path = Path(path)
             if path.is_file():
                 path_set.add(os.path.realpath(path))
             elif path.is_dir():
-                all_files = set(pathspec.util.iter_tree_files(path, follow_links=False))
-                repo = git.Repo(self.git_root)
-                ignore_files = set(
-                    repo.ignored(*all_files)
-                    + list(filter(lambda p: p.startswith(".git"), all_files))
+                nonignored_files = set(
+                    filter(
+                        lambda p: p != "",
+                        subprocess.check_output(
+                            # -c shows cached (regular) files, -o shows other (untracked/ new) files
+                            ["git", "ls-files", "-c", "-o", "--exclude-standard"],
+                            cwd=path,
+                            text=True,
+                        ).split("\n"),
+                    )
                 )
-                repo.close()
-                nonignored_files = all_files - ignore_files
                 non_text_files = filter(
                     lambda f: not _is_file_text(
                         os.path.realpath(os.path.join(path, f))
                     ),
                     nonignored_files,
                 )
                 self.non_text_file_paths.extend(
@@ -305,15 +306,15 @@
         changes = resolve_insertion_conflicts(changes, self.user_input_manager, self)
         if not changes:
             return []
 
         rel_path = changes[0].file
         abs_path = os.path.join(self.git_root, rel_path)
         new_code_lines = self.file_lines[abs_path].copy()
-        if new_code_lines != self._read_file(rel_path):
+        if new_code_lines != self._read_file(abs_path):
             logging.info(f"File '{rel_path}' changed while generating changes")
             cprint(
                 (
                     f"File '{rel_path}' changed while generating; current file changes"
                     " will be erased. Continue?"
                 ),
                 color="light_yellow",
```

### Comparing `mentat-ai-0.1.2/mentat/config_manager.py` & `mentat-ai-0.1.3/mentat/config_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/conversation.py` & `mentat-ai-0.1.3/mentat/conversation.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/llm_api.py` & `mentat-ai-0.1.3/mentat/llm_api.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/logging_config.py` & `mentat-ai-0.1.3/mentat/logging_config.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/parsing.py` & `mentat-ai-0.1.3/mentat/parsing.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/prompts.py` & `mentat-ai-0.1.3/mentat/prompts.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/streaming_printer.py` & `mentat-ai-0.1.3/mentat/streaming_printer.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat/user_input_manager.py` & `mentat-ai-0.1.3/mentat/user_input_manager.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat_ai.egg-info/SOURCES.txt` & `mentat-ai-0.1.3/mentat_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/mentat_ai.egg-info/requires.txt` & `mentat-ai-0.1.3/mentat_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/testbed/multifile_calculator/calculator.py` & `mentat-ai-0.1.3/testbed/multifile_calculator/calculator.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/tests/benchmark_test.py` & `mentat-ai-0.1.3/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/tests/code_file_manager_test.py` & `mentat-ai-0.1.3/tests/code_file_manager_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,31 +8,32 @@
 from mentat.config_manager import ConfigManager
 
 config = ConfigManager()
 
 
 def test_path_gitignoring(temp_testbed):
     gitignore_path = ".gitignore"
-    ignored_path = "ignored_file.txt"
-    nonignored_path = "nonignored_file.txt"
+    testing_dir_path = "git_testing_dir"
+    os.makedirs(testing_dir_path)
+    ignored_path = os.path.join(testing_dir_path, "ignored_file.txt")
+    nonignored_path = os.path.join(testing_dir_path, "nonignored_file.txt")
     with open(gitignore_path, "a") as gitignore_file:
         gitignore_file.write("\nignored_file.txt\nnonignored_file.txt")
     with open(ignored_path, "w") as ignored_file:
         ignored_file.write("I am ignored")
     with open(nonignored_path, "w") as nonignored_file:
         nonignored_file.write("I am not ignored")
 
-    os.makedirs("git_testing_dir")
     in_dir_path = os.path.join("git_testing_dir", "in_dir.txt")
     with open(in_dir_path, "w") as in_dir_file:
         in_dir_file.write("I am in a directory")
 
     # Gets all non-git-ignored files inside directory
     # Doesn't get git-ignored files unless specifically asked for
-    paths = ["git_testing_dir", "nonignored_file.txt"]
+    paths = ["git_testing_dir", "git_testing_dir/nonignored_file.txt"]
     code_file_manager = CodeFileManager(paths, user_input_manager=None, config=config)
 
     expected_file_paths = [
         os.path.join(temp_testbed, nonignored_path),
         os.path.join(temp_testbed, in_dir_path),
     ]
```

### Comparing `mentat-ai-0.1.2/tests/codechange_test.py` & `mentat-ai-0.1.3/tests/codechange_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/tests/conftest.py` & `mentat-ai-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/tests/measure_api_speed.py` & `mentat-ai-0.1.3/tests/measure_api_speed.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/tests/record_benchmark.py` & `mentat-ai-0.1.3/tests/record_benchmark.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/tests/system_test.py` & `mentat-ai-0.1.3/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `mentat-ai-0.1.2/tests/ui_test.py` & `mentat-ai-0.1.3/tests/ui_test.py`

 * *Files identical despite different names*

