# Comparing `tmp/pinnwand-1.4.0.tar.gz` & `tmp/pinnwand-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinnwand-1.4.0.tar", max compression
+gzip compressed data, was "pinnwand-1.5.0.tar", last modified: Thu Jul 27 06:56:18 2023, max compression
```

## Comparing `pinnwand-1.4.0.tar` & `pinnwand-1.5.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1048 2022-03-05 12:06:22.490243 pinnwand-1.4.0/LICENSE
--rw-r--r--   0        0        0     3539 2022-07-17 13:31:20.229586 pinnwand-1.4.0/README.md
--rw-r--r--   0        0        0     2220 2022-11-27 10:49:29.631129 pinnwand-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-27 09:16:12.933473 pinnwand-1.4.0/src/pinnwand/__init__.py
--rw-r--r--   0        0        0       42 2022-11-27 09:16:12.933473 pinnwand-1.4.0/src/pinnwand/__main__.py
--rw-r--r--   0        0        0     5193 2022-11-27 10:34:22.782996 pinnwand-1.4.0/src/pinnwand/command.py
--rw-r--r--   0        0        0     1225 2022-11-27 09:16:12.933473 pinnwand-1.4.0/src/pinnwand/configuration.py
--rw-r--r--   0        0        0     4249 2022-11-27 09:16:12.933473 pinnwand-1.4.0/src/pinnwand/database.py
--rw-r--r--   0        0        0     2284 2022-11-27 09:16:12.933473 pinnwand-1.4.0/src/pinnwand/defensive.py
--rw-r--r--   0        0        0      457 2022-11-27 09:16:12.933473 pinnwand-1.4.0/src/pinnwand/error.py
--rw-r--r--   0        0        0       79 2022-11-27 09:16:12.933473 pinnwand-1.4.0/src/pinnwand/handler/__init__.py
--rw-r--r--   0        0        0     2467 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/handler/api_curl.py
--rw-r--r--   0        0        0     7153 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/handler/api_deprecated.py
--rw-r--r--   0        0        0     3849 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/handler/api_v1.py
--rw-r--r--   0        0        0    18559 2022-11-27 10:23:13.649451 pinnwand-1.4.0/src/pinnwand/handler/website.py
--rw-r--r--   0        0        0     2861 2022-11-27 10:23:13.649451 pinnwand-1.4.0/src/pinnwand/http.py
--rw-r--r--   0        0        0      349 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/page/about.rst
--rw-r--r--   0        0        0      112 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/page/expiry.rst
--rw-r--r--   0        0        0      497 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/page/removal.rst
--rw-r--r--   0        0        0      315 2022-11-27 10:23:13.649451 pinnwand-1.4.0/src/pinnwand/path.py
--rw-r--r--   0        0        0     6668 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/static/favicon.png
--rw-r--r--   0        0        0     9887 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/static/logo.png
--rw-r--r--   0        0        0    21479 2022-11-27 09:16:12.934473 pinnwand-1.4.0/src/pinnwand/static/pinnwand.css
--rw-r--r--   0        0        0     8196 2022-11-27 09:16:12.935473 pinnwand-1.4.0/src/pinnwand/static/pinnwand.js
--rw-r--r--   0        0        0     2677 2022-11-27 10:23:13.649451 pinnwand-1.4.0/src/pinnwand/template/create.html
--rw-r--r--   0        0        0      129 2022-11-27 09:16:12.935473 pinnwand-1.4.0/src/pinnwand/template/error.html
--rw-r--r--   0        0        0      709 2022-11-27 09:16:12.935473 pinnwand-1.4.0/src/pinnwand/template/layout.html
--rw-r--r--   0        0        0      592 2022-11-27 09:16:12.935473 pinnwand-1.4.0/src/pinnwand/template/part/lexer-select.html
--rw-r--r--   0        0        0       96 2022-11-27 09:16:12.935473 pinnwand-1.4.0/src/pinnwand/template/restructuredtextpage.html
--rw-r--r--   0        0        0     2220 2022-11-27 09:16:12.935473 pinnwand-1.4.0/src/pinnwand/template/show.html
--rw-r--r--   0        0        0     6030 2022-11-27 09:16:12.935473 pinnwand-1.4.0/src/pinnwand/utility.py
--rw-r--r--   0        0        0     4857 1970-01-01 00:00:00.000000 pinnwand-1.4.0/setup.py
--rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 pinnwand-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-07-14 06:50:37.970916 pinnwand-1.5.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1048 2023-07-14 06:50:37.971916 pinnwand-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3327 2023-07-14 06:50:37.971916 pinnwand-1.5.0/README.md
+-rw-r--r--   0        0        0     2164 2023-07-27 06:54:28.541791 pinnwand-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 06:50:37.978916 pinnwand-1.5.0/src/pinnwand/__init__.py
+-rw-r--r--   0        0        0       42 2023-07-14 06:50:37.978916 pinnwand-1.5.0/src/pinnwand/__main__.py
+-rw-r--r--   0        0        0     5352 2023-07-27 06:53:34.497836 pinnwand-1.5.0/src/pinnwand/command.py
+-rw-r--r--   0        0        0     1257 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/configuration.py
+-rw-r--r--   0        0        0     4249 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/database.py
+-rw-r--r--   0        0        0     2284 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/defensive.py
+-rw-r--r--   0        0        0      457 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/error.py
+-rw-r--r--   0        0        0       79 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/handler/__init__.py
+-rw-r--r--   0        0        0     2467 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/handler/api_curl.py
+-rw-r--r--   0        0        0     7153 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/handler/api_deprecated.py
+-rw-r--r--   0        0        0     3849 2023-07-14 06:50:37.979916 pinnwand-1.5.0/src/pinnwand/handler/api_v1.py
+-rw-r--r--   0        0        0    18540 2023-07-14 06:50:37.980916 pinnwand-1.5.0/src/pinnwand/handler/website.py
+-rw-r--r--   0        0        0     2901 2023-07-27 06:53:34.498836 pinnwand-1.5.0/src/pinnwand/http.py
+-rw-r--r--   0        0        0      348 2023-07-14 06:50:37.980916 pinnwand-1.5.0/src/pinnwand/page/about.rst
+-rw-r--r--   0        0        0      112 2023-07-14 06:50:37.980916 pinnwand-1.5.0/src/pinnwand/page/expiry.rst
+-rw-r--r--   0        0        0      497 2023-07-14 06:50:37.980916 pinnwand-1.5.0/src/pinnwand/page/removal.rst
+-rw-r--r--   0        0        0      315 2023-07-14 06:50:37.980916 pinnwand-1.5.0/src/pinnwand/path.py
+-rw-r--r--   0        0        0     6668 2023-07-14 06:50:37.980916 pinnwand-1.5.0/src/pinnwand/static/favicon.png
+-rw-r--r--   0        0        0     9887 2023-07-14 06:50:37.980916 pinnwand-1.5.0/src/pinnwand/static/logo.png
+-rw-r--r--   0        0        0    21937 2023-07-27 06:53:34.499836 pinnwand-1.5.0/src/pinnwand/static/pinnwand.css
+-rw-r--r--   0        0        0    13128 2023-07-27 06:53:34.500836 pinnwand-1.5.0/src/pinnwand/static/pinnwand.js
+-rw-r--r--   0        0        0     3010 2023-07-27 06:53:34.501836 pinnwand-1.5.0/src/pinnwand/template/create.html
+-rw-r--r--   0        0        0      129 2023-07-14 06:50:37.981916 pinnwand-1.5.0/src/pinnwand/template/error.html
+-rw-r--r--   0        0        0      709 2023-07-14 06:50:37.981916 pinnwand-1.5.0/src/pinnwand/template/layout.html
+-rw-r--r--   0        0        0      592 2023-07-14 06:50:37.981916 pinnwand-1.5.0/src/pinnwand/template/part/lexer-select.html
+-rw-r--r--   0        0        0       96 2023-07-14 06:50:37.981916 pinnwand-1.5.0/src/pinnwand/template/restructuredtextpage.html
+-rw-r--r--   0        0        0     2220 2023-07-14 06:50:37.981916 pinnwand-1.5.0/src/pinnwand/template/show.html
+-rw-r--r--   0        0        0     6030 2023-07-14 06:50:37.981916 pinnwand-1.5.0/src/pinnwand/utility.py
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 pinnwand-1.5.0/PKG-INFO
```

### Comparing `pinnwand-1.4.0/LICENSE` & `pinnwand-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/README.md` & `pinnwand-1.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ![pinnwand logo, a rabbit](https://pinnwand.readthedocs.io/en/latest/_static/logo-doc.png)
 
 # pinnwand
 
-[![](https://travis-ci.org/supakeen/pinnwand.svg?branch=master)](https://travis-ci.org/supakeen/pinnwand) [![](https://readthedocs.org/projects/pinnwand/badge/?version=latest)](https://pinnwand.readthedocs.io/en/latest/) [![](https://pinnwand.readthedocs.io/en/latest/_static/license.svg)](https://github.com/supakeen/pinnwand/blob/master/LICENSE) [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![](https://img.shields.io/pypi/v/pinnwand)](https://pypi.org/project/pinnwand) [![](https://codecov.io/gh/supakeen/pinnwand/branch/master/graph/badge.svg)](https://codecov.io/gh/supakeen/pinnwand) [![](https://quay.io/repository/supakeen/pinnwand/status)](https://quay.io/repository/supakeen/pinnwand)
+[![](https://readthedocs.org/projects/pinnwand/badge/?version=latest)](https://pinnwand.readthedocs.io/en/latest/) [![](https://pinnwand.readthedocs.io/en/latest/_static/license.svg)](https://github.com/supakeen/pinnwand/blob/master/LICENSE) [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![](https://img.shields.io/pypi/v/pinnwand)](https://pypi.org/project/pinnwand) [![](https://codecov.io/gh/supakeen/pinnwand/branch/master/graph/badge.svg)](https://codecov.io/gh/supakeen/pinnwand)
 
 ## About
 
 `pinnwand` is Python pastebin software that tried to keep it simple but got
 a little more complex.
 
 Prerequisites
 =============
-* Python >= 3.7
+* Python >= 3.8
 * Tornado
 * sqlalchemy
 * click
 * docutils
 * tomli
 * pygments-better-html
 * a database driver
@@ -25,15 +25,15 @@
 
 Web
 ---
 Enter text, click "Paste", easy enough.
 
 steck
 -----
-[steck](https://supakeen.com/project/steck) is a command line client to pinnwand instances:
+[steck](https://github.com/supakeen/steck) is a command line client to pinnwand instances:
 
 ```
 € pip install --user steck
 ...
 € steck paste *
 You are about to paste the following 7 files. Do you want to continue?
 - LICENSE
```

### Comparing `pinnwand-1.4.0/src/pinnwand/command.py` & `pinnwand-1.5.0/src/pinnwand/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,41 +53,47 @@
     for key, value in os.environ.items():
         if key.startswith("PINNWAND_"):
             key = key.removeprefix("PINNWAND_")
             key = key.lower()
 
             try:
                 value = ast.literal_eval(value)
-            except ValueError:
+            except (ValueError, SyntaxError):
                 # When `ast.literal_eval` can't parse the value into another
                 # type we take it at string value
                 pass
 
             setattr(configuration, key, value)
 
     from pinnwand import database
 
     database.Base.metadata.create_all(database._engine)
 
 
 @main.command()
 @click.option("--port", default=8000, help="Port to listen to.")
-def http(port: int) -> None:
+@click.option(
+    "--debug",
+    is_flag=True,
+    default=False,
+    help="To start tornado server in debug mode or not",
+)
+def http(port: int, debug: bool) -> None:
     """Run pinnwand's HTTP server."""
     from pinnwand import utility
     from pinnwand.http import make_application
 
     # Reap expired pastes on startup (we might've been shut down for a while)
     utility.reap()
 
     # Schedule reaping every 1800 seconds
     reap_task = tornado.ioloop.PeriodicCallback(utility.async_reap, 1_800_000)
     reap_task.start()
 
-    application = make_application()
+    application = make_application(debug)
     application.listen(port, xheaders=True)
 
     tornado.ioloop.IOLoop.current().start()
 
 
 @main.command()
 @click.option("--lexer", default="text", help="Lexer to use.")
```

### Comparing `pinnwand-1.4.0/src/pinnwand/configuration.py` & `pinnwand-1.5.0/src/pinnwand/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 database_uri = "sqlite:///:memory:"
 paste_size = 256 * 1024  # in bytes
 footer = 'View <a href="//github.com/supakeen/pinnwand" target="_BLANK">source code</a>, the <a href="/removal">removal</a> or <a href="/expiry">expiry</a> stories, or read the <a href="/about">about</a> page.'
 paste_help = "<p>Welcome to pinnwand, this site is a pastebin. It allows you to share code with others. If you write code in the text area below and press the paste button you will be given a link you can share with others so they can view your code as well.</p><p>People with the link can view your pasted code, only you can remove your paste and it expires automatically. Note that anyone could guess the URI to your paste so don't rely on it being private.</p>"
 page_path = None
 page_list = ["about", "removal", "expiry"]
+default_selected_lexer = "text"
 preferred_lexers = []  # type: ignore
 logo_path = None
 report_email = None
 expiries = {"1day": 86400, "1week": 604800}
 ratelimit = {
     "read": {
         "capacity": 100,
```

#### html2text {}

```diff
@@ -4,12 +4,13 @@
 Welcome to pinnwand, this site is a pastebin. It allows you to share code with
 others. If you write code in the text area below and press the paste button you
 will be given a link you can share with others so they can view your code as
 well.
 People with the link can view your pasted code, only you can remove your paste
 and it expires automatically. Note that anyone could guess the URI to your
 paste so don't rely on it being private.
-" page_path = None page_list = ["about", "removal", "expiry"] preferred_lexers
-= [] # type: ignore logo_path = None report_email = None expiries = {"1day":
-86400, "1week": 604800} ratelimit = { "read": { "capacity": 100, "consume": 1,
-"refill": 2, }, "create": { "capacity": 2, "consume": 2, "refill": 1, },
-"delete": { "capacity": 2, "consume": 2, "refill": 1, }, } spamscore = 50
+" page_path = None page_list = ["about", "removal", "expiry"]
+default_selected_lexer = "text" preferred_lexers = [] # type: ignore logo_path
+= None report_email = None expiries = {"1day": 86400, "1week": 604800}
+ratelimit = { "read": { "capacity": 100, "consume": 1, "refill": 2, },
+"create": { "capacity": 2, "consume": 2, "refill": 1, }, "delete":
+{ "capacity": 2, "consume": 2, "refill": 1, }, } spamscore = 50
```

### Comparing `pinnwand-1.4.0/src/pinnwand/database.py` & `pinnwand-1.5.0/src/pinnwand/database.py`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/defensive.py` & `pinnwand-1.5.0/src/pinnwand/defensive.py`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/handler/api_curl.py` & `pinnwand-1.5.0/src/pinnwand/handler/api_curl.py`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/handler/api_deprecated.py` & `pinnwand-1.5.0/src/pinnwand/handler/api_deprecated.py`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/handler/api_v1.py` & `pinnwand-1.5.0/src/pinnwand/handler/api_v1.py`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/handler/website.py` & `pinnwand-1.5.0/src/pinnwand/handler/website.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,16 @@
             raise error.RatelimitError()
 
         lexers_available = utility.list_languages()
         lexers_selected = [
             lexer for lexer in lexers.split("+") if lexer.strip()
         ]
 
-        # Our default lexer is just that, text
         if not lexers_selected:
-            lexers_selected = ["text"]
+            lexers_selected = [configuration.default_selected_lexer]
 
         # Make sure all lexers are available
         if not all(lexer in lexers_available for lexer in lexers_selected):
             log.debug("CreatePaste.get: non-existent lexer requested")
             raise tornado.web.HTTPError(404)
 
         await self.render(
@@ -208,15 +207,15 @@
         with database.session() as session, utility.SlugContext(
             auto_scale
         ) as slug_context:
             paste = database.Paste(
                 next(slug_context), configuration.expiries[expiry], "web"
             )
 
-            for (lexer, raw, filename) in zip(lexers, raws, filenames):
+            for lexer, raw, filename in zip(lexers, raws, filenames):
                 paste.files.append(
                     database.File(
                         next(slug_context),
                         raw,
                         lexer,
                         filename if filename else None,
                     )
```

### Comparing `pinnwand-1.4.0/src/pinnwand/http.py` & `pinnwand-1.5.0/src/pinnwand/http.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tornado.web
 
 from pinnwand import configuration, handler, path
 
 log = logging.getLogger(__name__)
 
 
-def make_application() -> tornado.web.Application:
+def make_application(debug: bool = False) -> tornado.web.Application:
     pages: List[Any] = [
         (r"/", handler.website.Create),
         (r"/\+(.*)", handler.website.Create),
         (r"/create", handler.website.CreateAction),
         (r"/show/([A-Z2-7]+)(?:#.+)?", handler.website.RedirectShow),
         (r"/repaste/([A-Z2-7]+)(?:#.+)?", handler.website.Repaste),
         (r"/raw/([A-Z2-7]+)(?:#.+)?", handler.website.FileRaw),
@@ -81,12 +81,13 @@
         pages,
         template_path=path.template,
         default_handler_class=handler.website.Base,
         xsrf_cookies=True,
         cookie_secret=secrets.token_hex(),
         static_path=path.static,
         xheaders=True,
+        debug=debug,
     )
 
     app.configuration = configuration  # type: ignore
 
     return app
```

### Comparing `pinnwand-1.4.0/src/pinnwand/static/favicon.png` & `pinnwand-1.5.0/src/pinnwand/static/favicon.png`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/static/logo.png` & `pinnwand-1.5.0/src/pinnwand/static/logo.png`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/static/pinnwand.css` & `pinnwand-1.5.0/src/pinnwand/static/pinnwand.css`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 a {
   color: var(--color3); }
 
 a:hover {
   background-color: var(--color3);
   color: var(--color1); }
 
+a.file-upload {
+  text-decoration: underline var(--color3);
+}
+
 button.btn-link {
   background: none;
   border: none;
   padding: 0;
   color: var(--color3);
   font-family: sans-serif;
   font-size: 13px;
@@ -69,14 +73,31 @@
   padding: .5rem;
   margin-bottom: .5rem;
   opacity: .5; }
   section.paste-help:hover {
     opacity: .9;
     transition: opacity .1s; }
 
+section.file-drop {
+  background-color: var(--color1);
+  display: flex;
+  justify-content: center;
+  align-items: center;
+  height: 5em;
+  font-weight: bold;
+  padding: .5rem;
+  margin-bottom: .5rem;
+  opacity: .5; }
+section.file-drop:hover {
+  opacity: .9;
+  transition: opacity .1s; }
+section.file-drop.dragover {
+  outline: 1px solid var(--color3);
+}
+
 section.file-part {
   width: 100%;
   margin-bottom: .5rem; }
   section.file-part textarea {
     background-color: var(--color1);
     width: 100%;
     resize: vertical;
@@ -114,15 +135,17 @@
 section.file-part div.file-meta {
   background-color: var(--color1);
   padding: .5rem;
   margin-bottom: .0625rem; }
 
 section.paste-submit {
   background-color: var(--color1);
-  padding: .5rem; }
+  padding: .5rem;
+  margin-bottom: .5rem;
+}
 
 div.file-meta button,
 section.paste-submit button {
   box-sizing: border-box;
   border: 0.0625rem solid var(--color3);
   padding: .4rem 1.4rem;
   margin: 0 .2rem;
@@ -167,15 +190,15 @@
 header nav ul {
   margin: 0;
   padding: 0; }
   header nav ul li {
     display: inline-block;
     vertical-align: middle; }
     header nav ul li img.logo {
-      width: 3rem; }
+      height: 5rem; }
 
 div.file-show {
   margin-top: .5rem; }
 
 div.file-show div.code {
   background-color: var(--color1);
   padding: .5rem; }
@@ -196,15 +219,16 @@
   background: var(--color0);
   padding: 0 .25rem;
   opacity: .5;
   cursor: pointer; }
 
 div.code {
   font-size: 1.2rem;
-  overflow-x: auto; }
+  overflow-x: auto;
+  tab-size: 4; }
   div.code:hover td.linenos {
     opacity: .75; }
 
 td.code {
   padding-left: .5rem;
   width: 100%; }
```

### Comparing `pinnwand-1.4.0/src/pinnwand/template/create.html` & `pinnwand-1.5.0/src/pinnwand/template/create.html`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,18 @@
             <select name="expiry">
                 {% for expiry in expiries %}
                 <option value="{{ expiry }}">Expiry ({{ expiry }})</option>
                 {% end %}
             </select>
             <input type="checkbox" name="long"> Use a longer URI
         </section>
+        <section class="file-drop" id="file-drop">
+            Drop files&nbsp;<a id="file-upload" class="file-upload" onclick="document.getElementById('file-input').click();">or click here</a>&nbsp;to upload files
+            <input id="file-input" type="file" name="file-input" style="display: none;" multiple/>
+        </section>
     </main>
 </form>
 <section class="file-template">
     <div class="file-meta">
         {% module Template("part/lexer-select.html", selected=lexers[0], lexers=lexers_available) %}
         <input name="filename" placeholder="Filename (optional)">
         <button class="remove">Remove this file</button>
```

### Comparing `pinnwand-1.4.0/src/pinnwand/template/layout.html` & `pinnwand-1.5.0/src/pinnwand/template/layout.html`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/template/part/lexer-select.html` & `pinnwand-1.5.0/src/pinnwand/template/part/lexer-select.html`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/template/show.html` & `pinnwand-1.5.0/src/pinnwand/template/show.html`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/src/pinnwand/utility.py` & `pinnwand-1.5.0/src/pinnwand/utility.py`

 * *Files identical despite different names*

### Comparing `pinnwand-1.4.0/setup.py` & `pinnwand-1.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,128 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pinnwand
+Version: 1.5.0
+Summary: Straightforward pastebin software.
+License: MIT
+Author-email: Simon de Vlieger <cmdr@supakeen.com>
+Requires-Python: >=3.8
+Provides-Extra: dev
+Project-URL: Bug Tracker, https://github.com/supakeen/pinnwand/issues
+Project-URL: Homepage, https://github.com/supakeen/pinnwand
+Project-URL: Repository, https://github.com/supakeen/pinnwand
+Description-Content-Type: text/markdown
+
+![pinnwand logo, a rabbit](https://pinnwand.readthedocs.io/en/latest/_static/logo-doc.png)
+
+# pinnwand
+
+[![](https://readthedocs.org/projects/pinnwand/badge/?version=latest)](https://pinnwand.readthedocs.io/en/latest/) [![](https://pinnwand.readthedocs.io/en/latest/_static/license.svg)](https://github.com/supakeen/pinnwand/blob/master/LICENSE) [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![](https://img.shields.io/pypi/v/pinnwand)](https://pypi.org/project/pinnwand) [![](https://codecov.io/gh/supakeen/pinnwand/branch/master/graph/badge.svg)](https://codecov.io/gh/supakeen/pinnwand)
+
+## About
+
+`pinnwand` is Python pastebin software that tried to keep it simple but got
+a little more complex.
+
+Prerequisites
+=============
+* Python >= 3.8
+* Tornado
+* sqlalchemy
+* click
+* docutils
+* tomli
+* pygments-better-html
+* a database driver
+
+Usage
+=====
+
+Web
+---
+Enter text, click "Paste", easy enough.
+
+steck
+-----
+[steck](https://github.com/supakeen/steck) is a command line client to pinnwand instances:
+
+```
+€ pip install --user steck
+...
+€ steck paste *
+You are about to paste the following 7 files. Do you want to continue?
+- LICENSE
+- mypy.ini
+- poetry.lock
+- pyproject.toml
+- README.rst
+- requirements.txt
+- steck.py
+
+Continue? [y/N] y
+
+Completed paste.
+View link:    https://localhost:8000/W5
+Removal link: https://localhost:8000/remove/TS2AFFIEHEWUBUV5HLKNAUZFEI
+```
+
+curl
+----
+`pinnwand` has a direct endpoint for `curl` users:
+
+```
+€ echo "foo" | curl -X POST http://localhost:8000/curl -F 'raw=<-'
+Paste URL:   http://localhost:8000/OE
+Raw URL:     http://localhost:8000/raw/GU
+Removal URL: http://localhost:8000/remove/GQBHGJYKRWIS34D6FNU6CJ3B5M
+€ curl http://localhost:8000/raw/GU
+foo%
+```
+
+This will preselect the `lexer` and `expiry` arguments to be `text` and
+`1day` respectively. You can provide those to change them.
+
+API
+---
+`pinnwand` provides a straight forward JSON API, here's an example using the
+common requests library:
+
+```
+>>> requests.post(
+...     "http://localhost:8000/api/v1/paste",
+...     json={
+...             "expiry": "1day",
+...             "files": [
+...                     {"name": "spam", "lexer": "python", "content": "eggs"},
+...             ],
+...     }
+... ).json()
+{'link': 'http://localhost:8000/74', 'removal': 'http://localhost:8000/remove/KYXQLPZQEWV2L4YZM7NYGTR7TY'}
+```
+
+More information about this API is available in the [documentation](https://pinnwand.readthedocs.io/en/latest/).
+
+
+More ways to use pinnwand
+-------------------------
+Various deprecated ways of posting are still supported, don't implement these
+for any new software but if you are maintaining old software and want to know
+how they used to work you can read our documentation_.
+
+If you do use a deprecated endpoint to post a warning will be shown below any
+pastes that are created this way.
+
+Reporting bugs
+==============
+Bugs are reported best at `pinnwand`'s [project page](https://github.com/supakeen/pinnwand) on github. If you just
+want to hang out and chat about `pinnwand` then I'm available in the
+`#pinnwand` channel on Freenode IRC.
+
+License
+=======
+`pinnwand` is distributed under the MIT license. See `LICENSE`
+for details.
+
+History
+=======
+This pastebin has quite a long history which isn't reflected entirely in its
+repository.
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['pinnwand', 'pinnwand.handler']
-
-package_data = \
-{'': ['*'], 'pinnwand': ['page/*', 'static/*', 'template/*', 'template/part/*']}
-
-install_requires = \
-['click>=8.1,<9.0',
- 'docutils>=0.19,<0.20',
- 'pygments-better-html>=0.1.4,<0.2.0',
- 'pygments>=2.13,<3.0',
- 'sqlalchemy>=1.4,<2.0',
- 'token-bucket>=0.3.0,<0.4.0',
- 'tornado>=6.2,<7.0']
-
-extras_require = \
-{':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['pinnwand = pinnwand.__main__:main']}
-
-setup_kwargs = {
-    'name': 'pinnwand',
-    'version': '1.4.0',
-    'description': 'Straightforward pastebin software.',
-    'long_description': '![pinnwand logo, a rabbit](https://pinnwand.readthedocs.io/en/latest/_static/logo-doc.png)\n\n# pinnwand\n\n[![](https://travis-ci.org/supakeen/pinnwand.svg?branch=master)](https://travis-ci.org/supakeen/pinnwand) [![](https://readthedocs.org/projects/pinnwand/badge/?version=latest)](https://pinnwand.readthedocs.io/en/latest/) [![](https://pinnwand.readthedocs.io/en/latest/_static/license.svg)](https://github.com/supakeen/pinnwand/blob/master/LICENSE) [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black) [![](https://img.shields.io/pypi/v/pinnwand)](https://pypi.org/project/pinnwand) [![](https://codecov.io/gh/supakeen/pinnwand/branch/master/graph/badge.svg)](https://codecov.io/gh/supakeen/pinnwand) [![](https://quay.io/repository/supakeen/pinnwand/status)](https://quay.io/repository/supakeen/pinnwand)\n\n## About\n\n`pinnwand` is Python pastebin software that tried to keep it simple but got\na little more complex.\n\nPrerequisites\n=============\n* Python >= 3.7\n* Tornado\n* sqlalchemy\n* click\n* docutils\n* tomli\n* pygments-better-html\n* a database driver\n\nUsage\n=====\n\nWeb\n---\nEnter text, click "Paste", easy enough.\n\nsteck\n-----\n[steck](https://supakeen.com/project/steck) is a command line client to pinnwand instances:\n\n```\n€ pip install --user steck\n...\n€ steck paste *\nYou are about to paste the following 7 files. Do you want to continue?\n- LICENSE\n- mypy.ini\n- poetry.lock\n- pyproject.toml\n- README.rst\n- requirements.txt\n- steck.py\n\nContinue? [y/N] y\n\nCompleted paste.\nView link:    https://localhost:8000/W5\nRemoval link: https://localhost:8000/remove/TS2AFFIEHEWUBUV5HLKNAUZFEI\n```\n\ncurl\n----\n`pinnwand` has a direct endpoint for `curl` users:\n\n```\n€ echo "foo" | curl -X POST http://localhost:8000/curl -F \'raw=<-\'\nPaste URL:   http://localhost:8000/OE\nRaw URL:     http://localhost:8000/raw/GU\nRemoval URL: http://localhost:8000/remove/GQBHGJYKRWIS34D6FNU6CJ3B5M\n€ curl http://localhost:8000/raw/GU\nfoo%\n```\n\nThis will preselect the `lexer` and `expiry` arguments to be `text` and\n`1day` respectively. You can provide those to change them.\n\nAPI\n---\n`pinnwand` provides a straight forward JSON API, here\'s an example using the\ncommon requests library:\n\n```\n>>> requests.post(\n...     "http://localhost:8000/api/v1/paste",\n...     json={\n...             "expiry": "1day",\n...             "files": [\n...                     {"name": "spam", "lexer": "python", "content": "eggs"},\n...             ],\n...     }\n... ).json()\n{\'link\': \'http://localhost:8000/74\', \'removal\': \'http://localhost:8000/remove/KYXQLPZQEWV2L4YZM7NYGTR7TY\'}\n```\n\nMore information about this API is available in the [documentation](https://pinnwand.readthedocs.io/en/latest/).\n\n\nMore ways to use pinnwand\n-------------------------\nVarious deprecated ways of posting are still supported, don\'t implement these\nfor any new software but if you are maintaining old software and want to know\nhow they used to work you can read our documentation_.\n\nIf you do use a deprecated endpoint to post a warning will be shown below any\npastes that are created this way.\n\nReporting bugs\n==============\nBugs are reported best at `pinnwand`\'s [project page](https://github.com/supakeen/pinnwand) on github. If you just\nwant to hang out and chat about `pinnwand` then I\'m available in the\n`#pinnwand` channel on Freenode IRC.\n\nLicense\n=======\n`pinnwand` is distributed under the MIT license. See `LICENSE`\nfor details.\n\nHistory\n=======\nThis pastebin has quite a long history which isn\'t reflected entirely in its\nrepository.\n',
-    'author': 'Simon de Vlieger',
-    'author_email': 'cmdr@supakeen.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/supakeen/pinnwand',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4',
-}
-
-
-setup(**setup_kwargs)
```

