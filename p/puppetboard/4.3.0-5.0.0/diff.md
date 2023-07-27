# Comparing `tmp/puppetboard-4.3.0.tar.gz` & `tmp/puppetboard-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puppetboard-4.3.0.tar", last modified: Tue Apr  4 17:27:39 2023, max compression
+gzip compressed data, was "puppetboard-5.0.0.tar", last modified: Thu Jul 27 11:45:46 2023, max compression
```

## Comparing `puppetboard-4.3.0.tar` & `puppetboard-5.0.0.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.244805 puppetboard-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    22743 2023-04-04 17:27:35.000000 puppetboard-4.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-04 17:27:35.000000 puppetboard-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-04 17:27:35.000000 puppetboard-4.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    42500 2023-04-04 17:27:39.244805 puppetboard-4.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18760 2023-04-04 17:27:35.000000 puppetboard-4.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.220804 puppetboard-4.3.0/puppetboard/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/docker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.224804 puppetboard-4.3.0/puppetboard/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.224804 puppetboard-4.3.0/puppetboard/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/css/fonts.css
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/css/puppetboard.css
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/css/radiator.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.224804 puppetboard-4.3.0/puppetboard/static/custom-natural-time-delta/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/custom-natural-time-delta/natural-time-delta.js
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.220804 puppetboard-4.3.0/puppetboard/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.224804 puppetboard-4.3.0/puppetboard/static/fonts/cousine/
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SAvzAbt.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SQvzA.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SYvzAbt.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_ScvzAbt.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SgvzAbt.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SkvzAbt.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    36348 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SovzAbt.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SsvzAbt.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.224804 puppetboard-4.3.0/puppetboard/static/fonts/lato/
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAUi-qJCY.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    24408 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAXC-q.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwaPGR_p.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwiPGQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_FQft1dw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_Gwft.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjx4wXg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjxAwXjeu.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.228804 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/
--rw-r--r--   0 runner    (1001) docker     (123)    16720 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4gaVI.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4iaVIGxA.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4jaVIGxA.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4kaVIGxA.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4saVIGxA.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4taVIGxA.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4uaVIGxA.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4vaVIGxA.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.228804 puppetboard-4.3.0/puppetboard/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/js/dailychart.js
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/js/pretty.js
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/js/radiator.js
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/js/scroll.top.js
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/js/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.220804 puppetboard-4.3.0/puppetboard/static/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.228804 puppetboard-4.3.0/puppetboard/static/libs/billboard.js/
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/billboard.js/billboard.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   540910 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/billboard.js/billboard.pkgd.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.228804 puppetboard-4.3.0/puppetboard/static/libs/datatables.net/
--rw-r--r--   0 runner    (1001) docker     (123)    90265 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net/jquery.dataTables.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.228804 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons/buttons.colVis.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25107 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons/buttons.html5.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25577 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons/dataTables.buttons.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.228804 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons-se/
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.228804 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-se/
--rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.232805 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/
--rw-r--r--   0 runner    (1001) docker     (123)  1373804 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/semantic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   369693 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/semantic.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.220804 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.220804 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.220804 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.236805 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.236805 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28123 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/images/flags.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.236805 puppetboard-4.3.0/puppetboard/static/libs/jquery/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/jquery/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.236805 puppetboard-4.3.0/puppetboard/static/libs/jszip/
--rw-r--r--   0 runner    (1001) docker     (123)    97587 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/jszip/jszip.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.236805 puppetboard-4.3.0/puppetboard/static/libs/moment.js/
--rw-r--r--   0 runner    (1001) docker     (123)   369019 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/static/libs/moment.js/moment-with-locales.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.240805 puppetboard-4.3.0/puppetboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/412.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/_macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/_static_offline.html
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/_static_online.html
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/catalog.html
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/catalog_compare.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/catalogs.html
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/catalogs.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/class.html
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/class_resource.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/classes.html
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/classes.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/fact.html
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/facts.html
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/failures.html
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/inventory.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/inventory.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/metric.html
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/metrics.html
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/node.html
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/nodes.html
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/query.html
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/radiator.html
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/reports.html
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/templates/reports.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.244805 puppetboard-4.3.0/puppetboard/views/
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/dailychart.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/failures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/radiator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-04-04 17:27:35.000000 puppetboard-4.3.0/puppetboard/views/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.224804 puppetboard-4.3.0/puppetboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42500 2023-04-04 17:27:39.000000 puppetboard-4.3.0/puppetboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-04-04 17:27:39.000000 puppetboard-4.3.0/puppetboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 17:27:39.000000 puppetboard-4.3.0/puppetboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 17:27:39.000000 puppetboard-4.3.0/puppetboard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-04 17:27:39.000000 puppetboard-4.3.0/puppetboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-04 17:27:39.000000 puppetboard-4.3.0/puppetboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-04 17:27:35.000000 puppetboard-4.3.0/requirements-docker.txt
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-04 17:27:35.000000 puppetboard-4.3.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-04 17:27:35.000000 puppetboard-4.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-04 17:27:39.244805 puppetboard-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-04 17:27:35.000000 puppetboard-4.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 17:27:39.244805 puppetboard-4.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-04 17:27:35.000000 puppetboard-4.3.0/test/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-04 17:27:35.000000 puppetboard-4.3.0/test/test_app_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-04 17:27:35.000000 puppetboard-4.3.0/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-04 17:27:35.000000 puppetboard-4.3.0/test/test_docker_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-04 17:27:35.000000 puppetboard-4.3.0/test/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-04 17:27:35.000000 puppetboard-4.3.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.543624 puppetboard-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-07-27 11:45:42.000000 puppetboard-5.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-27 11:45:42.000000 puppetboard-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-27 11:45:42.000000 puppetboard-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    42863 2023-07-27 11:45:46.543624 puppetboard-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18193 2023-07-27 11:45:42.000000 puppetboard-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/docker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/css/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/css/puppetboard.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/css/radiator.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/static/custom-natural-time-delta/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/custom-natural-time-delta/natural-time-delta.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.519624 puppetboard-5.0.0/puppetboard/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.527624 puppetboard-5.0.0/puppetboard/static/fonts/cousine/
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SAvzAbt.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SQvzA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SYvzAbt.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_ScvzAbt.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SgvzAbt.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SkvzAbt.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    36348 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SovzAbt.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SsvzAbt.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.527624 puppetboard-5.0.0/puppetboard/static/fonts/lato/
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAUi-qJCY.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24408 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAXC-q.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwaPGR_p.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwiPGQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_FQft1dw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_Gwft.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    23580 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjx4wXg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjxAwXjeu.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.527624 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/
+-rw-r--r--   0 runner    (1001) docker     (123)    16720 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4gaVI.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4iaVIGxA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4jaVIGxA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4kaVIGxA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4saVIGxA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    17472 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4taVIGxA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4uaVIGxA.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4vaVIGxA.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.527624 puppetboard-5.0.0/puppetboard/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/js/dailychart.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/js/pretty.js
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/js/radiator.js
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/js/scroll.top.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/js/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/static/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.527624 puppetboard-5.0.0/puppetboard/static/libs/billboard.js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/billboard.js/billboard.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   540910 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/billboard.js/billboard.pkgd.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.527624 puppetboard-5.0.0/puppetboard/static/libs/datatables.net/
+-rw-r--r--   0 runner    (1001) docker     (123)    90265 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net/jquery.dataTables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.531624 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons/buttons.colVis.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25107 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons/buttons.html5.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25577 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons/dataTables.buttons.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.531624 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons-se/
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.531624 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-se/
+-rw-r--r--   0 runner    (1001) docker     (123)     9160 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.531624 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/
+-rw-r--r--   0 runner    (1001) docker     (123)  1373804 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/semantic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   369693 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/semantic.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.535624 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   133034 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   715890 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   132728 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    89824 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76612 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   202902 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   897426 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   202616 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   103300 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    79444 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34390 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144322 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16800 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.535624 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28123 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/images/flags.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.535624 puppetboard-5.0.0/puppetboard/static/libs/jquery/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/jquery/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.539624 puppetboard-5.0.0/puppetboard/static/libs/jszip/
+-rw-r--r--   0 runner    (1001) docker     (123)    97587 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/jszip/jszip.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.539624 puppetboard-5.0.0/puppetboard/static/libs/moment.js/
+-rw-r--r--   0 runner    (1001) docker     (123)   369019 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/static/libs/moment.js/moment-with-locales.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.539624 puppetboard-5.0.0/puppetboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/412.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/_macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/_static_offline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/_static_online.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/catalog.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/catalog_compare.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/catalogs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/catalogs.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/class.html
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/class_resource.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/classes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/classes.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/fact.html
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/facts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/failures.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/inventory.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/inventory.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/metric.html
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/metrics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/node.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/nodes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/query.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/radiator.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/reports.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/templates/reports.json.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.543624 puppetboard-5.0.0/puppetboard/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/dailychart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/radiator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-27 11:45:42.000000 puppetboard-5.0.0/puppetboard/views/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.523624 puppetboard-5.0.0/puppetboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    42863 2023-07-27 11:45:46.000000 puppetboard-5.0.0/puppetboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-27 11:45:46.000000 puppetboard-5.0.0/puppetboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:45:46.000000 puppetboard-5.0.0/puppetboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:45:46.000000 puppetboard-5.0.0/puppetboard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-27 11:45:46.000000 puppetboard-5.0.0/puppetboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 11:45:46.000000 puppetboard-5.0.0/puppetboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 11:45:42.000000 puppetboard-5.0.0/requirements-docker.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-27 11:45:42.000000 puppetboard-5.0.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-27 11:45:42.000000 puppetboard-5.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-27 11:45:46.543624 puppetboard-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-27 11:45:42.000000 puppetboard-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:46.543624 puppetboard-5.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-27 11:45:42.000000 puppetboard-5.0.0/test/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-27 11:45:42.000000 puppetboard-5.0.0/test/test_app_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-27 11:45:42.000000 puppetboard-5.0.0/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-07-27 11:45:42.000000 puppetboard-5.0.0/test/test_docker_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-27 11:45:42.000000 puppetboard-5.0.0/test/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-27 11:45:42.000000 puppetboard-5.0.0/test/test_utils.py
```

### Comparing `puppetboard-4.3.0/CHANGELOG.md` & `puppetboard-5.0.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 Changelog
 =========
 
 This is the changelog for Puppetboard.
 
+5.0.0
+-----
+
+* Stop setting `SECRET_KEY` value to a random string by default. This has caused issues in deployments with more than one app replica or when the app was restarted. Please set this to your own long, random string, **the same for each application replica**. Implements [#721](https://github.com/voxpupuli/puppetboard/issues/721).
+* Drop support for Python 3.7 (end-of-life in June 2023). PR [#899](https://github.com/voxpupuli/puppetboard/pull/899)
+* Fix broken links in Classes view. PR [#868](https://github.com/voxpupuli/puppetboard/pull/868), fixes [#816](https://github.com/voxpupuli/puppetboard/issues/816).
+* Fix if fact is `None` (default for full node view). PR [#908](https://github.com/voxpupuli/puppetboard/pull/908), fixes [#907](https://github.com/voxpupuli/puppetboard/issues/907).
+* Dependencies update.
+
+Thanks to the following contributors of this release:
+* [Louis Charreau](https://github.com/lcharreau)
+* [Yehuda Katz](https://github.com/yakatz)
+
 4.3.0
 -----
 
 * Add new **Classes** view. This view lists the Puppet classes that have had at least one of their resources changed (event). ([#799](https://github.com/voxpupuli/puppetboard/pull/799)).
 
 Big thanks to [Louis Charreau](https://github.com/lcharreau) who contributed the above feature!
```

### Comparing `puppetboard-4.3.0/LICENSE` & `puppetboard-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/PKG-INFO` & `puppetboard-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: puppetboard
-Version: 4.3.0
+Version: 5.0.0
 Summary: Web frontend for PuppetDB
 Home-page: https://github.com/voxpupuli/puppetboard
 Author: Vox Pupuli
 Author-email: voxpupuli@groups.io
 License: Apache License 2.0
 Keywords: puppet puppetdb puppetboard
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Puppetboard
 
 [![PyPI Version](https://img.shields.io/pypi/v/puppetboard)](https://pypi.org/project/puppetboard/)
@@ -49,16 +48,16 @@
 * [Configuration](#configuration)
 * [Getting Help](#getting-help)
 * [Contributing](#contributing)
 * [Legal](#legal)
 
 ## Requirements<a id="requirements"></a>
 
-* PuppetDB v. 5.2-7.10 (will most probably work with newer, but this has not been tested yet)
-* Python 3.7-3.11 or Docker
+* PuppetDB v. 5.2-7.*
+* Python 3.8-3.11 or Docker
 
 ## Installation<a id="installation"></a>
 
 Puppetboard is packaged and available on PyPI.
 
 ### With Puppet module
 
@@ -190,24 +189,25 @@
 
 For information about how to generate the correct keys please refer to the
 [pypuppetdb documentation](https://pypuppetdb.readthedocs.io/en/latest/connecting.html#ssl). Alternatively it is possible
 to explicitly specify the protocol to be used setting the `PUPPETDB_PROTO` variable.
 
 Other settings that might be interesting, in no particular order:
 
+- `SECRET_KEY`: set this to a long string, **the same for each application replica** and keep it secret. Refer to
+    [Flask documentation](https://flask.palletsprojects.com/en/2.1.x/quickstart/#sessions), section
+    "How to generate good secret keys" for more info.
 - `FAVORITE_ENVS`: an ordered list of Puppet environment names that will be shown immediately after "All Environments"
     and before other environments (which are sorted by name) in the dropdown for choosing the environment shown
     in the top-right of the UI. Environments listed here that do not really exist in your deployment are silently ignored.
 - `SHOW_ERROR_AS`: `friendly` or `raw`. The former makes Puppet run errors in Report and Failures views shown
     in a modified, (arguably) more user-friendly form. The latter shows them as they are.
     Defaults to `friendly`.
 - `CODE_PREFIX_TO_REMOVE`: what code path that should be shortened in "Friendly errors" to "…" for readability.
     A regexp. Defaults to `/etc/puppetlabs/code/environments(/.*?/modules)?`.
-- `SECRET_KEY`: Refer to [Flask documentation](https://flask.palletsprojects.com/en/2.0.x/quickstart/#sessions),
-    section "How to generate good secret keys" for more info. Defaults to a random 64-char string generated by `secrets.token_hex(32)`, prepended with a `default-` string. **Warning** Leaving SECRET_KEY set to a default value WILL cause issues when the app is restarted or has more than 1 replica (f.e. uWSGI workers, k8s replicas etc.) and some features (in particular: queries) are used. Please set SECRET_KEY to your own value, the same for all app replicas. This will be REQUIRED starting with Puppetboard 5.x which will NOT contain the default value anymore. Please see [#721](https://github.com/voxpupuli/puppetboard/issues/721) for more info.
 - `PUPPETDB_TIMEOUT`: Defaults to 20 seconds, but you might need to increase this value. It depends on how big the
     results are when querying PuppetDB. This behaviour will change in a future release when pagination will be introduced.
 - `UNRESPONSIVE_HOURS`: The amount of hours since the last check-in after which a node is considered unresponsive.
 - `LOGLEVEL`: A string representing the loglevel. It defaults to `'info'` but can be changed to `'warning'` or
     `'critical'` for less verbose logging or `'debug'` for more information.
 - `ENABLE_QUERY`: Defaults to `True` causing a Query tab to show up in the web interface allowing users to write
     and execute arbitrary queries against a set of endpoints in PuppetDB. Change this to `False` to disable this.
@@ -406,14 +406,27 @@
 downloaded from the [Noun Project](https://thenounproject.com).
 
 Changelog
 =========
 
 This is the changelog for Puppetboard.
 
+5.0.0
+-----
+
+* Stop setting `SECRET_KEY` value to a random string by default. This has caused issues in deployments with more than one app replica or when the app was restarted. Please set this to your own long, random string, **the same for each application replica**. Implements [#721](https://github.com/voxpupuli/puppetboard/issues/721).
+* Drop support for Python 3.7 (end-of-life in June 2023). PR [#899](https://github.com/voxpupuli/puppetboard/pull/899)
+* Fix broken links in Classes view. PR [#868](https://github.com/voxpupuli/puppetboard/pull/868), fixes [#816](https://github.com/voxpupuli/puppetboard/issues/816).
+* Fix if fact is `None` (default for full node view). PR [#908](https://github.com/voxpupuli/puppetboard/pull/908), fixes [#907](https://github.com/voxpupuli/puppetboard/issues/907).
+* Dependencies update.
+
+Thanks to the following contributors of this release:
+* [Louis Charreau](https://github.com/lcharreau)
+* [Yehuda Katz](https://github.com/yakatz)
+
 4.3.0
 -----
 
 * Add new **Classes** view. This view lists the Puppet classes that have had at least one of their resources changed (event). ([#799](https://github.com/voxpupuli/puppetboard/pull/799)).
 
 Big thanks to [Louis Charreau](https://github.com/lcharreau) who contributed the above feature!
```

### Comparing `puppetboard-4.3.0/README.md` & `puppetboard-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 * [Configuration](#configuration)
 * [Getting Help](#getting-help)
 * [Contributing](#contributing)
 * [Legal](#legal)
 
 ## Requirements<a id="requirements"></a>
 
-* PuppetDB v. 5.2-7.10 (will most probably work with newer, but this has not been tested yet)
-* Python 3.7-3.11 or Docker
+* PuppetDB v. 5.2-7.*
+* Python 3.8-3.11 or Docker
 
 ## Installation<a id="installation"></a>
 
 Puppetboard is packaged and available on PyPI.
 
 ### With Puppet module
 
@@ -163,24 +163,25 @@
 
 For information about how to generate the correct keys please refer to the
 [pypuppetdb documentation](https://pypuppetdb.readthedocs.io/en/latest/connecting.html#ssl). Alternatively it is possible
 to explicitly specify the protocol to be used setting the `PUPPETDB_PROTO` variable.
 
 Other settings that might be interesting, in no particular order:
 
+- `SECRET_KEY`: set this to a long string, **the same for each application replica** and keep it secret. Refer to
+    [Flask documentation](https://flask.palletsprojects.com/en/2.1.x/quickstart/#sessions), section
+    "How to generate good secret keys" for more info.
 - `FAVORITE_ENVS`: an ordered list of Puppet environment names that will be shown immediately after "All Environments"
     and before other environments (which are sorted by name) in the dropdown for choosing the environment shown
     in the top-right of the UI. Environments listed here that do not really exist in your deployment are silently ignored.
 - `SHOW_ERROR_AS`: `friendly` or `raw`. The former makes Puppet run errors in Report and Failures views shown
     in a modified, (arguably) more user-friendly form. The latter shows them as they are.
     Defaults to `friendly`.
 - `CODE_PREFIX_TO_REMOVE`: what code path that should be shortened in "Friendly errors" to "…" for readability.
     A regexp. Defaults to `/etc/puppetlabs/code/environments(/.*?/modules)?`.
-- `SECRET_KEY`: Refer to [Flask documentation](https://flask.palletsprojects.com/en/2.0.x/quickstart/#sessions),
-    section "How to generate good secret keys" for more info. Defaults to a random 64-char string generated by `secrets.token_hex(32)`, prepended with a `default-` string. **Warning** Leaving SECRET_KEY set to a default value WILL cause issues when the app is restarted or has more than 1 replica (f.e. uWSGI workers, k8s replicas etc.) and some features (in particular: queries) are used. Please set SECRET_KEY to your own value, the same for all app replicas. This will be REQUIRED starting with Puppetboard 5.x which will NOT contain the default value anymore. Please see [#721](https://github.com/voxpupuli/puppetboard/issues/721) for more info.
 - `PUPPETDB_TIMEOUT`: Defaults to 20 seconds, but you might need to increase this value. It depends on how big the
     results are when querying PuppetDB. This behaviour will change in a future release when pagination will be introduced.
 - `UNRESPONSIVE_HOURS`: The amount of hours since the last check-in after which a node is considered unresponsive.
 - `LOGLEVEL`: A string representing the loglevel. It defaults to `'info'` but can be changed to `'warning'` or
     `'critical'` for less verbose logging or `'debug'` for more information.
 - `ENABLE_QUERY`: Defaults to `True` causing a Query tab to show up in the web interface allowing users to write
     and execute arbitrary queries against a set of endpoints in PuppetDB. Change this to `False` to disable this.
```

### Comparing `puppetboard-4.3.0/puppetboard/app.py` & `puppetboard-5.0.0/puppetboard/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 app = get_app()
 puppetdb = get_puppetdb()
 get_scheduler()
 running_as = os.path.basename(sys.argv[0])
 if not is_a_test():
     check_db_version(puppetdb)
-check_secret_key(app.config.get('SECRET_KEY'))
+    check_secret_key(app.config.get('SECRET_KEY'))
 
 logging.basicConfig(level=app.config['LOGLEVEL'].upper())
 log = logging.getLogger(__name__)
 
 menu_entries = [
     ('index', 'Overview'),
     ('failures', 'Failures'),
```

### Comparing `puppetboard-4.3.0/puppetboard/core.py` & `puppetboard-5.0.0/puppetboard/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 import socket
+from importlib.metadata import version
 
-import pkg_resources
 from flask import Flask
 from flask_caching import Cache
 from flask_apscheduler import APScheduler
 from pypuppetdb import connect
 
 from puppetboard.utils import (get_or_abort, jsonprint,
                                url_for_field, quote_columns_data)
@@ -66,15 +66,15 @@
                            port=app.config['PUPPETDB_PORT'],
                            ssl_verify=app.config['PUPPETDB_SSL_VERIFY'],
                            ssl_key=app.config['PUPPETDB_KEY'],
                            ssl_cert=app.config['PUPPETDB_CERT'],
                            timeout=app.config['PUPPETDB_TIMEOUT'],
                            protocol=app.config['PUPPETDB_PROTO'], )
 
-        requests_version = pkg_resources.get_distribution("requests").version
+        requests_version = version("requests")
         user_agent_header = {
             "user-agent": f"puppetboard/{own_version} (r/{requests_version})",
         }
         puppetdb.session.headers = {**puppetdb.session.headers, **user_agent_header}
 
         PUPPETDB = puppetdb
```

### Comparing `puppetboard-4.3.0/puppetboard/default_settings.py` & `puppetboard-5.0.0/puppetboard/default_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 PUPPETDB_PORT = 8080
 PUPPETDB_PROTO = None
 PUPPETDB_SSL_VERIFY = True
 PUPPETDB_KEY = None
 PUPPETDB_CERT = None
 PUPPETDB_TIMEOUT = 20
 DEFAULT_ENVIRONMENT = 'production'
-SECRET_KEY = f"default-{secrets.token_hex(32)}"
+# this empty string has to be changed, we validate it with check_secret_key()
+SECRET_KEY = ''  # nosec
 UNRESPONSIVE_HOURS = 2
 ENABLE_QUERY = True
 # Uncomment to restrict the enabled PuppetDB endpoints in the query page.
 # ENABLED_QUERY_ENDPOINTS = ['facts', 'nodes']
 LOCALISE_TIMESTAMP = True
 LOGLEVEL = 'info'
 NORMAL_TABLE_COUNT = 100
@@ -74,15 +75,15 @@
 CLASS_EVENTS_STATUS_COLUMNS = [
     # ('skipped', 'Skipped'),
     ('failure', 'Failure'),
     ('success', 'Success'),
     ('noop', 'Noop'),
 ]
 # Type of caching object to use when `SCHEDULER_ENABLED` is set to `True`.
-# If more than one worker, use a shared backend (e.g. `MemcachedCache`) 
+# If more than one worker, use a shared backend (e.g. `MemcachedCache`)
 # to allow the sharing of the cache between the processes.
 CACHE_TYPE = 'SimpleCache'
 # Cache litefime in second
 CACHE_DEFAULT_TIMEOUT = 3600
 
 # List of scheduled jobs to trigger
 #   * `id`: job's ID
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
 import secrets PUPPETDB_HOST = 'localhost' PUPPETDB_PORT = 8080 PUPPETDB_PROTO
 = None PUPPETDB_SSL_VERIFY = True PUPPETDB_KEY = None PUPPETDB_CERT = None
-PUPPETDB_TIMEOUT = 20 DEFAULT_ENVIRONMENT = 'production' SECRET_KEY =
-f"default-{secrets.token_hex(32)}" UNRESPONSIVE_HOURS = 2 ENABLE_QUERY = True #
-Uncomment to restrict the enabled PuppetDB endpoints in the query page. #
-ENABLED_QUERY_ENDPOINTS = ['facts', 'nodes'] LOCALISE_TIMESTAMP = True LOGLEVEL
-= 'info' NORMAL_TABLE_COUNT = 100 LITTLE_TABLE_COUNT = 10 TABLE_COUNT_SELECTOR
-= [10, 20, 50, 100, 500] DISPLAYED_METRICS = ['resources.total',
-'events.failure', 'events.success', 'resources.skipped', 'events.noop']
-OFFLINE_MODE = False ENABLE_CATALOG = False OVERVIEW_FILTER = None PAGE_TITLE =
-"Puppetboard" GRAPH_TYPE = 'pie' GRAPH_FACTS = ['architecture',
-'clientversion', 'domain', 'lsbcodename', 'lsbdistcodename', 'lsbdistid',
-'lsbdistrelease', 'lsbmajdistrelease', 'netmask', 'osfamily', 'puppetversion',
-'processorcount'] INVENTORY_FACTS = [('Hostname', 'trusted'), ('IP Address',
-'ipaddress'), ('OS', 'os'), ('Architecture', 'hardwaremodel'), ('Kernel
-Version', 'kernelrelease'), ('Puppet Version', 'puppetversion'), ]
-INVENTORY_FACT_TEMPLATES = { 'trusted': ( """"""_"""{{value.hostname}}"""
-"""""" ), 'os': "{{ fact_os_detection(value) }}", } REFRESH_RATE = 30
-DAILY_REPORTS_CHART_ENABLED = True DAILY_REPORTS_CHART_DAYS = 8
-WITH_EVENT_NUMBERS = True SHOW_ERROR_AS = 'friendly' # or 'raw'
-CODE_PREFIX_TO_REMOVE = '/etc/puppetlabs/code/environments(/.*?/modules)?'
-FAVORITE_ENVS = [ 'production', 'staging', 'qa', 'test', 'dev', ] ENABLE_CLASS
-= False # mapping between the status of the events (from PuppetDB) and the
-columns of the table to display CLASS_EVENTS_STATUS_COLUMNS = [ # ('skipped',
-'Skipped'), ('failure', 'Failure'), ('success', 'Success'), ('noop', 'Noop'), ]
-# Type of caching object to use when `SCHEDULER_ENABLED` is set to `True`. # If
-more than one worker, use a shared backend (e.g. `MemcachedCache`) # to allow
-the sharing of the cache between the processes. CACHE_TYPE = 'SimpleCache' #
-Cache litefime in second CACHE_DEFAULT_TIMEOUT = 3600 # List of scheduled jobs
-to trigger # * `id`: job's ID # * `func`: full path of the function to execute
-# * `trigger`: should be 'interval' if you want to run the job at regular
-intervals # * `seconds`: number of seconds between 2 triggered jobs
-SCHEDULER_JOBS = [{ 'id': 'do_build_async_cache_1', 'func':
-'puppetboard.schedulers.classes:build_async_cache', 'trigger': 'interval',
-'seconds': 300, }] SCHEDULER_ENABLED = False SCHEDULER_LOCK_BIND_PORT = 49100
+PUPPETDB_TIMEOUT = 20 DEFAULT_ENVIRONMENT = 'production' # this empty string
+has to be changed, we validate it with check_secret_key() SECRET_KEY = '' #
+nosec UNRESPONSIVE_HOURS = 2 ENABLE_QUERY = True # Uncomment to restrict the
+enabled PuppetDB endpoints in the query page. # ENABLED_QUERY_ENDPOINTS =
+['facts', 'nodes'] LOCALISE_TIMESTAMP = True LOGLEVEL = 'info'
+NORMAL_TABLE_COUNT = 100 LITTLE_TABLE_COUNT = 10 TABLE_COUNT_SELECTOR = [10,
+20, 50, 100, 500] DISPLAYED_METRICS = ['resources.total', 'events.failure',
+'events.success', 'resources.skipped', 'events.noop'] OFFLINE_MODE = False
+ENABLE_CATALOG = False OVERVIEW_FILTER = None PAGE_TITLE = "Puppetboard"
+GRAPH_TYPE = 'pie' GRAPH_FACTS = ['architecture', 'clientversion', 'domain',
+'lsbcodename', 'lsbdistcodename', 'lsbdistid', 'lsbdistrelease',
+'lsbmajdistrelease', 'netmask', 'osfamily', 'puppetversion', 'processorcount']
+INVENTORY_FACTS = [('Hostname', 'trusted'), ('IP Address', 'ipaddress'), ('OS',
+'os'), ('Architecture', 'hardwaremodel'), ('Kernel Version', 'kernelrelease'),
+('Puppet Version', 'puppetversion'), ] INVENTORY_FACT_TEMPLATES = { 'trusted':
+( """"""_"""{{value.hostname}}"""_"""""" ), 'os': "{{ fact_os_detection(value)
+}}", } REFRESH_RATE = 30 DAILY_REPORTS_CHART_ENABLED = True
+DAILY_REPORTS_CHART_DAYS = 8 WITH_EVENT_NUMBERS = True SHOW_ERROR_AS =
+'friendly' # or 'raw' CODE_PREFIX_TO_REMOVE = '/etc/puppetlabs/code/
+environments(/.*?/modules)?' FAVORITE_ENVS = [ 'production', 'staging', 'qa',
+'test', 'dev', ] ENABLE_CLASS = False # mapping between the status of the
+events (from PuppetDB) and the columns of the table to display
+CLASS_EVENTS_STATUS_COLUMNS = [ # ('skipped', 'Skipped'), ('failure',
+'Failure'), ('success', 'Success'), ('noop', 'Noop'), ] # Type of caching
+object to use when `SCHEDULER_ENABLED` is set to `True`. # If more than one
+worker, use a shared backend (e.g. `MemcachedCache`) # to allow the sharing of
+the cache between the processes. CACHE_TYPE = 'SimpleCache' # Cache litefime in
+second CACHE_DEFAULT_TIMEOUT = 3600 # List of scheduled jobs to trigger # *
+`id`: job's ID # * `func`: full path of the function to execute # * `trigger`:
+should be 'interval' if you want to run the job at regular intervals # *
+`seconds`: number of seconds between 2 triggered jobs SCHEDULER_JOBS = [{ 'id':
+'do_build_async_cache_1', 'func': 'puppetboard.schedulers.classes:
+build_async_cache', 'trigger': 'interval', 'seconds': 300, }] SCHEDULER_ENABLED
+= False SCHEDULER_LOCK_BIND_PORT = 49100
```

### Comparing `puppetboard-4.3.0/puppetboard/docker_settings.py` & `puppetboard-5.0.0/puppetboard/docker_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
 )
 
 PUPPETDB_KEY = cert_to_file(os.getenv('PUPPETDB_KEY', None))
 PUPPETDB_CERT = cert_to_file(os.getenv('PUPPETDB_CERT', None))
 PUPPETDB_PROTO = os.getenv('PUPPETDB_PROTO', None)
 PUPPETDB_TIMEOUT = int(os.getenv('PUPPETDB_TIMEOUT', '20'))
 DEFAULT_ENVIRONMENT = os.getenv('DEFAULT_ENVIRONMENT', 'production')
-SECRET_KEY = os.getenv('SECRET_KEY', f"default-{secrets.token_hex(32)}")
+# this empty string has to be changed, we validate it with check_secret_key()
+SECRET_KEY = os.getenv('SECRET_KEY', '')  # nosec
 UNRESPONSIVE_HOURS = int(os.getenv('UNRESPONSIVE_HOURS', '2'))
 ENABLE_QUERY = coerce_bool(os.getenv('ENABLE_QUERY'), True)
 # Uncomment to restrict the enabled PuppetDB endpoints in the query page.
 # ENABLED_QUERY_ENDPOINTS = ['facts', 'nodes']
 
 LOCALISE_TIMESTAMP = coerce_bool(os.getenv('LOCALISE_TIMESTAMP'), True)
 LOGLEVEL = os.getenv('LOGLEVEL', 'info')
@@ -173,15 +174,15 @@
 
 CLASS_EVENTS_STATUS_COLUMNS_STR = os.getenv('CLASS_EVENTS_STATUS_COLUMNS', CLASS_EVENTS_STATUS_COLUMNS_DEFAULT).split(',')
 
 # Take the Array and convert it to a tuple
 CLASS_EVENTS_STATUS_COLUMNS = [(CLASS_EVENTS_STATUS_COLUMNS_STR[i].strip(),
                                 CLASS_EVENTS_STATUS_COLUMNS_STR[i + 1].strip()) for i in range(0, len(CLASS_EVENTS_STATUS_COLUMNS_STR), 2)]
 
-# Enabled a scheduler instance to trigger jobs in background. 
+# Enabled a scheduler instance to trigger jobs in background.
 SCHEDULER_ENABLED = coerce_bool(os.getenv('SCHEDULER_ENABLED'), False)
 
 # Tuples are hard to express as an environment variable, so here
 # the tuple can be listed as a list of items
 # Examples:
 #   export SCHEDULER_JOBS="id, <id>, func, <func>, trigger, <trigger>, seconds, <seconds>"
 # The scheduled jobs are separated by the character ";".
```

### Comparing `puppetboard-4.3.0/puppetboard/errors.py` & `puppetboard-5.0.0/puppetboard/errors.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/forms.py` & `puppetboard-5.0.0/puppetboard/forms.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/css/fonts.css` & `puppetboard-5.0.0/puppetboard/static/css/fonts.css`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/css/puppetboard.css` & `puppetboard-5.0.0/puppetboard/static/css/puppetboard.css`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/css/radiator.css` & `puppetboard-5.0.0/puppetboard/static/css/radiator.css`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/custom-natural-time-delta/natural-time-delta.js` & `puppetboard-5.0.0/puppetboard/static/custom-natural-time-delta/natural-time-delta.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/favicon.ico` & `puppetboard-5.0.0/puppetboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/favicon.svg` & `puppetboard-5.0.0/puppetboard/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SAvzAbt.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SAvzAbt.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SQvzA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SQvzA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SYvzAbt.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SYvzAbt.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_ScvzAbt.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_ScvzAbt.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SgvzAbt.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SgvzAbt.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SkvzAbt.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SkvzAbt.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SovzAbt.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SovzAbt.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SsvzAbt.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/cousine/d6lIkaiiRdih4SpP_SsvzAbt.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAUi-qJCY.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAUi-qJCY.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAXC-q.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u8w4BMUTPHjxsAXC-q.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwaPGR_p.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwaPGR_p.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwiPGQ.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u9w4BMUTPHh6UVSwiPGQ.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_FQft1dw.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_FQft1dw.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_Gwft.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6u_w4BMUTPHjxsI5wq_Gwft.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjx4wXg.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjx4wXg.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjxAwXjeu.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/lato/S6uyw4BMUTPHjxAwXjeu.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4gaVI.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4gaVI.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4iaVIGxA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4iaVIGxA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4jaVIGxA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4jaVIGxA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4kaVIGxA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4kaVIGxA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4saVIGxA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4saVIGxA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4taVIGxA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4taVIGxA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4uaVIGxA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4uaVIGxA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4vaVIGxA.woff2` & `puppetboard-5.0.0/puppetboard/static/fonts/open-sans/memSYaGs126MiZpBA-UvWbX2vVnXBbObj2OVZyOOSr4dVJWUgsjZ0B4vaVIGxA.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/js/dailychart.js` & `puppetboard-5.0.0/puppetboard/static/js/dailychart.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/js/pretty.js` & `puppetboard-5.0.0/puppetboard/static/js/pretty.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/js/radiator.js` & `puppetboard-5.0.0/puppetboard/static/js/radiator.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/js/utils.js` & `puppetboard-5.0.0/puppetboard/static/js/utils.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/billboard.js/billboard.min.css` & `puppetboard-5.0.0/puppetboard/static/libs/billboard.js/billboard.min.css`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/billboard.js/billboard.pkgd.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/billboard.js/billboard.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net/jquery.dataTables.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons/buttons.colVis.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons/buttons.colVis.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons/buttons.html5.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons/buttons.html5.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons/dataTables.buttons.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons/dataTables.buttons.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.css` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net-buttons-se/buttons.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.css` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/datatables.net-se/dataTables.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/semantic.min.css` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/semantic.min.css`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/semantic.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/semantic.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.eot` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.eot`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.svg` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.svg`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.ttf` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.ttf`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff2` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.eot` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.svg` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.ttf` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff2` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.eot` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.eot`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.svg` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.svg`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.ttf` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.ttf`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff2` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/images/flags.png` & `puppetboard-5.0.0/puppetboard/static/libs/fomantic-ui/themes/default/assets/images/flags.png`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/jquery/jquery.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/jszip/jszip.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/jszip/jszip.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/static/libs/moment.js/moment-with-locales.min.js` & `puppetboard-5.0.0/puppetboard/static/libs/moment.js/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/_macros.html` & `puppetboard-5.0.0/puppetboard/templates/_macros.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/_static_offline.html` & `puppetboard-5.0.0/puppetboard/templates/_static_offline.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/_static_online.html` & `puppetboard-5.0.0/puppetboard/templates/_static_online.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/catalog.html` & `puppetboard-5.0.0/puppetboard/templates/catalog.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/catalog_compare.html` & `puppetboard-5.0.0/puppetboard/templates/catalog_compare.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/catalogs.html` & `puppetboard-5.0.0/puppetboard/templates/catalogs.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/catalogs.json.tpl` & `puppetboard-5.0.0/puppetboard/templates/catalogs.json.tpl`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/class.html` & `puppetboard-5.0.0/puppetboard/templates/class.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/class_resource.json.tpl` & `puppetboard-5.0.0/puppetboard/templates/class_resource.json.tpl`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/classes.html` & `puppetboard-5.0.0/puppetboard/templates/classes.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/classes.json.tpl` & `puppetboard-5.0.0/puppetboard/templates/classes.json.tpl`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/fact.html` & `puppetboard-5.0.0/puppetboard/templates/fact.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/facts.html` & `puppetboard-5.0.0/puppetboard/templates/facts.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/failures.html` & `puppetboard-5.0.0/puppetboard/templates/failures.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/index.html` & `puppetboard-5.0.0/puppetboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/inventory.html` & `puppetboard-5.0.0/puppetboard/templates/inventory.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/inventory.json.tpl` & `puppetboard-5.0.0/puppetboard/templates/inventory.json.tpl`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/layout.html` & `puppetboard-5.0.0/puppetboard/templates/layout.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/metric.html` & `puppetboard-5.0.0/puppetboard/templates/metric.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/node.html` & `puppetboard-5.0.0/puppetboard/templates/node.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/nodes.html` & `puppetboard-5.0.0/puppetboard/templates/nodes.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/query.html` & `puppetboard-5.0.0/puppetboard/templates/query.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/radiator.html` & `puppetboard-5.0.0/puppetboard/templates/radiator.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/report.html` & `puppetboard-5.0.0/puppetboard/templates/report.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/reports.html` & `puppetboard-5.0.0/puppetboard/templates/reports.html`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/templates/reports.json.tpl` & `puppetboard-5.0.0/puppetboard/templates/reports.json.tpl`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/utils.py` & `puppetboard-5.0.0/puppetboard/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,33 +45,19 @@
         sys.exit(2)
     except EmptyResponseError as e:
         log.error(str(e))
         sys.exit(2)
 
 
 def check_secret_key(secret_key_value):
-    """
-    Check if the secret key value is set to a default value, that will stop
-    being accepted in v5.x of the app.
-    """
-
-    if type(secret_key_value) is str and secret_key_value.startswith("default-"):
-        log.warning(
-            "Leaving SECRET_KEY set to a default value WILL cause issues"
-            " when the app is restarted or has more than 1 replica"
-            " (f.e. uWSGI workers, k8s replicas etc.) and some features"
-            " (in particular: queries) are used.\n"
-            "Please set SECRET_KEY to your own value, the same for all app"
-            " replicas.\n"
-            "This will be REQUIRED starting with Puppetboard 5.x which"
-            " will NOT contain the default value anymore.\n"
-            "Please see"
-            " https://github.com/voxpupuli/puppetboard/issues/721"
-            " for more info."
-        )
+    if not secret_key_value:
+        log.critical('Please set SECRET_KEY to a long, random string,'
+                     ' **the same for each application replica**,'
+                     ' and do not share it.')
+        sys.exit(1)
 
 
 def parse_python(value: str):
     """
     :param value: any string, number, bool, list or a dict
                   casted to a string (f.e. "{'up': ['eth0'], (...)}")
     :return: the same value but with a proper type
```

### Comparing `puppetboard-4.3.0/puppetboard/views/catalogs.py` & `puppetboard-5.0.0/puppetboard/views/catalogs.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/classes.py` & `puppetboard-5.0.0/puppetboard/views/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,43 +49,44 @@
 
 
 @app.route('/classes/json', defaults={'env': app.config['DEFAULT_ENVIRONMENT']})
 @app.route('/<env>/classes/json')
 def classes_ajax(env):
     """Backend endpoint for classes table"""
 
+    env_cache_key = env
     draw = int(request.args.get('draw', 0))
     envs = environments()
     check_env(env, envs)
 
     columns = [col for col in app.config['CLASS_EVENTS_STATUS_COLUMNS'] if col[0] in events_status_columns]
 
     query = AndOperator()
-    if env != '*':
-        query.add(EqualsOperator("report_environment", env))
+    if env == '*':
+        env_cache_key = 'all'
     else:
-        env = 'all'
+        query.add(EqualsOperator("report_environment", env))
     query.add(NullOperator('deactivated', True))
     nodelist = puppetdb.nodes(query=query, with_status=True)
 
     new_cache = {}
-    cached_classes = cache.get(f'classes_resource_{env}')
+    cached_classes = cache.get(f'classes_resource_{env_cache_key}')
     if cached_classes is None:
-        cached_classes = {} 
+        cached_classes = {}
 
     classes = {}
     for node in yield_or_stop(nodelist):
         last_report = node.latest_report_hash
         if last_report is None:
             continue
         is_new_report = True
         for class_name, cached_last_reports in cached_classes.items():
             if class_name in new_cache and last_report in new_cache[class_name]:
                 is_new_report = False
-                continue 
+                continue
             if last_report in cached_last_reports:
                 is_new_report = False
                 new_cache[class_name] = new_cache.get(class_name, {})
                 new_cache[class_name][last_report] = cached_last_reports[last_report]
 
                 classes[class_name] = classes.get(class_name, {})
                 classes[class_name]['nb_events_per_status'] = classes[class_name].get('nb_events_per_status', {col[0]: 0 for col in columns})
@@ -124,20 +125,20 @@
         for report_hash, report in new_cache[class_name].items():
             class_status = get_status_from_events(report['nb_events_per_status'])
             new_cache[class_name][report_hash]['class_status'] = class_status
             if class_status in classes[class_name]['nb_nodes_per_class_status']:
                 disable_class = False
                 classes[class_name]['nb_nodes_per_class_status'][class_status] += 1
         if disable_class:
-            class_to_remove.append(class_name) 
+            class_to_remove.append(class_name)
 
     for class_name in class_to_remove:
         del classes[class_name]
 
-    cache.set(f'classes_resource_{env}', new_cache)
+    cache.set(f'classes_resource_{env_cache_key}', new_cache)
 
     total = len(classes)
 
     return render_template(
         'classes.json.tpl',
         draw=draw,
         total=total,
@@ -160,15 +161,15 @@
             yield event
 
 
 @app.route('/class_resource/<class_name>',
            defaults={'env': app.config['DEFAULT_ENVIRONMENT']})
 @app.route('/<env>/class_resource/<class_name>')
 def class_resource(env, class_name):
-    """Fetches the nodes from PuppetDB for which there was 
+    """Fetches the nodes from PuppetDB for which there was
     at least one event on a resource declared in a given Class.
     It streams a table displaying those nodes along with the status
     of the node and the status of the class (aka resource(s)).
 
     :param env: Searches for resource events in this environment
     :type env: :obj:`string`
     :param class_name: Find all nodes executing the resources declared in the
@@ -191,54 +192,55 @@
 
 @app.route('/class_resource/<class_name>/json',
            defaults={'env': app.config['DEFAULT_ENVIRONMENT']})
 @app.route('/<env>/class_resource/<class_name>/json')
 def class_resource_ajax(env, class_name):
     """Backend endpoint for class table"""
 
+    env_cache_key = env
     draw = int(request.args.get('draw', 0))
     envs = environments()
     check_env(env, envs)
 
     columns = [col for col in app.config['CLASS_EVENTS_STATUS_COLUMNS'] if col[0] in events_status_columns]
 
     query = InOperator('certname')
     query_from = FromOperator('resources')
     query_extract = ExtractOperator()
     query_extract.add_field('certname')
     resources_in_query = InOperator('certname')
     query_and = AndOperator()
     query_and.add(EqualsOperator('type', 'Class'))
     query_and.add(EqualsOperator('title', class_name))
-    if env != '*':
-        query_and.add(EqualsOperator("environment", env))
+    if env == '*':
+        env_cache_key = 'all'
     else:
-        env = 'all'
+        query_and.add(EqualsOperator("environment", env))
 
     query_extract.add_query(query_and)
     query_from.add_query(query_extract)
     query.add_query(query_from)
     nodelist = puppetdb.nodes(query=query, with_status=True)
 
-    cached_classes = cache.get(f'classes_resource_{env}')
+    cached_classes = cache.get(f'classes_resource_{env_cache_key}')
     if cached_classes is None:
         cached_classes = {}
 
     cached_class = cached_classes.get(class_name, {})
     reports = {}
     for node in yield_or_stop(nodelist):
         node_name = node.name
         last_report = node.latest_report_hash
 
         if last_report is None or node.deactivated:
             continue
         if last_report in reports:
             continue
         if last_report in cached_class:
-            reports[last_report] = cached_class[last_report] 
+            reports[last_report] = cached_class[last_report]
             continue
 
         for event in yield_or_stop(get_events(last_report, env)):
             if class_name != event.item['class']:
                 continue
             reports[last_report] = reports.get(last_report, {
                 'node_name': node_name,
@@ -249,15 +251,15 @@
             })
             if event.status in reports[last_report]['nb_events_per_status']:
                 reports[last_report]['nb_events_per_status'][event.status] += 1
         if last_report in reports:
             reports[last_report]['class_status'] = get_status_from_events(reports[last_report]['nb_events_per_status'])
 
     cached_classes[class_name] = reports
-    cache.set(f'classes_resource_{env}', cached_classes)
+    cache.set(f'classes_resource_{env_cache_key}', cached_classes)
 
     total = len(reports)
 
     return render_template(
         'class_resource.json.tpl',
         draw=draw,
         total=total,
```

### Comparing `puppetboard-4.3.0/puppetboard/views/dailychart.py` & `puppetboard-5.0.0/puppetboard/views/dailychart.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/facts.py` & `puppetboard-5.0.0/puppetboard/views/facts.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """
     draw = int(request.args.get('draw', 0))
 
     envs = environments()
     check_env(env, envs)
 
     render_graph = False
-    if fact in app.config['GRAPH_FACTS'] and value is None and node is None:
+    if fact is not None and fact in app.config['GRAPH_FACTS'] and value is None and node is None:
         render_graph = True
 
     query = AndOperator()
     if node is not None:
         query.add(EqualsOperator("certname", node))
 
     if env != '*':
```

### Comparing `puppetboard-4.3.0/puppetboard/views/failures.py` & `puppetboard-5.0.0/puppetboard/views/failures.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/index.py` & `puppetboard-5.0.0/puppetboard/views/index.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/inventory.py` & `puppetboard-5.0.0/puppetboard/views/inventory.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/metrics.py` & `puppetboard-5.0.0/puppetboard/views/metrics.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/nodes.py` & `puppetboard-5.0.0/puppetboard/views/nodes.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/query.py` & `puppetboard-5.0.0/puppetboard/views/query.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/radiator.py` & `puppetboard-5.0.0/puppetboard/views/radiator.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard/views/reports.py` & `puppetboard-5.0.0/puppetboard/views/reports.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard.egg-info/PKG-INFO` & `puppetboard-5.0.0/puppetboard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: puppetboard
-Version: 4.3.0
+Version: 5.0.0
 Summary: Web frontend for PuppetDB
 Home-page: https://github.com/voxpupuli/puppetboard
 Author: Vox Pupuli
 Author-email: voxpupuli@groups.io
 License: Apache License 2.0
 Keywords: puppet puppetdb puppetboard
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Puppetboard
 
 [![PyPI Version](https://img.shields.io/pypi/v/puppetboard)](https://pypi.org/project/puppetboard/)
@@ -49,16 +48,16 @@
 * [Configuration](#configuration)
 * [Getting Help](#getting-help)
 * [Contributing](#contributing)
 * [Legal](#legal)
 
 ## Requirements<a id="requirements"></a>
 
-* PuppetDB v. 5.2-7.10 (will most probably work with newer, but this has not been tested yet)
-* Python 3.7-3.11 or Docker
+* PuppetDB v. 5.2-7.*
+* Python 3.8-3.11 or Docker
 
 ## Installation<a id="installation"></a>
 
 Puppetboard is packaged and available on PyPI.
 
 ### With Puppet module
 
@@ -190,24 +189,25 @@
 
 For information about how to generate the correct keys please refer to the
 [pypuppetdb documentation](https://pypuppetdb.readthedocs.io/en/latest/connecting.html#ssl). Alternatively it is possible
 to explicitly specify the protocol to be used setting the `PUPPETDB_PROTO` variable.
 
 Other settings that might be interesting, in no particular order:
 
+- `SECRET_KEY`: set this to a long string, **the same for each application replica** and keep it secret. Refer to
+    [Flask documentation](https://flask.palletsprojects.com/en/2.1.x/quickstart/#sessions), section
+    "How to generate good secret keys" for more info.
 - `FAVORITE_ENVS`: an ordered list of Puppet environment names that will be shown immediately after "All Environments"
     and before other environments (which are sorted by name) in the dropdown for choosing the environment shown
     in the top-right of the UI. Environments listed here that do not really exist in your deployment are silently ignored.
 - `SHOW_ERROR_AS`: `friendly` or `raw`. The former makes Puppet run errors in Report and Failures views shown
     in a modified, (arguably) more user-friendly form. The latter shows them as they are.
     Defaults to `friendly`.
 - `CODE_PREFIX_TO_REMOVE`: what code path that should be shortened in "Friendly errors" to "…" for readability.
     A regexp. Defaults to `/etc/puppetlabs/code/environments(/.*?/modules)?`.
-- `SECRET_KEY`: Refer to [Flask documentation](https://flask.palletsprojects.com/en/2.0.x/quickstart/#sessions),
-    section "How to generate good secret keys" for more info. Defaults to a random 64-char string generated by `secrets.token_hex(32)`, prepended with a `default-` string. **Warning** Leaving SECRET_KEY set to a default value WILL cause issues when the app is restarted or has more than 1 replica (f.e. uWSGI workers, k8s replicas etc.) and some features (in particular: queries) are used. Please set SECRET_KEY to your own value, the same for all app replicas. This will be REQUIRED starting with Puppetboard 5.x which will NOT contain the default value anymore. Please see [#721](https://github.com/voxpupuli/puppetboard/issues/721) for more info.
 - `PUPPETDB_TIMEOUT`: Defaults to 20 seconds, but you might need to increase this value. It depends on how big the
     results are when querying PuppetDB. This behaviour will change in a future release when pagination will be introduced.
 - `UNRESPONSIVE_HOURS`: The amount of hours since the last check-in after which a node is considered unresponsive.
 - `LOGLEVEL`: A string representing the loglevel. It defaults to `'info'` but can be changed to `'warning'` or
     `'critical'` for less verbose logging or `'debug'` for more information.
 - `ENABLE_QUERY`: Defaults to `True` causing a Query tab to show up in the web interface allowing users to write
     and execute arbitrary queries against a set of endpoints in PuppetDB. Change this to `False` to disable this.
@@ -406,14 +406,27 @@
 downloaded from the [Noun Project](https://thenounproject.com).
 
 Changelog
 =========
 
 This is the changelog for Puppetboard.
 
+5.0.0
+-----
+
+* Stop setting `SECRET_KEY` value to a random string by default. This has caused issues in deployments with more than one app replica or when the app was restarted. Please set this to your own long, random string, **the same for each application replica**. Implements [#721](https://github.com/voxpupuli/puppetboard/issues/721).
+* Drop support for Python 3.7 (end-of-life in June 2023). PR [#899](https://github.com/voxpupuli/puppetboard/pull/899)
+* Fix broken links in Classes view. PR [#868](https://github.com/voxpupuli/puppetboard/pull/868), fixes [#816](https://github.com/voxpupuli/puppetboard/issues/816).
+* Fix if fact is `None` (default for full node view). PR [#908](https://github.com/voxpupuli/puppetboard/pull/908), fixes [#907](https://github.com/voxpupuli/puppetboard/issues/907).
+* Dependencies update.
+
+Thanks to the following contributors of this release:
+* [Louis Charreau](https://github.com/lcharreau)
+* [Yehuda Katz](https://github.com/yakatz)
+
 4.3.0
 -----
 
 * Add new **Classes** view. This view lists the Puppet classes that have had at least one of their resources changed (event). ([#799](https://github.com/voxpupuli/puppetboard/pull/799)).
 
 Big thanks to [Louis Charreau](https://github.com/lcharreau) who contributed the above feature!
```

### Comparing `puppetboard-4.3.0/puppetboard.egg-info/SOURCES.txt` & `puppetboard-5.0.0/puppetboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/puppetboard.egg-info/requires.txt` & `puppetboard-5.0.0/puppetboard.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-certifi==2022.12.7
-charset-normalizer==3.1.0
-click==8.1.3
+certifi==2023.7.22
+charset-normalizer==3.2.0
+click==8.1.6
 commonmark==0.9.1
-Flask==2.2.3
+Flask==2.2.5
 Flask-APScheduler==1.12.4
-Flask-Caching==2.0.1
+Flask-Caching==2.0.2
 Flask-WTF==1.1.1
 idna==3.4
 itsdangerous==2.1.2
 Jinja2==3.1.2
-MarkupSafe==2.1.2
-packaging==23.0
-pyparsing==3.0.9
+MarkupSafe==2.1.3
+packaging==23.1
+pyparsing==3.1.0
 pypuppetdb==3.1.0
-requests==2.28.2
-typing_extensions==4.5.0
-urllib3==1.26.14
-Werkzeug==2.2.3
+requests==2.31.0
+typing_extensions==4.7.1
+urllib3==2.0.4
+Werkzeug==2.3.6
 WTForms==3.0.1
-zipp==3.15.0
+zipp==3.16.2
 
 [test]
 pep8==1.7.1
-coverage==7.2.2
-mock==5.0.1
-pytest==7.2.2
-pylint==2.17.2
+coverage==7.2.7
+mock==5.1.0
+pytest==7.4.0
+pylint==2.17.5
 pytest-pylint==0.19.0
-pytest-cov==4.0.0
-pytest-mock==3.10.0
+pytest-cov==4.1.0
+pytest-mock==3.11.1
 pytest-mypy==0.10.3
-pytest-randomly==3.12.0
+pytest-randomly==3.13.0
 cov-core==1.15.0
-beautifulsoup4==4.11.2
-bandit==1.7.4
-mypy==1.0.1
-types-requests==2.28.11.15
-types-setuptools==67.6.0.7
-types-toml==0.10.8.5
+beautifulsoup4==4.12.2
+bandit==1.7.5
+mypy==1.4.1
+types-requests==2.31.0.2
+types-setuptools==68.0.0.3
+types-toml==0.10.8.7
```

### Comparing `puppetboard-4.3.0/setup.py` & `puppetboard-5.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     url='https://github.com/voxpupuli/puppetboard',
     license='Apache License 2.0',
     description='Web frontend for PuppetDB',
     include_package_data=True,
     long_description='\n'.join((README, CHANGELOG)),
     long_description_content_type='text/markdown',
     zip_safe=False,
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     install_requires=requirements,
     tests_require=requirements_test,
     extras_require={'test': requirements_test},
     data_files=[('requirements_for_tests', ['requirements-test.txt']),
                 ('requirements_for_docker', ['requirements-docker.txt'])],
     keywords="puppet puppetdb puppetboard",
     cmdclass={'test': PyTest},
@@ -64,14 +64,13 @@
         'Environment :: Web Environment',
         'Framework :: Flask',
         'Intended Audience :: System Administrators',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `puppetboard-4.3.0/test/test_app.py` & `puppetboard-5.0.0/test/test_app.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/test/test_app_error.py` & `puppetboard-5.0.0/test/test_app_error.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/test/test_core.py` & `puppetboard-5.0.0/test/test_core.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/test/test_docker_settings.py` & `puppetboard-5.0.0/test/test_docker_settings.py`

 * *Files identical despite different names*

### Comparing `puppetboard-4.3.0/test/test_utils.py` & `puppetboard-5.0.0/test/test_utils.py`

 * *Files identical despite different names*

