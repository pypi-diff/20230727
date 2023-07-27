# Comparing `tmp/binsize-0.1.2.tar.gz` & `tmp/binsize-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binsize-0.1.2.tar", max compression
+gzip compressed data, was "binsize-0.1.3.tar", max compression
```

## Comparing `binsize-0.1.2.tar` & `binsize-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0     1085 2022-11-04 16:52:24.201229 binsize-0.1.2/LICENSE
--rw-r--r--   0        0        0     2115 2022-10-04 16:46:00.808025 binsize-0.1.2/README.md
--rw-r--r--   0        0        0      819 2022-11-04 16:55:58.446568 binsize-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       12 2022-10-04 12:34:11.870838 binsize-0.1.2/src/binsize/.gitignore
--rw-r--r--   0        0        0      503 2022-10-04 09:54:13.939366 binsize-0.1.2/src/binsize/__init__.py
--rw-r--r--   0        0        0        0 2022-09-29 15:02:49.307216 binsize-0.1.2/src/binsize/cli/__init__.py
--rw-r--r--   0        0        0      739 2022-10-04 09:54:13.991366 binsize-0.1.2/src/binsize/cli/binsize.py
--rw-r--r--   0        0        0     1109 2022-10-04 07:39:52.616780 binsize-0.1.2/src/binsize/cli/build.py
--rw-r--r--   0        0        0     1359 2022-10-04 09:06:44.178767 binsize-0.1.2/src/binsize/cli/commit.py
--rw-r--r--   0        0        0      995 2022-10-04 10:18:05.892333 binsize-0.1.2/src/binsize/cli/compare.py
--rwxr-xr-x   0        0        0     3823 2022-10-04 09:06:44.248768 binsize-0.1.2/src/binsize/cli/get.py
--rw-r--r--   0        0        0     4467 2022-11-04 16:52:24.201229 binsize-0.1.2/src/binsize/cli/history.py
--rw-r--r--   0        0        0      759 2022-10-04 09:06:44.169767 binsize-0.1.2/src/binsize/cli/tree.py
--rw-r--r--   0        0        0        0 2022-09-29 15:07:16.777868 binsize-0.1.2/src/binsize/lib/__init__.py
--rw-r--r--   0        0        0     7918 2022-09-29 11:48:57.116151 binsize-0.1.2/src/binsize/lib/api.py
--rw-r--r--   0        0        0    10910 2022-10-04 15:19:36.766646 binsize-0.1.2/src/binsize/lib/binary_size.py
--rw-r--r--   0        0        0     1523 2022-10-04 07:49:14.645891 binsize-0.1.2/src/binsize/lib/build_definition_loader.py
--rw-r--r--   0        0        0     2197 2022-10-04 14:56:41.740808 binsize-0.1.2/src/binsize/lib/common.py
--rw-r--r--   0        0        0     1196 2022-09-29 11:48:57.116151 binsize-0.1.2/src/binsize/lib/data_handler.py
--rw-r--r--   0        0        0     2347 2022-10-04 09:02:51.011862 binsize-0.1.2/src/binsize/lib/data_loader.py
--rw-r--r--   0        0        0     4600 2022-10-04 10:31:44.342711 binsize-0.1.2/src/binsize/lib/map_file_analyzer.py
--rw-r--r--   0        0        0     3898 2022-10-03 15:44:09.706221 binsize-0.1.2/src/binsize/lib/map_file_includer.py
--rw-r--r--   0        0        0     7974 2022-10-04 15:19:36.769646 binsize-0.1.2/src/binsize/lib/row_handler_c.py
--rw-r--r--   0        0        0     3560 2022-10-03 11:32:08.728018 binsize-0.1.2/src/binsize/lib/row_handler_common.py
--rw-r--r--   0        0        0    10791 2022-10-03 15:44:09.895222 binsize-0.1.2/src/binsize/lib/row_handler_mpy.py
--rw-r--r--   0        0        0     6453 2022-10-03 15:44:09.864222 binsize-0.1.2/src/binsize/lib/row_handler_rust.py
--rw-r--r--   0        0        0     3350 2022-10-04 10:03:26.921409 binsize-0.1.2/src/binsize/lib/source_definition_cache.py
--rw-r--r--   0        0        0        0 2022-09-29 11:48:57.116151 binsize-0.1.2/src/binsize/plugins/__init__.py
--rw-r--r--   0        0        0     3407 2022-10-03 14:28:03.859332 binsize-0.1.2/src/binsize/plugins/size_tree.py
--rw-r--r--   0        0        0     4503 2022-10-03 15:44:09.814221 binsize-0.1.2/src/binsize/plugins/statistics.py
--rw-r--r--   0        0        0     2234 2022-10-04 15:20:11.772786 binsize-0.1.2/src/binsize/settings.py
--rw-r--r--   0        0        0      214 2022-10-04 15:02:33.626022 binsize-0.1.2/src/binsize/settings_template.json
--rw-r--r--   0        0        0      486 2022-10-04 15:19:31.071623 binsize-0.1.2/src/binsize/user_data.py
--rw-r--r--   0        0        0     1326 2022-10-04 08:29:33.299979 binsize-0.1.2/src/binsize/utils.py
--rw-r--r--   0        0        0     3139 2022-11-04 16:56:06.494592 binsize-0.1.2/setup.py
--rw-r--r--   0        0        0     2969 2022-11-04 16:56:06.496440 binsize-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-11-04 16:52:24.201229 binsize-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2115 2022-10-04 16:46:00.808025 binsize-0.1.3/README.md
+-rw-r--r--   0        0        0      819 2023-07-27 08:21:32.250578 binsize-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       12 2022-10-04 12:34:11.870838 binsize-0.1.3/src/binsize/.gitignore
+-rw-r--r--   0        0        0      526 2023-07-27 08:21:32.250578 binsize-0.1.3/src/binsize/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-29 15:02:49.307216 binsize-0.1.3/src/binsize/cli/__init__.py
+-rw-r--r--   0        0        0      981 2023-07-27 08:21:32.250578 binsize-0.1.3/src/binsize/cli/binsize.py
+-rw-r--r--   0        0        0     1109 2022-10-04 07:39:52.616780 binsize-0.1.3/src/binsize/cli/build.py
+-rw-r--r--   0        0        0     1359 2022-10-04 09:06:44.178767 binsize-0.1.3/src/binsize/cli/commit.py
+-rw-r--r--   0        0        0      995 2022-10-04 10:18:05.892333 binsize-0.1.3/src/binsize/cli/compare.py
+-rwxr-xr-x   0        0        0     3906 2023-07-27 08:21:32.250578 binsize-0.1.3/src/binsize/cli/get.py
+-rw-r--r--   0        0        0     4715 2023-07-27 08:21:32.250578 binsize-0.1.3/src/binsize/cli/history.py
+-rw-r--r--   0        0        0      759 2022-10-04 09:06:44.169767 binsize-0.1.3/src/binsize/cli/tree.py
+-rw-r--r--   0        0        0        0 2022-09-29 15:07:16.777868 binsize-0.1.3/src/binsize/lib/__init__.py
+-rw-r--r--   0        0        0     7918 2022-09-29 11:48:57.116151 binsize-0.1.3/src/binsize/lib/api.py
+-rw-r--r--   0        0        0    10910 2022-10-04 15:19:36.766646 binsize-0.1.3/src/binsize/lib/binary_size.py
+-rw-r--r--   0        0        0     1523 2022-10-04 07:49:14.645891 binsize-0.1.3/src/binsize/lib/build_definition_loader.py
+-rw-r--r--   0        0        0     2197 2022-10-04 14:56:41.740808 binsize-0.1.3/src/binsize/lib/common.py
+-rw-r--r--   0        0        0     1196 2022-09-29 11:48:57.116151 binsize-0.1.3/src/binsize/lib/data_handler.py
+-rw-r--r--   0        0        0     2347 2022-10-04 09:02:51.011862 binsize-0.1.3/src/binsize/lib/data_loader.py
+-rw-r--r--   0        0        0     4600 2022-10-04 10:31:44.342711 binsize-0.1.3/src/binsize/lib/map_file_analyzer.py
+-rw-r--r--   0        0        0     3898 2022-10-03 15:44:09.706221 binsize-0.1.3/src/binsize/lib/map_file_includer.py
+-rw-r--r--   0        0        0     7974 2022-10-04 15:19:36.769646 binsize-0.1.3/src/binsize/lib/row_handler_c.py
+-rw-r--r--   0        0        0     3630 2023-07-27 08:21:32.250578 binsize-0.1.3/src/binsize/lib/row_handler_common.py
+-rw-r--r--   0        0        0    11329 2023-07-27 08:21:32.250578 binsize-0.1.3/src/binsize/lib/row_handler_mpy.py
+-rw-r--r--   0        0        0     6681 2023-07-27 08:21:32.251578 binsize-0.1.3/src/binsize/lib/row_handler_rust.py
+-rw-r--r--   0        0        0     3350 2022-10-04 10:03:26.921409 binsize-0.1.3/src/binsize/lib/source_definition_cache.py
+-rw-r--r--   0        0        0        0 2022-09-29 11:48:57.116151 binsize-0.1.3/src/binsize/plugins/__init__.py
+-rw-r--r--   0        0        0     3407 2022-10-03 14:28:03.859332 binsize-0.1.3/src/binsize/plugins/size_tree.py
+-rw-r--r--   0        0        0     4503 2022-10-03 15:44:09.814221 binsize-0.1.3/src/binsize/plugins/statistics.py
+-rw-r--r--   0        0        0     2234 2022-10-04 15:20:11.772786 binsize-0.1.3/src/binsize/settings.py
+-rw-r--r--   0        0        0      214 2022-10-04 15:02:33.626022 binsize-0.1.3/src/binsize/settings_template.json
+-rw-r--r--   0        0        0      486 2022-10-04 15:19:31.071623 binsize-0.1.3/src/binsize/user_data.py
+-rw-r--r--   0        0        0     1326 2022-10-04 08:29:33.299979 binsize-0.1.3/src/binsize/utils.py
+-rw-r--r--   0        0        0     3020 1970-01-01 00:00:00.000000 binsize-0.1.3/PKG-INFO
```

### Comparing `binsize-0.1.2/LICENSE` & `binsize-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/README.md` & `binsize-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/pyproject.toml` & `binsize-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "binsize"
-version = "0.1.2"
+version = "0.1.3"
 description = "Tool to analyze the size of a binary from .elf file"
 license = "MIT"
 authors = [
     "SatoshiLabs <info@satoshilabs.com>",
     "grdddj <jiri.musil06@seznam.cz>",
 ]
 readme = "README.md"
```

### Comparing `binsize-0.1.2/src/binsize/cli/binsize.py` & `binsize-0.1.3/src/binsize/cli/binsize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """
 Main entry-point of the CLI for the `binsize` command.
 """
 
 from __future__ import annotations
 
 import click
+import sys
 
 from .. import set_root_dir
 from . import build, commit, compare, get, history, tree
 
 
-@click.group()
+@click.group(invoke_without_command=True)
 @click.option("-r", "--root-dir", help="Root directory of the project")
-def cli(root_dir: str | None) -> None:
+@click.option("-v", "--version", is_flag=True, help="Show current version and exit")
+def cli(root_dir: str | None, version: bool) -> None:
     """
     CLI for binary size analysis based on `.elf` file.
 
     Requires `bloaty` and `nm` to run.
 
     See subcommands for details.
     """
+    if version:
+        from .. import __version__
+
+        click.echo(__version__)
+        sys.exit(0)
     if root_dir:
         set_root_dir(root_dir)
 
 
 cli.add_command(build.build)
 cli.add_command(commit.commit)
 cli.add_command(compare.compare)
```

### Comparing `binsize-0.1.2/src/binsize/cli/build.py` & `binsize-0.1.3/src/binsize/cli/build.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/cli/commit.py` & `binsize-0.1.3/src/binsize/cli/commit.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/cli/compare.py` & `binsize-0.1.3/src/binsize/cli/compare.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/cli/get.py` & `binsize-0.1.3/src/binsize/cli/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,40 +72,42 @@
     "--no-aggregation",
     "--na",
     is_flag=True,
     help="Do not aggregate symbols together",
 )
 @click.option("-S", "--no-sort", "--ns", is_flag=True, help="Do not sort by size")
 @click.option("-P", "--no-processing", "--np", is_flag=True, help="See just raw data")
+@click.option("-D", "--debug", is_flag=True, help="See also raw symbol data")
 def get(
     elf_file: str,
     map_file: str | None,
     sections: list[str] | None,
     output_file: str,
     language: str,
     grep: str,
     module_name: str,
     func_name: str,
     build: bool,
     add_definitions: bool,
     no_processing: bool,
     no_sort: bool,
     no_aggregation: bool,
+    debug: bool,
 ) -> None:
     """Analyze a single binary."""
 
     if build:
         build_binary()
 
     BS = BinarySize()
 
     BS.load_file(elf_file, sections=sections)
 
     if no_processing:
-        return BS.show()
+        return BS.show(output_file or None)
 
     if map_file and sections:
         BS.use_map_file(map_file, sections=sections)
 
     BS.add_basic_info()
 
     if not no_aggregation:
@@ -128,15 +130,12 @@
             )
     if grep:
         BS.filter(lambda row: grep.lower() in str(row).lower())
 
     if add_definitions:
         BS.add_definitions()
 
-    if output_file:
-        BS.show(output_file)
-    else:
-        BS.show()
+    BS.show(output_file or None, debug=debug)
 
 
 if "__main__" == __name__:
     get()
```

### Comparing `binsize-0.1.2/src/binsize/cli/history.py` & `binsize-0.1.3/src/binsize/cli/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import shutil
 import subprocess
+import sys
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from typing import Generator, Sequence
 
 import click
 
@@ -61,15 +62,17 @@
     return Path(f"{ELF_FILE}_{commit_hash}")
 
 
 @contextmanager
 def change_to_commit_and_back(commit_hash: str) -> Generator[None, None, None]:
     """Context manager that changes to the given commit and then back."""
     current_branch = get_current_branch_name()
-    # NOTE: will fail if there are some local uncommited changed
+    # Fails if there are some local uncommited changes
+    if are_there_local_changes():
+        sys.exit(1)
     run_cmd(["git", "checkout", commit_hash])
     yield
     run_cmd(["git", "reset", "--hard", "HEAD"])
     run_cmd(["git", "checkout", current_branch])
 
 
 def build_and_rename_fw(commit_hash: str) -> None:
@@ -86,16 +89,20 @@
         run_cmd(BUILD_CMD.split())
         shutil.copyfile(ELF_FILE, new_path)
 
 
 def create_binaries(commit_hashes: list[str]) -> None:
     """Build multiple binaries given list of commit hashes."""
     for commit_hash in commit_hashes:
-        print(commit_hash, get_commit_date(commit_hash))
-        build_and_rename_fw(commit_hash)
+        try:
+            print(commit_hash, get_commit_date(commit_hash))
+            build_and_rename_fw(commit_hash)
+        except Exception as e:
+            print(f"ERRROOOR: Failed to build binary for commit {commit_hash}: {e}")
+            run_cmd(["git", "reset", "--hard", "HEAD"])
 
 
 def analyze_sizes(
     commit_hashes: list[str], sections: Sequence[str] | None = None
 ) -> None:
     sizes: dict[str, dict[str, int]] = {}
     for commit_hash in commit_hashes:
```

### Comparing `binsize-0.1.2/src/binsize/cli/tree.py` & `binsize-0.1.3/src/binsize/cli/tree.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/api.py` & `binsize-0.1.3/src/binsize/lib/api.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/binary_size.py` & `binsize-0.1.3/src/binsize/lib/binary_size.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/build_definition_loader.py` & `binsize-0.1.3/src/binsize/lib/build_definition_loader.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/common.py` & `binsize-0.1.3/src/binsize/lib/common.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/data_handler.py` & `binsize-0.1.3/src/binsize/lib/data_handler.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/data_loader.py` & `binsize-0.1.3/src/binsize/lib/data_loader.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/map_file_analyzer.py` & `binsize-0.1.3/src/binsize/lib/map_file_analyzer.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/map_file_includer.py` & `binsize-0.1.3/src/binsize/lib/map_file_includer.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/row_handler_c.py` & `binsize-0.1.3/src/binsize/lib/row_handler_c.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/lib/row_handler_common.py` & `binsize-0.1.3/src/binsize/lib/row_handler_common.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,22 @@
 if TYPE_CHECKING:  # pragma: no cover
     from .api import DataRow, SourceDefinitionCacheAPI
 
 INVALID_FILE_PREFIX = "--invalid_file--"
 
 # Defining all the prefixes here at one place,
 # so we see they are not clashing with each other
-MPY_PREFIXES = ("fun_data_", "const_table_data_", "const_obj_", "raw_code_")
+MPY_PREFIXES = (
+    "fun_data_",
+    "const_qstr_table_data_",
+    "const_obj_table_data_",
+    "const_obj_",
+    "raw_code_",
+    "children_",
+)
 RUST_PREFIXES = (
     "trezor_lib",
     "compiler_builtins",
     "core::",
     "_$LT$",
     "heapless::",
     "cstr_core::",
```

### Comparing `binsize-0.1.2/src/binsize/lib/row_handler_mpy.py` & `binsize-0.1.3/src/binsize/lib/row_handler_mpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,29 +143,50 @@
         return row.symbol_name.startswith("const_obj_")
 
     def _get_module_and_function(self, symbol_name: str) -> tuple[str, str]:
         for prefix in MPY_PREFIXES:
             if symbol_name.startswith(prefix):
                 symbol_name = symbol_name[len(prefix) :]
 
-        # There are possible numbers at the end, delete them
-        symbol_name = re.sub(r"__lt_module_gt__\d+$", "__lt_module_gt__", symbol_name)
+        # There are possible numbers at the end, delete them, unless it really is there
+        exceptions = [
+            "blake_hash_writer_32",
+            "_migrate_from_version_01",
+            "sha256d_32",
+            "groestl512d_32",
+            "blake256d_32",
+            "keccak_32",
+            "ripemd160_32",
+        ]
+        if not any(symbol_name.endswith(ex) for ex in exceptions):
+            symbol_name = re.sub(r"_\d+$", "", symbol_name)
 
-        # Splitting between module and function, if both exist
-        if "__lt_module_gt__" in symbol_name:
-            module_name, func_name = symbol_name.split("__lt_module_gt__", maxsplit=1)
-        else:
-            module_name = symbol_name.replace("__lt_module_gt_", "")  # stuff at the end
+        module_end = "__lt_module_gt_"
+        if symbol_name.endswith(module_end):
+            # It is only module name, no function
+            module_path = symbol_name[: -len(module_end)]
+            module_name, module_is_valid = resolve_module(module_path)
             func_name = ""
+        else:
+            # Iterating from back to front, trying to resolve the valid module name
+            split_symbol = symbol_name.split("_")
+            for i in range(len(split_symbol), 0, -1):
+                module_part = "_".join(split_symbol[:i])
+                func_part = "_".join(split_symbol[i:])
+                module_name, module_is_valid = resolve_module(module_part)
+                func_name = resolve_function_name(func_part, module_name)
+                if module_is_valid:
+                    break
+            else:
+                module_is_valid = False
+                module_name = "_".join(split_symbol[:-1])
+                func_name = split_symbol[-1]
 
-        module_name, is_valid = resolve_module(module_name)
-        if not is_valid:
+        if not module_is_valid:
             module_name = f"{INVALID_FILE_PREFIX}{module_name}"
-        else:
-            func_name = resolve_function_name(func_name, module_name)
 
         return module_name, func_name
 
     def _get_definition(self, row: DataRow) -> str:
         # There is only a module, no need to locate any function definition
         if not row.func_name:
             return row.module_name
@@ -282,19 +303,12 @@
     # are both valid directories
     if (
         not Path(settings.ROOT_DIR / file_path).exists()
         and "apps/monero/" in file_path
         and "serialize/messages" in file_path
     ):
         file_path = file_path.replace("serialize/messages_", "serialize_messages/")
-    # Special case for src/trezor/ui/layouts, where both "tt" and "tt_v2" are valid
-    if (
-        not Path(settings.ROOT_DIR / file_path).exists()
-        and "ui/layouts/" in file_path
-        and "tt/v2_" in file_path
-    ):
-        file_path = file_path.replace("tt/v2_", "tt_v2/")
 
     # It may happen that the file does not exist - it may not even be a python file
     is_valid = Path(settings.ROOT_DIR / file_path).exists()
 
     return file_path, is_valid
```

### Comparing `binsize-0.1.2/src/binsize/lib/row_handler_rust.py` & `binsize-0.1.3/src/binsize/lib/row_handler_rust.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,18 +85,24 @@
     else:
         struct_name = ""
 
     file_path = "embed/rust/src"
     for item in items:
         file_path += f"/{item}"
 
-    file_path = f"{file_path}.rs"
+    if Path(settings.ROOT_DIR / f"{file_path}.rs").exists():
+        file_path = f"{file_path}.rs"
+    else:
+        # could be that it points to mod.rs
+        mod_file_path = f"{file_path}/mod.rs"
 
-    if not Path(settings.ROOT_DIR / file_path).exists():
-        file_path = f"{INVALID_FILE_PREFIX}{file_path}"
+        if Path(settings.ROOT_DIR / mod_file_path).exists():
+            file_path = mod_file_path
+        else:
+            file_path = f"{INVALID_FILE_PREFIX}{file_path}.rs"
 
     if struct_name:
         struct_and_function = f"{struct_name}::{function_name}()"
     else:
         struct_and_function = f"{function_name}()"
 
     return file_path, struct_and_function
```

### Comparing `binsize-0.1.2/src/binsize/lib/source_definition_cache.py` & `binsize-0.1.3/src/binsize/lib/source_definition_cache.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/plugins/size_tree.py` & `binsize-0.1.3/src/binsize/plugins/size_tree.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/plugins/statistics.py` & `binsize-0.1.3/src/binsize/plugins/statistics.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/settings.py` & `binsize-0.1.3/src/binsize/settings.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/src/binsize/utils.py` & `binsize-0.1.3/src/binsize/utils.py`

 * *Files identical despite different names*

### Comparing `binsize-0.1.2/PKG-INFO` & `binsize-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: binsize
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tool to analyze the size of a binary from .elf file
 Home-page: https://github.com/grdddj/binsize
 License: MIT
 Keywords: binary size,code size,.elf file
 Author: SatoshiLabs
 Author-email: info@satoshilabs.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: platformdirs (>=2.5.2,<3.0.0)
 Requires-Dist: termcolor (>=2.0.1,<3.0.0)
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/grdddj/binsize
 Description-Content-Type: text/markdown
```

