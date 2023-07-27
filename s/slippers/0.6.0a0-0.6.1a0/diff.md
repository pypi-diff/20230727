# Comparing `tmp/slippers-0.6.0a0.tar.gz` & `tmp/slippers-0.6.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slippers-0.6.0a0.tar", max compression
+gzip compressed data, was "slippers-0.6.1a0.tar", max compression
```

## Comparing `slippers-0.6.0a0.tar` & `slippers-0.6.1a0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1072 2022-12-29 13:18:15.967791 slippers-0.6.0a0/LICENSE
--rw-r--r--   0        0        0     2059 2022-12-29 13:18:15.967791 slippers-0.6.0a0/README.md
--rw-r--r--   0        0        0     1208 2022-12-29 13:18:15.979791 slippers-0.6.0a0/pyproject.toml
--rw-r--r--   0        0        0       52 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/__init__.py
--rw-r--r--   0        0        0     1861 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/apps.py
--rw-r--r--   0        0        0      807 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/conf.py
--rw-r--r--   0        0        0     6215 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/props.py
--rw-r--r--   0        0        0     7367 2022-12-29 13:19:16.988254 slippers-0.6.0a0/slippers/static/slippers/main.css
--rw-r--r--   0        0        0   145904 2022-12-29 13:19:16.988254 slippers-0.6.0a0/slippers/static/slippers/main.js
--rw-r--r--   0        0        0     5801 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/template.py
--rw-r--r--   0        0        0      179 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/templates/slippers/errors.html
--rw-r--r--   0        0        0        0 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/templatetags/__init__.py
--rw-r--r--   0        0        0     9037 2022-12-29 13:18:15.979791 slippers-0.6.0a0/slippers/templatetags/slippers.py
--rw-r--r--   0        0        0     3175 1970-01-01 00:00:00.000000 slippers-0.6.0a0/setup.py
--rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 slippers-0.6.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-27 15:26:20.255319 slippers-0.6.1a0/LICENSE
+-rw-r--r--   0        0        0     2059 2023-07-27 15:26:20.255319 slippers-0.6.1a0/README.md
+-rw-r--r--   0        0        0     1213 2023-07-27 15:26:20.267319 slippers-0.6.1a0/pyproject.toml
+-rw-r--r--   0        0        0       52 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/__init__.py
+-rw-r--r--   0        0        0     1861 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/apps.py
+-rw-r--r--   0        0        0      783 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/conf.py
+-rw-r--r--   0        0        0     4833 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/props.py
+-rw-r--r--   0        0        0     7361 2023-07-27 15:27:36.693054 slippers-0.6.1a0/slippers/static/slippers/main.css
+-rw-r--r--   0        0        0   146850 2023-07-27 15:27:36.693054 slippers-0.6.1a0/slippers/static/slippers/main.js
+-rw-r--r--   0        0        0     5801 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/template.py
+-rw-r--r--   0        0        0      327 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templates/slippers/overlay.html
+-rw-r--r--   0        0        0        0 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templatetags/__init__.py
+-rw-r--r--   0        0        0     8957 2023-07-27 15:26:20.267319 slippers-0.6.1a0/slippers/templatetags/slippers.py
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 slippers-0.6.1a0/PKG-INFO
```

### Comparing `slippers-0.6.0a0/LICENSE` & `slippers-0.6.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `slippers-0.6.0a0/README.md` & `slippers-0.6.1a0/README.md`

 * *Files identical despite different names*

### Comparing `slippers-0.6.0a0/pyproject.toml` & `slippers-0.6.1a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slippers"
-version = "0.6.0a0"
+version = "0.6.1a0"
 description = "Build reusable components in Django without writing a single line of Python."
 authors = ["Mitchel Cabuloy <mixxorz@gmail.com>"]
 keywords = ["django", "components"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/mixxorz/slippers"
 repository = "https://github.com/mixxorz/slippers"
@@ -14,28 +14,28 @@
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Framework :: Django",
     "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
 ]
 include = [
     "LICENSE",
     "slippers/static/slippers/main.js",
     "slippers/static/slippers/main.css",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
-Django = ">=3.2, <4.2"
-PyYAML = ">=5.4.0, <7.0.0"
+python = ">=3.7.0"
+Django = ">=3.2"
+PyYAML = ">=5.4.0"
 typeguard = "^2.13.3"
-rich = "^12.6.0"
-typing-extensions = "^4.4.0"
+typing-extensions = ">=4.4.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 isort = "^5.9.2"
 flake8 = "^3.9.2"
 ipdb = "^0.13.9"
 tox = "^3.23.1"
```

### Comparing `slippers-0.6.0a0/slippers/apps.py` & `slippers-0.6.1a0/slippers/apps.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.0a0/slippers/conf.py` & `slippers-0.6.1a0/slippers/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     def SLIPPERS_RUNTIME_TYPE_CHECKING(self) -> bool:
         """Enable runtime type checking of props"""
         return getattr(django_settings, "SLIPPERS_RUNTIME_TYPE_CHECKING", django_settings.DEBUG)  # type: ignore
 
     @property
     def SLIPPERS_TYPE_CHECKING_OUTPUT(
         self,
-    ) -> List[Literal["shell", "browser_console", "ui"]]:
+    ) -> List[Literal["console", "overlay"]]:
         """Where to output type checking errors"""
         return getattr(
             django_settings,
             "SLIPPERS_TYPE_CHECKING_OUTPUT",
-            ["shell", "browser_console", "ui"],
+            ["console", "overlay"],
         )
 
 
 settings = Settings()
```

### Comparing `slippers-0.6.0a0/slippers/props.py` & `slippers-0.6.1a0/slippers/props.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,16 @@
     from typing import Literal, get_args, get_origin
 else:
     from typing_extensions import Literal, get_args, get_origin
 
 from django.utils.html import SafeString
 from django.utils.safestring import mark_safe
 
-from rich.console import Console
-from rich.panel import Panel
 from typeguard import check_type, get_type_name
 
-console = Console()
-
 
 class Props(Mapping):
     """Props object used in component code"""
 
     def __init__(
         self,
         attributes: Dict[str, Any],
@@ -136,70 +132,22 @@
 error_message_templates = {
     "invalid": "Invalid prop '{name}' set on '{component}'. Expected '{expected}', got '{actual}'.",
     "missing": "Required prop '{name}' of type '{expected}' not set on '{component}'.",
     "extra": "Extra prop '{name}' of type '{actual}' set on '{component}'.",
 }
 
 
-def print_errors(
-    *, errors: List[PropError], tag_name: str, template_name: str, lineno: int
-):
-    """Print errors to the console"""
-
-    error_messages = [
-        error_message_templates[error.error].format(
-            name=error.name,
-            component=tag_name,
-            expected=get_type_name(error.expected),
-            actual=get_type_name(error.actual),
-        )
-        for error in errors
-    ]
-
-    console.print(
-        Panel(
-            "\n".join(error_messages),
-            style="yellow",
-            expand=False,
-            title=(
-                r"\[slippers] "
-                f"Failed prop types: {tag_name} at "
-                f"{template_name}:{lineno}"
-            ),
-            title_align="left",
-        )
-    )
-
-
 def render_error_html(
     *, errors: List[PropError], tag_name: str, template_name: str, lineno: int
 ) -> SafeString:
     """Output errors to the browser console"""
 
     # Remove # from tag name
     tag_name = tag_name.lstrip("#")
 
-    error_messages = [
-        error_message_templates[error.error].format(
-            name=error.name,
-            component=tag_name,
-            expected=get_type_name(error.expected),
-            actual=get_type_name(error.actual),
-        )
-        for error in errors
-    ]
-
-    error_message = (
-        f"[slippers] Failed prop types: {tag_name} at {template_name}:{lineno}\\n  "
-    )
-
-    error_message += "\\n  ".join(error_messages)
-
-    warnings_html = f'<script>console.error("{error_message}")</script>'
-
     # Output the error as JSON
     data = json.dumps(
         {
             "tag_name": tag_name,
             "template_name": template_name,
             "lineno": lineno,
             "errors": [
@@ -217,8 +165,8 @@
     data_html = f"""
         <script>
             window.slippersPropErrors = window.slippersPropErrors || [];
             window.slippersPropErrors.push({data});
         </script>
     """
 
-    return mark_safe(warnings_html + data_html)  # type: ignore
+    return mark_safe(data_html)  # type: ignore
```

### Comparing `slippers-0.6.0a0/slippers/static/slippers/main.css` & `slippers-0.6.1a0/slippers/static/slippers/main.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,4 +1,3 @@
 /*
 ! tailwindcss v3.2.4 | MIT License | https://tailwindcss.com
-*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;-webkit-font-feature-settings:normal;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;line-height:1.5;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-webkit-input-placeholder,textarea::-webkit-input-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::-webkit-backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }#slippers_errors_ui_root .fixed{position:fixed}#slippers_errors_ui_root .inset-0{bottom:0;left:0;right:0;top:0}#slippers_errors_ui_root .mt-4{margin-top:1rem}#slippers_errors_ui_root .mb-8{margin-bottom:2rem}#slippers_errors_ui_root .ml-auto{margin-left:auto}#slippers_errors_ui_root .flex{display:flex}#slippers_errors_ui_root .flex-col{flex-direction:column}#slippers_errors_ui_root .items-start{align-items:flex-start}#slippers_errors_ui_root .space-y-8>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:calc(2rem*var(--tw-space-y-reverse));margin-top:calc(2rem*(1 - var(--tw-space-y-reverse)))}#slippers_errors_ui_root .overflow-auto{overflow:auto}#slippers_errors_ui_root .break-words{overflow-wrap:break-word}#slippers_errors_ui_root .bg-zinc-800{--tw-bg-opacity:1;background-color:rgb(39 39 42/var(--tw-bg-opacity))}#slippers_errors_ui_root .bg-black\/90{background-color:rgba(0,0,0,.9)}#slippers_errors_ui_root .bg-black{--tw-bg-opacity:1;background-color:rgb(0 0 0/var(--tw-bg-opacity))}#slippers_errors_ui_root .p-4{padding:1rem}#slippers_errors_ui_root .p-12{padding:3rem}#slippers_errors_ui_root .px-4{padding-left:1rem;padding-right:1rem}#slippers_errors_ui_root .py-2{padding-bottom:.5rem;padding-top:.5rem}#slippers_errors_ui_root .font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}#slippers_errors_ui_root .text-2xl{font-size:1.5rem;line-height:2rem}#slippers_errors_ui_root .text-indigo-400{--tw-text-opacity:1;color:rgb(129 140 248/var(--tw-text-opacity))}#slippers_errors_ui_root .text-orange-400{--tw-text-opacity:1;color:rgb(251 146 60/var(--tw-text-opacity))}#slippers_errors_ui_root .text-teal-400{--tw-text-opacity:1;color:rgb(45 212 191/var(--tw-text-opacity))}#slippers_errors_ui_root .text-zinc-400{--tw-text-opacity:1;color:rgb(161 161 170/var(--tw-text-opacity))}#slippers_errors_ui_root .text-zinc-200{--tw-text-opacity:1;color:rgb(228 228 231/var(--tw-text-opacity))}#slippers_errors_ui_root .text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}#slippers_errors_ui_root .text-red-400{--tw-text-opacity:1;color:rgb(248 113 113/var(--tw-text-opacity))}
-/*# sourceMappingURL=main.css.map*/
+*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;-webkit-font-feature-settings:normal;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;line-height:1.5;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-webkit-input-placeholder,textarea::-webkit-input-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::-webkit-backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }#slippers_errors_ui_root .fixed{position:fixed}#slippers_errors_ui_root .inset-0{bottom:0;left:0;right:0;top:0}#slippers_errors_ui_root .mt-4{margin-top:1rem}#slippers_errors_ui_root .mb-8{margin-bottom:2rem}#slippers_errors_ui_root .ml-auto{margin-left:auto}#slippers_errors_ui_root .flex{display:flex}#slippers_errors_ui_root .flex-col{flex-direction:column}#slippers_errors_ui_root .items-start{align-items:flex-start}#slippers_errors_ui_root .space-y-8>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:calc(2rem*var(--tw-space-y-reverse));margin-top:calc(2rem*(1 - var(--tw-space-y-reverse)))}#slippers_errors_ui_root .overflow-auto{overflow:auto}#slippers_errors_ui_root .break-words{overflow-wrap:break-word}#slippers_errors_ui_root .bg-zinc-800{--tw-bg-opacity:1;background-color:rgb(39 39 42/var(--tw-bg-opacity))}#slippers_errors_ui_root .bg-black\/90{background-color:rgba(0,0,0,.9)}#slippers_errors_ui_root .bg-black{--tw-bg-opacity:1;background-color:rgb(0 0 0/var(--tw-bg-opacity))}#slippers_errors_ui_root .p-4{padding:1rem}#slippers_errors_ui_root .px-4{padding-left:1rem;padding-right:1rem}#slippers_errors_ui_root .py-2{padding-bottom:.5rem;padding-top:.5rem}#slippers_errors_ui_root .font-mono{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}#slippers_errors_ui_root .text-2xl{font-size:1.5rem;line-height:2rem}#slippers_errors_ui_root .text-indigo-400{--tw-text-opacity:1;color:rgb(129 140 248/var(--tw-text-opacity))}#slippers_errors_ui_root .text-orange-400{--tw-text-opacity:1;color:rgb(251 146 60/var(--tw-text-opacity))}#slippers_errors_ui_root .text-teal-400{--tw-text-opacity:1;color:rgb(45 212 191/var(--tw-text-opacity))}#slippers_errors_ui_root .text-zinc-400{--tw-text-opacity:1;color:rgb(161 161 170/var(--tw-text-opacity))}#slippers_errors_ui_root .text-zinc-200{--tw-text-opacity:1;color:rgb(228 228 231/var(--tw-text-opacity))}#slippers_errors_ui_root .text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}#slippers_errors_ui_root .text-red-400{--tw-text-opacity:1;color:rgb(248 113 113/var(--tw-text-opacity))}@media (min-width:768px){#slippers_errors_ui_root .md\:p-12{padding:3rem}}
```

### Comparing `slippers-0.6.0a0/slippers/static/slippers/main.js` & `slippers-0.6.1a0/slippers/static/slippers/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 /*! For license information please see main.js.LICENSE.txt */ ! function() {
     "use strict";
     var e = {
-            463: function(e, n, t) {
-                var r = t(791),
-                    l = t(296);
+            534: function(e, n, t) {
+                var r = t(313),
+                    l = t(224);
 
                 function a(e) {
                     for (var n = "https://reactjs.org/docs/error-decoder.html?invariant=" + e, t = 1; t < arguments.length; t++) n += "&args[]=" + encodeURIComponent(arguments[t]);
                     return "Minified React error #" + e + "; visit " + n + " for the full message or use the non-minified dev environment for full errors and additional helpful warnings."
                 }
                 var o = new Set,
                     u = {};
@@ -111,16 +111,16 @@
                     x = Symbol.for("react.fragment"),
                     E = Symbol.for("react.strict_mode"),
                     _ = Symbol.for("react.profiler"),
                     C = Symbol.for("react.provider"),
                     N = Symbol.for("react.context"),
                     P = Symbol.for("react.forward_ref"),
                     z = Symbol.for("react.suspense"),
-                    T = Symbol.for("react.suspense_list"),
-                    L = Symbol.for("react.memo"),
+                    L = Symbol.for("react.suspense_list"),
+                    T = Symbol.for("react.memo"),
                     R = Symbol.for("react.lazy");
                 Symbol.for("react.scope"), Symbol.for("react.debug_trace_mode");
                 var O = Symbol.for("react.offscreen");
                 Symbol.for("react.legacy_hidden"), Symbol.for("react.cache"), Symbol.for("react.tracing_marker");
                 var M = Symbol.iterator;
 
                 function F(e) {
@@ -230,26 +230,26 @@
                             return "Portal";
                         case _:
                             return "Profiler";
                         case E:
                             return "StrictMode";
                         case z:
                             return "Suspense";
-                        case T:
+                        case L:
                             return "SuspenseList"
                     }
                     if ("object" === typeof e) switch (e.$$typeof) {
                         case N:
                             return (e.displayName || "Context") + ".Consumer";
                         case C:
                             return (e._context.displayName || "Context") + ".Provider";
                         case P:
                             var n = e.render;
                             return (e = e.displayName) || (e = "" !== (e = n.displayName || n.name || "") ? "ForwardRef(" + e + ")" : "ForwardRef"), e;
-                        case L:
+                        case T:
                             return null !== (n = e.displayName || null) ? n : $(e.type) || "Memo";
                         case R:
                             n = e._payload, e = e._init;
                             try {
                                 return $(e(n))
                             } catch (t) {}
                     }
@@ -650,23 +650,23 @@
                 }
 
                 function Pe(e, n) {
                     return e(n)
                 }
 
                 function ze() {}
-                var Te = !1;
+                var Le = !1;
 
-                function Le(e, n, t) {
-                    if (Te) return e(n, t);
-                    Te = !0;
+                function Te(e, n, t) {
+                    if (Le) return e(n, t);
+                    Le = !0;
                     try {
                         return Pe(e, n, t)
                     } finally {
-                        Te = !1, (null !== xe || null !== Ee) && (ze(), Ne())
+                        Le = !1, (null !== xe || null !== Ee) && (ze(), Ne())
                     }
                 }
 
                 function Re(e, n) {
                     var t = e.stateNode;
                     if (null === t) return null;
                     var r = kl(t);
@@ -973,34 +973,34 @@
 
                 function kn(e) {
                     return 1 < (e &= -e) ? 4 < e ? 0 !== (268435455 & e) ? 16 : 536870912 : 4 : 1
                 }
                 var Sn, xn, En, _n, Cn, Nn = !1,
                     Pn = [],
                     zn = null,
-                    Tn = null,
                     Ln = null,
+                    Tn = null,
                     Rn = new Map,
                     On = new Map,
                     Mn = [],
                     Fn = "mousedown mouseup touchcancel touchend touchstart auxclick dblclick pointercancel pointerdown pointerup dragend dragstart drop compositionend compositionstart keydown keypress keyup input textInput copy cut paste click change contextmenu reset submit".split(" ");
 
                 function Dn(e, n) {
                     switch (e) {
                         case "focusin":
                         case "focusout":
                             zn = null;
                             break;
                         case "dragenter":
                         case "dragleave":
-                            Tn = null;
+                            Ln = null;
                             break;
                         case "mouseover":
                         case "mouseout":
-                            Ln = null;
+                            Tn = null;
                             break;
                         case "pointerover":
                         case "pointerout":
                             Rn.delete(n.pointerId);
                             break;
                         case "gotpointercapture":
                         case "lostpointercapture":
@@ -1044,15 +1044,15 @@
                 }
 
                 function An(e, n, t) {
                     Un(e) && t.delete(n)
                 }
 
                 function Vn() {
-                    Nn = !1, null !== zn && Un(zn) && (zn = null), null !== Tn && Un(Tn) && (Tn = null), null !== Ln && Un(Ln) && (Ln = null), Rn.forEach(An), On.forEach(An)
+                    Nn = !1, null !== zn && Un(zn) && (zn = null), null !== Ln && Un(Ln) && (Ln = null), null !== Tn && Un(Tn) && (Tn = null), Rn.forEach(An), On.forEach(An)
                 }
 
                 function $n(e, n) {
                     e.blockedOn === n && (e.blockedOn = null, Nn || (Nn = !0, l.unstable_scheduleCallback(l.unstable_NormalPriority, Vn)))
                 }
 
                 function Bn(e) {
@@ -1062,15 +1062,15 @@
                     if (0 < Pn.length) {
                         $n(Pn[0], e);
                         for (var t = 1; t < Pn.length; t++) {
                             var r = Pn[t];
                             r.blockedOn === e && (r.blockedOn = null)
                         }
                     }
-                    for (null !== zn && $n(zn, e), null !== Tn && $n(Tn, e), null !== Ln && $n(Ln, e), Rn.forEach(n), On.forEach(n), t = 0; t < Mn.length; t++)(r = Mn[t]).blockedOn === e && (r.blockedOn = null);
+                    for (null !== zn && $n(zn, e), null !== Ln && $n(Ln, e), null !== Tn && $n(Tn, e), Rn.forEach(n), On.forEach(n), t = 0; t < Mn.length; t++)(r = Mn[t]).blockedOn === e && (r.blockedOn = null);
                     for (; 0 < Mn.length && null === (t = Mn[0]).blockedOn;) jn(t), null === t.blockedOn && Mn.shift()
                 }
                 var Hn = w.ReactCurrentBatchConfig,
                     Wn = !0;
 
                 function Qn(e, n, t, r) {
                     var l = wn,
@@ -1099,17 +1099,17 @@
                         var l = Xn(e, n, t, r);
                         if (null === l) Hr(e, n, r, Yn, t), Dn(e, r);
                         else if (function(e, n, t, r, l) {
                                 switch (n) {
                                     case "focusin":
                                         return zn = In(zn, e, n, t, r, l), !0;
                                     case "dragenter":
-                                        return Tn = In(Tn, e, n, t, r, l), !0;
-                                    case "mouseover":
                                         return Ln = In(Ln, e, n, t, r, l), !0;
+                                    case "mouseover":
+                                        return Tn = In(Tn, e, n, t, r, l), !0;
                                     case "pointerover":
                                         var a = l.pointerId;
                                         return Rn.set(a, In(Rn.get(a) || null, e, n, t, r, l)), !0;
                                     case "gotpointercapture":
                                         return a = l.pointerId, On.set(a, In(On.get(a) || null, e, n, t, r, l)), !0
                                 }
                                 return !1
@@ -1453,30 +1453,30 @@
                         changedTouches: 0,
                         altKey: 0,
                         metaKey: 0,
                         ctrlKey: 0,
                         shiftKey: 0,
                         getModifierState: _t
                     })),
-                    Tt = at(I({}, st, {
+                    Lt = at(I({}, st, {
                         propertyName: 0,
                         elapsedTime: 0,
                         pseudoElement: 0
                     })),
-                    Lt = I({}, pt, {
+                    Tt = I({}, pt, {
                         deltaX: function(e) {
                             return "deltaX" in e ? e.deltaX : "wheelDeltaX" in e ? -e.wheelDeltaX : 0
                         },
                         deltaY: function(e) {
                             return "deltaY" in e ? e.deltaY : "wheelDeltaY" in e ? -e.wheelDeltaY : "wheelDelta" in e ? -e.wheelDelta : 0
                         },
                         deltaZ: 0,
                         deltaMode: 0
                     }),
-                    Rt = at(Lt),
+                    Rt = at(Tt),
                     Ot = [9, 13, 27, 32],
                     Mt = c && "CompositionEvent" in window,
                     Ft = null;
                 c && "documentMode" in document && (Ft = document.documentMode);
                 var Dt = c && "TextEvent" in window && !Ft,
                     It = c && (!Mt || Ft && 8 < Ft && 11 >= Ft),
                     jt = String.fromCharCode(32),
@@ -1561,15 +1561,15 @@
                 function nr() {
                     Qt && (Qt.detachEvent("onpropertychange", tr), qt = Qt = null)
                 }
 
                 function tr(e) {
                     if ("value" === e.propertyName && Yt(qt)) {
                         var n = [];
-                        Wt(n, qt, e, ke(e)), Le(Kt, n)
+                        Wt(n, qt, e, ke(e)), Te(Kt, n)
                     }
                 }
 
                 function rr(e, n, t) {
                     "focusin" === e ? (nr(), qt = t, (Qt = n).attachEvent("onpropertychange", tr)) : "focusout" === e && nr()
                 }
 
@@ -1719,22 +1719,22 @@
                     return e
                 }
                 c && (Er = document.createElement("div").style, "AnimationEvent" in window || (delete Sr.animationend.animation, delete Sr.animationiteration.animation, delete Sr.animationstart.animation), "TransitionEvent" in window || delete Sr.transitionend.transition);
                 var Cr = _r("animationend"),
                     Nr = _r("animationiteration"),
                     Pr = _r("animationstart"),
                     zr = _r("transitionend"),
-                    Tr = new Map,
-                    Lr = "abort auxClick cancel canPlay canPlayThrough click close contextMenu copy cut drag dragEnd dragEnter dragExit dragLeave dragOver dragStart drop durationChange emptied encrypted ended error gotPointerCapture input invalid keyDown keyPress keyUp load loadedData loadedMetadata loadStart lostPointerCapture mouseDown mouseMove mouseOut mouseOver mouseUp paste pause play playing pointerCancel pointerDown pointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");
+                    Lr = new Map,
+                    Tr = "abort auxClick cancel canPlay canPlayThrough click close contextMenu copy cut drag dragEnd dragEnter dragExit dragLeave dragOver dragStart drop durationChange emptied encrypted ended error gotPointerCapture input invalid keyDown keyPress keyUp load loadedData loadedMetadata loadStart lostPointerCapture mouseDown mouseMove mouseOut mouseOver mouseUp paste pause play playing pointerCancel pointerDown pointerMove pointerOut pointerOver pointerUp progress rateChange reset resize seeked seeking stalled submit suspend timeUpdate touchCancel touchEnd touchStart volumeChange scroll toggle touchMove waiting wheel".split(" ");
 
                 function Rr(e, n) {
-                    Tr.set(e, n), i(n, [e])
+                    Lr.set(e, n), i(n, [e])
                 }
-                for (var Or = 0; Or < Lr.length; Or++) {
-                    var Mr = Lr[Or];
+                for (var Or = 0; Or < Tr.length; Or++) {
+                    var Mr = Tr[Or];
                     Rr(Mr.toLowerCase(), "on" + (Mr[0].toUpperCase() + Mr.slice(1)))
                 }
                 Rr(Cr, "onAnimationEnd"), Rr(Nr, "onAnimationIteration"), Rr(Pr, "onAnimationStart"), Rr("dblclick", "onDoubleClick"), Rr("focusin", "onFocus"), Rr("focusout", "onBlur"), Rr(zr, "onTransitionEnd"), s("onMouseEnter", ["mouseout", "mouseover"]), s("onMouseLeave", ["mouseout", "mouseover"]), s("onPointerEnter", ["pointerout", "pointerover"]), s("onPointerLeave", ["pointerout", "pointerover"]), i("onChange", "change click focusin focusout input keydown keyup selectionchange".split(" ")), i("onSelect", "focusout contextmenu dragend focusin keydown keyup mousedown mouseup selectionchange".split(" ")), i("onBeforeInput", ["compositionend", "keypress", "textInput", "paste"]), i("onCompositionEnd", "compositionend focusout keydown keypress keyup mousedown".split(" ")), i("onCompositionStart", "compositionstart focusout keydown keypress keyup mousedown".split(" ")), i("onCompositionUpdate", "compositionupdate focusout keydown keypress keyup mousedown".split(" "));
                 var Fr = "abort canplay canplaythrough durationchange emptied encrypted ended error loadeddata loadedmetadata loadstart pause play playing progress ratechange resize seeked seeking stalled suspend timeupdate volumechange waiting".split(" "),
                     Dr = new Set("cancel close invalid load scroll toggle".split(" ").concat(Fr));
 
                 function Ir(e, n, t) {
@@ -1837,20 +1837,20 @@
                                     continue e
                                 }
                                 u = u.parentNode
                             }
                         }
                         r = r.return
                     }
-                    Le((function() {
+                    Te((function() {
                         var r = a,
                             l = ke(t),
                             o = [];
                         e: {
-                            var u = Tr.get(e);
+                            var u = Lr.get(e);
                             if (void 0 !== u) {
                                 var i = ct,
                                     s = e;
                                 switch (e) {
                                     case "keypress":
                                         if (0 === tt(t)) break e;
                                     case "keydown":
@@ -1897,15 +1897,15 @@
                                         break;
                                     case Cr:
                                     case Nr:
                                     case Pr:
                                         i = gt;
                                         break;
                                     case zr:
-                                        i = Tt;
+                                        i = Lt;
                                         break;
                                     case "scroll":
                                         i = dt;
                                         break;
                                     case "wheel":
                                         i = Rt;
                                         break;
@@ -2202,17 +2202,17 @@
 
                 function Cl(e, n) {
                     xl++, Sl[xl] = e.current, e.current = n
                 }
                 var Nl = {},
                     Pl = El(Nl),
                     zl = El(!1),
-                    Tl = Nl;
+                    Ll = Nl;
 
-                function Ll(e, n) {
+                function Tl(e, n) {
                     var t = e.type.contextTypes;
                     if (!t) return Nl;
                     var r = e.stateNode;
                     if (r && r.__reactInternalMemoizedUnmaskedChildContext === n) return r.__reactInternalMemoizedMaskedChildContext;
                     var l, a = {};
                     for (l in t) a[l] = n[l];
                     return r && ((e = e.stateNode).__reactInternalMemoizedUnmaskedChildContext = n, e.__reactInternalMemoizedMaskedChildContext = a), a
@@ -2236,21 +2236,21 @@
                     if (n = n.childContextTypes, "function" !== typeof r.getChildContext) return t;
                     for (var l in r = r.getChildContext())
                         if (!(l in n)) throw Error(a(108, B(e) || "Unknown", l));
                     return I({}, t, r)
                 }
 
                 function Dl(e) {
-                    return e = (e = e.stateNode) && e.__reactInternalMemoizedMergedChildContext || Nl, Tl = Pl.current, Cl(Pl, e), Cl(zl, zl.current), !0
+                    return e = (e = e.stateNode) && e.__reactInternalMemoizedMergedChildContext || Nl, Ll = Pl.current, Cl(Pl, e), Cl(zl, zl.current), !0
                 }
 
                 function Il(e, n, t) {
                     var r = e.stateNode;
                     if (!r) throw Error(a(169));
-                    t ? (e = Fl(e, n, Tl), r.__reactInternalMemoizedMergedChildContext = e, _l(zl), _l(Pl), Cl(Pl, e)) : _l(zl), Cl(zl, t)
+                    t ? (e = Fl(e, n, Ll), r.__reactInternalMemoizedMergedChildContext = e, _l(zl), _l(Pl), Cl(Pl, e)) : _l(zl), Cl(zl, t)
                 }
                 var jl = null,
                     Ul = !1,
                     Al = !1;
 
                 function Vl(e) {
                     null === jl ? jl = [e] : jl.push(e)
@@ -2315,15 +2315,15 @@
                 }
                 var ta = null,
                     ra = null,
                     la = !1,
                     aa = null;
 
                 function oa(e, n) {
-                    var t = Ls(5, null, null, 0);
+                    var t = Ts(5, null, null, 0);
                     t.elementType = "DELETED", t.stateNode = n, t.return = e, null === (n = e.deletions) ? (e.deletions = [t], e.flags |= 16) : n.push(t)
                 }
 
                 function ua(e, n) {
                     switch (e.tag) {
                         case 5:
                             var t = e.type;
@@ -2334,15 +2334,15 @@
                             return null !== (n = 8 !== n.nodeType ? null : n) && (t = null !== Yl ? {
                                 id: Xl,
                                 overflow: Gl
                             } : null, e.memoizedState = {
                                 dehydrated: n,
                                 treeContext: t,
                                 retryLane: 1073741824
-                            }, (t = Ls(18, null, null, 0)).stateNode = n, t.return = e, e.child = t, ta = e, ra = null, !0);
+                            }, (t = Ts(18, null, null, 0)).stateNode = n, t.return = e, e.child = t, ta = e, ra = null, !0);
                         default:
                             return !1
                     }
                 }
 
                 function ia(e) {
                     return 0 !== (1 & e.mode) && 0 === (128 & e.flags)
@@ -2476,17 +2476,17 @@
 
                 function za(e, n) {
                     e.lanes |= n;
                     var t = e.alternate;
                     for (null !== t && (t.lanes |= n), t = e, e = e.return; null !== e;) e.childLanes |= n, null !== (t = e.alternate) && (t.childLanes |= n), t = e, e = e.return;
                     return 3 === t.tag ? t.stateNode : null
                 }
-                var Ta = !1;
+                var La = !1;
 
-                function La(e) {
+                function Ta(e) {
                     e.updateQueue = {
                         baseState: e.memoizedState,
                         firstBaseUpdate: null,
                         lastBaseUpdate: null,
                         shared: {
                             pending: null,
                             interleaved: null,
@@ -2563,15 +2563,15 @@
                         }, void(e.updateQueue = t)
                     }
                     null === (e = t.lastBaseUpdate) ? t.firstBaseUpdate = n : e.next = n, t.lastBaseUpdate = n
                 }
 
                 function Ia(e, n, t, r) {
                     var l = e.updateQueue;
-                    Ta = !1;
+                    La = !1;
                     var a = l.firstBaseUpdate,
                         o = l.lastBaseUpdate,
                         u = l.shared.pending;
                     if (null !== u) {
                         l.shared.pending = null;
                         var i = u,
                             s = i.next;
@@ -2607,15 +2607,15 @@
                                         case 3:
                                             m.flags = -65537 & m.flags | 128;
                                         case 0:
                                             if (null === (d = "function" === typeof(m = h.payload) ? m.call(p, f, d) : m) || void 0 === d) break e;
                                             f = I({}, f, d);
                                             break e;
                                         case 2:
-                                            Ta = !0
+                                            La = !0
                                     }
                                 }
                                 null !== u.callback && 0 !== u.lane && (e.flags |= 64, null === (d = l.effects) ? l.effects = [u] : d.push(u))
                             } else p = {
                                 eventTime: p,
                                 lane: d,
                                 tag: u.tag,
@@ -2685,26 +2685,26 @@
                     return "function" === typeof(e = e.stateNode).shouldComponentUpdate ? e.shouldComponentUpdate(r, a, o) : !n.prototype || !n.prototype.isPureReactComponent || (!ir(t, r) || !ir(l, a))
                 }
 
                 function Ba(e, n, t) {
                     var r = !1,
                         l = Nl,
                         a = n.contextType;
-                    return "object" === typeof a && null !== a ? a = _a(a) : (l = Rl(n) ? Tl : Pl.current, a = (r = null !== (r = n.contextTypes) && void 0 !== r) ? Ll(e, l) : Nl), n = new n(t, a), e.memoizedState = null !== n.state && void 0 !== n.state ? n.state : null, n.updater = Va, e.stateNode = n, n._reactInternals = e, r && ((e = e.stateNode).__reactInternalMemoizedUnmaskedChildContext = l, e.__reactInternalMemoizedMaskedChildContext = a), n
+                    return "object" === typeof a && null !== a ? a = _a(a) : (l = Rl(n) ? Ll : Pl.current, a = (r = null !== (r = n.contextTypes) && void 0 !== r) ? Tl(e, l) : Nl), n = new n(t, a), e.memoizedState = null !== n.state && void 0 !== n.state ? n.state : null, n.updater = Va, e.stateNode = n, n._reactInternals = e, r && ((e = e.stateNode).__reactInternalMemoizedUnmaskedChildContext = l, e.__reactInternalMemoizedMaskedChildContext = a), n
                 }
 
                 function Ha(e, n, t, r) {
                     e = n.state, "function" === typeof n.componentWillReceiveProps && n.componentWillReceiveProps(t, r), "function" === typeof n.UNSAFE_componentWillReceiveProps && n.UNSAFE_componentWillReceiveProps(t, r), n.state !== e && Va.enqueueReplaceState(n, n.state, null)
                 }
 
                 function Wa(e, n, t, r) {
                     var l = e.stateNode;
-                    l.props = t, l.state = e.memoizedState, l.refs = Ua, La(e);
+                    l.props = t, l.state = e.memoizedState, l.refs = Ua, Ta(e);
                     var a = n.contextType;
-                    "object" === typeof a && null !== a ? l.context = _a(a) : (a = Rl(n) ? Tl : Pl.current, l.context = Ll(e, a)), l.state = e.memoizedState, "function" === typeof(a = n.getDerivedStateFromProps) && (Aa(e, n, a, t), l.state = e.memoizedState), "function" === typeof n.getDerivedStateFromProps || "function" === typeof l.getSnapshotBeforeUpdate || "function" !== typeof l.UNSAFE_componentWillMount && "function" !== typeof l.componentWillMount || (n = l.state, "function" === typeof l.componentWillMount && l.componentWillMount(), "function" === typeof l.UNSAFE_componentWillMount && l.UNSAFE_componentWillMount(), n !== l.state && Va.enqueueReplaceState(l, l.state, null), Ia(e, t, l, r), l.state = e.memoizedState), "function" === typeof l.componentDidMount && (e.flags |= 4194308)
+                    "object" === typeof a && null !== a ? l.context = _a(a) : (a = Rl(n) ? Ll : Pl.current, l.context = Tl(e, a)), l.state = e.memoizedState, "function" === typeof(a = n.getDerivedStateFromProps) && (Aa(e, n, a, t), l.state = e.memoizedState), "function" === typeof n.getDerivedStateFromProps || "function" === typeof l.getSnapshotBeforeUpdate || "function" !== typeof l.UNSAFE_componentWillMount && "function" !== typeof l.componentWillMount || (n = l.state, "function" === typeof l.componentWillMount && l.componentWillMount(), "function" === typeof l.UNSAFE_componentWillMount && l.UNSAFE_componentWillMount(), n !== l.state && Va.enqueueReplaceState(l, l.state, null), Ia(e, t, l, r), l.state = e.memoizedState), "function" === typeof l.componentDidMount && (e.flags |= 4194308)
                 }
 
                 function Qa(e, n, t) {
                     if (null !== (e = t.ref) && "function" !== typeof e && "object" !== typeof e) {
                         if (t._owner) {
                             if (t = t._owner) {
                                 if (1 !== t.tag) throw Error(a(309));
@@ -3114,15 +3114,15 @@
                         do {
                             o = l.lane, ho.lanes |= o, Di |= o, l = l.next
                         } while (l !== e)
                     } else null === l && (t.lanes = 0);
                     return [n.memoizedState, t.dispatch]
                 }
 
-                function To(e) {
+                function Lo(e) {
                     var n = No(),
                         t = n.queue;
                     if (null === t) throw Error(a(311));
                     t.lastRenderedReducer = e;
                     var r = t.dispatch,
                         l = t.pending,
                         o = n.memoizedState;
@@ -3133,15 +3133,15 @@
                             o = e(o, u.action), u = u.next
                         } while (u !== l);
                         ur(o, n.memoizedState) || (wu = !0), n.memoizedState = o, null === n.baseQueue && (n.baseState = o), t.lastRenderedState = o
                     }
                     return [o, r]
                 }
 
-                function Lo() {}
+                function To() {}
 
                 function Ro(e, n) {
                     var t = ho,
                         r = No(),
                         l = n(),
                         o = !ur(r.memoizedState, l);
                     if (o && (r.memoizedState = l, wu = !0), r = r.queue, Ho(Fo.bind(null, t, r, e), [e]), r.getSnapshot !== n || o || null !== go && 1 & go.memoizedState.tag) {
@@ -3463,42 +3463,42 @@
                         useDebugValue: Yo,
                         useDeferredValue: function(e) {
                             return Zo(No(), vo.memoizedState, e)
                         },
                         useTransition: function() {
                             return [zo(Po)[0], No().memoizedState]
                         },
-                        useMutableSource: Lo,
+                        useMutableSource: To,
                         useSyncExternalStore: Ro,
                         useId: eu,
                         unstable_isNewReconciler: !1
                     },
                     su = {
                         readContext: _a,
                         useCallback: Xo,
                         useContext: _a,
                         useEffect: Ho,
                         useImperativeHandle: Ko,
                         useInsertionEffect: Wo,
                         useLayoutEffect: Qo,
                         useMemo: Go,
-                        useReducer: To,
+                        useReducer: Lo,
                         useRef: Ao,
                         useState: function() {
-                            return To(Po)
+                            return Lo(Po)
                         },
                         useDebugValue: Yo,
                         useDeferredValue: function(e) {
                             var n = No();
                             return null === vo ? n.memoizedState = e : Zo(n, vo.memoizedState, e)
                         },
                         useTransition: function() {
-                            return [To(Po)[0], No().memoizedState]
+                            return [Lo(Po)[0], No().memoizedState]
                         },
-                        useMutableSource: Lo,
+                        useMutableSource: To,
                         useSyncExternalStore: Ro,
                         useId: eu,
                         unstable_isNewReconciler: !1
                     };
 
                 function cu(e, n) {
                     try {
@@ -3656,61 +3656,61 @@
 
                 function Cu(e, n) {
                     var t = n.ref;
                     (null === e && null !== t || null !== e && e.ref !== t) && (n.flags |= 512, n.flags |= 2097152)
                 }
 
                 function Nu(e, n, t, r, l) {
-                    var a = Rl(t) ? Tl : Pl.current;
-                    return a = Ll(n, a), Ea(n, l), t = Eo(e, n, t, r, a, l), r = _o(), null === e || wu ? (la && r && ea(n), n.flags |= 1, ku(e, n, t, l), n.child) : (n.updateQueue = e.updateQueue, n.flags &= -2053, e.lanes &= ~l, Hu(e, n, l))
+                    var a = Rl(t) ? Ll : Pl.current;
+                    return a = Tl(n, a), Ea(n, l), t = Eo(e, n, t, r, a, l), r = _o(), null === e || wu ? (la && r && ea(n), n.flags |= 1, ku(e, n, t, l), n.child) : (n.updateQueue = e.updateQueue, n.flags &= -2053, e.lanes &= ~l, Hu(e, n, l))
                 }
 
                 function Pu(e, n, t, r, l) {
                     if (Rl(t)) {
                         var a = !0;
                         Dl(n)
                     } else a = !1;
                     if (Ea(n, l), null === n.stateNode) Bu(e, n), Ba(n, t, r), Wa(n, t, r, l), r = !0;
                     else if (null === e) {
                         var o = n.stateNode,
                             u = n.memoizedProps;
                         o.props = u;
                         var i = o.context,
                             s = t.contextType;
-                        "object" === typeof s && null !== s ? s = _a(s) : s = Ll(n, s = Rl(t) ? Tl : Pl.current);
+                        "object" === typeof s && null !== s ? s = _a(s) : s = Tl(n, s = Rl(t) ? Ll : Pl.current);
                         var c = t.getDerivedStateFromProps,
                             f = "function" === typeof c || "function" === typeof o.getSnapshotBeforeUpdate;
-                        f || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== r || i !== s) && Ha(n, o, r, s), Ta = !1;
+                        f || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== r || i !== s) && Ha(n, o, r, s), La = !1;
                         var d = n.memoizedState;
-                        o.state = d, Ia(n, r, o, l), i = n.memoizedState, u !== r || d !== i || zl.current || Ta ? ("function" === typeof c && (Aa(n, t, c, r), i = n.memoizedState), (u = Ta || $a(n, t, u, r, d, i, s)) ? (f || "function" !== typeof o.UNSAFE_componentWillMount && "function" !== typeof o.componentWillMount || ("function" === typeof o.componentWillMount && o.componentWillMount(), "function" === typeof o.UNSAFE_componentWillMount && o.UNSAFE_componentWillMount()), "function" === typeof o.componentDidMount && (n.flags |= 4194308)) : ("function" === typeof o.componentDidMount && (n.flags |= 4194308), n.memoizedProps = r, n.memoizedState = i), o.props = r, o.state = i, o.context = s, r = u) : ("function" === typeof o.componentDidMount && (n.flags |= 4194308), r = !1)
+                        o.state = d, Ia(n, r, o, l), i = n.memoizedState, u !== r || d !== i || zl.current || La ? ("function" === typeof c && (Aa(n, t, c, r), i = n.memoizedState), (u = La || $a(n, t, u, r, d, i, s)) ? (f || "function" !== typeof o.UNSAFE_componentWillMount && "function" !== typeof o.componentWillMount || ("function" === typeof o.componentWillMount && o.componentWillMount(), "function" === typeof o.UNSAFE_componentWillMount && o.UNSAFE_componentWillMount()), "function" === typeof o.componentDidMount && (n.flags |= 4194308)) : ("function" === typeof o.componentDidMount && (n.flags |= 4194308), n.memoizedProps = r, n.memoizedState = i), o.props = r, o.state = i, o.context = s, r = u) : ("function" === typeof o.componentDidMount && (n.flags |= 4194308), r = !1)
                     } else {
-                        o = n.stateNode, Ra(e, n), u = n.memoizedProps, s = n.type === n.elementType ? u : va(n.type, u), o.props = s, f = n.pendingProps, d = o.context, "object" === typeof(i = t.contextType) && null !== i ? i = _a(i) : i = Ll(n, i = Rl(t) ? Tl : Pl.current);
+                        o = n.stateNode, Ra(e, n), u = n.memoizedProps, s = n.type === n.elementType ? u : va(n.type, u), o.props = s, f = n.pendingProps, d = o.context, "object" === typeof(i = t.contextType) && null !== i ? i = _a(i) : i = Tl(n, i = Rl(t) ? Ll : Pl.current);
                         var p = t.getDerivedStateFromProps;
-                        (c = "function" === typeof p || "function" === typeof o.getSnapshotBeforeUpdate) || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== f || d !== i) && Ha(n, o, r, i), Ta = !1, d = n.memoizedState, o.state = d, Ia(n, r, o, l);
+                        (c = "function" === typeof p || "function" === typeof o.getSnapshotBeforeUpdate) || "function" !== typeof o.UNSAFE_componentWillReceiveProps && "function" !== typeof o.componentWillReceiveProps || (u !== f || d !== i) && Ha(n, o, r, i), La = !1, d = n.memoizedState, o.state = d, Ia(n, r, o, l);
                         var m = n.memoizedState;
-                        u !== f || d !== m || zl.current || Ta ? ("function" === typeof p && (Aa(n, t, p, r), m = n.memoizedState), (s = Ta || $a(n, t, s, r, d, m, i) || !1) ? (c || "function" !== typeof o.UNSAFE_componentWillUpdate && "function" !== typeof o.componentWillUpdate || ("function" === typeof o.componentWillUpdate && o.componentWillUpdate(r, m, i), "function" === typeof o.UNSAFE_componentWillUpdate && o.UNSAFE_componentWillUpdate(r, m, i)), "function" === typeof o.componentDidUpdate && (n.flags |= 4), "function" === typeof o.getSnapshotBeforeUpdate && (n.flags |= 1024)) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 1024), n.memoizedProps = r, n.memoizedState = m), o.props = r, o.state = m, o.context = i, r = s) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 1024), r = !1)
+                        u !== f || d !== m || zl.current || La ? ("function" === typeof p && (Aa(n, t, p, r), m = n.memoizedState), (s = La || $a(n, t, s, r, d, m, i) || !1) ? (c || "function" !== typeof o.UNSAFE_componentWillUpdate && "function" !== typeof o.componentWillUpdate || ("function" === typeof o.componentWillUpdate && o.componentWillUpdate(r, m, i), "function" === typeof o.UNSAFE_componentWillUpdate && o.UNSAFE_componentWillUpdate(r, m, i)), "function" === typeof o.componentDidUpdate && (n.flags |= 4), "function" === typeof o.getSnapshotBeforeUpdate && (n.flags |= 1024)) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 1024), n.memoizedProps = r, n.memoizedState = m), o.props = r, o.state = m, o.context = i, r = s) : ("function" !== typeof o.componentDidUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 4), "function" !== typeof o.getSnapshotBeforeUpdate || u === e.memoizedProps && d === e.memoizedState || (n.flags |= 1024), r = !1)
                     }
                     return zu(e, n, t, r, a, l)
                 }
 
                 function zu(e, n, t, r, l, a) {
                     Cu(e, n);
                     var o = 0 !== (128 & n.flags);
                     if (!r && !o) return l && Il(n, t, !1), Hu(e, n, a);
                     r = n.stateNode, bu.current = n;
                     var u = o && "function" !== typeof t.getDerivedStateFromError ? null : r.render();
                     return n.flags |= 1, null !== e && o ? (n.child = Xa(n, e.child, null, a), n.child = Xa(n, null, u, a)) : ku(e, n, u, a), n.memoizedState = r.state, l && Il(n, t, !0), n.child
                 }
 
-                function Tu(e) {
+                function Lu(e) {
                     var n = e.stateNode;
                     n.pendingContext ? Ml(0, n.pendingContext, n.pendingContext !== n.context) : n.context && Ml(0, n.context, !1), ro(e, n.containerInfo)
                 }
 
-                function Lu(e, n, t, r, l) {
+                function Tu(e, n, t, r, l) {
                     return pa(), ma(l), n.flags |= 256, ku(e, n, t, r), n.child
                 }
                 var Ru, Ou, Mu, Fu = {
                     dehydrated: null,
                     treeContext: null,
                     retryLane: 0
                 };
@@ -4832,16 +4832,16 @@
                 }
                 var xi, Ei = Math.ceil,
                     _i = w.ReactCurrentDispatcher,
                     Ci = w.ReactCurrentOwner,
                     Ni = w.ReactCurrentBatchConfig,
                     Pi = 0,
                     zi = null,
-                    Ti = null,
-                    Li = 0,
+                    Li = null,
+                    Ti = 0,
                     Ri = 0,
                     Oi = El(0),
                     Mi = 0,
                     Fi = null,
                     Di = 0,
                     Ii = 0,
                     ji = 0,
@@ -4862,32 +4862,32 @@
                     Ji = 0;
 
                 function es() {
                     return 0 !== (6 & Pi) ? Ge() : -1 !== Zi ? Zi : Zi = Ge()
                 }
 
                 function ns(e) {
-                    return 0 === (1 & e.mode) ? 1 : 0 !== (2 & Pi) && 0 !== Li ? Li & -Li : null !== ha.transition ? (0 === Ji && (Ji = vn()), Ji) : 0 !== (e = wn) ? e : e = void 0 === (e = window.event) ? 16 : Gn(e.type)
+                    return 0 === (1 & e.mode) ? 1 : 0 !== (2 & Pi) && 0 !== Ti ? Ti & -Ti : null !== ha.transition ? (0 === Ji && (Ji = vn()), Ji) : 0 !== (e = wn) ? e : e = void 0 === (e = window.event) ? 16 : Gn(e.type)
                 }
 
                 function ts(e, n, t, r) {
                     if (50 < Xi) throw Xi = 0, Gi = null, Error(a(185));
-                    yn(e, t, r), 0 !== (2 & Pi) && e === zi || (e === zi && (0 === (2 & Pi) && (Ii |= t), 4 === Mi && us(e, Li)), rs(e, r), 1 === t && 0 === Pi && 0 === (1 & n.mode) && ($i = Ge() + 500, Ul && $l()))
+                    yn(e, t, r), 0 !== (2 & Pi) && e === zi || (e === zi && (0 === (2 & Pi) && (Ii |= t), 4 === Mi && us(e, Ti)), rs(e, r), 1 === t && 0 === Pi && 0 === (1 & n.mode) && ($i = Ge() + 500, Ul && $l()))
                 }
 
                 function rs(e, n) {
                     var t = e.callbackNode;
                     ! function(e, n) {
                         for (var t = e.suspendedLanes, r = e.pingedLanes, l = e.expirationTimes, a = e.pendingLanes; 0 < a;) {
                             var o = 31 - on(a),
                                 u = 1 << o,
                                 i = l[o]; - 1 === i ? 0 !== (u & t) && 0 === (u & r) || (l[o] = mn(u, n)) : i <= n && (e.expiredLanes |= u), a &= ~u
                         }
                     }(e, n);
-                    var r = pn(e, e === zi ? Li : 0);
+                    var r = pn(e, e === zi ? Ti : 0);
                     if (0 === r) null !== t && Ke(t), e.callbackNode = null, e.callbackPriority = 0;
                     else if (n = r & -r, e.callbackPriority !== n) {
                         if (null != t && Ke(t), 1 === n) 0 === e.tag ? function(e) {
                             Ul = !0, Vl(e)
                         }(is.bind(null, e)) : Vl(is.bind(null, e)), ol((function() {
                             0 === (6 & Pi) && $l()
                         })), t = null;
@@ -4912,29 +4912,29 @@
                     }
                 }
 
                 function ls(e, n) {
                     if (Zi = -1, Ji = 0, 0 !== (6 & Pi)) throw Error(a(327));
                     var t = e.callbackNode;
                     if (Ss() && e.callbackNode !== t) return null;
-                    var r = pn(e, e === zi ? Li : 0);
+                    var r = pn(e, e === zi ? Ti : 0);
                     if (0 === r) return null;
                     if (0 !== (30 & r) || 0 !== (r & e.expiredLanes) || n) n = vs(e, r);
                     else {
                         n = r;
                         var l = Pi;
                         Pi |= 2;
                         var o = ms();
-                        for (zi === e && Li === n || (Bi = null, $i = Ge() + 500, ds(e, n));;) try {
+                        for (zi === e && Ti === n || (Bi = null, $i = Ge() + 500, ds(e, n));;) try {
                             ys();
                             break
                         } catch (i) {
                             ps(e, i)
                         }
-                        ka(), _i.current = o, Pi = l, null !== Ti ? n = 0 : (zi = null, Li = 0, n = Mi)
+                        ka(), _i.current = o, Pi = l, null !== Li ? n = 0 : (zi = null, Ti = 0, n = Mi)
                     }
                     if (0 !== n) {
                         if (2 === n && (0 !== (l = hn(e)) && (r = l, n = as(e, l))), 1 === n) throw t = Fi, ds(e, 0), us(e, r), rs(e, Ge()), t;
                         if (6 === n) us(e, r);
                         else {
                             if (l = e.current.alternate, 0 === (30 & r) && ! function(e) {
                                     for (var n = e;;) {
@@ -5062,16 +5062,16 @@
                 function fs() {
                     Ri = Oi.current, _l(Oi)
                 }
 
                 function ds(e, n) {
                     e.finishedWork = null, e.finishedLanes = 0;
                     var t = e.timeoutHandle;
-                    if (-1 !== t && (e.timeoutHandle = -1, ll(t)), null !== Ti)
-                        for (t = Ti.return; null !== t;) {
+                    if (-1 !== t && (e.timeoutHandle = -1, ll(t)), null !== Li)
+                        for (t = Li.return; null !== t;) {
                             var r = t;
                             switch (na(r), r.tag) {
                                 case 1:
                                     null !== (r = r.type.childContextTypes) && void 0 !== r && Ol();
                                     break;
                                 case 3:
                                     lo(), _l(zl), _l(Pl), co();
@@ -5091,15 +5091,15 @@
                                     break;
                                 case 22:
                                 case 23:
                                     fs()
                             }
                             t = t.return
                         }
-                    if (zi = e, Ti = e = Os(e.current, null), Li = Ri = n, Mi = 0, Fi = null, ji = Ii = Di = 0, Ai = Ui = null, null !== Ca) {
+                    if (zi = e, Li = e = Os(e.current, null), Ti = Ri = n, Mi = 0, Fi = null, ji = Ii = Di = 0, Ai = Ui = null, null !== Ca) {
                         for (n = 0; n < Ca.length; n++)
                             if (null !== (r = (t = Ca[n]).interleaved)) {
                                 t.interleaved = null;
                                 var l = r.next,
                                     a = t.pending;
                                 if (null !== a) {
                                     var o = a.next;
@@ -5109,33 +5109,33 @@
                             } Ca = null
                     }
                     return e
                 }
 
                 function ps(e, n) {
                     for (;;) {
-                        var t = Ti;
+                        var t = Li;
                         try {
                             if (ka(), fo.current = ou, yo) {
                                 for (var r = ho.memoizedState; null !== r;) {
                                     var l = r.queue;
                                     null !== l && (l.pending = null), r = r.next
                                 }
                                 yo = !1
                             }
                             if (mo = 0, go = vo = ho = null, bo = !1, wo = 0, Ci.current = null, null === t || null === t.return) {
-                                Mi = 1, Fi = n, Ti = null;
+                                Mi = 1, Fi = n, Li = null;
                                 break
                             }
                             e: {
                                 var o = e,
                                     u = t.return,
                                     i = t,
                                     s = n;
-                                if (n = Li, i.flags |= 32768, null !== s && "object" === typeof s && "function" === typeof s.then) {
+                                if (n = Ti, i.flags |= 32768, null !== s && "object" === typeof s && "function" === typeof s.then) {
                                     var c = s,
                                         f = i,
                                         d = f.tag;
                                     if (0 === (1 & f.mode) && (0 === d || 11 === d || 15 === d)) {
                                         var p = f.alternate;
                                         p ? (f.updateQueue = p.updateQueue, f.memoizedState = p.memoizedState, f.lanes = p.lanes) : (f.updateQueue = null, f.memoizedState = null)
                                     }
@@ -5179,70 +5179,70 @@
                                             }
                                     }
                                     o = o.return
                                 } while (null !== o)
                             }
                             ws(t)
                         } catch (w) {
-                            n = w, Ti === t && null !== t && (Ti = t = t.return);
+                            n = w, Li === t && null !== t && (Li = t = t.return);
                             continue
                         }
                         break
                     }
                 }
 
                 function ms() {
                     var e = _i.current;
                     return _i.current = ou, null === e ? ou : e
                 }
 
                 function hs() {
-                    0 !== Mi && 3 !== Mi && 2 !== Mi || (Mi = 4), null === zi || 0 === (268435455 & Di) && 0 === (268435455 & Ii) || us(zi, Li)
+                    0 !== Mi && 3 !== Mi && 2 !== Mi || (Mi = 4), null === zi || 0 === (268435455 & Di) && 0 === (268435455 & Ii) || us(zi, Ti)
                 }
 
                 function vs(e, n) {
                     var t = Pi;
                     Pi |= 2;
                     var r = ms();
-                    for (zi === e && Li === n || (Bi = null, ds(e, n));;) try {
+                    for (zi === e && Ti === n || (Bi = null, ds(e, n));;) try {
                         gs();
                         break
                     } catch (l) {
                         ps(e, l)
                     }
-                    if (ka(), Pi = t, _i.current = r, null !== Ti) throw Error(a(261));
-                    return zi = null, Li = 0, Mi
+                    if (ka(), Pi = t, _i.current = r, null !== Li) throw Error(a(261));
+                    return zi = null, Ti = 0, Mi
                 }
 
                 function gs() {
-                    for (; null !== Ti;) bs(Ti)
+                    for (; null !== Li;) bs(Li)
                 }
 
                 function ys() {
-                    for (; null !== Ti && !Ye();) bs(Ti)
+                    for (; null !== Li && !Ye();) bs(Li)
                 }
 
                 function bs(e) {
                     var n = xi(e.alternate, e, Ri);
-                    e.memoizedProps = e.pendingProps, null === n ? ws(e) : Ti = n, Ci.current = null
+                    e.memoizedProps = e.pendingProps, null === n ? ws(e) : Li = n, Ci.current = null
                 }
 
                 function ws(e) {
                     var n = e;
                     do {
                         var t = n.alternate;
                         if (e = n.return, 0 === (32768 & n.flags)) {
-                            if (null !== (t = qu(t, n, Ri))) return void(Ti = t)
+                            if (null !== (t = qu(t, n, Ri))) return void(Li = t)
                         } else {
-                            if (null !== (t = Ku(t, n))) return t.flags &= 32767, void(Ti = t);
-                            if (null === e) return Mi = 6, void(Ti = null);
+                            if (null !== (t = Ku(t, n))) return t.flags &= 32767, void(Li = t);
+                            if (null === e) return Mi = 6, void(Li = null);
                             e.flags |= 32768, e.subtreeFlags = 0, e.deletions = null
                         }
-                        if (null !== (n = n.sibling)) return void(Ti = n);
-                        Ti = n = e
+                        if (null !== (n = n.sibling)) return void(Li = n);
+                        Li = n = e
                     } while (null !== n);
                     0 === Mi && (Mi = 5)
                 }
 
                 function ks(e, n, t) {
                     var r = wn,
                         l = Ni.transition;
@@ -5264,15 +5264,15 @@
                                         e.pendingLanes = n, e.suspendedLanes = 0, e.pingedLanes = 0, e.expiredLanes &= n, e.mutableReadLanes &= n, e.entangledLanes &= n, n = e.entanglements;
                                         var r = e.eventTimes;
                                         for (e = e.expirationTimes; 0 < t;) {
                                             var l = 31 - on(t),
                                                 a = 1 << l;
                                             n[l] = 0, r[l] = -1, e[l] = -1, t &= ~a
                                         }
-                                    }(e, o), e === zi && (Ti = zi = null, Li = 0), 0 === (2064 & t.subtreeFlags) && 0 === (2064 & t.flags) || qi || (qi = !0, zs(nn, (function() {
+                                    }(e, o), e === zi && (Li = zi = null, Ti = 0), 0 === (2064 & t.subtreeFlags) && 0 === (2064 & t.flags) || qi || (qi = !0, zs(nn, (function() {
                                         return Ss(), null
                                     }))), o = 0 !== (15990 & t.flags), 0 !== (15990 & t.subtreeFlags) || o) {
                                     o = Ni.transition, Ni.transition = null;
                                     var u = wn;
                                     wn = 1;
                                     var i = Pi;
                                     Pi |= 4, Ci.current = null,
@@ -5522,15 +5522,15 @@
                             }
                             n = n.return
                         }
                 }
 
                 function _s(e, n, t) {
                     var r = e.pingCache;
-                    null !== r && r.delete(n), n = es(), e.pingedLanes |= e.suspendedLanes & t, zi === e && (Li & t) === t && (4 === Mi || 3 === Mi && (130023424 & Li) === Li && 500 > Ge() - Vi ? ds(e, 0) : ji |= t), rs(e, n)
+                    null !== r && r.delete(n), n = es(), e.pingedLanes |= e.suspendedLanes & t, zi === e && (Ti & t) === t && (4 === Mi || 3 === Mi && (130023424 & Ti) === Ti && 500 > Ge() - Vi ? ds(e, 0) : ji |= t), rs(e, n)
                 }
 
                 function Cs(e, n) {
                     0 === n && (0 === (1 & e.mode) ? n = 1 : (n = fn, 0 === (130023424 & (fn <<= 1)) && (fn = 4194304)));
                     var t = es();
                     null !== (e = za(e, n)) && (yn(e, n, t), rs(e, t))
                 }
@@ -5558,29 +5558,29 @@
                     null !== r && r.delete(n), Cs(e, t)
                 }
 
                 function zs(e, n) {
                     return qe(e, n)
                 }
 
-                function Ts(e, n, t, r) {
+                function Ls(e, n, t, r) {
                     this.tag = e, this.key = t, this.sibling = this.child = this.return = this.stateNode = this.type = this.elementType = null, this.index = 0, this.ref = null, this.pendingProps = n, this.dependencies = this.memoizedState = this.updateQueue = this.memoizedProps = null, this.mode = r, this.subtreeFlags = this.flags = 0, this.deletions = null, this.childLanes = this.lanes = 0, this.alternate = null
                 }
 
-                function Ls(e, n, t, r) {
-                    return new Ts(e, n, t, r)
+                function Ts(e, n, t, r) {
+                    return new Ls(e, n, t, r)
                 }
 
                 function Rs(e) {
                     return !(!(e = e.prototype) || !e.isReactComponent)
                 }
 
                 function Os(e, n) {
                     var t = e.alternate;
-                    return null === t ? ((t = Ls(e.tag, n, e.key, e.mode)).elementType = e.elementType, t.type = e.type, t.stateNode = e.stateNode, t.alternate = e, e.alternate = t) : (t.pendingProps = n, t.type = e.type, t.flags = 0, t.subtreeFlags = 0, t.deletions = null), t.flags = 14680064 & e.flags, t.childLanes = e.childLanes, t.lanes = e.lanes, t.child = e.child, t.memoizedProps = e.memoizedProps, t.memoizedState = e.memoizedState, t.updateQueue = e.updateQueue, n = e.dependencies, t.dependencies = null === n ? null : {
+                    return null === t ? ((t = Ts(e.tag, n, e.key, e.mode)).elementType = e.elementType, t.type = e.type, t.stateNode = e.stateNode, t.alternate = e, e.alternate = t) : (t.pendingProps = n, t.type = e.type, t.flags = 0, t.subtreeFlags = 0, t.deletions = null), t.flags = 14680064 & e.flags, t.childLanes = e.childLanes, t.lanes = e.lanes, t.child = e.child, t.memoizedProps = e.memoizedProps, t.memoizedState = e.memoizedState, t.updateQueue = e.updateQueue, n = e.dependencies, t.dependencies = null === n ? null : {
                         lanes: n.lanes,
                         firstContext: n.firstContext
                     }, t.sibling = e.sibling, t.index = e.index, t.ref = e.ref, t
                 }
 
                 function Ms(e, n, t, r, l, o) {
                     var u = 2;
@@ -5589,78 +5589,78 @@
                     else e: switch (e) {
                         case x:
                             return Fs(t.children, l, o, n);
                         case E:
                             u = 8, l |= 8;
                             break;
                         case _:
-                            return (e = Ls(12, t, n, 2 | l)).elementType = _, e.lanes = o, e;
+                            return (e = Ts(12, t, n, 2 | l)).elementType = _, e.lanes = o, e;
                         case z:
-                            return (e = Ls(13, t, n, l)).elementType = z, e.lanes = o, e;
-                        case T:
-                            return (e = Ls(19, t, n, l)).elementType = T, e.lanes = o, e;
+                            return (e = Ts(13, t, n, l)).elementType = z, e.lanes = o, e;
+                        case L:
+                            return (e = Ts(19, t, n, l)).elementType = L, e.lanes = o, e;
                         case O:
                             return Ds(t, l, o, n);
                         default:
                             if ("object" === typeof e && null !== e) switch (e.$$typeof) {
                                 case C:
                                     u = 10;
                                     break e;
                                 case N:
                                     u = 9;
                                     break e;
                                 case P:
                                     u = 11;
                                     break e;
-                                case L:
+                                case T:
                                     u = 14;
                                     break e;
                                 case R:
                                     u = 16, r = null;
                                     break e
                             }
                             throw Error(a(130, null == e ? e : typeof e, ""))
                     }
-                    return (n = Ls(u, t, n, l)).elementType = e, n.type = r, n.lanes = o, n
+                    return (n = Ts(u, t, n, l)).elementType = e, n.type = r, n.lanes = o, n
                 }
 
                 function Fs(e, n, t, r) {
-                    return (e = Ls(7, e, r, n)).lanes = t, e
+                    return (e = Ts(7, e, r, n)).lanes = t, e
                 }
 
                 function Ds(e, n, t, r) {
-                    return (e = Ls(22, e, r, n)).elementType = O, e.lanes = t, e.stateNode = {
+                    return (e = Ts(22, e, r, n)).elementType = O, e.lanes = t, e.stateNode = {
                         isHidden: !1
                     }, e
                 }
 
                 function Is(e, n, t) {
-                    return (e = Ls(6, e, null, n)).lanes = t, e
+                    return (e = Ts(6, e, null, n)).lanes = t, e
                 }
 
                 function js(e, n, t) {
-                    return (n = Ls(4, null !== e.children ? e.children : [], e.key, n)).lanes = t, n.stateNode = {
+                    return (n = Ts(4, null !== e.children ? e.children : [], e.key, n)).lanes = t, n.stateNode = {
                         containerInfo: e.containerInfo,
                         pendingChildren: null,
                         implementation: e.implementation
                     }, n
                 }
 
                 function Us(e, n, t, r, l) {
                     this.tag = n, this.containerInfo = e, this.finishedWork = this.pingCache = this.current = this.pendingChildren = null, this.timeoutHandle = -1, this.callbackNode = this.pendingContext = this.context = null, this.callbackPriority = 0, this.eventTimes = gn(0), this.expirationTimes = gn(-1), this.entangledLanes = this.finishedLanes = this.mutableReadLanes = this.expiredLanes = this.pingedLanes = this.suspendedLanes = this.pendingLanes = 0, this.entanglements = gn(0), this.identifierPrefix = r, this.onRecoverableError = l, this.mutableSourceEagerHydrationData = null
                 }
 
                 function As(e, n, t, r, l, a, o, u, i) {
-                    return e = new Us(e, n, t, u, i), 1 === n ? (n = 1, !0 === a && (n |= 8)) : n = 0, a = Ls(3, null, null, n), e.current = a, a.stateNode = e, a.memoizedState = {
+                    return e = new Us(e, n, t, u, i), 1 === n ? (n = 1, !0 === a && (n |= 8)) : n = 0, a = Ts(3, null, null, n), e.current = a, a.stateNode = e, a.memoizedState = {
                         element: r,
                         isDehydrated: t,
                         cache: null,
                         transitions: null,
                         pendingSuspenseBoundaries: null
-                    }, La(a), e
+                    }, Ta(a), e
                 }
 
                 function Vs(e, n, t) {
                     var r = 3 < arguments.length && void 0 !== arguments[3] ? arguments[3] : null;
                     return {
                         $$typeof: S,
                         key: null == r ? null : "" + r,
@@ -5727,15 +5727,15 @@
                     if (null !== e)
                         if (e.memoizedProps !== n.pendingProps || zl.current) wu = !0;
                         else {
                             if (0 === (e.lanes & t) && 0 === (128 & n.flags)) return wu = !1,
                                 function(e, n, t) {
                                     switch (n.tag) {
                                         case 3:
-                                            Tu(n), pa();
+                                            Lu(n), pa();
                                             break;
                                         case 5:
                                             ao(n);
                                             break;
                                         case 1:
                                             Rl(n.type) && Dl(n);
                                             break;
@@ -5767,26 +5767,26 @@
                             wu = 0 !== (131072 & e.flags)
                         }
                     else wu = !1, la && 0 !== (1048576 & n.flags) && Jl(n, Ql, n.index);
                     switch (n.lanes = 0, n.tag) {
                         case 2:
                             var r = n.type;
                             Bu(e, n), e = n.pendingProps;
-                            var l = Ll(n, Pl.current);
+                            var l = Tl(n, Pl.current);
                             Ea(n, t), l = Eo(null, n, r, e, l, t);
                             var o = _o();
-                            return n.flags |= 1, "object" === typeof l && null !== l && "function" === typeof l.render && void 0 === l.$$typeof ? (n.tag = 1, n.memoizedState = null, n.updateQueue = null, Rl(r) ? (o = !0, Dl(n)) : o = !1, n.memoizedState = null !== l.state && void 0 !== l.state ? l.state : null, La(n), l.updater = Va, n.stateNode = l, l._reactInternals = n, Wa(n, r, e, t), n = zu(null, n, r, !0, o, t)) : (n.tag = 0, la && o && ea(n), ku(null, n, l, t), n = n.child), n;
+                            return n.flags |= 1, "object" === typeof l && null !== l && "function" === typeof l.render && void 0 === l.$$typeof ? (n.tag = 1, n.memoizedState = null, n.updateQueue = null, Rl(r) ? (o = !0, Dl(n)) : o = !1, n.memoizedState = null !== l.state && void 0 !== l.state ? l.state : null, Ta(n), l.updater = Va, n.stateNode = l, l._reactInternals = n, Wa(n, r, e, t), n = zu(null, n, r, !0, o, t)) : (n.tag = 0, la && o && ea(n), ku(null, n, l, t), n = n.child), n;
                         case 16:
                             r = n.elementType;
                             e: {
                                 switch (Bu(e, n), e = n.pendingProps, r = (l = r._init)(r._payload), n.type = r, l = n.tag = function(e) {
                                         if ("function" === typeof e) return Rs(e) ? 1 : 0;
                                         if (void 0 !== e && null !== e) {
                                             if ((e = e.$$typeof) === P) return 11;
-                                            if (e === L) return 14
+                                            if (e === T) return 14
                                         }
                                         return 2
                                     }(r), e = va(r, e), l) {
                                     case 0:
                                         n = Nu(null, n, r, e, t);
                                         break e;
                                     case 1:
@@ -5804,32 +5804,32 @@
                             return n;
                         case 0:
                             return r = n.type, l = n.pendingProps, Nu(e, n, r, l = n.elementType === r ? l : va(r, l), t);
                         case 1:
                             return r = n.type, l = n.pendingProps, Pu(e, n, r, l = n.elementType === r ? l : va(r, l), t);
                         case 3:
                             e: {
-                                if (Tu(n), null === e) throw Error(a(387));r = n.pendingProps,
+                                if (Lu(n), null === e) throw Error(a(387));r = n.pendingProps,
                                 l = (o = n.memoizedState).element,
                                 Ra(e, n),
                                 Ia(n, r, null, t);
                                 var u = n.memoizedState;
                                 if (r = u.element, o.isDehydrated) {
                                     if (o = {
                                             element: r,
                                             isDehydrated: !1,
                                             cache: u.cache,
                                             pendingSuspenseBoundaries: u.pendingSuspenseBoundaries,
                                             transitions: u.transitions
                                         }, n.updateQueue.baseState = o, n.memoizedState = o, 256 & n.flags) {
-                                        n = Lu(e, n, r, t, l = cu(Error(a(423)), n));
+                                        n = Tu(e, n, r, t, l = cu(Error(a(423)), n));
                                         break e
                                     }
                                     if (r !== l) {
-                                        n = Lu(e, n, r, t, l = cu(Error(a(424)), n));
+                                        n = Tu(e, n, r, t, l = cu(Error(a(424)), n));
                                         break e
                                     }
                                     for (ra = sl(n.stateNode.containerInfo.firstChild), ta = n, la = !0, aa = null, t = Ga(n, null, r, t), n.child = t; t;) t.flags = -3 & t.flags | 4096, t = t.sibling
                                 } else {
                                     if (pa(), r === l) {
                                         n = Hu(e, n, t);
                                         break e
@@ -6157,29 +6157,29 @@
                     })), !0)
                 }, n.unstable_batchedUpdates = ss, n.unstable_renderSubtreeIntoContainer = function(e, n, t, r) {
                     if (!Zs(t)) throw Error(a(200));
                     if (null == e || void 0 === e._reactInternals) throw Error(a(38));
                     return ec(e, n, t, !1, r)
                 }, n.version = "18.2.0-next-9e3b772b8-20220608"
             },
-            250: function(e, n, t) {
-                var r = t(164);
+            739: function(e, n, t) {
+                var r = t(168);
                 n.createRoot = r.createRoot, n.hydrateRoot = r.hydrateRoot
             },
-            164: function(e, n, t) {
+            168: function(e, n, t) {
                 ! function e() {
                     if ("undefined" !== typeof __REACT_DEVTOOLS_GLOBAL_HOOK__ && "function" === typeof __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE) try {
                         __REACT_DEVTOOLS_GLOBAL_HOOK__.checkDCE(e)
                     } catch (n) {
                         console.error(n)
                     }
-                }(), e.exports = t(463)
+                }(), e.exports = t(534)
             },
-            374: function(e, n, t) {
-                var r = t(791),
+            918: function(e, n, t) {
+                var r = t(313),
                     l = Symbol.for("react.element"),
                     a = Symbol.for("react.fragment"),
                     o = Object.prototype.hasOwnProperty,
                     u = r.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED.ReactCurrentOwner,
                     i = {
                         key: !0,
                         ref: !0,
@@ -6201,15 +6201,15 @@
                         ref: c,
                         props: a,
                         _owner: u.current
                     }
                 }
                 n.Fragment = a, n.jsx = s, n.jsxs = s
             },
-            117: function(e, n) {
+            306: function(e, n) {
                 var t = Symbol.for("react.element"),
                     r = Symbol.for("react.portal"),
                     l = Symbol.for("react.fragment"),
                     a = Symbol.for("react.strict_mode"),
                     o = Symbol.for("react.profiler"),
                     u = Symbol.for("react.provider"),
                     i = Symbol.for("react.context"),
@@ -6336,24 +6336,24 @@
                                 return null === e || "object" !== typeof e ? null : "function" === typeof(e = p && e[p] || e["@@iterator"]) ? e : null
                             }(e), "function" === typeof c)
                             for (e = c.call(e), s = 0; !(u = e.next()).done;) i += z(u = u.value, n, l, c = a + P(u, s++), o);
                         else if ("object" === u) throw n = String(e), Error("Objects are not valid as a React child (found: " + ("[object Object]" === n ? "object with keys {" + Object.keys(e).join(", ") + "}" : n) + "). If you meant to render a collection of children, use an array instead.");
                     return i
                 }
 
-                function T(e, n, t) {
+                function L(e, n, t) {
                     if (null == e) return e;
                     var r = [],
                         l = 0;
                     return z(e, r, "", "", (function(e) {
                         return n.call(t, e, l++)
                     })), r
                 }
 
-                function L(e) {
+                function T(e) {
                     if (-1 === e._status) {
                         var n = e._result;
                         (n = n()).then((function(n) {
                             0 !== e._status && -1 !== e._status || (e._status = 1, e._result = n)
                         }), (function(n) {
                             0 !== e._status && -1 !== e._status || (e._status = 2, e._result = n)
                         })), -1 === e._status && (e._status = 0, e._result = n)
@@ -6369,28 +6369,28 @@
                     },
                     M = {
                         ReactCurrentDispatcher: R,
                         ReactCurrentBatchConfig: O,
                         ReactCurrentOwner: x
                     };
                 n.Children = {
-                    map: T,
+                    map: L,
                     forEach: function(e, n, t) {
-                        T(e, (function() {
+                        L(e, (function() {
                             n.apply(this, arguments)
                         }), t)
                     },
                     count: function(e) {
                         var n = 0;
-                        return T(e, (function() {
+                        return L(e, (function() {
                             n++
                         })), n
                     },
                     toArray: function(e) {
-                        return T(e, (function(e) {
+                        return L(e, (function(e) {
                             return e
                         })) || []
                     },
                     only: function(e) {
                         if (!C(e)) throw Error("React.Children.only expected to receive a single React element child.");
                         return e
                     }
@@ -6448,15 +6448,15 @@
                 }, n.isValidElement = C, n.lazy = function(e) {
                     return {
                         $$typeof: d,
                         _payload: {
                             _status: -1,
                             _result: e
                         },
-                        _init: L
+                        _init: T
                     }
                 }, n.memo = function(e, n) {
                     return {
                         $$typeof: f,
                         type: e,
                         compare: void 0 === n ? null : n
                     }
@@ -6496,21 +6496,21 @@
                     return R.current.useState(e)
                 }, n.useSyncExternalStore = function(e, n, t) {
                     return R.current.useSyncExternalStore(e, n, t)
                 }, n.useTransition = function() {
                     return R.current.useTransition()
                 }, n.version = "18.2.0"
             },
-            791: function(e, n, t) {
-                e.exports = t(117)
+            313: function(e, n, t) {
+                e.exports = t(306)
             },
-            184: function(e, n, t) {
-                e.exports = t(374)
+            417: function(e, n, t) {
+                e.exports = t(918)
             },
-            813: function(e, n) {
+            95: function(e, n) {
                 function t(e, n) {
                     var t = e.length;
                     e.push(n);
                     e: for (; 0 < t;) {
                         var r = t - 1 >>> 1,
                             l = e[r];
                         if (!(0 < a(l, n))) break e;
@@ -6621,37 +6621,37 @@
                     N = 5,
                     P = -1;
 
                 function z() {
                     return !(n.unstable_now() - P < N)
                 }
 
-                function T() {
+                function L() {
                     if (null !== _) {
                         var e = n.unstable_now();
                         P = e;
                         var t = !0;
                         try {
                             t = _(!0, e)
                         } finally {
                             t ? x() : (E = !1, _ = null)
                         }
                     } else E = !1
                 }
                 if ("function" === typeof b) x = function() {
-                    b(T)
+                    b(L)
                 };
                 else if ("undefined" !== typeof MessageChannel) {
-                    var L = new MessageChannel,
-                        R = L.port2;
-                    L.port1.onmessage = T, x = function() {
+                    var T = new MessageChannel,
+                        R = T.port2;
+                    T.port1.onmessage = L, x = function() {
                         R.postMessage(null)
                     }
                 } else x = function() {
-                    g(T, 0)
+                    g(L, 0)
                 };
 
                 function O(e) {
                     _ = e, E || (E = !0, x())
                 }
 
                 function M(e, t) {
@@ -6739,30 +6739,30 @@
                             return e.apply(this, arguments)
                         } finally {
                             p = t
                         }
                     }
                 }
             },
-            296: function(e, n, t) {
-                e.exports = t(813)
+            224: function(e, n, t) {
+                e.exports = t(95)
             }
         },
         n = {};
 
     function t(r) {
         var l = n[r];
         if (void 0 !== l) return l.exports;
         var a = n[r] = {
             exports: {}
         };
         return e[r](a, a.exports, t), a.exports
     }! function() {
-        var e = t(791),
-            n = t(250);
+        var e = t(313),
+            n = t(739);
 
         function r(e, n) {
             (null == n || n > e.length) && (n = e.length);
             for (var t = 0, r = new Array(n); t < n; t++) r[t] = e[t];
             return r
         }
 
@@ -6858,15 +6858,15 @@
                     if (e) return function() {
                         l(e)
                     }
                 }), [])
             } : function(e, n) {
                 void 0 === e && (e = !0)
             },
-            p = t(184),
+            p = t(417),
             m = function(e) {
                 var n = e.children;
                 return (0, p.jsx)("span", {
                     className: "text-indigo-400 font-mono",
                     children: n
                 })
             },
@@ -6894,15 +6894,15 @@
                     "data-testid": "error-box",
                     children: [(0, p.jsx)("p", {
                         children: t
                     }), (0, p.jsxs)("p", {
                         className: "text-zinc-400 font-mono break-words",
                         children: [r, ":", l]
                     }), (0, p.jsx)("ul", {
-                        className: "mt-4 p-4 bg-zinc-800 text-zinc-200",
+                        className: "mt-4 p-4 bg-zinc-800 text-zinc-200 break-words",
                         children: a.map((function(e, n) {
                             return (0, p.jsxs)("li", {
                                 children: ["invalid" === e.error && (0, p.jsxs)("span", {
                                     children: ["Invalid prop ", (0, p.jsx)(m, {
                                         children: e.name
                                     }), " set on", " ", (0, p.jsx)(h, {
                                         children: t
@@ -6929,57 +6929,68 @@
                                     }), "."]
                                 })]
                             }, n)
                         }))
                     })]
                 })
             },
-            y = function(n) {
-                var t = n.errors,
-                    r = l((0, e.useState)(!1), 2),
-                    a = r[0],
-                    o = r[1];
-                return (0, e.useEffect)((function() {
-                    t.length > 0 && o(!0)
-                }), [t.length]), d(a), (0, p.jsx)(p.Fragment, {
-                    children: a && (0, p.jsx)("div", {
-                        className: "fixed inset-0 bg-black/90 text-white p-12 overflow-auto",
-                        children: (0, p.jsxs)("div", {
-                            className: "flex flex-col",
-                            children: [(0, p.jsxs)("div", {
-                                className: "flex items-start",
-                                children: [(0, p.jsx)("h1", {
-                                    className: "text-2xl text-red-400 mb-8",
-                                    children: "Slippers: Failed prop types"
-                                }), (0, p.jsx)("button", {
-                                    className: "ml-auto px-4 py-2 bg-black",
-                                    onClick: function() {
-                                        return o(!1)
-                                    },
-                                    children: "Close"
-                                })]
-                            }), (0, p.jsx)("div", {
-                                className: "space-y-8",
-                                children: t.map((function(e, n) {
-                                    return (0, p.jsx)(g, {
-                                        error: e
-                                    }, n)
-                                }))
+            y = function(e) {
+                var n = e.errors,
+                    t = e.setShowModal;
+                return (0, p.jsx)("div", {
+                    className: "fixed inset-0 bg-black/90 text-white p-4 md:p-12 overflow-auto",
+                    children: (0, p.jsxs)("div", {
+                        className: "flex flex-col",
+                        children: [(0, p.jsxs)("div", {
+                            className: "flex items-start",
+                            children: [(0, p.jsx)("h1", {
+                                className: "text-2xl text-red-400 mb-8",
+                                children: "Slippers: Failed prop types"
+                            }), (0, p.jsx)("button", {
+                                className: "ml-auto px-4 py-2 bg-black",
+                                onClick: function() {
+                                    return t(!1)
+                                },
+                                children: "Close"
                             })]
-                        })
+                        }), (0, p.jsx)("div", {
+                            className: "space-y-8",
+                            children: n.map((function(e, n) {
+                                return (0, p.jsx)(g, {
+                                    error: e
+                                }, n)
+                            }))
+                        })]
                     })
                 })
             };
-        var b = function(e) {
-            var n = e.errors;
-            return (0, p.jsx)(y, {
-                errors: n
+        var b = function(n) {
+            var t = n.errors,
+                r = l((0, e.useState)(!1), 2),
+                a = r[0],
+                o = r[1];
+            return (0, e.useEffect)((function() {
+                t.length > 0 && o(!0)
+            }), [t.length]), d(a), (0, p.jsx)(p.Fragment, {
+                children: a && (0, p.jsx)(y, {
+                    errors: t,
+                    setShowModal: o
+                })
             })
         };
-        n.createRoot(document.getElementById("slippers_errors_ui_root")).render((0, p.jsx)(e.StrictMode, {
-            children: (0, p.jsx)(b, {
-                errors: window.slippersPropErrors || []
-            })
+        document.addEventListener("DOMContentLoaded", (function() {
+            var t, r = window.slippersPropErrors || [],
+                l = JSON.parse((null === (t = document.getElementById("slippers_type_checking_output")) || void 0 === t ? void 0 : t.textContent) || "[]");
+            r.length > 0 && (l.includes("console") && function(e) {
+                console.group("Slippers: Failed prop types"), e.forEach((function(e) {
+                    console.groupCollapsed("".concat(e.tag_name, " in ").concat(e.template_name, ":").concat(e.lineno)), e.errors.forEach((function(n) {
+                        "invalid" === n.error ? console.error("Invalid prop ".concat(n.name, " set on ").concat(e.tag_name, ". Expected ").concat(n.expected, ", got ").concat(n.actual, ".")) : "missing" === n.error ? console.error("Required prop ".concat(n.name, " of type ").concat(n.expected, " not set on ").concat(e.tag_name, ".")) : "extra" === n.error && console.error("Extra prop ".concat(n.name, " of type ").concat(n.actual, " set on ").concat(e.tag_name, "."))
+                    })), console.groupEnd()
+                })), console.groupEnd()
+            }(r), l.includes("overlay") && n.createRoot(document.getElementById("slippers_errors_ui_root")).render((0, p.jsx)(e.StrictMode, {
+                children: (0, p.jsx)(b, {
+                    errors: r
+                })
+            })))
         }))
     }()
-}();
-//# sourceMappingURL=main.js.map
+}();
```

### Comparing `slippers-0.6.0a0/slippers/template.py` & `slippers-0.6.1a0/slippers/template.py`

 * *Files identical despite different names*

### Comparing `slippers-0.6.0a0/slippers/templatetags/slippers.py` & `slippers-0.6.1a0/slippers/templatetags/slippers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from django import template
 from django.conf import settings as django_settings
 from django.template import Context
 from django.utils.safestring import mark_safe
 
 from slippers.conf import settings
-from slippers.props import Props, check_prop_types, print_errors, render_error_html
+from slippers.props import Props, check_prop_types, render_error_html
 from slippers.template import slippers_token_kwargs
 
 register = template.Library()
 
 
 ##
 # Component tags
@@ -112,33 +112,28 @@
             if settings.SLIPPERS_RUNTIME_TYPE_CHECKING:
                 prop_errors = check_prop_types(
                     attributes=attributes,
                     types=props.types,
                     defaults=props.defaults,
                 )
 
-            if "shell" in settings.SLIPPERS_TYPE_CHECKING_OUTPUT and prop_errors:
-                print_errors(
-                    errors=prop_errors,
-                    tag_name=self.tag_name,
-                    template_name=self.origin_template_name,
-                    lineno=self.origin_lineno,
-                )
-
             # Load prop defaults into props
             attributes = {**props}
 
         # Stage 2: Render template
         raw_output = template.render(
             Context({**attributes, "children": children}, autoescape=context.autoescape)
         )
 
         output_template_section = mark_safe(extract_template_parts(raw_output)[1])
 
-        if "browser_console" in settings.SLIPPERS_TYPE_CHECKING_OUTPUT and prop_errors:
+        if prop_errors and (
+            "console" in settings.SLIPPERS_TYPE_CHECKING_OUTPUT
+            or "overlay" in settings.SLIPPERS_TYPE_CHECKING_OUTPUT
+        ):
             # Append prop errors to output
             output = output_template_section + render_error_html(  # type: ignore
                 errors=prop_errors,
                 tag_name=self.tag_name,
                 template_name=self.origin_template_name,
                 lineno=self.origin_lineno,
             )
@@ -292,10 +287,13 @@
         return ""
 
     return FragmentNode(nodelist, target_var)
 
 
 ##
 # slippers errors UI
-@register.inclusion_tag("slippers/errors.html")
-def slippers_errors():
-    return
+@register.inclusion_tag("slippers/overlay.html")
+def slippers_overlay():
+    return {
+        "SLIPPERS_RUNTIME_TYPE_CHECKING": settings.SLIPPERS_RUNTIME_TYPE_CHECKING,
+        "SLIPPERS_TYPE_CHECKING_OUTPUT": settings.SLIPPERS_TYPE_CHECKING_OUTPUT,
+    }
```

### Comparing `slippers-0.6.0a0/PKG-INFO` & `slippers-0.6.1a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: slippers
-Version: 0.6.0a0
+Version: 0.6.1a0
 Summary: Build reusable components in Django without writing a single line of Python.
 Home-page: https://github.com/mixxorz/slippers
 License: MIT
 Keywords: django,components
 Author: Mitchel Cabuloy
 Author-email: mixxorz@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.7.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=3.2,<4.2)
-Requires-Dist: PyYAML (>=5.4.0,<7.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: Django (>=3.2)
+Requires-Dist: PyYAML (>=5.4.0)
 Requires-Dist: typeguard (>=2.13.3,<3.0.0)
-Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.4.0)
 Project-URL: Repository, https://github.com/mixxorz/slippers
 Description-Content-Type: text/markdown
 
 [![Slippers](https://mitchel.me/slippers/img/slippers.svg)](https://github.com/mixxorz/slippers)
 
 ---
```

