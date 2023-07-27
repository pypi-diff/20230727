# Comparing `tmp/jupysql_plugin-0.1.8.tar.gz` & `tmp/jupysql_plugin-0.1.9.tar.gz`

## Comparing `jupysql_plugin-0.1.8.tar` & `jupysql_plugin-0.1.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/babel.config.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/environment.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jest.config.js
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/noxfile.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/package.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/setup.cfg
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/setup.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/tsconfig.json
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/doc/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/_version.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/_widgets.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/package.json
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/122.83febd31f97f409ed32e.js
--rw-r--r--   0        0        0   448079 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js.LICENSE.txt
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js
--rw-r--r--   0        0        0    33851 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/238.47dc92159927183c530c.js
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js
--rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js.LICENSE.txt
--rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js
--rw-r--r--   0        0        0    40330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js.LICENSE.txt
--rw-r--r--   0        0        0    60929 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/520.482c287db47780739825.js
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/520.482c287db47780739825.js.LICENSE.txt
--rw-r--r--   0        0        0   237389 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js
--rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js
--rw-r--r--   0        0        0    23542 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js
--rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js
--rw-r--r--   0        0        0   228074 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js
--rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/remoteEntry.1515ab0c4408d370a1f1.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/style.js
--rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/server_handlers/dashboard.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/widgets/__init__.py
--rw-r--r--   0        0        0    10534 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupysql_plugin/widgets/connector_widget.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupyter-config/jupyter_notebook_config.d/jupysql_plugin.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/jupyter-config/jupyter_server_config.d/jupysql_plugin.json
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/comm.ts
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/connector.ts
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/customconnector.ts
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/dialog.tsx
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/extension.ts
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/formatter.ts
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/index-widgets.ts
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/index.ts
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/keywords.json
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/version.ts
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/__tests__/dialog.spec.tsx
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/__tests__/jupysql_plugin.spec.ts
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/const/env.ts
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/utils/util.ts
--rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/widgets/connector.ts
--rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/widgets/form.ts
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/src/widgets/table.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/base.css
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/connector.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/index.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/widget.css
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/icons/add_primary.svg
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/style/icons/delete_outline_black.svg
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/.gitignore
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/README.md
--rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/babel.config.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/environment.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jest.config.js
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/noxfile.py
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/package.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/setup.cfg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/setup.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/tsconfig.json
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/doc/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/_version.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/_widgets.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/package.json
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/122.83febd31f97f409ed32e.js
+-rw-r--r--   0        0        0   448079 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js.LICENSE.txt
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js
+-rw-r--r--   0        0        0    33851 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/238.f4c3f46e2fe42910e39d.js
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js.LICENSE.txt
+-rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js
+-rw-r--r--   0        0        0    40330 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js.LICENSE.txt
+-rw-r--r--   0        0        0    60929 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/520.482c287db47780739825.js
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/520.482c287db47780739825.js.LICENSE.txt
+-rw-r--r--   0        0        0   237389 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js
+-rw-r--r--   0        0        0    22082 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js
+-rw-r--r--   0        0        0    23542 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js
+-rw-r--r--   0        0        0   228074 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js
+-rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/remoteEntry.82e9a55d6d8fadd144b8.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/style.js
+-rw-r--r--   0        0        0    43486 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/server_handlers/dashboard.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/widgets/__init__.py
+-rw-r--r--   0        0        0    10677 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupysql_plugin/widgets/connector_widget.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupyter-config/jupyter_notebook_config.d/jupysql_plugin.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/jupyter-config/jupyter_server_config.d/jupysql_plugin.json
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/comm.ts
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/connector.ts
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/customconnector.ts
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/dialog.tsx
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/extension.ts
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/formatter.ts
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/index-widgets.ts
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/index.ts
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/keywords.json
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/version.ts
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/__tests__/dialog.spec.tsx
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/__tests__/jupysql_plugin.spec.ts
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/const/env.ts
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/utils/util.ts
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/widgets/connector.ts
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/widgets/form.ts
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/src/widgets/table.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/style/base.css
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/style/connector.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/style/index.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/style/widget.css
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/style/icons/add_primary.svg
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/style/icons/delete_outline_black.svg
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/README.md
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 jupysql_plugin-0.1.9/PKG-INFO
```

### Comparing `jupysql_plugin-0.1.8/RELEASE.md` & `jupysql_plugin-0.1.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jest.config.js` & `jupysql_plugin-0.1.9/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/noxfile.py` & `jupysql_plugin-0.1.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/package.json` & `jupysql_plugin-0.1.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -123,15 +123,15 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.8",
+    "version": "0.1.9",
     "workspaces": {
         "packages": [
             "jupysql_plugin",
             "ui-tests"
         ]
     }
 }
```

### Comparing `jupysql_plugin-0.1.8/tsconfig.json` & `jupysql_plugin-0.1.9/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/doc/README.md` & `jupysql_plugin-0.1.9/doc/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/__init__.py` & `jupysql_plugin-0.1.9/jupysql_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/_widgets.py` & `jupysql_plugin-0.1.9/jupysql_plugin/_widgets.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/package.json` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.82e9a55d6d8fadd144b8.js'}}",*

 * * "'version'": "'0.1.9'"}*

```diff
@@ -66,15 +66,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/ploomber/jupysql-plugin.git",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1515ab0c4408d370a1f1.js",
+            "load": "static/remoteEntry.82e9a55d6d8fadd144b8.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupysql_plugin/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
@@ -128,15 +128,15 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.8",
+    "version": "0.1.9",
     "workspaces": {
         "packages": [
             "jupysql_plugin",
             "ui-tests"
         ]
     }
 }
```

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/126.dde4a9689e634492f076.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/171.256ff36dbd88e97f7d85.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/238.47dc92159927183c530c.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/238.f4c3f46e2fe42910e39d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -865,11 +865,11 @@
             e.exports = "data:image/svg+xml,%3Csvg width='14' height='14' viewBox='0 0 14 14' fill='none' xmlns='http://www.w3.org/2000/svg'%3E %3Cpath d='M14 8H8V14H6V8H0V6H6V0H8V6H14V8Z' fill='%23206EEF'/%3E %3C/svg%3E"
         },
         9941: e => {
             e.exports = "data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' height='24px' viewBox='0 0 24 24' width='24px' fill='%23000000'%3E%3Cpath d='M0 0h24v24H0V0z' fill='none'/%3E%3Cpath d='M6 19c0 1.1.9 2 2 2h8c1.1 0 2-.9 2-2V7H6v12zM8 9h8v10H8V9zm7.5-5l-1-1h-5l-1 1H5v2h14V4z'/%3E%3C/svg%3E"
         },
         4147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"jupysql-plugin","version":"0.1.8","description":"Jupyterlab extension for JupySQL","private":true,"keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/ploomber/jupysql-plugin.git","bugs":{"url":"https://github.com/ploomber/jupysql-plugin.git/issues"},"license":"BSD-3-Clause","author":{"name":"Ploomber","email":"contact@ploomber.io"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/ploomber/jupysql-plugin.git.git"},"workspaces":{"packages":["jupysql_plugin","ui-tests"]},"scripts":{"build":"jlpm build:lib && jlpm build:labextension:dev","build:prod":"jlpm clean && jlpm build:lib:prod && jlpm build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc --sourceMap","build:lib:prod":"tsc","clean":"jlpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf jupysql_plugin/labextension jupysql_plugin/_version.py","clean:all":"jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache","eslint":"jlpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"jlpm build","lint":"jlpm stylelint && jlpm prettier && jlpm eslint","lint:check":"jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check","prettier":"jlpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"jlpm prettier:base --check","stylelint":"jlpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"@comment":{"dependencies":{"@lumino/widgets":"An official library to implement the frontend of the widgets: https://github.com/jupyterlab/lumino"}},"dependencies":{"@emotion/react":"^11.11.0","@emotion/styled":"^11.11.0","@jupyter-widgets/base":"^6.0.4","@jupyterlab/application":"^3.6.2","@jupyterlab/codeeditor":"^3.6.2","@jupyterlab/codemirror":"^3.6.3","@jupyterlab/completer":"^3.6.2","@jupyterlab/notebook":"^3.6.2","@jupyterlab/statedb":"^3.6.2","@lumino/widgets":"<2.0.0","@mui/icons-material":"^5.11.16","@mui/material":"^5.13.4","@types/codemirror":"^5.60.7","@types/underscore":"^1.11.4","bootstrap":"^5.2.3","clean":"^4.0.2","react":"^17.0.2","sql-formatter":"^12.2.0","underscore":"^1.13.6"},"devDependencies":{"@babel/core":"^7.0.0","@babel/preset-env":"^7.0.0","@jupyterlab/builder":"^3.1.0","@jupyterlab/testutils":"^3.0.0","@testing-library/jest-dom":"^5.16.5","@testing-library/react":"^12.1.2","@types/bootstrap":"^5.2.6","@types/jest":"^26.0.0","@types/jest-when":"^3.5.2","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-prettier":"^3.1.4","jest":"^26.0.0","jest-when":"^3.5.2","npm-run-all":"^4.1.5","prettier":"^2.1.1","react-dom":"^17.0.2","rimraf":"^3.0.2","stylelint":"^14.3.0","stylelint-config-prettier":"^9.0.4","stylelint-config-recommended":"^6.0.0","stylelint-config-standard":"~24.0.0","stylelint-prettier":"^2.0.0","ts-jest":"^26.0.0","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"outputDir":"jupysql_plugin/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"jupysql-plugin","version":"0.1.9","description":"Jupyterlab extension for JupySQL","private":true,"keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/ploomber/jupysql-plugin.git","bugs":{"url":"https://github.com/ploomber/jupysql-plugin.git/issues"},"license":"BSD-3-Clause","author":{"name":"Ploomber","email":"contact@ploomber.io"},"files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/ploomber/jupysql-plugin.git.git"},"workspaces":{"packages":["jupysql_plugin","ui-tests"]},"scripts":{"build":"jlpm build:lib && jlpm build:labextension:dev","build:prod":"jlpm clean && jlpm build:lib:prod && jlpm build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc --sourceMap","build:lib:prod":"tsc","clean":"jlpm clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:lintcache":"rimraf .eslintcache .stylelintcache","clean:labextension":"rimraf jupysql_plugin/labextension jupysql_plugin/_version.py","clean:all":"jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache","eslint":"jlpm eslint:check --fix","eslint:check":"eslint . --cache --ext .ts,.tsx","install:extension":"jlpm build","lint":"jlpm stylelint && jlpm prettier && jlpm eslint","lint:check":"jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check","prettier":"jlpm prettier:base --write --list-different","prettier:base":"prettier \\"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\\"","prettier:check":"jlpm prettier:base --check","stylelint":"jlpm stylelint:check --fix","stylelint:check":"stylelint --cache \\"style/**/*.css\\"","test":"jest --coverage","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"@comment":{"dependencies":{"@lumino/widgets":"An official library to implement the frontend of the widgets: https://github.com/jupyterlab/lumino"}},"dependencies":{"@emotion/react":"^11.11.0","@emotion/styled":"^11.11.0","@jupyter-widgets/base":"^6.0.4","@jupyterlab/application":"^3.6.2","@jupyterlab/codeeditor":"^3.6.2","@jupyterlab/codemirror":"^3.6.3","@jupyterlab/completer":"^3.6.2","@jupyterlab/notebook":"^3.6.2","@jupyterlab/statedb":"^3.6.2","@lumino/widgets":"<2.0.0","@mui/icons-material":"^5.11.16","@mui/material":"^5.13.4","@types/codemirror":"^5.60.7","@types/underscore":"^1.11.4","bootstrap":"^5.2.3","clean":"^4.0.2","react":"^17.0.2","sql-formatter":"^12.2.0","underscore":"^1.13.6"},"devDependencies":{"@babel/core":"^7.0.0","@babel/preset-env":"^7.0.0","@jupyterlab/builder":"^3.1.0","@jupyterlab/testutils":"^3.0.0","@testing-library/jest-dom":"^5.16.5","@testing-library/react":"^12.1.2","@types/bootstrap":"^5.2.6","@types/jest":"^26.0.0","@types/jest-when":"^3.5.2","@typescript-eslint/eslint-plugin":"^4.8.1","@typescript-eslint/parser":"^4.8.1","eslint":"^7.14.0","eslint-config-prettier":"^6.15.0","eslint-plugin-prettier":"^3.1.4","jest":"^26.0.0","jest-when":"^3.5.2","npm-run-all":"^4.1.5","prettier":"^2.1.1","react-dom":"^17.0.2","rimraf":"^3.0.2","stylelint":"^14.3.0","stylelint-config-prettier":"^9.0.4","stylelint-config-recommended":"^6.0.0","stylelint-config-standard":"~24.0.0","stylelint-prettier":"^2.0.0","ts-jest":"^26.0.0","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","publishConfig":{"access":"public"},"jupyterlab":{"extension":true,"outputDir":"jupysql_plugin/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/282.1bb9d755cf1f2c786d16.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/338.49da1189f91bad8b01b4.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/378.d4abe61f25a998d75e66.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/40.2e8dd60e0a5a8bf83e3e.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/520.482c287db47780739825.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/520.482c287db47780739825.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/646.2440cc17aba449886588.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/747.233d2b03fe10fa309835.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/794.a07de7512354fbf79bee.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/804.d8cbf6a18594a5e5e734.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/846.1e01de8e428bb8d890c8.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/906.0dfaf4363c1e58ef89b0.js`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/remoteEntry.1515ab0c4408d370a1f1.js` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/remoteEntry.82e9a55d6d8fadd144b8.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -49,15 +49,15 @@
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
         40: "2e8dd60e0a5a8bf83e3e",
         122: "83febd31f97f409ed32e",
         126: "dde4a9689e634492f076",
         171: "256ff36dbd88e97f7d85",
         211: "4b143901e7c7d43ccb73",
         222: "3135377346670d94cf92",
-        238: "47dc92159927183c530c",
+        238: "f4c3f46e2fe42910e39d",
         271: "c80d65561d8463123810",
         282: "1bb9d755cf1f2c786d16",
         338: "49da1189f91bad8b01b4",
         378: "d4abe61f25a998d75e66",
         456: "6bda2ceb2cddaccc7e9c",
         520: "482c287db47780739825",
         646: "2440cc17aba449886588",
@@ -70,15 +70,15 @@
     } [e] + ".js?v=" + {
         40: "2e8dd60e0a5a8bf83e3e",
         122: "83febd31f97f409ed32e",
         126: "dde4a9689e634492f076",
         171: "256ff36dbd88e97f7d85",
         211: "4b143901e7c7d43ccb73",
         222: "3135377346670d94cf92",
-        238: "47dc92159927183c530c",
+        238: "f4c3f46e2fe42910e39d",
         271: "c80d65561d8463123810",
         282: "1bb9d755cf1f2c786d16",
         338: "49da1189f91bad8b01b4",
         378: "d4abe61f25a998d75e66",
         456: "6bda2ceb2cddaccc7e9c",
         520: "482c287db47780739825",
         646: "2440cc17aba449886588",
@@ -143,15 +143,15 @@
                         (!i || !i.loaded && (!a != !i.eager ? a : l > i.from)) && (o[r] = {
                             get: t,
                             from: l,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([S.e(846), S.e(338), S.e(271), S.e(171)]).then((() => () => S(338))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(378), S.e(271), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@mui/material", "5.14.0", (() => Promise.all([S.e(846), S.e(804), S.e(126), S.e(40), S.e(271), S.e(211), S.e(222), S.e(456)]).then((() => () => S(7126))))), i("bootstrap", "5.3.0", (() => Promise.all([S.e(804), S.e(520)]).then((() => () => S(7520))))), i("jupysql-plugin", "0.1.8", (() => Promise.all([S.e(40), S.e(646), S.e(271), S.e(222), S.e(238)]).then((() => () => S(3238))))), i("sql-formatter", "12.2.3", (() => S.e(906).then((() => () => S(9906))))), i("underscore", "1.13.6", (() => S.e(794).then((() => () => S(7794)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (i("@emotion/react", "11.11.1", (() => Promise.all([S.e(846), S.e(338), S.e(271), S.e(171)]).then((() => () => S(338))))), i("@emotion/styled", "11.11.0", (() => Promise.all([S.e(378), S.e(271), S.e(211), S.e(799), S.e(122)]).then((() => () => S(4378))))), i("@mui/material", "5.14.0", (() => Promise.all([S.e(846), S.e(804), S.e(126), S.e(40), S.e(271), S.e(211), S.e(222), S.e(456)]).then((() => () => S(7126))))), i("bootstrap", "5.3.0", (() => Promise.all([S.e(804), S.e(520)]).then((() => () => S(7520))))), i("jupysql-plugin", "0.1.9", (() => Promise.all([S.e(40), S.e(646), S.e(271), S.e(222), S.e(238)]).then((() => () => S(3238))))), i("sql-formatter", "12.2.3", (() => S.e(906).then((() => () => S(9906))))), i("underscore", "1.13.6", (() => S.e(794).then((() => () => S(7794)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/labextension/static/third-party-licenses.json` & `jupysql_plugin-0.1.9/jupysql_plugin/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/server_handlers/dashboard.py` & `jupysql_plugin-0.1.9/jupysql_plugin/server_handlers/dashboard.py`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/jupysql_plugin/widgets/connector_widget.py` & `jupysql_plugin-0.1.9/jupysql_plugin/widgets/connector_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from jupysql_plugin import __version__, _module_name
 
 from ipywidgets import DOMWidget
 from traitlets import Unicode
 import json
-from sql.connection import Connection
 from sqlalchemy import create_engine
 from sql.parse import connection_from_dsn_section
 from configparser import ConfigParser
 from pathlib import Path
 
+try:
+    from sql.connection import SQLAlchemyConnection
+except ImportError:
+    # if using jupysql<0.9
+    from sql.connection import Connection as SQLAlchemyConnection
+
 CONNECTIONS_TEMPLATES = dict(
     {
         "sqlite": {
             "driver": "sqlite",
             "fields": [
                 {
                     "id": "connectionName",
@@ -316,15 +321,15 @@
         """
         Connects to database
         """
         name = connection["name"]
         connection_string = _get_connection_string(name)
 
         engine = create_engine(connection_string)
-        Connection(engine=engine, alias=name)
+        SQLAlchemyConnection(engine=engine, alias=name)
 
     def _delete_connection(self, connection):
         """
         Delets connection from ini file
         """
         connection_name = connection["name"]
```

### Comparing `jupysql_plugin-0.1.8/src/comm.ts` & `jupysql_plugin-0.1.9/src/comm.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/connector.ts` & `jupysql_plugin-0.1.9/src/connector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/customconnector.ts` & `jupysql_plugin-0.1.9/src/customconnector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/dialog.tsx` & `jupysql_plugin-0.1.9/src/dialog.tsx`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/formatter.ts` & `jupysql_plugin-0.1.9/src/formatter.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/index.ts` & `jupysql_plugin-0.1.9/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/keywords.json` & `jupysql_plugin-0.1.9/src/keywords.json`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/__tests__/dialog.spec.tsx` & `jupysql_plugin-0.1.9/src/__tests__/dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/utils/util.ts` & `jupysql_plugin-0.1.9/src/utils/util.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/widgets/connector.ts` & `jupysql_plugin-0.1.9/src/widgets/connector.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/widgets/form.ts` & `jupysql_plugin-0.1.9/src/widgets/form.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/src/widgets/table.ts` & `jupysql_plugin-0.1.9/src/widgets/table.ts`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/style/connector.css` & `jupysql_plugin-0.1.9/style/connector.css`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/.gitignore` & `jupysql_plugin-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/LICENSE` & `jupysql_plugin-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/README.md` & `jupysql_plugin-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/pyproject.toml` & `jupysql_plugin-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql_plugin-0.1.8/PKG-INFO` & `jupysql_plugin-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql-plugin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Jupyterlab extension for JupySQL
 Project-URL: Homepage, https://github.com/ploomber/jupysql-plugin.git
 Project-URL: Bug Tracker, https://github.com/ploomber/jupysql-plugin.git/issues
 Project-URL: Repository, https://github.com/ploomber/jupysql-plugin.git.git
 Author-email: Ploomber <contact@ploomber.io>
 License: BSD 3-Clause License
```

