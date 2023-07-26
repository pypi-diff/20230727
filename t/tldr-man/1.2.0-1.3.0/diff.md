# Comparing `tmp/tldr_man-1.2.0.tar.gz` & `tmp/tldr_man-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldr_man-1.2.0.tar", max compression
+gzip compressed data, was "tldr_man-1.3.0.tar", max compression
```

## Comparing `tldr_man-1.2.0.tar` & `tldr_man-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2022-07-17 04:30:22.662713 tldr_man-1.2.0/LICENSE
--rw-r--r--   0        0        0     3448 2023-06-16 06:22:32.619707 tldr_man-1.2.0/README.md
--rwxr-xr-x   0        0        0      953 2023-06-16 07:23:05.228692 tldr_man-1.2.0/generate_completions.sh
--rw-r--r--   0        0        0     1502 2023-06-16 07:25:33.049272 tldr_man-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       28 2022-07-29 03:20:39.631247 tldr_man-1.2.0/src/tldr_man/__init__.py
--rw-r--r--   0        0        0       37 2022-07-29 03:10:10.456815 tldr_man-1.2.0/src/tldr_man/__main__.py
--rw-r--r--   0        0        0     3347 2023-06-16 00:38:00.476437 tldr_man-1.2.0/src/tldr_man/languages.py
--rwxr-xr-x   0        0        0     5931 2023-06-16 06:19:30.171795 tldr_man-1.2.0/src/tldr_man/main.py
--rw-r--r--   0        0        0    11806 2023-06-16 07:24:14.611691 tldr_man-1.2.0/src/tldr_man/pages.py
--rw-r--r--   0        0        0     1614 2023-06-16 00:35:28.327932 tldr_man-1.2.0/src/tldr_man/platforms.py
--rw-r--r--   0        0        0     1812 2023-06-16 04:54:01.856938 tldr_man-1.2.0/src/tldr_man/shell_completion.py
--rw-r--r--   0        0        0     1359 2023-06-16 04:55:12.255927 tldr_man-1.2.0/src/tldr_man/util.py
--rw-r--r--   0        0        0     5045 1970-01-01 00:00:00.000000 tldr_man-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-17 04:30:22.662713 tldr_man-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3448 2023-06-16 06:22:32.619707 tldr_man-1.3.0/README.md
+-rwxr-xr-x   0        0        0      953 2023-07-26 23:52:09.973286 tldr_man-1.3.0/generate_completions.sh
+-rw-r--r--   0        0        0     1615 2023-07-26 23:49:13.826183 tldr_man-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       28 2022-07-29 03:20:39.631247 tldr_man-1.3.0/src/tldr_man/__init__.py
+-rw-r--r--   0        0        0       37 2022-07-29 03:10:10.456815 tldr_man-1.3.0/src/tldr_man/__main__.py
+-rw-r--r--   0        0        0     3329 2023-07-23 05:50:52.182165 tldr_man-1.3.0/src/tldr_man/languages.py
+-rwxr-xr-x   0        0        0     6028 2023-07-01 00:18:58.750251 tldr_man-1.3.0/src/tldr_man/main.py
+-rw-r--r--   0        0        0    11909 2023-07-26 23:51:52.449555 tldr_man-1.3.0/src/tldr_man/pages.py
+-rw-r--r--   0        0        0     1614 2023-06-16 00:35:28.327932 tldr_man-1.3.0/src/tldr_man/platforms.py
+-rw-r--r--   0        0        0     1792 2023-07-23 05:50:52.180370 tldr_man-1.3.0/src/tldr_man/shell_completion.py
+-rw-r--r--   0        0        0     1359 2023-06-16 04:55:12.255927 tldr_man-1.3.0/src/tldr_man/util.py
+-rw-r--r--   0        0        0     6291 2023-07-26 23:53:11.514605 tldr_man-1.3.0/tldr-man.1
+-rw-r--r--   0        0        0     5138 1970-01-01 00:00:00.000000 tldr_man-1.3.0/PKG-INFO
```

### Comparing `tldr_man-1.2.0/LICENSE` & `tldr_man-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tldr_man-1.2.0/README.md` & `tldr_man-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tldr_man-1.2.0/generate_completions.sh` & `tldr_man-1.3.0/generate_completions.sh`

 * *Files identical despite different names*

### Comparing `tldr_man-1.2.0/pyproject.toml` & `tldr_man-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 [tool.poetry]
 name = "tldr-man"
-version = "1.2.0"
+version = "1.3.0"
 description = "Command-line TLDR client that displays tldr-pages as manpages"
 license = 'Apache-2.0'
 readme = "README.md"
 authors = ["Olivia Kinnear <contact@superatomic.dev>"]
 homepage = 'https://tldr-man.superatomic.dev/'
 repository = 'https://github.com/superatomic/tldr-man-client'
 documentation = 'https://github.com/superatomic/tldr-man-client#readme'
 keywords = ['tldr', 'tldr-pages', 'man', 'manpage', 'tldr-client']
 classifiers = [
     'Development Status :: 5 - Production/Stable',
+    'Environment :: Console',
     'Intended Audience :: Developers',
     'Intended Audience :: End Users/Desktop',
     'Intended Audience :: System Administrators',
     'Natural Language :: English',
     'Operating System :: MacOS',
     'Operating System :: POSIX',
     'Operating System :: POSIX :: Linux',
     'Operating System :: POSIX :: SunOS/Solaris',
     'Operating System :: Unix',
     'Programming Language :: Unix Shell',
+    'Topic :: Documentation',
+    'Topic :: Software Development :: Documentation',
     'Topic :: Text Processing :: Markup :: Markdown',
     'Topic :: Utilities',
 ]
-include = ["generate_completions.sh"]
+include = ["generate_completions.sh", "tldr-man.1"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/superatomic/tldr-man-client/issues"
 "Say Thanks!" = "https://saythanks.io/to/superatomic"
 
 [tool.poetry.dependencies]
 python = "^3.10.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
-xdg = "^5.1.1"
 requests = "^2.28.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `tldr_man-1.2.0/src/tldr_man/languages.py` & `tldr_man-1.3.0/src/tldr_man/languages.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 """Handle languages for the client."""
 
 from os import getenv
 from collections.abc import Iterator
 
 from click import Context
 
-from tldr_man.pages import TLDR_CACHE_HOME, language_directory_to_code
+from tldr_man.pages import CACHE_DIR, language_directory_to_code
 from tldr_man.util import exit_with
 
 
 def all_languages() -> Iterator[str]:
     """Returns an iterator of all languages directory names."""
     return map(get_language_directory, all_language_codes())
 
 
 def all_language_codes() -> Iterator[str]:
     """Returns an iterator of all language codes, based on all language directories."""
     return (
         language_directory_to_code(pages_dir)
-        for pages_dir in TLDR_CACHE_HOME.iterdir()
+        for pages_dir in CACHE_DIR.iterdir()
         if pages_dir.is_dir()
     )
 
 
 def get_environment_languages() -> Iterator[str]:
     """
     Returns an iterator of the user's preferred languages,
@@ -79,15 +79,15 @@
 def get_language_directory(language_code: str) -> str:
     """Get the name of the directory for a language code."""
     language, region = _language_code_as_parts(language_code)
     if language == 'en':
         return 'pages'
     else:
         full_locale = f'pages.{language}_{region}'
-        if (TLDR_CACHE_HOME / full_locale).is_dir():
+        if (CACHE_DIR / full_locale).is_dir():
             return full_locale
         else:
             return f'pages.{language}'
 
 
 def get_locales(ctx: Context) -> list[str]:
     """Return an ordered list of the languages that the user specifies."""
```

### Comparing `tldr_man-1.2.0/src/tldr_man/main.py` & `tldr_man-1.3.0/src/tldr_man/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
             print(format_exc(), file=stderr)
             exited_with_error = True  # Don't call the `ctx.exit()` in the `finally` block
             ctx.exit(1)
         except SystemExit as err:
             # If `sys.exit()` was called, exit that context with the given status code.
             exited_with_error = True  # Don't call the `ctx.exit()` in the `finally` block
             ctx.exit(err.code)
+        except KeyboardInterrupt:
+            exited_with_error = True
+            ctx.exit(130)
         finally:
             if not exited_with_error:
                 ctx.exit()
 
     return wrapper
 
 def require_tldr_cache(func):
```

### Comparing `tldr_man-1.2.0/src/tldr_man/pages.py` & `tldr_man-1.3.0/src/tldr_man/pages.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,34 +15,33 @@
 """Interact with tldr-pages and the tldr-pages manpage cache."""
 
 import re
 import zipfile
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import suppress
 from pathlib import Path
-from os import remove, makedirs
+from os import remove, makedirs, getenv
 from shutil import rmtree, move
 from subprocess import run, PIPE, DEVNULL
 from typing import Optional
 from collections.abc import Iterable
 
 import requests
 from click import secho, progressbar, style, echo
-from xdg import XDG_CACHE_HOME
 
 from tldr_man.util import mkstemp_path, mkdtemp_path, eprint, exit_with
 
-TLDR_CACHE_DIR_NAME = 'tldr-man'
+CACHE_DIR_NAME = 'tldr-man'
 
-TLDR_ZIP_ARCHIVE_URL = "https://tldr.sh/assets/tldr.zip"
+ZIP_ARCHIVE_URL = "https://tldr.sh/assets/tldr.zip"
 
-TLDR_MANPAGE_SECTION = '1'
+MANPAGE_SECTION = '1'
 
 MANPAGE_HEADER = f"""
-% {{name}}({TLDR_MANPAGE_SECTION}) {{name}}
+% {{name}}({MANPAGE_SECTION}) {{name}}
 %
 % tldr-man-client
 
 # NAME
 {{name}} - {{desc}}
 
 # DESCRIPTION
@@ -74,22 +73,30 @@
 
 CACHE_DOES_NOT_EXIST_MESSAGE = """
 The tldr-pages cache needs to be generated before `tldr` can be used.
     Run `tldr --update` to generate the cache.
 """[1:-1]
 
 
-def tldr_cache_home(location: Path = XDG_CACHE_HOME) -> Path:
-    return location / TLDR_CACHE_DIR_NAME
+def getenv_dir(key: str, default: Optional[Path] = None) -> Optional[Path]:
+    if value := getenv(key):
+        path = Path(value)
+        if path.is_absolute():
+            return path.resolve()
+    return default
 
 
-TLDR_CACHE_HOME: Path = tldr_cache_home()
+def get_cache_dir() -> Path:
+    return getenv_dir('XDG_CACHE_HOME', Path.home() / '.cache') / CACHE_DIR_NAME
 
 
-def download_tldr_zip_archive(location: Path, url: str = TLDR_ZIP_ARCHIVE_URL) -> None:
+CACHE_DIR: Path = get_cache_dir()
+
+
+def download_archive(location: Path, url: str = ZIP_ARCHIVE_URL) -> None:
     """Downloads the current tldr-pages zip archive into a specific location."""
 
     try:
         r = requests.get(url, timeout=10)
     except requests.ConnectionError:
         exit_with(f"Error: Could not make connection to {url}")
     except requests.Timeout:
@@ -109,55 +116,55 @@
 
     secho('Updating tldr-pages cache...', fg='cyan')
 
     created, updated, unchanged = 0, 0, 0
 
     try:
         # Create a temporary file for the tldr-pages zip archive to generate manpages from.
-        tldr_zip_archive = mkstemp_path('tldr.zip')
-        download_tldr_zip_archive(tldr_zip_archive)
+        zip_archive_location = mkstemp_path('tldr.zip')
+        download_archive(zip_archive_location)
 
         # Create the cache directory that will be copied to `~/.cache/tldr-man`.
-        tldr_temp_dir = mkdtemp_path('tldr-man')
+        temp_cache_dir = mkdtemp_path('tldr-man')
 
         # Get the zip file
         try:
-            tldr_zip_path = zipfile.Path(tldr_zip_archive)
+            zip_path = zipfile.Path(zip_archive_location)
         except zipfile.BadZipFile:
-            eprint(f"Error: Got a bad zipfile from {TLDR_ZIP_ARCHIVE_URL}")
+            eprint(f"Error: Got a bad zipfile from {ZIP_ARCHIVE_URL}")
             raise
 
         # Iterate through each language and section in the zip file.
-        for language_dir in tldr_zip_path.iterdir():
+        for language_dir in zip_path.iterdir():
             if not language_dir.is_dir():
                 continue
             for sections_dir in language_dir.iterdir():
                 # Get the full path to the directory where all manpages for this language and section will be extracted.
-                res_dir = tldr_temp_dir / language_dir.name / sections_dir.name / ('man' + TLDR_MANPAGE_SECTION)
+                res_dir = temp_cache_dir / language_dir.name / sections_dir.name / ('man' + MANPAGE_SECTION)
                 res_dir.mkdir(parents=True, exist_ok=True)  # Create the directories if they don't exist.
 
                 # Get the directory where the old versions of the manpages are located,
                 # to compare it with the new versions that are generated:
                 original_dir = (
-                    TLDR_CACHE_HOME / language_dir.name / sections_dir.name / ('man' + TLDR_MANPAGE_SECTION)
-                    if TLDR_CACHE_HOME.exists() else None
+                    CACHE_DIR / language_dir.name / sections_dir.name / ('man' + MANPAGE_SECTION)
+                    if CACHE_DIR.exists() else None
                 )
 
                 # Create the label for the progress bars that are shown.
                 progressbar_label = (style(f"{language_directory_to_code(language_dir):5s}", fg='blue')
                                      + ' / '
                                      + style(f'{sections_dir.name:7s}', fg='blue'))
 
                 # `render_manpage()` takes a significant amount of time to run.
                 # Due to the number of pages that need to be rendered,
                 # this function is invoked simultaneously using threads.
                 def to_manpage(tldr_page: zipfile.Path) -> tuple[str, str]:
                     """Convert a tldr-page into a manpage"""
                     rendered_manpage = render_manpage(tldr_page.read_text())
-                    manpage_filename = tldr_page.name.removesuffix('.md') + '.' + TLDR_MANPAGE_SECTION
+                    manpage_filename = tldr_page.name.removesuffix('.md') + '.' + MANPAGE_SECTION
                     # Return the filename to save the manpage to along with the rendered manpage itself.
                     return manpage_filename, rendered_manpage
 
                 # Get a list of all tldr-pages in the current language and section.
                 # The generator needs to be collected into a list to give the progressbar a length.
                 pages = list(filter(lambda p: p.is_file(), sections_dir.iterdir()))
 
@@ -190,27 +197,27 @@
                         pool.shutdown(wait=False, cancel_futures=True)
                         raise
 
         # Now that the updated cache has been generated, remove the old cache, make sure the parent directory exists,
         # and move the new cache into the correct directory from the temporary directory.
 
         with suppress(FileNotFoundError):
-            rmtree(TLDR_CACHE_HOME)
+            rmtree(CACHE_DIR)
 
-        makedirs(TLDR_CACHE_HOME.parent, exist_ok=True)
-        move(tldr_temp_dir, TLDR_CACHE_HOME)
+        makedirs(CACHE_DIR.parent, exist_ok=True)
+        move(temp_cache_dir, CACHE_DIR)
 
     finally:
         # Clean up any temporary files that aren't gone.
         with suppress(NameError, FileNotFoundError):
             # noinspection PyUnboundLocalVariable
-            remove(tldr_zip_archive)
+            remove(zip_archive_location)
         with suppress(NameError, FileNotFoundError):
             # noinspection PyUnboundLocalVariable
-            rmtree(tldr_temp_dir)
+            rmtree(temp_cache_dir)
 
     # Display the details for the cache update:
     echo(', '.join([
         style(f'{created} Added', fg='green', bold=True),
         style(f'{updated} Updated', fg='blue', bold=True),
         style(f'{unchanged} Unchanged', bold=True),
     ]))
@@ -262,41 +269,41 @@
         return run(['pandoc', '--version'], stdout=DEVNULL).returncode == 0
     except FileNotFoundError:
         return False
 
 
 def verify_tldr_cache_exists():
     """Display a specific message if the tldr manpage cache doesn't exist yet, and then exit."""
-    if not TLDR_CACHE_HOME.exists():
-        exit_with(CACHE_DOES_NOT_EXIST_MESSAGE)
+    if not CACHE_DIR.exists():
+        exit_with(CACHE_DOES_NOT_EXIST_MESSAGE, exitcode=3)
 
 
 def display_page(page: Path) -> None:
     try:
         run(['man', page])
     except FileNotFoundError as err:
         if err.filename == 'man':
             exit_with(MANPAGE_MISSING_MESSAGE, exitcode=127)
         else:
             raise
 
 
 def find_page(page_name: str, /, locales: Iterable[str], page_sections: Iterable[str]) -> Optional[Path]:
     for search_dir in get_dir_search_order(locales, page_sections):
-        page = search_dir / (page_name + '.' + TLDR_MANPAGE_SECTION)
+        page = search_dir / (page_name + '.' + MANPAGE_SECTION)
 
         if page.exists():
             return page
     else:
-        eprint(PAGE_NOT_FOUND_MESSAGE.format(page_name=page_name))
+        exit_with(PAGE_NOT_FOUND_MESSAGE.format(page_name=page_name))
 
 
 def get_dir_search_order(locales: Iterable[str], page_sections: Iterable[str]) -> Iterable[Path]:
     return (
-        TLDR_CACHE_HOME / locale / section / ('man' + TLDR_MANPAGE_SECTION)
+        CACHE_DIR / locale / section / ('man' + MANPAGE_SECTION)
         for locale in locales
         for section in page_sections
     )
 
 
 def language_directory_to_code(language_dir: Path):
     return language_dir.name.removeprefix('pages').lstrip('.') or 'en'
```

### Comparing `tldr_man-1.2.0/src/tldr_man/platforms.py` & `tldr_man-1.3.0/src/tldr_man/platforms.py`

 * *Files identical despite different names*

### Comparing `tldr_man-1.2.0/src/tldr_man/shell_completion.py` & `tldr_man-1.3.0/src/tldr_man/shell_completion.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 # limitations under the License.
 
 """Rich shell completions for the client."""
 
 from click import Context, Parameter
 from click.shell_completion import CompletionItem
 
-from tldr_man.pages import TLDR_CACHE_HOME, get_dir_search_order
+from tldr_man.pages import CACHE_DIR, get_dir_search_order
 from tldr_man.languages import get_locales, all_language_codes
 from tldr_man.platforms import get_page_sections
 
 
 def page_shell_complete(ctx: Context, param: Parameter, incomplete: str) -> list[CompletionItem]:
-    if not TLDR_CACHE_HOME.exists() or param.name is None: # the `param.name is None` check makes the type checker happy
+    if not CACHE_DIR.exists() or param.name is None: # the `param.name is None` check makes the type checker happy
         return []
 
     locales: list[str] = get_locales(ctx)
     page_sections: list[str] = get_page_sections(ctx)
 
-    completed_part = ''.join([part + '-' for part in ctx.params[param.name] or []])
+    completed_part = ''.join(part + '-' for part in ctx.params[param.name] or [])
 
     return [
         CompletionItem(page.stem.removeprefix(completed_part))
         for section in get_dir_search_order(locales, page_sections)
         for page in section.iterdir()
         if page.is_file()
         if page.stem.startswith(completed_part + incomplete)
     ]
 
 
 def language_shell_complete(_ctx: Context, _param: Parameter, _incomplete: str) -> list[CompletionItem]:
-    if not TLDR_CACHE_HOME.exists():
+    if not CACHE_DIR.exists():
         return []
     return [CompletionItem(code) for code in all_language_codes()]
```

### Comparing `tldr_man-1.2.0/src/tldr_man/util.py` & `tldr_man-1.3.0/src/tldr_man/util.py`

 * *Files identical despite different names*

### Comparing `tldr_man-1.2.0/PKG-INFO` & `tldr_man-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: tldr-man
-Version: 1.2.0
+Version: 1.3.0
 Summary: Command-line TLDR client that displays tldr-pages as manpages
 Home-page: https://tldr-man.superatomic.dev/
 License: Apache-2.0
 Keywords: tldr,tldr-pages,man,manpage,tldr-client
 Author: Olivia Kinnear
 Author-email: contact@superatomic.dev
 Requires-Python: >=3.10.4,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX :: SunOS/Solaris
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Unix Shell
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-help-colors (>=0.9.1,<0.10.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: xdg (>=5.1.1,<6.0.0)
 Project-URL: Bug Tracker, https://github.com/superatomic/tldr-man-client/issues
 Project-URL: Documentation, https://github.com/superatomic/tldr-man-client#readme
 Project-URL: Repository, https://github.com/superatomic/tldr-man-client
 Project-URL: Say Thanks!, https://saythanks.io/to/superatomic
 Description-Content-Type: text/markdown
 
 <div>
```

