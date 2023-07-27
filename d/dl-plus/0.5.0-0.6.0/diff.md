# Comparing `tmp/dl-plus-0.5.0.tar.gz` & `tmp/dl-plus-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dl-plus-0.5.0.tar", last modified: Thu Jan  7 13:09:09 2021, max compression
+gzip compressed data, was "dl-plus-0.6.0.tar", last modified: Thu Jul 27 11:01:24 2023, max compression
```

## Comparing `dl-plus-0.5.0.tar` & `dl-plus-0.6.0.tar`

### file list

```diff
@@ -1,45 +1,52 @@
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.910997 dl-plus-0.5.0/
--rw-rw-r--   0 def       (1000) def       (1004)     1077 2020-10-25 11:55:34.000000 dl-plus-0.5.0/LICENSE
--rw-rw-r--   0 def       (1000) def       (1004)     4567 2021-01-07 13:09:09.910997 dl-plus-0.5.0/PKG-INFO
--rw-rw-r--   0 def       (1000) def       (1004)     2865 2021-01-07 13:07:05.000000 dl-plus-0.5.0/README.md
--rw-rw-r--   0 def       (1000) def       (1004)     1045 2021-01-07 13:09:09.910997 dl-plus-0.5.0/setup.cfg
--rw-rw-r--   0 def       (1000) def       (1004)       39 2020-10-18 10:59:22.000000 dl-plus-0.5.0/setup.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.906997 dl-plus-0.5.0/src/
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.906997 dl-plus-0.5.0/src/dl_plus/
--rw-rw-r--   0 def       (1000) def       (1004)       38 2020-12-03 17:26:06.000000 dl-plus-0.5.0/src/dl_plus/__main__.py
--rw-rw-r--   0 def       (1000) def       (1004)     1935 2020-12-07 16:16:35.000000 dl-plus-0.5.0/src/dl_plus/backend.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.910997 dl-plus-0.5.0/src/dl_plus/cli/
--rw-rw-r--   0 def       (1000) def       (1004)       43 2020-11-24 13:16:53.000000 dl-plus-0.5.0/src/dl_plus/cli/__init__.py
--rw-rw-r--   0 def       (1000) def       (1004)      924 2020-12-01 20:27:27.000000 dl-plus-0.5.0/src/dl_plus/cli/args.py
--rw-rw-r--   0 def       (1000) def       (1004)     3694 2020-12-01 20:21:52.000000 dl-plus-0.5.0/src/dl_plus/cli/cli.py
--rw-rw-r--   0 def       (1000) def       (1004)     2558 2020-11-24 15:41:01.000000 dl-plus-0.5.0/src/dl_plus/cli/command.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.910997 dl-plus-0.5.0/src/dl_plus/cli/commands/
--rw-rw-r--   0 def       (1000) def       (1004)      277 2020-12-07 15:52:33.000000 dl-plus-0.5.0/src/dl_plus/cli/commands/__init__.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.910997 dl-plus-0.5.0/src/dl_plus/cli/commands/backend/
--rw-rw-r--   0 def       (1000) def       (1004)      313 2020-12-01 20:25:18.000000 dl-plus-0.5.0/src/dl_plus/cli/commands/backend/__init__.py
--rw-rw-r--   0 def       (1000) def       (1004)      790 2020-12-01 20:25:42.000000 dl-plus-0.5.0/src/dl_plus/cli/commands/backend/info.py
--rw-rw-r--   0 def       (1000) def       (1004)     1058 2020-12-07 16:05:42.000000 dl-plus-0.5.0/src/dl_plus/cli/commands/backend/install.py
--rw-rw-r--   0 def       (1000) def       (1004)     3232 2020-12-07 16:17:52.000000 dl-plus-0.5.0/src/dl_plus/cli/commands/base.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.910997 dl-plus-0.5.0/src/dl_plus/cli/commands/extractor/
--rw-rw-r--   0 def       (1000) def       (1004)      257 2020-12-07 15:33:39.000000 dl-plus-0.5.0/src/dl_plus/cli/commands/extractor/__init__.py
--rw-rw-r--   0 def       (1000) def       (1004)     1533 2020-12-07 16:56:07.000000 dl-plus-0.5.0/src/dl_plus/cli/commands/extractor/install.py
--rw-rw-r--   0 def       (1000) def       (1004)     3744 2020-12-26 11:11:09.000000 dl-plus-0.5.0/src/dl_plus/config.py
--rw-rw-r--   0 def       (1000) def       (1004)       65 2021-01-07 13:07:52.000000 dl-plus-0.5.0/src/dl_plus/const.py
--rw-rw-r--   0 def       (1000) def       (1004)     1896 2020-12-07 17:15:23.000000 dl-plus-0.5.0/src/dl_plus/core.py
--rw-rw-r--   0 def       (1000) def       (1004)      564 2020-11-25 16:32:48.000000 dl-plus-0.5.0/src/dl_plus/exceptions.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.910997 dl-plus-0.5.0/src/dl_plus/extractor/
--rw-rw-r--   0 def       (1000) def       (1004)      757 2020-11-14 15:24:20.000000 dl-plus-0.5.0/src/dl_plus/extractor/__init__.py
--rw-rw-r--   0 def       (1000) def       (1004)      839 2020-11-14 15:24:20.000000 dl-plus-0.5.0/src/dl_plus/extractor/extractor.py
--rw-rw-r--   0 def       (1000) def       (1004)     2116 2020-11-09 10:05:17.000000 dl-plus-0.5.0/src/dl_plus/extractor/machinery.py
--rw-rw-r--   0 def       (1000) def       (1004)     3134 2020-11-17 01:27:58.000000 dl-plus-0.5.0/src/dl_plus/extractor/peqn.py
--rw-rw-r--   0 def       (1000) def       (1004)     5817 2020-11-14 15:24:20.000000 dl-plus-0.5.0/src/dl_plus/extractor/plugin.py
--rw-rw-r--   0 def       (1000) def       (1004)     3809 2020-12-07 15:52:33.000000 dl-plus-0.5.0/src/dl_plus/pypi.py
--rw-rw-r--   0 def       (1000) def       (1004)      276 2020-10-20 23:32:21.000000 dl-plus-0.5.0/src/dl_plus/utils.py
--rw-rw-r--   0 def       (1000) def       (1004)     5218 2020-11-25 16:32:48.000000 dl-plus-0.5.0/src/dl_plus/ytdl.py
-drwxrwxr-x   0 def       (1000) def       (1004)        0 2021-01-07 13:09:09.910997 dl-plus-0.5.0/src/dl_plus.egg-info/
--rw-rw-r--   0 def       (1000) def       (1004)     4567 2021-01-07 13:09:09.000000 dl-plus-0.5.0/src/dl_plus.egg-info/PKG-INFO
--rw-rw-r--   0 def       (1000) def       (1004)     1006 2021-01-07 13:09:09.000000 dl-plus-0.5.0/src/dl_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 def       (1000) def       (1004)        1 2021-01-07 13:09:09.000000 dl-plus-0.5.0/src/dl_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 def       (1000) def       (1004)       46 2021-01-07 13:09:09.000000 dl-plus-0.5.0/src/dl_plus.egg-info/entry_points.txt
--rw-rw-r--   0 def       (1000) def       (1004)        1 2021-01-07 13:09:09.000000 dl-plus-0.5.0/src/dl_plus.egg-info/not-zip-safe
--rw-rw-r--   0 def       (1000) def       (1004)        8 2021-01-07 13:09:09.000000 dl-plus-0.5.0/src/dl_plus.egg-info/top_level.txt
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.239970 dl-plus-0.6.0/
+-rw-rw-r--   0 def       (1000) def       (1000)     1077 2022-04-23 13:15:25.000000 dl-plus-0.6.0/LICENSE
+-rw-rw-r--   0 def       (1000) def       (1000)     5090 2023-07-27 11:01:24.239970 dl-plus-0.6.0/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)     2994 2023-07-27 10:36:26.000000 dl-plus-0.6.0/README.md
+-rw-rw-r--   0 def       (1000) def       (1000)     2283 2023-07-25 10:53:08.000000 dl-plus-0.6.0/pyproject.toml
+-rw-rw-r--   0 def       (1000) def       (1000)       38 2023-07-27 11:01:24.239970 dl-plus-0.6.0/setup.cfg
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.235970 dl-plus-0.6.0/src/
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.235970 dl-plus-0.6.0/src/dl_plus/
+-rw-rw-r--   0 def       (1000) def       (1000)       38 2022-04-23 13:15:25.000000 dl-plus-0.6.0/src/dl_plus/__main__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3659 2023-07-27 08:30:33.000000 dl-plus-0.6.0/src/dl_plus/backend.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.235970 dl-plus-0.6.0/src/dl_plus/cli/
+-rw-rw-r--   0 def       (1000) def       (1000)       43 2022-04-23 13:15:25.000000 dl-plus-0.6.0/src/dl_plus/cli/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1931 2023-07-03 14:42:02.000000 dl-plus-0.6.0/src/dl_plus/cli/args.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3911 2023-07-05 12:55:03.000000 dl-plus-0.6.0/src/dl_plus/cli/cli.py
+-rw-rw-r--   0 def       (1000) def       (1000)     2773 2023-07-25 09:51:10.000000 dl-plus-0.6.0/src/dl_plus/cli/command.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.235970 dl-plus-0.6.0/src/dl_plus/cli/commands/
+-rw-rw-r--   0 def       (1000) def       (1000)      372 2023-07-03 13:49:40.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/__init__.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.239970 dl-plus-0.6.0/src/dl_plus/cli/commands/backend/
+-rw-rw-r--   0 def       (1000) def       (1000)      384 2023-07-03 14:49:37.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/backend/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)      437 2023-07-03 14:56:11.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/backend/base.py
+-rw-rw-r--   0 def       (1000) def       (1000)      852 2023-07-03 15:07:49.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/backend/info.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1019 2023-07-03 15:24:37.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/backend/install.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1090 2023-07-03 15:26:11.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/backend/update.py
+-rw-rw-r--   0 def       (1000) def       (1000)     8112 2023-07-03 15:12:09.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/base.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.239970 dl-plus-0.6.0/src/dl_plus/cli/commands/extractor/
+-rw-rw-r--   0 def       (1000) def       (1000)      332 2023-07-01 13:45:38.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/extractor/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1059 2023-07-03 15:12:18.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/extractor/base.py
+-rw-rw-r--   0 def       (1000) def       (1000)      987 2023-07-03 12:11:53.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/extractor/install.py
+-rw-rw-r--   0 def       (1000) def       (1000)      524 2023-07-03 12:11:48.000000 dl-plus-0.6.0/src/dl_plus/cli/commands/extractor/update.py
+-rw-rw-r--   0 def       (1000) def       (1000)     4186 2023-07-27 08:30:33.000000 dl-plus-0.6.0/src/dl_plus/config.py
+-rw-rw-r--   0 def       (1000) def       (1000)       65 2023-07-27 10:39:09.000000 dl-plus-0.6.0/src/dl_plus/const.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1930 2023-07-27 08:30:33.000000 dl-plus-0.6.0/src/dl_plus/core.py
+-rw-rw-r--   0 def       (1000) def       (1000)      765 2023-07-24 13:28:25.000000 dl-plus-0.6.0/src/dl_plus/deprecated.py
+-rw-rw-r--   0 def       (1000) def       (1000)      564 2022-04-23 13:15:25.000000 dl-plus-0.6.0/src/dl_plus/exceptions.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.239970 dl-plus-0.6.0/src/dl_plus/extractor/
+-rw-rw-r--   0 def       (1000) def       (1000)      413 2023-07-25 09:52:48.000000 dl-plus-0.6.0/src/dl_plus/extractor/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1532 2023-07-24 13:29:10.000000 dl-plus-0.6.0/src/dl_plus/extractor/extractor.py
+-rw-rw-r--   0 def       (1000) def       (1000)     2116 2022-04-23 13:15:25.000000 dl-plus-0.6.0/src/dl_plus/extractor/machinery.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3134 2022-04-23 13:15:25.000000 dl-plus-0.6.0/src/dl_plus/extractor/peqn.py
+-rw-rw-r--   0 def       (1000) def       (1000)     5817 2022-04-23 13:15:25.000000 dl-plus-0.6.0/src/dl_plus/extractor/plugin.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3819 2023-07-01 13:45:38.000000 dl-plus-0.6.0/src/dl_plus/pypi.py
+-rw-rw-r--   0 def       (1000) def       (1000)      276 2022-04-23 13:15:25.000000 dl-plus-0.6.0/src/dl_plus/utils.py
+-rw-rw-r--   0 def       (1000) def       (1000)     6114 2023-07-02 11:13:30.000000 dl-plus-0.6.0/src/dl_plus/ytdl.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.235970 dl-plus-0.6.0/src/dl_plus.egg-info/
+-rw-rw-r--   0 def       (1000) def       (1000)     5090 2023-07-27 11:01:24.000000 dl-plus-0.6.0/src/dl_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)     1217 2023-07-27 11:01:24.000000 dl-plus-0.6.0/src/dl_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2023-07-27 11:01:24.000000 dl-plus-0.6.0/src/dl_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 def       (1000) def       (1000)       45 2023-07-27 11:01:24.000000 dl-plus-0.6.0/src/dl_plus.egg-info/entry_points.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2023-07-27 11:01:24.000000 dl-plus-0.6.0/src/dl_plus.egg-info/not-zip-safe
+-rw-rw-r--   0 def       (1000) def       (1000)        8 2023-07-27 11:01:24.000000 dl-plus-0.6.0/src/dl_plus.egg-info/top_level.txt
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-07-27 11:01:24.239970 dl-plus-0.6.0/tests/
+-rw-rw-r--   0 def       (1000) def       (1000)      402 2023-07-01 14:25:07.000000 dl-plus-0.6.0/tests/testlib.py
```

### Comparing `dl-plus-0.5.0/LICENSE` & `dl-plus-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dl-plus-0.5.0/README.md` & `dl-plus-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # dl-plus
 
 A [youtube-dl][youtube-dl-website] extension with pluggable extractors
 
 ## Description
 
-`dl-plus` is an extension and a drop-in replacement of `youtube-dl`. The main goal of the project is to add an easy-to-use extractor plugin system to `youtube-dl` while maintaining full backward compatibility.
+`dl-plus` is an extension and a drop-in replacement of `youtube-dl` (or any compatible fork, e.g., `yt-dlp`). The main goal of the project is to add an easy-to-use extractor plugin system to `youtube-dl` while maintaining full backward compatibility.
 
 `dl-plus` is not a fork of `youtube-dl` and does not contain code from `youtube-dl`, it is a pure dynamic wrapper (thanks to Python dynamic nature) hacking some `youtube-dl` internals.
 
 ## Installation
 
 1.  Install `dl-plus`:
 
@@ -20,37 +20,42 @@
 
     * using pip:
 
       ```
       pip install dl-plus
       ```
 
-2.  Install `youtube-dl` or any compatible package (fork):
+    (**\*nix**) Alternatively, you can download a single file binary (zipapp) and put it somewhere in your `PATH`:
+
+    ```
+    curl -L https://github.com/un-def/dl-plus/releases/latest/download/dl-plus -o dl-plus
+    chmod a+x dl-plus
+    ```
+
+2.  Install a backend — `youtube-dl` or any compatible package (fork), e.g., `yt-dlp`:
 
     * using `dl-plus` itself:
 
       ```
-      dl-plus --cmd backend install
+      dl-plus --cmd backend install yt-dlp
       ```
 
     * using [pipx][pipx-website]:
 
       ```
-      pipx inject dl-plus youtube-dl
+      pipx inject dl-plus yt-dlp
       ```
 
     * using pip:
 
       ```
-      pip install youtube-dl
+      pip install yt-dlp
       ```
 
-    **NOTE**: if you use a fork where an import path was changed (it is `youtube_dl` by default), you'll need to configure a backend using the config file or the `--backend` command line option.
-
-3.  (optional) Install some plugins:
+3.  (optional) Install some extractor plugins:
 
     * using `dl-plus` itself:
 
       ```
       dl-plus --cmd extractor install un1def/wasdtv
       ```
```

### Comparing `dl-plus-0.5.0/src/dl_plus/cli/cli.py` & `dl-plus-0.6.0/src/dl_plus/cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import argparse
-import os.path
+import pathlib
 import sys
 from textwrap import dedent
 
 from dl_plus import core, ytdl
-from dl_plus.backend import init_backend
+from dl_plus.backend import KnownBackend, init_backend
 from dl_plus.config import Config
 from dl_plus.const import DL_PLUS_VERSION
 from dl_plus.exceptions import DLPlusException
 
-from . import args
+from . import args as cli_args
 
 
 __all__ = ['main']
 
 _PROG = 'dl-plus'
 _CMD = '--cmd'
 
 
 def _dedent(text):
     return dedent(text).strip()
 
 
-def _is_running_as_youtube_dl(program_name: str) -> bool:
-    return os.path.basename(program_name) in ['youtube-dl', 'youtube-dl.exe']
+def _detect_compat_mode(program_name: str) -> bool:
+    path = pathlib.Path(program_name)
+    if path.suffix == '.exe':
+        name = path.stem
+    else:
+        name = path.name
+    return name in (backend.executable_name for backend in KnownBackend)
 
 
 class _MainArgParser(argparse.ArgumentParser):
 
     def format_help(self):
         return super().format_help() + ytdl.get_help()
 
@@ -46,16 +51,20 @@
 
             The following are %(prog)s options:
         """),
         epilog='The following are youtube-dl options:',
         add_help=False,
         formatter_class=argparse.RawTextHelpFormatter,
     )
-    args.dlp_config.add_to_parser(parser)
-    args.backend.add_to_parser(parser)
+    cli_args.dlp_config.add_to_parser(parser)
+    parser.add_argument(
+        '--backend',
+        metavar='BACKEND',
+        help='youtube-dl backend.',
+    )
     parser.add_argument(
         '--dlp-version',
         action='version',
         version=DL_PLUS_VERSION,
         help='Print dl-plus version and exit.',
     )
     extractor_group = parser.add_mutually_exclusive_group()
@@ -79,15 +88,15 @@
     return parser
 
 
 def _main(argv):
     args = argv[1:]
     if '-U' in args or '--update' in args:
         raise DLPlusException('update is not yet supported')
-    compat_mode = _is_running_as_youtube_dl(argv[0])
+    compat_mode = _detect_compat_mode(argv[0])
     config = Config()
     backend = None
     if not compat_mode:
         if _CMD in args:
             from .command import run_command
             run_command(prog=_PROG, cmd_arg=_CMD, args=args)
             return
```

### Comparing `dl-plus-0.5.0/src/dl_plus/cli/command.py` & `dl-plus-0.6.0/src/dl_plus/cli/command.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+from __future__ import annotations
+
 import argparse
-from typing import List
+from typing import TYPE_CHECKING, List, Type
 
 from .commands import RootCommandGroup
 from .commands.base import CommandGroup
 
 
+if TYPE_CHECKING:
+    from .commands.base import Command
+
+
 __all__ = ['run_command']
 
 
 _COMMAND_DEST = 'command'
 
 
 class CommandNamespace(argparse.Namespace):
@@ -29,19 +35,22 @@
 class CommandArgParser(argparse.ArgumentParser):
 
     def __init__(self, *args, **kwargs):
         kwargs.setdefault(
             'formatter_class', argparse.RawDescriptionHelpFormatter)
         super().__init__(*args, **kwargs)
 
-    def add_command_arguments(self, command):
+    def add_command_arguments(self, command: Type[Command]):
+        for parent in command.get_parents():
+            for arg in parent.arguments:
+                arg.add_to_parser(self)
         for arg in command.arguments:
             arg.add_to_parser(self)
 
-    def add_command_group(self, command_group):
+    def add_command_group(self, command_group: Type[CommandGroup]):
         command_group_subparsers = self.add_command_group_subparsers(
             title=command_group.short_description)
         for command_or_group in command_group.commands:
             description = (
                 command_or_group.long_description
                 or command_or_group.short_description
             )
@@ -55,17 +64,16 @@
             else:
                 command_parser.add_command_arguments(command_or_group)
 
     def add_command_group_subparsers(self, *args, **kwargs):
         kwargs.setdefault('dest', _COMMAND_DEST)
         kwargs.setdefault('metavar', 'COMMAND')
         kwargs.setdefault('parser_class', self.__class__)
-        # Python 3.6 — add_subparsers(required=...) is not supported
+        kwargs.setdefault('required', True)
         subparsers = self.add_subparsers(*args, **kwargs)
-        subparsers.required = True
         return subparsers
 
 
 def run_command(prog: str, cmd_arg: str, args: List[str]) -> None:
     parser = CommandArgParser(prog=f'{prog} {cmd_arg}')
     parser.add_argument(
         cmd_arg, action='store_true', required=True, help=argparse.SUPPRESS)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dl-plus-0.5.0/src/dl_plus/cli/commands/backend/info.py` & `dl-plus-0.6.0/src/dl_plus/cli/commands/backend/info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from dl_plus.backend import init_backend
-from dl_plus.cli import args
+from dl_plus.cli.args import Arg
 from dl_plus.cli.commands.base import Command
 
 
 class BackendInfoCommand(Command):
 
     short_description = 'Show backend information'
 
     arguments = (
-        args.dlp_config,
-        args.backend,
+        Arg(
+            'name', nargs='?', metavar='NAME',
+            help='Backend name.'
+        ),
     )
 
     def run(self):
-        backend = self.args.backend or self.config.backend
-        backend_info = init_backend(backend)
-        print('import name:', backend_info.import_name)
-        print('version:', backend_info.version)
-        print('path:', str(backend_info.path))
-        print('managed:', 'yes' if backend_info.is_managed else 'no')
+        backend_info = init_backend(self.args.name or self.config.backend)
+        self.print('import name:', backend_info.import_name)
+        self.print('version:', backend_info.version)
+        self.print('path:', str(backend_info.path))
+        self.print('managed:', 'yes' if backend_info.is_managed else 'no')
         metadata = backend_info.metadata
         if metadata:
-            print('project name:', metadata.name)
-            print('project version:', metadata.version)
+            self.print('project name:', metadata.name)
+            self.print('project version:', metadata.version)
```

### Comparing `dl-plus-0.5.0/src/dl_plus/config.py` & `dl-plus-0.6.0/src/dl_plus/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,44 @@
+import enum
 import itertools
 import os
 import shlex
 from configparser import ConfigParser
 from pathlib import Path
 from typing import List, Optional, Union
 
 from .exceptions import DLPlusException
 
 
-DEFAULT_CONFIG = """
+class _StrEnum(str, enum.Enum):
+    # enum.StrEnum is available since Python 3.11
+
+    def __str__(self) -> str:
+        return self.value
+
+
+class Option:
+
+    class Backend(_StrEnum):
+        AUTODETECT = ':autodetect:'
+
+    class Extractor(_StrEnum):
+        BUILTINS = ':builtins:'
+        PLUGINS = ':plugins:'
+        GENERIC = 'generic'
+
+
+DEFAULT_CONFIG = f"""
 [main]
-backend = youtube_dl
+backend = {Option.Backend.AUTODETECT}
 
 [extractors.enable]
-:builtins:
-:plugins:
-generic
+{Option.Extractor.PLUGINS}
+{Option.Extractor.BUILTINS}
+{Option.Extractor.GENERIC}
 """
 
 
 class ConfigError(DLPlusException):
 
     pass
 
@@ -79,15 +98,15 @@
             strict=True,
             empty_lines_in_values=False,
             default_section=None,
             interpolation=None,
         )
 
 
-class Option:
+class _ConfigOption:
 
     __slots__ = ('section', 'option')
 
     def __init__(self, section: str, option: str) -> None:
         self.section = section
         self.option = option
 
@@ -133,8 +152,8 @@
 
     def get_backend_options(self) -> Optional[List[str]]:
         if 'backend-options' not in self:
             return None
         return list(itertools.chain.from_iterable(
             map(shlex.split, self.options('backend-options'))))
 
-    backend = Option('main', 'backend')
+    backend = _ConfigOption('main', 'backend')
```

### Comparing `dl-plus-0.5.0/src/dl_plus/core.py` & `dl-plus-0.6.0/src/dl_plus/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Iterable, List, Set, Type
 
 from dl_plus import ytdl
-from dl_plus.config import get_config_home
+from dl_plus.config import Option, get_config_home
 from dl_plus.extractor import machinery
 from dl_plus.extractor.peqn import PEQN
 
 
 if TYPE_CHECKING:
     from .extractor.extractor import Extractor
 
@@ -28,17 +28,17 @@
             return
         path_str = str(path)
         if path_str not in added_search_paths:
             sys.path.insert(0, path_str)
             added_search_paths.add(path_str)
 
     for name in names:
-        if name == ':builtins:':
+        if name == Option.Extractor.BUILTINS:
             extractors = ytdl.get_all_extractors(include_generic=False)
-        elif name == ':plugins:':
+        elif name == Option.Extractor.PLUGINS:
             if extractor_plugins_dir.is_dir():
                 for path in extractor_plugins_dir.iterdir():
                     maybe_add_search_path(path)
             extractors = machinery.load_all_extractors()
         elif '/' in name:
             peqn = PEQN.from_string(name)
             maybe_add_search_path(get_extractor_plugin_dir(
```

### Comparing `dl-plus-0.5.0/src/dl_plus/exceptions.py` & `dl-plus-0.6.0/src/dl_plus/exceptions.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.5.0/src/dl_plus/extractor/machinery.py` & `dl-plus-0.6.0/src/dl_plus/extractor/machinery.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.5.0/src/dl_plus/extractor/peqn.py` & `dl-plus-0.6.0/src/dl_plus/extractor/peqn.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.5.0/src/dl_plus/extractor/plugin.py` & `dl-plus-0.6.0/src/dl_plus/extractor/plugin.py`

 * *Files identical despite different names*

### Comparing `dl-plus-0.5.0/src/dl_plus/pypi.py` & `dl-plus-0.6.0/src/dl_plus/pypi.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 def save_metadata(backend_dir: Path, metadata: Metadata) -> None:
     with open(backend_dir / 'metadata.json', 'w') as fobj:
         json.dump(metadata, fobj)
 
 
-def load_metadata(backend_dir: Path) -> Metadata:
+def load_metadata(backend_dir: Path) -> Optional[Metadata]:
     try:
         with open(backend_dir / 'metadata.json') as fobj:
             return Metadata(json.load(fobj))
     except OSError:
         return None
```

### Comparing `dl-plus-0.5.0/src/dl_plus/ytdl.py` & `dl-plus-0.6.0/src/dl_plus/ytdl.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,30 +18,35 @@
     def __str__(self):
         return f'unknown built-in extractor: {self.name}'
 
 
 _NAME_PART_SURROGATE = '_'
 
 
-_ytdl_module = None
-_ytdl_module_name = None
+_NOT_SET = object()
 
-_extractors = None
-_extractors_registry = None
+
+_ytdl_module = _NOT_SET
+_ytdl_module_name = _NOT_SET
+
+_extractors = _NOT_SET
+_extractors_registry = _NOT_SET
+
+_lazy_load_extractor_base = _NOT_SET
 
 
 def _check_initialized():
     global _ytdl_module
-    if not _ytdl_module:
+    if _ytdl_module is _NOT_SET:
         raise YoutubeDLError('not initialized')
 
 
 def init(ytdl_module_name: str) -> None:
     global _ytdl_module
-    if _ytdl_module:
+    if _ytdl_module is not _NOT_SET:
         raise YoutubeDLError('already initialized')
     try:
         _ytdl_module = importlib.import_module(ytdl_module_name)
     except ImportError as exc:
         raise YoutubeDLError(f'failed to initialize: {exc}') from exc
     global _ytdl_module_name
     _ytdl_module_name = ytdl_module_name
@@ -95,33 +100,54 @@
     module = import_module(module_name)
     if isinstance(names, str):
         return _import_from(module, names)
     return tuple(_import_from(module, name) for name in names)
 
 
 def get_all_extractors(*, include_generic: bool):
+    _check_initialized()
     global _extractors
-    if _extractors is None:
-        extractor_module = import_module('extractor')
-        _extractors = tuple(extractor_module._ALL_CLASSES)
+    if _extractors is _NOT_SET:
+        _extractors = tuple(import_module('extractor')._ALL_CLASSES)
     if include_generic:
         return _extractors
     return _extractors[:-1]
 
 
+def _get_real_extractor(extractor):
+    global _lazy_load_extractor_base
+    if _lazy_load_extractor_base is None:
+        return extractor
+    if _lazy_load_extractor_base is _NOT_SET:
+        try:
+            _lazy_load_extractor_base = import_from(
+                'extractor.lazy_extractors', 'LazyLoadExtractor')
+        except ImportError:
+            _lazy_load_extractor_base = None
+            return extractor
+    if not issubclass(extractor, _lazy_load_extractor_base):
+        return extractor
+    if 'real_class' in _lazy_load_extractor_base.__dict__:
+        return extractor.real_class
+    if '_get_real_class' in _lazy_load_extractor_base.__dict__:
+        return extractor._get_real_class()
+    return extractor
+
+
 def _get_extractor_name(extractor):
     ie_name = extractor.IE_NAME
     if isinstance(ie_name, property):
         return extractor().IE_NAME
     return ie_name
 
 
 def _build_extractors_registry():
     registry = {}
     for extractor in get_all_extractors(include_generic=True):
+        extractor = _get_real_extractor(extractor)
         name_parts = _get_extractor_name(extractor).split(':')
         name_parts.reverse()
         _store_extractor_in_registry(extractor, name_parts, registry)
     return registry
 
 
 def _store_extractor_in_registry(extractor, name_parts, registry):
@@ -162,16 +188,17 @@
         return list(_flatten_registry_gen(stored))
     if not isinstance(stored, dict):
         raise KeyError(name_part)
     return _get_extractors_from_registry(name_parts, stored)
 
 
 def get_extractors_by_name(name):
+    _check_initialized()
     global _extractors_registry
-    if _extractors_registry is None:
+    if _extractors_registry is _NOT_SET:
         _extractors_registry = _build_extractors_registry()
     name_parts = name.split(':')
     name_parts.reverse()
     try:
         return _get_extractors_from_registry(name_parts, _extractors_registry)
     except KeyError:
         raise UnknownBuiltinExtractor(name)
```

### Comparing `dl-plus-0.5.0/src/dl_plus.egg-info/SOURCES.txt` & `dl-plus-0.6.0/src/dl_plus.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE
 README.md
-setup.cfg
-setup.py
+pyproject.toml
 src/dl_plus/__main__.py
 src/dl_plus/backend.py
 src/dl_plus/config.py
 src/dl_plus/const.py
 src/dl_plus/core.py
+src/dl_plus/deprecated.py
 src/dl_plus/exceptions.py
 src/dl_plus/pypi.py
 src/dl_plus/utils.py
 src/dl_plus/ytdl.py
 src/dl_plus.egg-info/PKG-INFO
 src/dl_plus.egg-info/SOURCES.txt
 src/dl_plus.egg-info/dependency_links.txt
@@ -20,16 +20,21 @@
 src/dl_plus/cli/__init__.py
 src/dl_plus/cli/args.py
 src/dl_plus/cli/cli.py
 src/dl_plus/cli/command.py
 src/dl_plus/cli/commands/__init__.py
 src/dl_plus/cli/commands/base.py
 src/dl_plus/cli/commands/backend/__init__.py
+src/dl_plus/cli/commands/backend/base.py
 src/dl_plus/cli/commands/backend/info.py
 src/dl_plus/cli/commands/backend/install.py
+src/dl_plus/cli/commands/backend/update.py
 src/dl_plus/cli/commands/extractor/__init__.py
+src/dl_plus/cli/commands/extractor/base.py
 src/dl_plus/cli/commands/extractor/install.py
+src/dl_plus/cli/commands/extractor/update.py
 src/dl_plus/extractor/__init__.py
 src/dl_plus/extractor/extractor.py
 src/dl_plus/extractor/machinery.py
 src/dl_plus/extractor/peqn.py
-src/dl_plus/extractor/plugin.py
+src/dl_plus/extractor/plugin.py
+tests/testlib.py
```

