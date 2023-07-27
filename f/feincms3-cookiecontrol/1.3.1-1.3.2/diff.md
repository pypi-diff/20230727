# Comparing `tmp/feincms3_cookiecontrol-1.3.1.tar.gz` & `tmp/feincms3_cookiecontrol-1.3.2.tar.gz`

## Comparing `feincms3_cookiecontrol-1.3.1.tar` & `feincms3_cookiecontrol-1.3.2.tar`

### file list

```diff
@@ -1,49 +1,28 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.editorconfig
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.eslintrc.js
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     7880 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/esbuild.js
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/main.css
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/main.js
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tox.ini
--rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/yarn.lock
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0    45516 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/docs/banner.png
--rwxr-xr-x   0        0        0    41563 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/docs/embed.png
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/admin.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/apps.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/embedding.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/models.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/views.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/migrations/0001_rework.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/migrations/__init__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/static/f3cc.js
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templatetags/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
--rwxr-xr-x   0        0        0      349 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/settings.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/test_cookiecontrol.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/test_embed.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/tests/testapp/urls.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/LICENSE
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/README.rst
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/admin.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/apps.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/embedding.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/models.py
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/views.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/migrations/0001_rework.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/migrations/__init__.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/static/f3cc.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/templatetags/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/LICENSE
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/README.rst
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.3.2/PKG-INFO
```

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/embedding.py` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/models.py` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/models.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/views.py` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/views.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/migrations/0001_rework.py` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/migrations/0001_rework.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/static/f3cc.js` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/static/f3cc.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,29 @@
 (() => {
     (function() {
         var e = document.createElement("style");
         e.textContent = ".f3cc{font-size:16px;line-height:1.3;--_b:var(--f3cc-background,#e9e9e9);--_f:var(--f3cc-foreground,#000000);--_B:var(--f3cc-button-background,#cbcbcb);--_A:var(--f3cc-accept-background,#90f690);--_F:var(--f3cc-button-foreground,var(--_f));--_E:var(--f3cc-accept-foreground,var(--_F));}.f3cc .f3cc-banner{position:fixed;bottom:0;width:100%;background:var(--_b);color:var(--_f);z-index:2000;padding:1rem 1rem 1.25rem;}.f3cc .f3cc-embed{background:var(--_b);color:var(--_f);padding:4rem;}.f3cc .f3cc-container{display:flex;gap:2rem;max-width:70em;margin:0 auto;width:80%;}@media (max-width:60rem){.f3cc .f3cc-container{width:100%;flex-direction:column;}}.f3cc .f3cc-title{font-size:1.5em;font-weight:bold;margin-bottom:0.25em;}.f3cc .f3cc-description a{color:inherit;text-decoration:underline;}.f3cc .f3cc-description a:hover{opacity:0.7;}.f3cc .f3cc-buttons{display:flex;flex-direction:column;gap:1rem;justify-content:center;align-items:stretch;}.f3cc .f3cc-button{display:inline-block;background:var(--_B);color:var(--_F);padding:0.8rem 1.2rem;white-space:nowrap;text-decoration:none;text-align:center;cursor:pointer;border:none;}.f3cc .f3cc-button:hover{opacity:0.7;}.f3cc .f3cc-button.accept{background:var(--_A);color:var(--_E);}.f3cc .f3cc-button.modify{position:fixed;z-index:2000;bottom:1rem;right:1rem;}.f3cc-embed .f3cc-description{margin-bottom:1em;}", document.head.appendChild(e)
     })();
     var b = (e, t = document) => t.querySelector(e),
-        w = document.body,
+        x = document.body,
         r = "className",
         s = "textContent",
-        x = "f3cc",
+        _ = "f3cc",
         i = window.f3ccData || JSON.parse(b("#f3cc-data")[s]),
-        k = {},
+        w = {},
         m = "f3cc-embed-providers",
         p, f, l, o = (e, t = null, c = []) => {
             let n = document.createElement(e);
             if (t)
                 for (let [a, d] of Object.entries(t)) a.startsWith("data-") ? n.setAttribute(a, d) : n[a] = d;
             return n.append(...c), n
         },
         u = () => {
             if (f) {
-                N(f);
+                R(f);
                 return
             }
             let e = [o("div", {
                 [r]: "f3cc-title",
                 [s]: i.heading
             }), o("div", {
                 [r]: "f3cc-description",
@@ -32,33 +32,33 @@
             i.privacyPolicyURL && e[1].append(o("br"), o("a", {
                 [s]: i.privacyPolicyTitle,
                 href: i.privacyPolicyURL
             }));
             let t = [o("a", {
                 [r]: "f3cc-button accept",
                 [s]: i.buttonAccept,
-                onclick: D
+                onclick: P
             }), o("a", {
                 [r]: "f3cc-button reject",
                 [s]: i.buttonReject,
-                onclick: P
+                onclick: T
             })];
             f = o("div", {
                 [r]: "f3cc f3cc-banner"
             }, [o("div", {
                 [r]: "f3cc-container"
             }, [o("div", {
                 [r]: "f3cc-content"
             }, e), o("div", {
                 [r]: "f3cc-buttons"
-            }, t)])]), p.append(f)
+            }, t)])]), y().append(f)
         },
         v = () => {
             if (l) {
-                N(l);
+                R(l);
                 return
             }
             let e;
             if (e = b(".f3cc-modify")) {
                 e.addEventListener("click", n => {
                     n.preventDefault(), u()
                 });
@@ -68,108 +68,109 @@
                 c = window.location;
             i.buttonModify && (!t || t == `${c.protocol}//${c.host}${c.pathname}`) && (l = o("a", {
                 [r]: "f3cc-button modify",
                 [s]: i.buttonModify,
                 onclick: n => {
                     n.preventDefault(), h(l), u()
                 }
-            }), p.append(l))
+            }), y().append(l))
         },
-        _ = e => {
-            let t = `${x}=${e};max-age=31536000;path=/;sameSite=Strict`;
+        C = e => {
+            let t = `${_}=${e};max-age=31536000;path=/;sameSite=Strict`;
             i.domain && (t += `;domain=${i.domain}`), document.cookie = t
         },
-        C = () => {
-            let e = `${x}=`;
+        S = () => {
+            let e = `${_}=`;
             for (let t of document.cookie.split("; "))
                 if (t.startsWith(e)) return decodeURIComponent(t.substring(e.length))
         },
         g = "all",
-        S = "essential",
-        $ = () => {
-            let e = C();
-            return g == e || S == e
+        E = "essential",
+        D = () => {
+            let e = S();
+            return g == e || E == e
         },
-        E = () => C() === g,
-        N = e => {
+        N = () => S() === g,
+        R = e => {
             e.style.display = ""
         },
         h = e => {
             e && (e.style.display = "none")
         },
-        D = e => {
-            e.preventDefault(), _(g), h(f), v(), A(), y()
-        },
         P = e => {
-            e.preventDefault(), _(S), h(f), v()
+            e.preventDefault(), C(g), h(f), v(), A(), k()
+        },
+        T = e => {
+            e.preventDefault(), C(E), h(f), v()
         },
         A = () => {
             for (let e of i.cookies) {
-                let t = k[e.name];
-                t || (k[e.name] = t = o("div"), t.dataset.name = e.name, p.append(t)), t.innerHTML = e.script, j(t)
+                let t = w[e.name];
+                t || (w[e.name] = t = o("div"), t.dataset.name = e.name, y().append(t)), t.innerHTML = e.script, $(t)
             }
         },
-        T = () => {
-            p = o("div", {
-                [r]: "f3cc"
-            }), w.append(p), E() && A(), $() ? v() : u()
+        y = () => (p || (p = o("div", {
+            [r]: "f3cc"
+        }), x.append(p)), p),
+        I = () => {
+            N() && A(), D() ? v() : u()
         },
-        R = {},
-        I = (e, t) => {
+        L = {},
+        M = (e, t) => {
             try {
                 window.localStorage.setItem(e, JSON.stringify(t))
             } catch {
-                R[e] = t
+                L[e] = t
             }
         },
-        L = e => {
+        j = e => {
             try {
                 return JSON.parse(window.localStorage.getItem(e))
             } catch {
-                return R[e]
+                return L[e]
             }
         },
-        y = window.f3ccRenderEmbeds = () => {
-            let e = L(m) || [];
+        k = window.f3ccRenderEmbeds = () => {
+            let e = j(m) || [];
             document.querySelectorAll(".f3cc-embed").forEach(c => {
                 let n = b("template", c),
                     a = c.dataset.provider;
-                if (n && a && (E() || e.some(d => d === a))) {
+                if (n && a && (N() || e.some(d => d === a))) {
                     let d = n.content.cloneNode(!0);
                     c.closest(".f3cc").replaceWith(d)
                 }
             })
         },
-        M = () => {
-            w.addEventListener("click", e => {
+        z = () => {
+            x.addEventListener("click", e => {
                 let t = e.target.closest(".f3cc-button"),
                     c = t && t.closest(".f3cc-embed");
                 if (t && c) {
                     e.preventDefault();
-                    let n = L(m) || [];
-                    n.push(c.dataset.provider), I(m, n), y()
+                    let n = j(m) || [];
+                    n.push(c.dataset.provider), M(m, n), k()
                 }
             })
         },
-        j = e => {
-            if (B(e) === !0) e.parentNode.replaceChild(z(e), e);
+        $ = e => {
+            if (F(e) === !0) e.parentNode.replaceChild(B(e), e);
             else {
                 let t = -1,
                     c = e.childNodes;
-                for (; ++t < c.length;) j(c[t])
+                for (; ++t < c.length;) $(c[t])
             }
             return e
         },
-        z = e => {
+        B = e => {
             let t = o("script");
             t.text = e.innerHTML;
             let c = -1,
                 n = e.attributes,
                 a;
             for (; ++c < n.length;) t.setAttribute((a = n[c]).name, a.value);
             return t
         },
-        B = e => e.tagName === "SCRIPT";
-    T();
-    y();
-    M();
+        F = e => e.tagName === "SCRIPT";
+    I();
+    k();
+    z();
 })();
```

### Comparing `feincms3_cookiecontrol-1.3.1/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py` & `feincms3_cookiecontrol-1.3.2/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/LICENSE` & `feincms3_cookiecontrol-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/README.rst` & `feincms3_cookiecontrol-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.3.1/pyproject.toml` & `feincms3_cookiecontrol-1.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     "coverage",
     "requests",
 ]
 
 [project.urls]
 Homepage = "https://github.com/feinheit/feincms3-cookiecontrol/"
 
+[tool.hatch.build]
+include = ["feincms3_cookiecontrol/"]
+
 [tool.hatch.version]
 path = "feincms3_cookiecontrol/__init__.py"
 
 [tool.ruff]
 extend-select = [
   # pyflakes, pycodestyle
   "F", "E", "W",
```

### Comparing `feincms3_cookiecontrol-1.3.1/PKG-INFO` & `feincms3_cookiecontrol-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feincms3-cookiecontrol
-Version: 1.3.1
+Version: 1.3.2
 Summary: Cookie Control Panel for GDPR compliant feincms3 websites
 Project-URL: Homepage, https://github.com/feinheit/feincms3-cookiecontrol/
 Author-email: York Schickl <ys@feinheit.ch>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

