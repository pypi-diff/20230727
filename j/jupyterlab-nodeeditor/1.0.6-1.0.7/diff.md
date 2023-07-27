# Comparing `tmp/jupyterlab_nodeeditor-1.0.6.tar.gz` & `tmp/jupyterlab_nodeeditor-1.0.7.tar.gz`

## Comparing `jupyterlab_nodeeditor-1.0.6.tar` & `jupyterlab_nodeeditor-1.0.7.tar`

### file list

```diff
@@ -1,444 +1,444 @@
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.copier-answers.yml
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.gitmodules
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/CHANGELOG.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/RELEASE.md
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/dev.sh
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/init.sh
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/install.json
--rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/package.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/setup.py
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/tsconfig.json
--rwxr-xr-x   0        0        0   215696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/yarn.lock
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.vscode/settings.json
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.copier-answers.yml
--rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.gitignore
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/CHANGELOG.md
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/LICENSE
--rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/README.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/RELEASE.md
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/install.json
--rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/package.json
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/pyproject.toml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/setup.py
--rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/tsconfig.json
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/schema/plugin.json
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/src/index.ts
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/style/base.css
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/_temp_extension/style/index.js
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.babelrc
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.editorconfig
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.eslintrc
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.git
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.gitignore
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.npmignore
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.nvmrc
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/.travis.yml
--rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/LICENSE
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/README.md
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress.json
--rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/logo.ai
--rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/logo.png
--rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/logo.svg
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/package.json
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/rollup.config.js
--rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/yarn.lock
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/fixtures/example.json
--rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/integration/NodeEditorSpec.js
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/plugins/index.js
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/support/commands.js
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/cypress/support/index.js
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/.gitignore
--rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/README.md
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/babel.config.js
--rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docusaurus.config.js
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/package.json
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/sidebars.js
--rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/yarn.lock
--rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/blog/2019-05-28-hola.md
--rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/blog/2019-05-29-hello-world.md
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/blog/2019-05-30-welcome.md
--rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/AnatomyExample.js
--rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/Colors.js
--rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/ControlExamples.js
--rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicNodesExamples.js
--rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicThemingExample.js
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/FlexRow.js
--rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/components/GettingStartedExample.js
--rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/NodeEditor.mdx
--rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/RootEngine.mdx
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/anatomy.mdx
--rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/basic-config.mdx
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/colors.mdx
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/comments.mdx
--rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/controls.mdx
--rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/defining-nodes.mdx
--rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc1.md
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc2.md
--rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc3.md
--rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/dynamic-nodes.mdx
--rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/faq.mdx
--rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/flume-config.mdx
--rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/logic-nodes.mdx
--rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/mdx.md
--rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/node-editor.mdx
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/overview.mdx
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/quick-start.mdx
--rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-engine.mdx
--rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-node.mdx
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/running-logic.mdx
--rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/saving-nodes.mdx
--rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/theming.mdx
--rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/type-safety.mdx
--rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-with-react.mdx
--rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-without-react.mdx
--rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/exampleFlumeConfig.js
--rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/components/TypeSafe.js
--rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/css/custom.css
--rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/index.js
--rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/styles.module.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/.nojekyll
--rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/60fps.svg
--rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-192x192.png
--rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-512x512.png
--rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/apple-touch-icon.png
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-blue.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-green.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-red.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right-red_1.svg
--rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/arrow-right.svg
--rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/controls.svg
--rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/example_editors.png
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon-16x16.png
--rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon-32x32.png
--rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon.ico
--rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/fb-img.png
--rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/flume-short-web.mp4
--rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/friends-graph.svg
--rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/hero-nodes.svg
--rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo-dark.svg
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo.svg
--rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/netlify.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/page-curve-blue.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/page-curve-dark.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/page-curve.svg
--rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/performance-tile.svg
--rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/play-icon.svg
--rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/react-tile.svg
--rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/size-tile.svg
--rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme-tile.svg
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme.svg
--rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-node.svg
--rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-nodes.svg
--rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_mountain.svg
--rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_react.svg
--rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_tree.svg
--rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/valid_port_types.png
--rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/wordmark_white.svg
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/.eslintrc
--rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/README.md
--rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/package.json
--rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/yarn.lock
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/public/index.html
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/public/manifest.json
--rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/App.js
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/index.css
--rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/index.js
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/TestEditor.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/nodes.js
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Checkbox.js
--rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/FloatingNavigation.js
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Header.js
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/LogicEditor.js
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Modal.js
--rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/components/OptionsEditor.js
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/BoxIcon.js
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/FormIcon.js
--rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/GearIcon.js
--rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Attributes.js
--rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Body.js
--rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Field.js
--rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.css
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.js
--rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/InputTypes.js
--rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/NodeTypes.js
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/PreviewField.js
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Sidebar.js
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/defaultNodes.js
--rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/designerReducer.js
--rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldTypes.js
--rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldsReducer.js
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/formHandler.js
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/previewFieldsReducer.js
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/resolveLogic.js
--rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/wizardLogic/logicTypes.js
--rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.css
--rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.js
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.css
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.js
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/.eslintrc
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/Cache.js
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/RootEngine.js
--rwxr-xr-x   0        0        0     2060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/commentsReducer.js
--rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/connectionCalculator.js
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/constants.js
--rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/context.js
--rwxr-xr-x   0        0        0     9649 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/index.js
--rwxr-xr-x   0        0        0    14282 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/nodesReducer.js
--rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/stageReducer.js
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/styles.css
--rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/toastsReducer.js
--rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/typeBuilders.js
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/utilities.js
--rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Checkbox/Checkbox.css
--rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Checkbox/Checkbox.js
--rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.css
--rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.js
--rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.css
--rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.js
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connection/Connection.css
--rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connection/Connection.js
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connections/Connections.css
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Connections/Connections.js
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.css
--rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.js
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Control/Control.css
--rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Control/Control.js
--rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Draggable/Draggable.js
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.css
--rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.js
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Node/Node.css
--rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Node/Node.js
--rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.css
--rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.js
--rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.css
--rwxr-xr-x   0        0        0     9421 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.js
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/TextInput/TextInput.css
--rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/TextInput/TextInput.js
--rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.css
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.js
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/hooks/usePrevious.js
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/img/grid.png
--rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/dynamic.test.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/nodes.js
--rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/ssr.test.js
--rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/flume/src/tests/test.js
--rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/_version.py
--rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/select.py
--rwxr-xr-x   0        0        0     3962 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/utils.py
--rwxr-xr-x   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/package.json
--rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
--rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
--rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
--rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
--rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
--rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
--rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js
--rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js
--rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
--rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
--rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
--rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
--rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
--rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
--rwxr-xr-x   0        0        0   216372 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8863.82c89f078a753cb91d3d.js
--rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
--rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
--rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    13292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/remoteEntry.80729a1327f495afa265.js
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/style.js
--rwxr-xr-x   0        0        0     9868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
--rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/schema/plugin.json
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/ReRunIcon.tsx
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/arrownIcon.tsx
--rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/clearIcon.tsx
--rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/deleteIcon.tsx
--rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/exportIcon.tsx
--rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/factory.ts
--rwxr-xr-x   0        0        0    41954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/flumeConfig.tsx
--rwxr-xr-x   0        0        0     7454 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/imageViewer.tsx
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/index.ts
--rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/lockIcon.tsx
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/model.ts
--rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/newIcon.tsx
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/runIcon.tsx
--rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/utils.tsx
--rwxr-xr-x   0        0        0   176897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/widget.tsx
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/src/yesIcon.tsx
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/style/base.css
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/style/index.js
--rwxr-xr-x   0        0        0   254494 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/1.jpeg
--rwxr-xr-x   0        0        0   153675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/2.jpeg
--rwxr-xr-x   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/main.ipynb
--rwxr-xr-x   0        0        0   546624 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/test_ext/testlib.ipynb
--rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/.gitignore
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/LICENSE
--rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/README.md
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.copier-answers.yml
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.gitmodules
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/CHANGELOG.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/RELEASE.md
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/dev.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/init.sh
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/install.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/package.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/setup.py
+-rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/tsconfig.json
+-rwxr-xr-x   0        0        0   215696 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/yarn.lock
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.vscode/settings.json
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.copier-answers.yml
+-rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.gitignore
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/LICENSE
+-rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/README.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/RELEASE.md
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/install.json
+-rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/package.json
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/setup.py
+-rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/tsconfig.json
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/schema/plugin.json
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/src/index.ts
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/style/base.css
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/_temp_extension/style/index.js
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.babelrc
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.editorconfig
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.eslintrc
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.git
+-rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.gitignore
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.npmignore
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.nvmrc
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/.travis.yml
+-rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/LICENSE
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/README.md
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress.json
+-rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/logo.ai
+-rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/logo.png
+-rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/logo.svg
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/package.json
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/rollup.config.js
+-rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/yarn.lock
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/fixtures/example.json
+-rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/integration/NodeEditorSpec.js
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/plugins/index.js
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/support/commands.js
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/cypress/support/index.js
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/.gitignore
+-rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/README.md
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/babel.config.js
+-rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docusaurus.config.js
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/package.json
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/sidebars.js
+-rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/yarn.lock
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/blog/2019-05-28-hola.md
+-rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/blog/2019-05-29-hello-world.md
+-rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/blog/2019-05-30-welcome.md
+-rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/AnatomyExample.js
+-rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/Colors.js
+-rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/ControlExamples.js
+-rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicNodesExamples.js
+-rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicThemingExample.js
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/FlexRow.js
+-rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/components/GettingStartedExample.js
+-rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/NodeEditor.mdx
+-rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/RootEngine.mdx
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/anatomy.mdx
+-rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/basic-config.mdx
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/colors.mdx
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/comments.mdx
+-rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/controls.mdx
+-rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/defining-nodes.mdx
+-rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc1.md
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc2.md
+-rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc3.md
+-rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/dynamic-nodes.mdx
+-rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/faq.mdx
+-rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/flume-config.mdx
+-rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/logic-nodes.mdx
+-rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/mdx.md
+-rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/node-editor.mdx
+-rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/overview.mdx
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/quick-start.mdx
+-rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-engine.mdx
+-rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-node.mdx
+-rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/running-logic.mdx
+-rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/saving-nodes.mdx
+-rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/theming.mdx
+-rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/type-safety.mdx
+-rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-with-react.mdx
+-rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-without-react.mdx
+-rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/exampleFlumeConfig.js
+-rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/components/TypeSafe.js
+-rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/css/custom.css
+-rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/index.js
+-rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/styles.module.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/.nojekyll
+-rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/60fps.svg
+-rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-192x192.png
+-rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-512x512.png
+-rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/apple-touch-icon.png
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-blue.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-green.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-red.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right-red_1.svg
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/arrow-right.svg
+-rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/controls.svg
+-rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/example_editors.png
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon-16x16.png
+-rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon-32x32.png
+-rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon.ico
+-rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/fb-img.png
+-rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/flume-short-web.mp4
+-rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/friends-graph.svg
+-rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/hero-nodes.svg
+-rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo-dark.svg
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo.svg
+-rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/netlify.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/page-curve-blue.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/page-curve-dark.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/page-curve.svg
+-rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/performance-tile.svg
+-rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/play-icon.svg
+-rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/react-tile.svg
+-rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/size-tile.svg
+-rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme-tile.svg
+-rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme.svg
+-rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-node.svg
+-rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-nodes.svg
+-rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_mountain.svg
+-rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_react.svg
+-rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_tree.svg
+-rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/valid_port_types.png
+-rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/wordmark_white.svg
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/.eslintrc
+-rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/README.md
+-rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/package.json
+-rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/yarn.lock
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/public/index.html
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/public/manifest.json
+-rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/App.js
+-rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/index.css
+-rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/index.js
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/TestEditor.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/nodes.js
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Checkbox.js
+-rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/FloatingNavigation.js
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Header.js
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/LogicEditor.js
+-rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Modal.js
+-rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/components/OptionsEditor.js
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/BoxIcon.js
+-rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/FormIcon.js
+-rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/GearIcon.js
+-rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Attributes.js
+-rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Body.js
+-rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Field.js
+-rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.css
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.js
+-rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/InputTypes.js
+-rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/NodeTypes.js
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/PreviewField.js
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Sidebar.js
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/defaultNodes.js
+-rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/designerReducer.js
+-rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldTypes.js
+-rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldsReducer.js
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/formHandler.js
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/previewFieldsReducer.js
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/resolveLogic.js
+-rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/wizardLogic/logicTypes.js
+-rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.css
+-rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.js
+-rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.css
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.js
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/.eslintrc
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/Cache.js
+-rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/RootEngine.js
+-rwxr-xr-x   0        0        0     2060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/commentsReducer.js
+-rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/connectionCalculator.js
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/constants.js
+-rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/context.js
+-rwxr-xr-x   0        0        0     9649 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/index.js
+-rwxr-xr-x   0        0        0    14282 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/nodesReducer.js
+-rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/stageReducer.js
+-rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/styles.css
+-rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/toastsReducer.js
+-rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/typeBuilders.js
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/utilities.js
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Checkbox/Checkbox.css
+-rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Checkbox/Checkbox.js
+-rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.css
+-rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.js
+-rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.css
+-rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.js
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connection/Connection.css
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connection/Connection.js
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connections/Connections.css
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Connections/Connections.js
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.css
+-rwxr-xr-x   0        0        0     7071 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.js
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Control/Control.css
+-rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Control/Control.js
+-rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Draggable/Draggable.js
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.css
+-rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.js
+-rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Node/Node.css
+-rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Node/Node.js
+-rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.css
+-rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.js
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.css
+-rwxr-xr-x   0        0        0     9421 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.js
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/TextInput/TextInput.css
+-rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/TextInput/TextInput.js
+-rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.css
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.js
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/hooks/usePrevious.js
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/img/grid.png
+-rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/dynamic.test.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/nodes.js
+-rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/ssr.test.js
+-rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/flume/src/tests/test.js
+-rwxr-xr-x   0        0        0      205 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/_version.py
+-rwxr-xr-x   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/select.py
+-rwxr-xr-x   0        0        0     3962 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/utils.py
+-rwxr-xr-x   0        0        0     5572 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/package.json
+-rwxr-xr-x   0        0        0     6248 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
+-rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
+-rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
+-rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
+-rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js
+-rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7177 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js
+-rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
+-rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
+-rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0   220449 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8863.6ed3cbfeea198a6b6e21.js
+-rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
+-rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
+-rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    13292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/remoteEntry.05ee5c7186d725a070e5.js
+-rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/style.js
+-rwxr-xr-x   0        0        0     9868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
+-rwxr-xr-x   0        0        0     7391 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/schema/plugin.json
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/ReRunIcon.tsx
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/arrownIcon.tsx
+-rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/clearIcon.tsx
+-rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/deleteIcon.tsx
+-rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/exportIcon.tsx
+-rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/factory.ts
+-rwxr-xr-x   0        0        0    51346 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/flumeConfig.tsx
+-rwxr-xr-x   0        0        0     8089 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/imageViewer.tsx
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/index.ts
+-rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/lockIcon.tsx
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/model.ts
+-rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/newIcon.tsx
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/runIcon.tsx
+-rwxr-xr-x   0        0        0     2544 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/utils.tsx
+-rwxr-xr-x   0        0        0   182475 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/widget.tsx
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/src/yesIcon.tsx
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/style/base.css
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/style/index.js
+-rwxr-xr-x   0        0        0   254494 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/1.jpeg
+-rwxr-xr-x   0        0        0   153675 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/2.jpeg
+-rwxr-xr-x   0        0        0     2162 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/main.ipynb
+-rwxr-xr-x   0        0        0   546624 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/test_ext/testlib.ipynb
+-rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/.gitignore
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/LICENSE
+-rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/README.md
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.7/PKG-INFO
```

### Comparing `jupyterlab_nodeeditor-1.0.6/RELEASE.md` & `jupyterlab_nodeeditor-1.0.7/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/package.json` & `jupyterlab_nodeeditor-1.0.7/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.7'"}*

```diff
@@ -175,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.6"
+    "version": "1.0.7"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.6/tsconfig.json` & `jupyterlab_nodeeditor-1.0.7/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/yarn.lock` & `jupyterlab_nodeeditor-1.0.7/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/.gitignore` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/LICENSE` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/README.md` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/RELEASE.md` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/package.json` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/pyproject.toml` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/tsconfig.json` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/jupyterlab_nodeeditor/__init__.py` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/jupyterlab_nodeeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/_temp_extension/src/index.ts` & `jupyterlab_nodeeditor-1.0.7/_temp_extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/CODE_OF_CONDUCT.md` & `jupyterlab_nodeeditor-1.0.7/flume/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/LICENSE` & `jupyterlab_nodeeditor-1.0.7/flume/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/README.md` & `jupyterlab_nodeeditor-1.0.7/flume/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/logo.ai` & `jupyterlab_nodeeditor-1.0.7/flume/logo.ai`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/logo.png` & `jupyterlab_nodeeditor-1.0.7/flume/logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/logo.svg` & `jupyterlab_nodeeditor-1.0.7/flume/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/package.json` & `jupyterlab_nodeeditor-1.0.7/flume/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/rollup.config.js` & `jupyterlab_nodeeditor-1.0.7/flume/rollup.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/yarn.lock` & `jupyterlab_nodeeditor-1.0.7/flume/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/cypress/integration/NodeEditorSpec.js` & `jupyterlab_nodeeditor-1.0.7/flume/cypress/integration/NodeEditorSpec.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/cypress/plugins/index.js` & `jupyterlab_nodeeditor-1.0.7/flume/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/cypress/support/commands.js` & `jupyterlab_nodeeditor-1.0.7/flume/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/cypress/support/index.js` & `jupyterlab_nodeeditor-1.0.7/flume/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/README.md` & `jupyterlab_nodeeditor-1.0.7/flume/docs/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docusaurus.config.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/package.json` & `jupyterlab_nodeeditor-1.0.7/flume/docs/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/yarn.lock` & `jupyterlab_nodeeditor-1.0.7/flume/docs/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/components/AnatomyExample.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/components/AnatomyExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/components/Colors.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/components/Colors.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/components/ControlExamples.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/components/ControlExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicNodesExamples.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicNodesExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/components/DynamicThemingExample.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/components/DynamicThemingExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/components/GettingStartedExample.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/components/GettingStartedExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/NodeEditor.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/NodeEditor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/RootEngine.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/RootEngine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/anatomy.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/anatomy.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/basic-config.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/basic-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/colors.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/colors.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/comments.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/comments.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/controls.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/controls.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/defining-nodes.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/defining-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc1.md` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc1.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/doc3.md` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/doc3.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/dynamic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/dynamic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/faq.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/faq.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/flume-config.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/flume-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/logic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/logic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/mdx.md` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/mdx.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/node-editor.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/node-editor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/overview.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/overview.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/quick-start.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/quick-start.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-engine.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-engine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/root-node.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/root-node.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/running-logic.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/running-logic.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/saving-nodes.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/saving-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/theming.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/theming.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/type-safety.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/type-safety.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-with-react.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-with-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/docs/using-without-react.mdx` & `jupyterlab_nodeeditor-1.0.7/flume/docs/docs/using-without-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/src/exampleFlumeConfig.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/src/exampleFlumeConfig.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/src/components/TypeSafe.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/src/components/TypeSafe.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/src/css/custom.css` & `jupyterlab_nodeeditor-1.0.7/flume/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/index.js` & `jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/src/pages/styles.module.css` & `jupyterlab_nodeeditor-1.0.7/flume/docs/src/pages/styles.module.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/60fps.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/60fps.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-192x192.png` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/android-chrome-512x512.png` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/apple-touch-icon.png` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/controls.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/controls.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/example_editors.png` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/example_editors.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon-32x32.png` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/favicon.ico` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/fb-img.png` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/fb-img.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/flume-short-web.mp4` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/flume-short-web.mp4`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/friends-graph.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/friends-graph.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/hero-nodes.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/hero-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo-dark.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/logo.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/netlify.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/netlify.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/performance-tile.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/performance-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/react-tile.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/react-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/size-tile.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/size-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme-tile.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/theme.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/theme.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-node.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-node.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/type-safe-nodes.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/type-safe-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_mountain.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_react.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/undraw_docusaurus_tree.svg` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/docs/static/img/valid_port_types.png` & `jupyterlab_nodeeditor-1.0.7/flume/docs/static/img/valid_port_types.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/README.md` & `jupyterlab_nodeeditor-1.0.7/flume/example/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/package.json` & `jupyterlab_nodeeditor-1.0.7/flume/example/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/yarn.lock` & `jupyterlab_nodeeditor-1.0.7/flume/example/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/public/index.html` & `jupyterlab_nodeeditor-1.0.7/flume/example/public/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/App.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/App.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/index.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/TestEditor.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/TestEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/TestRoutes/nodes.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/TestRoutes/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/Checkbox.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/FloatingNavigation.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/FloatingNavigation.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/LogicEditor.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/LogicEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/components/OptionsEditor.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/components/OptionsEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/BoxIcon.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/BoxIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/FormIcon.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/FormIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/icons/GearIcon.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/icons/GearIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Attributes.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Attributes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Body.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Body.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Field.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Field.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.css` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Form.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Form.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/InputTypes.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/InputTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/NodeTypes.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/NodeTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/PreviewField.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/PreviewField.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/Sidebar.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/Sidebar.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/designerReducer.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/designerReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldTypes.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/fieldsReducer.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/fieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/previewFieldsReducer.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/previewFieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/resolveLogic.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/resolveLogic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Form/wizardLogic/logicTypes.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Form/wizardLogic/logicTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.css` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Forms/Forms.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Forms/Forms.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.css` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/example/src/pages/Records/Records.js` & `jupyterlab_nodeeditor-1.0.7/flume/example/src/pages/Records/Records.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/RootEngine.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/RootEngine.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/commentsReducer.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/commentsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/connectionCalculator.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/connectionCalculator.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/context.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/context.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/index.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/nodesReducer.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/nodesReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/toastsReducer.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/toastsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/typeBuilders.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/typeBuilders.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/utilities.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/utilities.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Checkbox/Checkbox.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Checkbox/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.css` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/ColorPicker/ColorPicker.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/ColorPicker/ColorPicker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.css` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Comment/Comment.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Comment/Comment.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Connection/Connection.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Connection/Connection.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.css` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/ContextMenu/ContextMenu.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/ContextMenu/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Control/Control.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Control/Control.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Draggable/Draggable.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Draggable/Draggable.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.css` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/IoPorts/IoPorts.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/IoPorts/IoPorts.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Node/Node.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Node/Node.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.css` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Select/Select.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Select/Select.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.css` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Stage/Stage.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Stage/Stage.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/TextInput/TextInput.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/TextInput/TextInput.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.css` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/components/Toaster/Toaster.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/components/Toaster/Toaster.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/tests/dynamic.test.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/tests/dynamic.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/tests/nodes.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/tests/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/tests/ssr.test.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/tests/ssr.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/flume/src/tests/test.js` & `jupyterlab_nodeeditor-1.0.7/flume/src/tests/test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/select.py` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/select.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/utils.py` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/utils.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/package.json` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.05ee5c7186d725a070e5.js'}}",*

 * * "'version'": "'1.0.7'"}*

```diff
@@ -107,15 +107,15 @@
         "schema/**/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_nodeeditor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.80729a1327f495afa265.js",
+            "load": "static/remoteEntry.05ee5c7186d725a070e5.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_nodeeditor/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -180,9 +180,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.6"
+    "version": "1.0.7"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.7'"}*

```diff
@@ -175,9 +175,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.6"
+    "version": "1.0.7"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5600.cb8c4c5c969d7f385fe8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5794.4a7528c68458a721936d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8863.82c89f078a753cb91d3d.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8863.6ed3cbfeea198a6b6e21.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -38,26 +38,26 @@
                     var o = document.head || document.getElementsByTagName("head")[0],
                         r = document.createElement("style");
                     r.type = "text/css", "top" === n && o.firstChild ? o.insertBefore(r, o.firstChild) : o.appendChild(r), r.styleSheet ? r.styleSheet.cssText = e : r.appendChild(document.createTextNode(e))
                 }
             }
             h(".Stage_wrapper__1X5K_ {\n  width: 100%;\n  height: 100%;\n  min-height: 100px;\n  background-color: #292C33;\n  /* background-image: linear-gradient(\n      0deg,\n      transparent 24%,\n      rgba(255, 255, 255, 0.04) 25%,\n      rgba(255, 255, 255, 0.04) 26%,\n      transparent 27%,\n      transparent 74%,\n      rgba(255, 255, 255, 0.04) 75%,\n      rgba(255, 255, 255, 0.04) 76%,\n      transparent 77%,\n      transparent\n    ),\n    linear-gradient(\n      90deg,\n      transparent 24%,\n      rgba(255, 255, 255, 0.04) 25%,\n      rgba(255, 255, 255, 0.04) 26%,\n      transparent 27%,\n      transparent 74%,\n      rgba(255, 255, 255, 0.04) 75%,\n      rgba(255, 255, 255, 0.04) 76%,\n      transparent 77%,\n      transparent\n    ); */\n  color: #000;\n  background-size: 30px 30px;\n  position: relative;\n  overflow: hidden;\n  -webkit-overflow-scrolling: touch;\n  font-family: Helvetica, sans-serif;\n  text-align: left;\n  line-height: 1;\n  outline: none !important;\n}\n.Stage_wrapper__1X5K_ * {\n  box-sizing: border-box;\n}\n.Stage_wrapper__1X5K_ input,\ntextarea,\nselect {\n  font-family: Helvetica, sans-serif;\n}\n.Stage_transformWrapper__3CfIp {\n  transform-origin: center center;\n  position: absolute;\n  left: 50%;\n  top: 50%;\n  width: 0px;\n  height: 0px;\n}\n.Stage_scaleWrapper__2Y7Ck {\n  position: absolute;\n  left: 0px;\n  top: 0px;\n  width: 0px;\n  height: 0px;\n}\n");
             var f = !("undefined" == typeof window || !window.document || !window.document.createElement),
-                m = function() {
+                g = function() {
                     function e(e, t) {
                         for (var n = 0; n < t.length; n++) {
                             var o = t[n];
                             o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                         }
                     }
                     return function(t, n, o) {
                         return n && e(t.prototype, n), o && e(t, o), t
                     }
                 }(),
-                g = function(e) {
+                m = function(e) {
                     function t() {
                         return function(e, t) {
                                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                             }(this, t),
                             function(e, t) {
                                 if (!e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                                 return !t || "object" != typeof t && "function" != typeof t ? e : t
@@ -69,27 +69,27 @@
                             constructor: {
                                 value: e,
                                 enumerable: !1,
                                 writable: !0,
                                 configurable: !0
                             }
                         }), t && (Object.setPrototypeOf ? Object.setPrototypeOf(e, t) : e.__proto__ = t)
-                    }(t, e), m(t, [{
+                    }(t, e), g(t, [{
                         key: "componentWillUnmount",
                         value: function() {
                             this.defaultNode && document.body.removeChild(this.defaultNode), this.defaultNode = null
                         }
                     }, {
                         key: "render",
                         value: function() {
                             return f ? (this.props.node || this.defaultNode || (this.defaultNode = document.createElement("div"), document.body.appendChild(this.defaultNode)), l().createPortal(this.props.children, this.props.node || this.defaultNode)) : null
                         }
                     }]), t
                 }(r().Component);
-            g.propTypes = {
+            m.propTypes = {
                 children: a().node.isRequired,
                 node: a().any
             };
             var y = function() {
                     function e(e, t) {
                         for (var n = 0; n < t.length; n++) {
                             var o = t[n];
@@ -149,15 +149,15 @@
                         }
                     }]), t
                 }(r().Component);
             E.propTypes = {
                 children: a().node.isRequired,
                 node: a().any
             };
-            var b = l().createPortal ? g : E,
+            var b = l().createPortal ? m : E,
                 v = function() {
                     function e(e, t) {
                         for (var n = 0; n < t.length; n++) {
                             var o = t[n];
                             o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                         }
                     }
@@ -260,49 +260,49 @@
             }, x.defaultProps = {
                 onOpen: function() {},
                 onClose: function() {}
             };
             h(".ContextMenu_menuWrapper__1BheJ{\n  position: fixed;\n  z-index: 9999;\n  background: rgba(29, 32, 34, 0.95);\n  border-radius: 5px;\n  box-shadow: 0px 6px 7px rgba(0,0,0,.3);\n  border: 1px solid rgba(0,0,0,.4);\n  font-size: 14px;\n  max-width: 600px;\n  min-width: 400px;\n  font-family: Helvetica, sans-serif;\n  line-height: 1.15;\n  outline: none;\n}\n@supports (backdrop-filter: blur(6px)){\n  .ContextMenu_menuWrapper__1BheJ{\n    backdrop-filter: blur(6px);\n    background: rgba(29, 32, 34, 0.8);\n  }\n}\n.ContextMenu_menuHeader__1Cw58{\n  padding: 5px;\n  border-bottom: 1px solid rgba(255,255,255,.1);\n  display: flex;\n  flex-direction: column;\n}\n.ContextMenu_menuLabel__158Pv{\n  margin: 0px;\n  color: #fff;\n  font-size: 16px;\n  font-weight: 600;\n}\n.ContextMenu_optionsWrapper__2YK_z{\n  max-height: 300px;\n  overflow-y: auto;\n  display: flex;\n  flex-direction: column;\n}\n.ContextMenu_menuFilter__1goBp{\n  border: none;\n  background: none;\n  height: 24px;\n  flex: 1 1 auto;\n  width: 100%;\n  outline: none;\n  color: #fff;\n}\n.ContextMenu_menuFilter__1goBp::placeholder{\n    font-style: italic;\n  }\n.ContextMenu_option__33MDL{\n  display: flex;\n  flex-direction: column;\n  flex-shrink: 0;\n  padding: 5px;\n  border-bottom: 1px solid rgba(255,255,255,.1);\n  color: #ffffff;\n}\n.ContextMenu_option__33MDL:last-child{\n    border-bottom: none;\n  }\n.ContextMenu_option__33MDL:hover{\n    background: rgba(255,255,255,.05);\n  }\n.ContextMenu_option__33MDL label{\n    margin-bottom: 5px;\n    user-select: none;\n  }\n.ContextMenu_option__33MDL label:last-child{\n      margin-bottom: 0px;\n    }\n.ContextMenu_option__33MDL p{\n    margin: 0px;\n    font-style: italic;\n    font-size: 12px;\n    color: rgb(182, 186, 194);\n    user-select: none;\n  }\n.ContextMenu_option__33MDL[data-selected=true]{\n    background: rgba(255,255,255,.05);\n  }\n.ContextMenu_emptyText__2rcXy{\n  color: #fff;\n  padding: 5px;\n}\n");
             var C = /\s/,
                 O = /^\s+/,
-                D = function(e) {
+                N = function(e) {
                     return e ? e.slice(0, function(e) {
                         for (var t = e.length; t-- && C.test(e.charAt(t)););
                         return t
                     }(e) + 1).replace(O, "") : e
                 },
-                N = function(e) {
+                D = function(e) {
                     var t = typeof e;
                     return null != e && ("object" == t || "function" == t)
                 },
                 w = "undefined" != typeof globalThis ? globalThis : "undefined" != typeof window ? window : void 0 !== n.g ? n.g : "undefined" != typeof self ? self : {};
 
             function M(e, t) {
                 return e(t = {
                     exports: {}
                 }, t.exports), t.exports
             }
             var I = "object" == typeof w && w && w.Object === Object && w,
                 T = "object" == typeof self && self && self.Object === Object && self,
                 P = I || T || Function("return this")(),
                 R = P.Symbol,
-                A = Object.prototype,
-                S = A.hasOwnProperty,
-                k = A.toString,
+                k = Object.prototype,
+                S = k.hasOwnProperty,
+                A = k.toString,
                 L = R ? R.toStringTag : void 0,
                 B = Object.prototype.toString,
                 W = R ? R.toStringTag : void 0,
                 K = function(e) {
                     return null == e ? void 0 === e ? "[object Undefined]" : "[object Null]" : W && W in Object(e) ? function(e) {
                         var t = S.call(e, L),
                             n = e[L];
                         try {
                             e[L] = void 0
                         } catch (e) {}
-                        var o = k.call(e);
+                        var o = A.call(e);
                         return t ? e[L] = n : delete e[L], o
                     }(e) : function(e) {
                         return B.call(e)
                     }(e)
                 },
                 U = function(e) {
                     return null != e && "object" == typeof e
@@ -310,31 +310,31 @@
                 j = function(e) {
                     return "symbol" == typeof e || U(e) && "[object Symbol]" == K(e)
                 },
                 V = /^[-+]0x[0-9a-f]+$/i,
                 $ = /^0b[01]+$/i,
                 z = /^0o[0-7]+$/i,
                 F = parseInt,
-                q = function(e) {
+                X = function(e) {
                     if ("number" == typeof e) return e;
                     if (j(e)) return NaN;
-                    if (N(e)) {
+                    if (D(e)) {
                         var t = "function" == typeof e.valueOf ? e.valueOf() : e;
-                        e = N(t) ? t + "" : t
+                        e = D(t) ? t + "" : t
                     }
                     if ("string" != typeof e) return 0 === e ? e : +e;
-                    e = D(e);
+                    e = N(e);
                     var n = $.test(e);
                     return n || z.test(e) ? F(e.slice(2), n ? 2 : 8) : V.test(e) ? NaN : +e
                 },
-                X = function(e, t, n) {
-                    return void 0 === n && (n = t, t = void 0), void 0 !== n && (n = (n = q(n)) == n ? n : 0), void 0 !== t && (t = (t = q(t)) == t ? t : 0),
+                q = function(e, t, n) {
+                    return void 0 === n && (n = t, t = void 0), void 0 !== n && (n = (n = X(n)) == n ? n : 0), void 0 !== t && (t = (t = X(t)) == t ? t : 0),
                         function(e, t, n) {
                             return e == e && (void 0 !== n && (e = e <= n ? e : n), void 0 !== t && (e = e >= t ? e : t)), e
-                        }(q(e), t, n)
+                        }(X(e), t, n)
                 };
             let Y = (e = 21) => {
                 let t = "",
                     n = e;
                 for (; n--;) t += "useandom-26T198340PX75pxJACKVERYMINDBUSHWOLF_GQZbfghjklqvwyzrict" [64 * Math.random() | 0];
                 return t
             };
@@ -427,123 +427,123 @@
                         u = e.hideHeader,
                         c = e.hideFilter,
                         d = e.emptyText,
                         _ = e.from,
                         p = void 0 === _ ? null : _,
                         h = e.onFilter,
                         f = void 0 === h ? null : h,
-                        m = r().useContext(ie),
-                        g = r().useRef(),
+                        g = r().useContext(ie),
+                        m = r().useRef(),
                         y = r().useRef(),
                         E = r().useRef(),
                         b = r().useState(""),
                         v = _e(b, 2),
                         x = v[0],
                         C = v[1],
                         O = r().useState(0),
-                        D = _e(O, 2),
-                        N = D[0],
-                        w = D[1],
+                        N = _e(O, 2),
+                        D = N[0],
+                        w = N[1],
                         M = r().useState(0),
                         I = _e(M, 2),
                         T = I[0],
                         P = I[1],
                         R = r().useRef(Y(10)),
-                        A = function(e) {
+                        k = function(e) {
                             s(e), a()
                         },
                         S = r().useCallback((function(e) {
-                            g.current && !g.current.contains(e.target) && (a(), document.removeEventListener("click", S, {
+                            m.current && !m.current.contains(e.target) && (a(), document.removeEventListener("click", S, {
                                 capture: !0
                             }), document.removeEventListener("contextmenu", S, {
                                 capture: !0
                             }))
-                        }), [g, a]),
-                        k = r().useCallback((function(e) {
-                            27 === e.keyCode && (a(), document.removeEventListener("keydown", k, {
+                        }), [m, a]),
+                        A = r().useCallback((function(e) {
+                            27 === e.keyCode && (a(), document.removeEventListener("keydown", A, {
                                 capture: !0
                             }))
                         }), [a]);
                     r().useEffect((function() {
-                        return E.current && E.current.focus(), w(g.current.getBoundingClientRect().width), document.addEventListener("keydown", k, {
+                        return E.current && E.current.focus(), w(m.current.getBoundingClientRect().width), document.addEventListener("keydown", A, {
                                 capture: !0
                             }), document.addEventListener("click", S, {
                                 capture: !0
                             }), document.addEventListener("contextmenu", S, {
                                 capture: !0
                             }),
                             function() {
                                 document.removeEventListener("click", S, {
                                     capture: !0
                                 }), document.removeEventListener("contextmenu", S, {
                                     capture: !0
-                                }), document.removeEventListener("keydown", k, {
+                                }), document.removeEventListener("keydown", A, {
                                     capture: !0
                                 })
                             }
-                    }), [S, k]);
+                    }), [S, A]);
                     var L = r().useState([]),
                         B = _e(L, 2),
                         W = B[0],
                         K = B[1];
 
                     function U(e, t) {
                         var n = e.toLowerCase();
                         return t.filter((function(e) {
                             return e.label.toLowerCase().includes(n)
                         }))
                     }
                     return r().useEffect((function() {
                         if (x) {
                             var e = U(x, i);
-                            K(e), m && m.onContextMenuFilter && m.onContextMenuFilter(x, e, K, U, p), f && f(x, e, K, U, p)
+                            K(e), g && g.onContextMenuFilter && g.onContextMenuFilter(x, e, K, U, p), f && f(x, e, K, U, p)
                         } else K(i)
                     }), [x, i]), r().useEffect((function() {
-                        (c || u) && g.current.focus()
+                        (c || u) && m.current.focus()
                     }), [c, u]), r().useEffect((function() {
                         var e = document.getElementById(R.current + "-" + T);
                         if (e) {
                             var t = y.current.getBoundingClientRect(),
                                 n = e.getBoundingClientRect();
                             (n.y + n.height > t.y + t.height || n.y < t.y) && e.scrollIntoView({
                                 block: "nearest"
                             })
                         }
-                    }), [T]), m && m.outOptions && (m.outOptions({
+                    }), [T]), g && g.outOptions && (g.outOptions({
                         setFilter: C,
                         setFilterOptions: K,
                         filterOptions: U,
                         menuInputRef: E
                     }), r().useEffect((function() {
-                        return m.onMenuStateChange(!0, c, p),
+                        return g.onMenuStateChange(!0, c, p),
                             function() {
-                                m.onMenuStateChange(!1, c, p)
+                                g.onMenuStateChange(!1, c, p)
                             }
                     }), [])), r().createElement("div", {
                         "data-flume-component": "ctx-menu",
                         className: "ContextMenu_menuWrapper__1BheJ",
                         onMouseDown: function(e) {
                             return e.stopPropagation()
                         },
                         onKeyDown: function(e) {
                             if (38 === e.which && (e.preventDefault(), null === T ? P(0) : T > 0 && P((function(e) {
                                     return e - 1
                                 }))), 40 === e.which && (e.preventDefault(), null === T ? P(0) : T < W.length - 1 && P((function(e) {
                                     return e + 1
                                 }))), 13 === e.which && null !== T) {
                                 var t = W[T];
-                                t && A(t)
+                                t && k(t)
                             }
                         },
                         style: {
                             left: t,
                             top: n,
-                            width: x ? N : "auto"
+                            width: x ? D : "auto"
                         },
-                        ref: g,
+                        ref: m,
                         tabIndex: 0,
                         role: "menu",
                         "aria-activedescendant": R.current + "-" + T
                     }, u || !l && !i.length ? null : r().createElement("div", {
                         className: "ContextMenu_menuHeader__1Cw58",
                         "data-flume-component": "ctx-menu-header"
                     }, r().createElement("label", {
@@ -563,22 +563,22 @@
                         ref: E
                     }) : null), r().createElement("div", {
                         "data-flume-component": "ctx-menu-list",
                         className: "ContextMenu_optionsWrapper__2YK_z",
                         role: "menu",
                         ref: y,
                         style: {
-                            maxHeight: X(window.innerHeight - n - 70, 10, 300)
+                            maxHeight: q(window.innerHeight - n - 70, 10, 300)
                         }
                     }, W.map((function(e, t) {
                         return r().createElement(fe, {
                             menuId: R.current,
                             selected: T === t,
                             onClick: function() {
-                                return A(e)
+                                return k(e)
                             },
                             onMouseEnter: function() {
                                 return P(null)
                             },
                             index: t,
                             key: e.value + t
                         }, r().createElement("label", null, e.label), e.description ? r().createElement("p", null, e.description) : null)
@@ -600,31 +600,31 @@
                         role: "menuitem",
                         onClick: i,
                         onMouseEnter: s,
                         "data-selected": a,
                         id: t + "-" + n
                     }, o)
                 },
-                me = function(e) {
+                ge = function(e) {
                     var t = e.children,
                         n = e.stageState,
                         o = e.stageRect,
                         i = e.onDragDelayStart,
                         a = e.onDragStart,
                         s = e.onDrag,
                         l = e.onDragEnd,
                         u = e.startDragDelayRef,
                         c = void 0 === u ? null : u,
                         d = e.onMouseDown,
                         _ = e.onTouchStart,
                         p = e.disabled,
                         h = e.delay,
                         f = void 0 === h ? 6 : h,
-                        m = e.innerRef,
-                        g = de(e, ["children", "stageState", "stageRect", "onDragDelayStart", "onDragStart", "onDrag", "onDragEnd", "startDragDelayRef", "onMouseDown", "onTouchStart", "disabled", "delay", "innerRef"]),
+                        g = e.innerRef,
+                        m = de(e, ["children", "stageState", "stageRect", "onDragDelayStart", "onDragStart", "onDrag", "onDragEnd", "startDragDelayRef", "onMouseDown", "onTouchStart", "disabled", "delay", "innerRef"]),
                         y = r().useRef(null),
                         E = r().useRef(),
                         b = r().useRef(),
                         v = function(e) {
                             return 1 / n.scale * e
                         },
                         x = function(e) {
@@ -637,133 +637,133 @@
                             var t = x(e);
                             s && s(t, e)
                         },
                         O = function e(t) {
                             var n = x(t);
                             l && l(t, n), window.removeEventListener("mouseup", e), window.removeEventListener("mousemove", C)
                         },
-                        D = function(e) {
+                        N = function(e) {
                             var t = void 0,
                                 n = void 0;
                             "ontouchstart" in window && e.touches ? (t = e.touches[0].clientX, n = e.touches[0].clientY) : (e.preventDefault(), t = e.clientX, n = e.clientY);
                             var o = Math.abs(y.current.x - t),
                                 r = Math.abs(y.current.y - n);
                             Math.round(Math.sqrt(Math.pow(o, 2) + Math.pow(r, 2))) >= f && (function(e) {
                                 a && a(e);
                                 var t = b.current.getBoundingClientRect();
                                 E.current = {
                                     x: y.current.x - t.left,
                                     y: y.current.y - t.top
                                 }, window.addEventListener("mouseup", O), window.addEventListener("mousemove", C)
-                            }(e), N())
+                            }(e), D())
                         },
-                        N = function e() {
-                            document.removeEventListener("mouseup", e), document.removeEventListener("mousemove", D), y.current = null
+                        D = function e() {
+                            document.removeEventListener("mouseup", e), document.removeEventListener("mousemove", N), y.current = null
                         },
                         w = function(e) {
                             i && i(e), e.stopPropagation();
                             var t = void 0,
                                 n = void 0;
                             "ontouchstart" in window && e.touches ? (t = e.touches[0].clientX, n = e.touches[0].clientY) : (e.preventDefault(), t = e.clientX, n = e.clientY), y.current = {
                                 x: t,
                                 y: n
-                            }, document.addEventListener("mouseup", N), document.addEventListener("mousemove", D)
+                            }, document.addEventListener("mouseup", D), document.addEventListener("mousemove", N)
                         };
                     return c && (c.current = w), r().createElement("div", ce({
                         onMouseDown: function(e) {
                             p || 0 == e.button && w(e), d && d(e)
                         },
                         onTouchStart: function(e) {
                             p || w(e), _ && _(e)
                         },
                         onDragStart: function(e) {
                             e.preventDefault(), e.stopPropagation()
                         },
                         ref: function(e) {
-                            b.current = e, m && (m.current = e)
+                            b.current = e, g && (g.current = e)
                         }
-                    }, g), t)
+                    }, m), t)
                 },
-                ge = function(e, t) {
+                me = function(e, t) {
                     for (var n = -1, o = null == e ? 0 : e.length, r = Array(o); ++n < o;) r[n] = t(e[n], n, e);
                     return r
                 },
                 ye = Array.isArray,
                 Ee = /\.|\[(?:[^[\]]*|(["'])(?:(?!\1)[^\\]|\\.)*?\1)\]/,
                 be = /^\w*$/,
                 ve = function(e, t) {
                     if (ye(e)) return !1;
                     var n = typeof e;
                     return !("number" != n && "symbol" != n && "boolean" != n && null != e && !j(e)) || be.test(e) || !Ee.test(e) || null != t && e in Object(t)
                 },
                 xe = function(e) {
-                    if (!N(e)) return !1;
+                    if (!D(e)) return !1;
                     var t = K(e);
                     return "[object Function]" == t || "[object GeneratorFunction]" == t || "[object AsyncFunction]" == t || "[object Proxy]" == t
                 },
                 Ce = P["__core-js_shared__"],
                 Oe = (Z = /[^.]+$/.exec(Ce && Ce.keys && Ce.keys.IE_PROTO || "")) ? "Symbol(src)_1." + Z : "",
-                De = Function.prototype.toString,
-                Ne = function(e) {
+                Ne = Function.prototype.toString,
+                De = function(e) {
                     if (null != e) {
                         try {
-                            return De.call(e)
+                            return Ne.call(e)
                         } catch (e) {}
                         try {
                             return e + ""
                         } catch (e) {}
                     }
                     return ""
                 },
                 we = /^\[object .+?Constructor\]$/,
                 Me = Function.prototype,
                 Ie = Object.prototype,
                 Te = Me.toString,
                 Pe = Ie.hasOwnProperty,
                 Re = RegExp("^" + Te.call(Pe).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
-                Ae = function(e) {
-                    return !(!N(e) || (t = e, Oe && Oe in t)) && (xe(e) ? Re : we).test(Ne(e));
+                ke = function(e) {
+                    return !(!D(e) || (t = e, Oe && Oe in t)) && (xe(e) ? Re : we).test(De(e));
                     var t
                 },
                 Se = function(e, t) {
                     var n = function(e, t) {
                         return null == e ? void 0 : e[t]
                     }(e, t);
-                    return Ae(n) ? n : void 0
+                    return ke(n) ? n : void 0
                 },
-                ke = Se(Object, "create"),
+                Ae = Se(Object, "create"),
                 Le = Object.prototype.hasOwnProperty,
                 Be = Object.prototype.hasOwnProperty;
 
             function We(e) {
                 var t = -1,
                     n = null == e ? 0 : e.length;
                 for (this.clear(); ++t < n;) {
                     var o = e[t];
                     this.set(o[0], o[1])
                 }
             }
             We.prototype.clear = function() {
-                this.__data__ = ke ? ke(null) : {}, this.size = 0
+                this.__data__ = Ae ? Ae(null) : {}, this.size = 0
             }, We.prototype.delete = function(e) {
                 var t = this.has(e) && delete this.__data__[e];
                 return this.size -= t ? 1 : 0, t
             }, We.prototype.get = function(e) {
                 var t = this.__data__;
-                if (ke) {
+                if (Ae) {
                     var n = t[e];
                     return "__lodash_hash_undefined__" === n ? void 0 : n
                 }
                 return Le.call(t, e) ? t[e] : void 0
             }, We.prototype.has = function(e) {
                 var t = this.__data__;
-                return ke ? void 0 !== t[e] : Be.call(t, e)
+                return Ae ? void 0 !== t[e] : Be.call(t, e)
             }, We.prototype.set = function(e, t) {
                 var n = this.__data__;
-                return this.size += this.has(e) ? 0 : 1, n[e] = ke && void 0 === t ? "__lodash_hash_undefined__" : t, this
+                return this.size += this.has(e) ? 0 : 1, n[e] = Ae && void 0 === t ? "__lodash_hash_undefined__" : t, this
             };
             var Ke = We,
                 Ue = function(e, t) {
                     return e === t || e != e && t != t
                 },
                 je = function(e, t) {
                     for (var n = e.length; n--;)
@@ -795,46 +795,46 @@
             }, $e.prototype.set = function(e, t) {
                 var n = this.__data__,
                     o = je(n, e);
                 return o < 0 ? (++this.size, n.push([e, t])) : n[o][1] = t, this
             };
             var ze = $e,
                 Fe = Se(P, "Map"),
-                qe = function(e, t) {
+                Xe = function(e, t) {
                     var n, o, r = e.__data__;
                     return ("string" == (o = typeof(n = t)) || "number" == o || "symbol" == o || "boolean" == o ? "__proto__" !== n : null === n) ? r["string" == typeof t ? "string" : "hash"] : r.map
                 };
 
-            function Xe(e) {
+            function qe(e) {
                 var t = -1,
                     n = null == e ? 0 : e.length;
                 for (this.clear(); ++t < n;) {
                     var o = e[t];
                     this.set(o[0], o[1])
                 }
             }
-            Xe.prototype.clear = function() {
+            qe.prototype.clear = function() {
                 this.size = 0, this.__data__ = {
                     hash: new Ke,
                     map: new(Fe || ze),
                     string: new Ke
                 }
-            }, Xe.prototype.delete = function(e) {
-                var t = qe(this, e).delete(e);
+            }, qe.prototype.delete = function(e) {
+                var t = Xe(this, e).delete(e);
                 return this.size -= t ? 1 : 0, t
-            }, Xe.prototype.get = function(e) {
-                return qe(this, e).get(e)
-            }, Xe.prototype.has = function(e) {
-                return qe(this, e).has(e)
-            }, Xe.prototype.set = function(e, t) {
-                var n = qe(this, e),
+            }, qe.prototype.get = function(e) {
+                return Xe(this, e).get(e)
+            }, qe.prototype.has = function(e) {
+                return Xe(this, e).has(e)
+            }, qe.prototype.set = function(e, t) {
+                var n = Xe(this, e),
                     o = n.size;
                 return n.set(e, t), this.size += n.size == o ? 0 : 1, this
             };
-            var Ye = Xe;
+            var Ye = qe;
 
             function Ze(e, t) {
                 if ("function" != typeof e || null != t && "function" != typeof t) throw new TypeError("Expected a function");
                 var n = function() {
                     var o = arguments,
                         r = t ? t.apply(this, o) : o[0],
                         i = n.cache;
@@ -855,15 +855,15 @@
                 }), (function(e) {
                     return 500 === Je.size && Je.clear(), e
                 })), Je = He.cache, He),
                 tt = R ? R.prototype : void 0,
                 nt = tt ? tt.toString : void 0,
                 ot = function e(t) {
                     if ("string" == typeof t) return t;
-                    if (ye(t)) return ge(t, e) + "";
+                    if (ye(t)) return me(t, e) + "";
                     if (j(t)) return nt ? nt.call(t) : "";
                     var n = t + "";
                     return "0" == n && 1 / t == -1 / 0 ? "-0" : n
                 },
                 rt = function(e) {
                     return null == e ? "" : ot(e)
                 },
@@ -934,17 +934,17 @@
                     if (u && c) return u == t && c == e;
                     var d = -1,
                         _ = !0,
                         p = 2 & n ? new dt : void 0;
                     for (i.set(e, t), i.set(t, e); ++d < s;) {
                         var h = e[d],
                             f = t[d];
-                        if (o) var m = a ? o(f, h, d, t, e, i) : o(h, f, d, e, t, i);
-                        if (void 0 !== m) {
-                            if (m) continue;
+                        if (o) var g = a ? o(f, h, d, t, e, i) : o(h, f, d, e, t, i);
+                        if (void 0 !== g) {
+                            if (g) continue;
                             _ = !1;
                             break
                         }
                         if (p) {
                             if (!_t(t, (function(e, t) {
                                     if (!pt(p, t) && (h === e || r(h, e, n, o, i))) return p.push(t)
                                 }))) {
@@ -955,22 +955,22 @@
                             _ = !1;
                             break
                         }
                     }
                     return i.delete(e), i.delete(t), _
                 },
                 ft = P.Uint8Array,
-                mt = function(e) {
+                gt = function(e) {
                     var t = -1,
                         n = Array(e.size);
                     return e.forEach((function(e, o) {
                         n[++t] = [o, e]
                     })), n
                 },
-                gt = function(e) {
+                mt = function(e) {
                     var t = -1,
                         n = Array(e.size);
                     return e.forEach((function(e) {
                         n[++t] = e
                     })), n
                 },
                 yt = R ? R.prototype : void 0,
@@ -990,20 +990,20 @@
                 } : function() {
                     return []
                 },
                 Ct = function(e) {
                     return U(e) && "[object Arguments]" == K(e)
                 },
                 Ot = Object.prototype,
-                Dt = Ot.hasOwnProperty,
-                Nt = Ot.propertyIsEnumerable,
+                Nt = Ot.hasOwnProperty,
+                Dt = Ot.propertyIsEnumerable,
                 wt = Ct(function() {
                     return arguments
                 }()) ? Ct : function(e) {
-                    return U(e) && Dt.call(e, "callee") && !Nt.call(e, "callee")
+                    return U(e) && Nt.call(e, "callee") && !Dt.call(e, "callee")
                 },
                 Mt = function() {
                     return !1
                 },
                 It = M((function(e, t) {
                     var n = t && !t.nodeType && t,
                         o = n && e && !e.nodeType && e,
@@ -1015,17 +1015,17 @@
                 Pt = function(e, t) {
                     var n = typeof e;
                     return !!(t = null == t ? 9007199254740991 : t) && ("number" == n || "symbol" != n && Tt.test(e)) && e > -1 && e % 1 == 0 && e < t
                 },
                 Rt = function(e) {
                     return "number" == typeof e && e > -1 && e % 1 == 0 && e <= 9007199254740991
                 },
-                At = {};
-            At["[object Float32Array]"] = At["[object Float64Array]"] = At["[object Int8Array]"] = At["[object Int16Array]"] = At["[object Int32Array]"] = At["[object Uint8Array]"] = At["[object Uint8ClampedArray]"] = At["[object Uint16Array]"] = At["[object Uint32Array]"] = !0, At["[object Arguments]"] = At["[object Array]"] = At["[object ArrayBuffer]"] = At["[object Boolean]"] = At["[object DataView]"] = At["[object Date]"] = At["[object Error]"] = At["[object Function]"] = At["[object Map]"] = At["[object Number]"] = At["[object Object]"] = At["[object RegExp]"] = At["[object Set]"] = At["[object String]"] = At["[object WeakMap]"] = !1;
-            var St, kt, Lt = function(e) {
+                kt = {};
+            kt["[object Float32Array]"] = kt["[object Float64Array]"] = kt["[object Int8Array]"] = kt["[object Int16Array]"] = kt["[object Int32Array]"] = kt["[object Uint8Array]"] = kt["[object Uint8ClampedArray]"] = kt["[object Uint16Array]"] = kt["[object Uint32Array]"] = !0, kt["[object Arguments]"] = kt["[object Array]"] = kt["[object ArrayBuffer]"] = kt["[object Boolean]"] = kt["[object DataView]"] = kt["[object Date]"] = kt["[object Error]"] = kt["[object Function]"] = kt["[object Map]"] = kt["[object Number]"] = kt["[object Object]"] = kt["[object RegExp]"] = kt["[object Set]"] = kt["[object String]"] = kt["[object WeakMap]"] = !1;
+            var St, At, Lt = function(e) {
                     return function(t) {
                         return e(t)
                     }
                 },
                 Bt = M((function(e, t) {
                     var n = t && !t.nodeType && t,
                         o = n && e && !e.nodeType && e,
@@ -1035,15 +1035,15 @@
                                 return o && o.require && o.require("util").types || r && r.binding && r.binding("util")
                             } catch (e) {}
                         }();
                     e.exports = i
                 })),
                 Wt = Bt && Bt.isTypedArray,
                 Kt = Wt ? Lt(Wt) : function(e) {
-                    return U(e) && Rt(e.length) && !!At[K(e)]
+                    return U(e) && Rt(e.length) && !!kt[K(e)]
                 },
                 Ut = Object.prototype.hasOwnProperty,
                 jt = function(e, t) {
                     var n = ye(e),
                         o = !n && wt(e),
                         r = !n && !o && It(e),
                         i = !n && !o && !r && Kt(e),
@@ -1053,59 +1053,59 @@
                             return o
                         }(e.length, String) : [],
                         l = s.length;
                     for (var u in e) !t && !Ut.call(e, u) || a && ("length" == u || r && ("offset" == u || "parent" == u) || i && ("buffer" == u || "byteLength" == u || "byteOffset" == u) || Pt(u, l)) || s.push(u);
                     return s
                 },
                 Vt = Object.prototype,
-                $t = (St = Object.keys, kt = Object, function(e) {
-                    return St(kt(e))
+                $t = (St = Object.keys, At = Object, function(e) {
+                    return St(At(e))
                 }),
                 zt = Object.prototype.hasOwnProperty,
                 Ft = function(e) {
                     if (n = (t = e) && t.constructor, t !== ("function" == typeof n && n.prototype || Vt)) return $t(e);
                     var t, n, o = [];
                     for (var r in Object(e)) zt.call(e, r) && "constructor" != r && o.push(r);
                     return o
                 },
-                qt = function(e) {
+                Xt = function(e) {
                     return null != e && Rt(e.length) && !xe(e)
                 },
-                Xt = function(e) {
-                    return qt(e) ? jt(e) : Ft(e)
+                qt = function(e) {
+                    return Xt(e) ? jt(e) : Ft(e)
                 },
                 Yt = function(e) {
                     return function(e, t, n) {
                         var o = t(e);
                         return ye(e) ? o : function(e, t) {
                             for (var n = -1, o = t.length, r = e.length; ++n < o;) e[r + n] = t[n];
                             return e
                         }(o, n(e))
-                    }(e, Xt, xt)
+                    }(e, qt, xt)
                 },
                 Zt = Object.prototype.hasOwnProperty,
                 Ht = Se(P, "DataView"),
                 Jt = Se(P, "Promise"),
                 Gt = Se(P, "Set"),
                 Qt = Se(P, "WeakMap"),
                 en = "[object Map]",
                 tn = "[object Promise]",
                 nn = "[object Set]",
                 on = "[object WeakMap]",
                 rn = "[object DataView]",
-                an = Ne(Ht),
-                sn = Ne(Fe),
-                ln = Ne(Jt),
-                un = Ne(Gt),
-                cn = Ne(Qt),
+                an = De(Ht),
+                sn = De(Fe),
+                ln = De(Jt),
+                un = De(Gt),
+                cn = De(Qt),
                 dn = K;
             (Ht && dn(new Ht(new ArrayBuffer(1))) != rn || Fe && dn(new Fe) != en || Jt && dn(Jt.resolve()) != tn || Gt && dn(new Gt) != nn || Qt && dn(new Qt) != on) && (dn = function(e) {
                 var t = K(e),
                     n = "[object Object]" == t ? e.constructor : void 0,
-                    o = n ? Ne(n) : "";
+                    o = n ? De(n) : "";
                 if (o) switch (o) {
                     case an:
                         return rn;
                     case sn:
                         return en;
                     case ln:
                         return tn;
@@ -1116,16 +1116,16 @@
                 }
                 return t
             });
             var _n = dn,
                 pn = "[object Arguments]",
                 hn = "[object Array]",
                 fn = "[object Object]",
-                mn = Object.prototype.hasOwnProperty,
-                gn = function(e, t, n, o, r, i) {
+                gn = Object.prototype.hasOwnProperty,
+                mn = function(e, t, n, o, r, i) {
                     var a = ye(e),
                         s = ye(t),
                         l = a ? hn : _n(e),
                         u = s ? hn : _n(t),
                         c = (l = l == pn ? fn : l) == fn,
                         d = (u = u == pn ? fn : u) == fn,
                         _ = l == u;
@@ -1146,35 +1146,35 @@
                                 return Ue(+e, +t);
                             case "[object Error]":
                                 return e.name == t.name && e.message == t.message;
                             case "[object RegExp]":
                             case "[object String]":
                                 return e == t + "";
                             case "[object Map]":
-                                var s = mt;
+                                var s = gt;
                             case "[object Set]":
                                 var l = 1 & o;
-                                if (s || (s = gt), e.size != t.size && !l) return !1;
+                                if (s || (s = mt), e.size != t.size && !l) return !1;
                                 var u = a.get(e);
                                 if (u) return u == t;
                                 o |= 2, a.set(e, t);
                                 var c = ht(s(e), s(t), o, r, i, a);
                                 return a.delete(e), c;
                             case "[object Symbol]":
                                 if (Et) return Et.call(e) == Et.call(t)
                         }
                         return !1
                     }(e, t, l, n, o, r, i);
                     if (!(1 & n)) {
-                        var p = c && mn.call(e, "__wrapped__"),
-                            h = d && mn.call(t, "__wrapped__");
+                        var p = c && gn.call(e, "__wrapped__"),
+                            h = d && gn.call(t, "__wrapped__");
                         if (p || h) {
                             var f = p ? e.value() : e,
-                                m = h ? t.value() : t;
-                            return i || (i = new ut), r(f, m, n, o, i)
+                                g = h ? t.value() : t;
+                            return i || (i = new ut), r(f, g, n, o, i)
                         }
                     }
                     return !!_ && (i || (i = new ut), function(e, t, n, o, r, i) {
                         var a = 1 & n,
                             s = Yt(e),
                             l = s.length;
                         if (l != Yt(t).length && !a) return !1;
@@ -1185,44 +1185,44 @@
                         var d = i.get(e),
                             _ = i.get(t);
                         if (d && _) return d == t && _ == e;
                         var p = !0;
                         i.set(e, t), i.set(t, e);
                         for (var h = a; ++u < l;) {
                             var f = e[c = s[u]],
-                                m = t[c];
-                            if (o) var g = a ? o(m, f, c, t, e, i) : o(f, m, c, e, t, i);
-                            if (!(void 0 === g ? f === m || r(f, m, n, o, i) : g)) {
+                                g = t[c];
+                            if (o) var m = a ? o(g, f, c, t, e, i) : o(f, g, c, e, t, i);
+                            if (!(void 0 === m ? f === g || r(f, g, n, o, i) : m)) {
                                 p = !1;
                                 break
                             }
                             h || (h = "constructor" == c)
                         }
                         if (p && !h) {
                             var y = e.constructor,
                                 E = t.constructor;
                             y == E || !("constructor" in e) || !("constructor" in t) || "function" == typeof y && y instanceof y && "function" == typeof E && E instanceof E || (p = !1)
                         }
                         return i.delete(e), i.delete(t), p
                     }(e, t, n, o, r, i))
                 },
                 yn = function e(t, n, o, r, i) {
-                    return t === n || (null == t || null == n || !U(t) && !U(n) ? t != t && n != n : gn(t, n, o, r, e, i))
+                    return t === n || (null == t || null == n || !U(t) && !U(n) ? t != t && n != n : mn(t, n, o, r, e, i))
                 },
                 En = function(e) {
-                    return e == e && !N(e)
+                    return e == e && !D(e)
                 },
                 bn = function(e, t) {
                     return function(n) {
                         return null != n && n[e] === t && (void 0 !== t || e in Object(n))
                     }
                 },
                 vn = function(e) {
                     var t = function(e) {
-                        for (var t = Xt(e), n = t.length; n--;) {
+                        for (var t = qt(e), n = t.length; n--;) {
                             var o = t[n],
                                 r = e[o];
                             t[n] = [o, r, En(r)]
                         }
                         return t
                     }(e);
                     return 1 == t.length && t[0][2] ? bn(t[0][0], t[0][1]) : function(n) {
@@ -1269,41 +1269,41 @@
                         var o = function(e, t, n) {
                             var o = null == e ? void 0 : st(e, t);
                             return void 0 === o ? n : o
                         }(n, e);
                         return void 0 === o && o === t ? Cn(n, e) : yn(t, o, 3)
                     }
                 },
-                Dn = function(e) {
+                Nn = function(e) {
                     return e
                 },
-                Nn = function(e) {
+                Dn = function(e) {
                     return ve(e) ? (t = at(e), function(e) {
                         return null == e ? void 0 : e[t]
                     }) : function(e) {
                         return function(t) {
                             return st(t, e)
                         }
                     }(e);
                     var t
                 },
                 wn = function(e) {
-                    return "function" == typeof e ? e : null == e ? Dn : "object" == typeof e ? ye(e) ? On(e[0], e[1]) : vn(e) : Nn(e)
+                    return "function" == typeof e ? e : null == e ? Nn : "object" == typeof e ? ye(e) ? On(e[0], e[1]) : vn(e) : Dn(e)
                 },
                 Mn = function(e, t, n) {
                     for (var o = -1, r = Object(e), i = n(e), a = i.length; a--;) {
                         var s = i[++o];
                         if (!1 === t(r[s], s, r)) break
                     }
                     return e
                 },
                 In = function(e, t) {
                     if (null == e) return e;
-                    if (!qt(e)) return function(e, t) {
-                        return e && Mn(e, t, Xt)
+                    if (!Xt(e)) return function(e, t) {
+                        return e && Mn(e, t, qt)
                     }(e, t);
                     for (var n = e.length, o = -1, r = Object(e); ++o < n && !1 !== t(r[o], o, r););
                     return e
                 },
                 Tn = function(e, t) {
                     if (e !== t) {
                         var n = void 0 !== e,
@@ -1316,30 +1316,30 @@
                             u = j(t);
                         if (!s && !u && !i && e > t || i && a && l && !s && !u || o && a && l || !n && l || !r) return 1;
                         if (!o && !i && !u && e < t || u && n && r && !o && !i || s && n && r || !a && r || !l) return -1
                     }
                     return 0
                 },
                 Pn = function(e, t, n) {
-                    t = t.length ? ge(t, (function(e) {
+                    t = t.length ? me(t, (function(e) {
                         return ye(e) ? function(t) {
                             return st(t, 1 === e.length ? e[0] : e)
                         } : e
-                    })) : [Dn];
+                    })) : [Nn];
                     var o = -1;
-                    t = ge(t, Lt(wn));
+                    t = me(t, Lt(wn));
                     var r = function(e, t) {
                         var n = -1,
-                            o = qt(e) ? Array(e.length) : [];
+                            o = Xt(e) ? Array(e.length) : [];
                         return In(e, (function(e, r, i) {
                             o[++n] = t(e, r, i)
                         })), o
                     }(e, (function(e, n, r) {
                         return {
-                            criteria: ge(t, (function(t) {
+                            criteria: me(t, (function(t) {
                                 return t(e)
                             })),
                             index: ++o,
                             value: e
                         }
                     }));
                     return function(e, t) {
@@ -1353,18 +1353,18 @@
                                 if (l) return o >= s ? l : l * ("desc" == n[o] ? -1 : 1)
                             }
                             return e.index - t.index
                         }(e, t, n)
                     }))
                 },
                 Rn = "__node_editor_stage__",
-                An = "__node_editor_drag_connection__",
+                kn = "__node_editor_drag_connection__",
                 Sn = "__node_editor_connections__";
 
-            function kn(e) {
+            function An(e) {
                 return {
                     value: e.type,
                     label: e.label,
                     description: e.description,
                     sortIndex: e.sortIndex,
                     node: e
                 }
@@ -1380,53 +1380,53 @@
                     u = e.stageRef,
                     c = e.spaceToPan,
                     d = e.dispatchComments,
                     _ = e.disableComments,
                     p = e.disablePan,
                     h = e.disableZoom,
                     f = r().useContext(ie),
-                    m = r().useContext(H),
-                    g = r().useContext(G),
+                    g = r().useContext(H),
+                    m = r().useContext(G),
                     y = r().useRef(),
                     E = r().useRef(),
                     v = r().useRef(),
                     x = r().useState(!1),
                     C = _e(x, 2),
                     O = C[0],
-                    D = C[1],
-                    N = r().useState({
+                    N = C[1],
+                    D = r().useState({
                         x: 0,
                         y: 0
                     }),
-                    w = _e(N, 2),
+                    w = _e(D, 2),
                     M = w[0],
                     I = w[1],
                     T = r().useRef({
                         x: 0,
                         y: 0
                     }),
                     P = r().useState(!1),
                     R = _e(P, 2),
-                    A = R[0],
+                    k = R[0],
                     S = R[1],
-                    k = r().useCallback((function() {
+                    A = r().useCallback((function() {
                         u.current = y.current.getBoundingClientRect()
                     }), []);
                 r().useEffect((function() {
-                    return u.current = y.current.getBoundingClientRect(), window.addEventListener("resize", k),
+                    return u.current = y.current.getBoundingClientRect(), window.addEventListener("resize", A),
                         function() {
-                            window.removeEventListener("resize", k)
+                            window.removeEventListener("resize", A)
                         }
-                }), [u, k]);
+                }), [u, A]);
                 var L = r().useCallback((function(e) {
                         ("TEXTAREA" === e.target.nodeName || e.target.dataset.comment) && e.target.clientHeight < e.target.scrollHeight || (e.preventDefault(), 0 !== l && i((function(t) {
                             var n = t.scale,
                                 o = t.translate,
                                 r = e.deltaY,
-                                i = X(n - .005 * X(r, -10, 10), .1, 7),
+                                i = q(n - .005 * q(r, -10, 10), .1, 7),
                                 a = function(e) {
                                     return e * (1 / n)
                                 },
                                 s = function(e) {
                                     return e * (1 / i)
                                 },
                                 l = y.current.getBoundingClientRect(),
@@ -1444,15 +1444,15 @@
                             }
                         })))
                     }), [i, l]),
                     B = function(e) {
                         return e.preventDefault(), I({
                             x: e.clientX,
                             y: e.clientY
-                        }), D(!0), !1
+                        }), N(!0), !1
                     },
                     W = function(e) {
                         return 1 / t * e
                     },
                     K = function(e) {
                         var t = e.node,
                             o = e.internalType,
@@ -1461,15 +1461,15 @@
                             a = y.current.getBoundingClientRect(),
                             s = 0,
                             l = 0;
                         i ? (s = i.x, l = i.y) : (s = W(M.x - a.x - a.width / 2) + W(n.x), l = W(M.y - a.y - a.height / 2) + W(n.y)), "comment" === o ? d({
                             type: "ADD_COMMENT",
                             x: s,
                             y: l
-                        }) : g({
+                        }) : m({
                             type: "ADD_NODE",
                             x: s,
                             y: l,
                             nodeType: t.type
                         })
                     },
                     U = function(e) {
@@ -1483,25 +1483,25 @@
                         var e = y.current;
                         return e.addEventListener("wheel", L),
                             function() {
                                 e.removeEventListener("wheel", L)
                             }
                     }
                 }), [L, h]);
-                var V, $, z, F, q, Y = ($ = Object.values(m).filter((function(e) {
+                var V, $, z, F, X, Y = ($ = Object.values(g).filter((function(e) {
                     return !1 !== e.addable
-                })).map(kn), z = ["sortIndex", "label"], V = null == $ ? [] : (ye(z) || (z = null == z ? [] : [z]), ye(F = q ? void 0 : F) || (F = null == F ? [] : [F]), Pn($, z, F)), _ || V.push({
+                })).map(An), z = ["sortIndex", "label"], V = null == $ ? [] : (ye(z) || (z = null == z ? [] : [z]), ye(F = X ? void 0 : F) || (F = null == F ? [] : [F]), Pn($, z, F)), _ || V.push({
                     value: "comment",
                     label: "Comment",
                     description: "A comment for documenting nodes",
                     internalType: "comment"
                 }), V);
                 return f && f.outOptions && f.outOptions({
                     addNode: K,
-                    setMenuOpen: D,
+                    setMenuOpen: N,
                     setMenuCoordinates: I,
                     handleContextMenu: B,
                     nodeXY2ClientXY: function(e, t) {
                         var o = y.current.getBoundingClientRect();
                         return {
                             x: U(e - W(n.x)) + o.x + o.width / 2,
                             y: U(t - W(n.y)) + o.y + o.height / 2
@@ -1509,15 +1509,15 @@
                     },
                     draggableRef: y,
                     translateWrapper: E,
                     scaleWrapper: v,
                     dispatchStageState: i,
                     stagetScale: t,
                     stagetTranslate: n
-                }), r().createElement(me, {
+                }), r().createElement(ge, {
                     "data-flume-component": "stage",
                     id: "" + Rn + o,
                     className: "Stage_wrapper__1X5K_",
                     innerRef: y,
                     onContextMenu: B,
                     onMouseEnter: function() {
                         y.current.contains(document.activeElement) || y.current.focus()
@@ -1557,30 +1557,30 @@
                     } : null,
                     tabIndex: -1,
                     stageState: {
                         scale: t,
                         translate: n
                     },
                     style: {
-                        cursor: A && c ? "grab" : ""
+                        cursor: k && c ? "grab" : ""
                     },
-                    disabled: p || c && !A,
+                    disabled: p || c && !k,
                     "data-flume-stage": !0,
                     onMouseDown: function(e) {
                         f && f.onStageDraggableMouseDown && e.target == y.current && f.onStageDraggableMouseDown(e)
                     },
                     onMouseUp: function(e) {
                         f && f.onStageDraggableMouseUp && e.target == y.current && f.onStageDraggableMouseUp(e)
                     }
                 }, O ? r().createElement(b, null, r().createElement(he, {
                     x: M.x,
                     y: M.y,
                     options: Y,
                     onRequestClose: function() {
-                        D(!1)
+                        N(!1)
                     },
                     onOptionSelected: function(e) {
                         f && f.onOptionSelected ? f.onOptionSelected(e) : K(e)
                     },
                     label: "Add Node",
                     from: "stage"
                 })) : null, r().createElement("div", {
@@ -1619,19 +1619,19 @@
                 }
             }
 
             function Fn(e) {
                 this._context = e
             }
 
-            function qn(e) {
+            function Xn(e) {
                 return new Fn(e)
             }
 
-            function Xn(e) {
+            function qn(e) {
                 return e[0]
             }
 
             function Yn(e) {
                 return e[1]
             }
 
@@ -1711,19 +1711,19 @@
                     if (null === this._x1) this._ += "M" + (this._x1 = e) + "," + (this._y1 = t);
                     else if (d > Un)
                         if (Math.abs(c * s - l * u) > Un && r) {
                             var _ = n - i,
                                 p = o - a,
                                 h = s * s + l * l,
                                 f = _ * _ + p * p,
-                                m = Math.sqrt(h),
-                                g = Math.sqrt(d),
-                                y = r * Math.tan((Wn - Math.acos((h + d - f) / (2 * m * g))) / 2),
-                                E = y / g,
-                                b = y / m;
+                                g = Math.sqrt(h),
+                                m = Math.sqrt(d),
+                                y = r * Math.tan((Wn - Math.acos((h + d - f) / (2 * g * m))) / 2),
+                                E = y / m,
+                                b = y / g;
                             Math.abs(E - 1) > Un && (this._ += "L" + (e + E * u) + "," + (t + E * c)), this._ += "A" + r + "," + r + ",0,0," + +(c * _ > u * p) + "," + (this._x1 = e + b * s) + "," + (this._y1 = t + b * l)
                         } else this._ += "L" + (this._x1 = e) + "," + (this._y1 = t)
                 },
                 arc: function(e, t, n, o, r, i) {
                     e = +e, t = +t, i = !!i;
                     var a = (n = +n) * Math.cos(o),
                         s = n * Math.sin(o),
@@ -1869,19 +1869,19 @@
                     }
                     var s = ro(e, t, n);
                     return s && s.getBoundingClientRect()
                 },
                 ao = function(e, t) {
                     var n = (t.x - e.x) / 3,
                         o = function() {
-                            var e = Xn,
+                            var e = qn,
                                 t = Yn,
                                 n = zn(!0),
                                 o = null,
-                                r = qn,
+                                r = Xn,
                                 i = null;
 
                             function a(a) {
                                 var s, l, u, c = a.length,
                                     d = !1;
                                 for (null == o && (i = r(u = $n())), s = 0; s <= c; ++s) !(s < c && n(l = a[s], s, a)) === d && ((d = !d) ? i.lineStart() : i.lineEnd()), d && i.point(+e(l, s, a), +t(l, s, a));
                                 if (u) return i = null, u + "" || null
@@ -1955,27 +1955,27 @@
                     u = void 0 === l ? null : l,
                     c = e.nodeId,
                     d = e.portName,
                     _ = e.name,
                     p = r().useRef(),
                     h = r().useContext(oe),
                     f = r().useContext(ie),
-                    m = r().useRef(!1),
-                    g = function e() {
+                    g = r().useRef(!1),
+                    m = function e() {
                         document.removeEventListener("mousemove", y), document.removeEventListener("mouseup", e)
                     },
                     y = function(e) {
                         e.stopPropagation(), n()
                     },
                     E = function(e) {
-                        e.stopPropagation(), h(), document.addEventListener("mousemove", y), document.addEventListener("mouseup", g), f && f.setInputing && (f.setInputing(!0), m.current = !0)
+                        e.stopPropagation(), h(), document.addEventListener("mousemove", y), document.addEventListener("mouseup", m), f && f.setInputing && (f.setInputing(!0), g.current = !0)
                     };
                 return r().useEffect((function() {
                     return function() {
-                        m.current && f && f.setInputing && (f.setInputing(!1), m.current = !1)
+                        g.current && f && f.setInputing && (f.setInputing(!1), g.current = !1)
                     }
                 }), []), r().createElement("div", {
                     className: "TextInput_wrapper__tefOZ",
                     "data-flume-component": "text-input"
                 }, "number" === s ? r().createElement("input", {
                     "data-flume-component": "text-input-number",
                     onKeyDown: function(e) {
@@ -2023,15 +2023,15 @@
                     "data-name": _,
                     onBlur: function(e) {
                         f && f.setInputing && f.setInputing(!1)
                     }
                 }))
             };
             h('.Select_wrapper__eAPoQ{\n  font-size: 14px;\n  padding: 3px 6px;\n  border-radius: 4px;\n  background: linear-gradient(to top, #5b5f62, #6f7477);\n  width: 100%;\n  border: 1px solid #3c3e40;\n  padding-right: 15px;\n  position: relative;\n}\n  .Select_wrapper__eAPoQ::after{\n    content: "";\n    position: absolute;\n    background: none;\n    right: 5px;\n    top: 8px;\n    width: 0;\n    height: 0;\n    border-style: solid;\n    border-width: 6px 5px 0 5px;\n    border-color: #191b1c transparent transparent transparent;\n  }\n  .Select_wrapper__eAPoQ:hover{\n    background: linear-gradient(to top, #63676a, #777b7e);\n  }\n.Select_chipWrapper__3hK2u{\n  font-size: 14px;\n  padding: 3px 6px;\n  border-radius: 4px;\n  background: linear-gradient(to top, #5b5f62, #6f7477);\n  border: 1px solid #3c3e40;\n  margin: 2px;\n  position: relative;\n}\n.Select_chipWrapper__3hK2u:hover .Select_deleteButton__1FnLK{\n  opacity: 1;\n}\n.Select_chipsWrapper__4Alw8{\n  display: flex;\n  flex-direction: column;\n  margin-bottom: 6px;\n}\n.Select_deleteButton__1FnLK{\n  position: absolute;\n  right: 0px;\n  top: 0px;\n  height: 100%;\n  width: 22px;\n  padding: 0px;\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  background: linear-gradient(to top, #5b5f62, #6f7477);\n  border-radius: 3px;\n  border: none;\n  font-weight: bold;\n  opacity: 0;\n}\n.Select_deleteButton__1FnLK:focus{\n  opacity: 1;\n}\n.Select_deleteButton__1FnLK:hover{\n  background: linear-gradient(to top, #64696c, #797f82);\n}\n.Select_selectedWrapper__SUs4D{\n  display: flex;\n  flex-direction: column;\n  border-radius: 4px;\n  background: linear-gradient(to top, #5b5f62, #6f7477);\n  width: 100%;\n  border: 1px solid #3c3e40;\n  font-size: 14px;\n  padding: 3px 6px;\n  padding-right: 15px;\n  position: relative;\n}\n.Select_selectedWrapper__SUs4D::after{\n    content: "";\n    position: absolute;\n    background: none;\n    right: 5px;\n    top: calc(50% - 4px);\n    width: 0;\n    height: 0;\n    border-style: solid;\n    border-width: 6px 5px 0 5px;\n    border-color: #191b1c transparent transparent transparent;\n  }\n.Select_selectedWrapper__SUs4D label{\n    margin: 0px;\n  }\n.Select_selectedWrapper__SUs4D p{\n    margin: 0px;\n    margin-top: 5px;\n    font-size: 12px;\n    font-style: italic;\n    color: rgb(50, 50, 50);\n  }\n');
-            var mo = function(e) {
+            var go = function(e) {
                     var t = e.options,
                         n = void 0 === t ? [] : t,
                         o = e.placeholder,
                         i = void 0 === o ? "[Select an option]" : o,
                         a = e.onChange,
                         s = e.data,
                         l = e.allowMultiple,
@@ -2041,20 +2041,20 @@
                         _ = c[1],
                         p = r().useState({
                             x: 0,
                             y: 0
                         }),
                         h = _e(p, 2),
                         f = h[0],
-                        m = h[1],
-                        g = r().useRef(),
+                        g = h[1],
+                        m = r().useRef(),
                         y = function() {
                             if (!d) {
-                                var e = g.current.getBoundingClientRect();
-                                m({
+                                var e = m.current.getBoundingClientRect();
+                                g({
                                     x: e.x,
                                     y: e.y + e.height
                                 }), _(!0)
                             }
                         },
                         E = r().useMemo((function() {
                             var e = n.find((function(e) {
@@ -2073,21 +2073,21 @@
                         return r().createElement(yo, {
                             onRequestDelete: function() {
                                 return e = t, void a([].concat(pe(s.slice(0, e)), pe(s.slice(e + 1))));
                                 var e
                             },
                             key: e
                         }, o)
-                    }))) : null : s || 0 == s ? r().createElement(go, {
-                        wrapperRef: g,
+                    }))) : null : s || 0 == s ? r().createElement(mo, {
+                        wrapperRef: m,
                         option: E,
                         onClick: y
                     }) : null, (l || !s && 0 != s) && r().createElement("div", {
                         className: "Select_wrapper__eAPoQ",
-                        ref: g,
+                        ref: m,
                         onClick: y
                     }, i), d && r().createElement(b, null, r().createElement(he, {
                         x: f.x,
                         y: f.y,
                         emptyText: "There are no options",
                         options: l ? n.filter((function(e) {
                             return !s.includes(e.value)
@@ -2097,15 +2097,15 @@
                         },
                         onRequestClose: function() {
                             _(!1)
                         },
                         from: "select"
                     })))
                 },
-                go = function(e) {
+                mo = function(e) {
                     var t = e.option,
                         n = (t = void 0 === t ? {} : t).label,
                         o = t.description,
                         i = e.wrapperRef,
                         a = e.onClick;
                     return r().createElement("div", {
                         className: "Select_selectedWrapper__SUs4D",
@@ -2142,82 +2142,82 @@
                         u = e.allData,
                         c = e.render,
                         d = e.step,
                         _ = e.options,
                         p = void 0 === _ ? [] : _,
                         h = e.placeholder,
                         f = e.inputData,
-                        m = e.triggerRecalculation,
-                        g = e.updateNodeConnections,
+                        g = e.triggerRecalculation,
+                        m = e.updateNodeConnections,
                         y = e.getOptions,
                         E = e.setValue,
                         b = e.defaultValue,
                         v = e.isMonoControl,
                         x = e.process,
                         C = void 0 === x ? null : x,
                         O = r().useContext(G),
-                        D = r().useContext(ee),
-                        N = v ? s : a,
+                        N = r().useContext(ee),
+                        D = v ? s : a,
                         w = function(e) {
                             O({
                                 type: "SET_PORT_DATA",
                                 data: e,
                                 nodeId: o,
                                 portName: i,
                                 controlName: n,
                                 setValue: E
-                            }), m()
+                            }), g()
                         };
                     return r().createElement("div", {
                         className: "Control_wrapper__VZIiC",
                         "data-flume-component": "control"
-                    }, N && "checkbox" !== t && "custom" !== t && r().createElement("label", {
+                    }, D && "checkbox" !== t && "custom" !== t && r().createElement("label", {
                         "data-flume-component": "control-label",
                         className: "Control_controlLabel__3ga2-"
-                    }, N), function(e) {
+                    }, D), function(e) {
                         var t = {
-                            triggerRecalculation: m,
-                            updateNodeConnections: g,
+                            triggerRecalculation: g,
+                            updateNodeConnections: m,
                             onChange: w,
                             data: l,
                             process: C,
                             nodeId: o,
                             portName: i,
                             name: n
                         };
                         switch (e) {
                             case "select":
-                                return r().createElement(mo, ce({}, t, {
-                                    options: y ? y(f, D) : p,
+                                return r().createElement(go, ce({}, t, {
+                                    options: y ? y(f, N) : p,
                                     placeholder: h
                                 }));
                             case "text":
                                 return r().createElement(fo, ce({}, t, {
                                     placeholder: h
                                 }));
                             case "number":
                                 return r().createElement(fo, ce({}, t, {
                                     step: d,
                                     type: "number",
                                     placeholder: h
                                 }));
                             case "checkbox":
                                 return r().createElement(po, ce({}, t, {
-                                    label: N
+                                    label: D
                                 }));
                             case "multiselect":
-                                return r().createElement(mo, ce({
+                                return r().createElement(go, ce({
                                     allowMultiple: !0
                                 }, t, {
-                                    options: y ? y(f, D) : p,
+                                    options: y ? y(f, N) : p,
                                     placeholder: h,
                                     label: a
                                 }));
                             case "custom":
-                                return c(l, w, D, m, {
+                                return c(l, w, N, g, {
                                     label: a,
                                     name: n,
                                     portName: i,
                                     inputLabel: s,
                                     defaultValue: b,
                                     nodeId: o
                                 }, u);
@@ -2330,15 +2330,15 @@
                             inputData: l,
                             key: e.name
                         }))
                     }))) : null, !!p.length && r().createElement("div", {
                         className: "IoPorts_outputs__3JGh-",
                         "data-flume-component": "ports-outputs"
                     }, p.map((function(e) {
-                        return r().createElement(Do, ce({}, e, {
+                        return r().createElement(No, ce({}, e, {
                             triggerRecalculation: d,
                             inputTypes: c,
                             nodeId: t,
                             inputData: l,
                             portOnRight: !0,
                             key: e.name
                         }))
@@ -2355,40 +2355,40 @@
                         u = e.noControls,
                         c = e.triggerRecalculation,
                         d = e.updateNodeConnections,
                         _ = e.isConnected,
                         p = e.inputData,
                         h = e.hidePort,
                         f = l[t] || {},
-                        m = f.label,
-                        g = f.color,
+                        g = f.label,
+                        m = f.color,
                         y = f.controls,
                         E = void 0 === y ? [] : y,
                         b = vo(_),
                         v = s || E;
                     return r().useEffect((function() {
                         _ !== b && c()
                     }), [_, b, c]), r().createElement("div", {
                         "data-flume-component": "port-input",
                         className: co,
                         "data-controlless": _ || u || !v.length,
                         onDragStart: function(e) {
                             e.preventDefault(), e.stopPropagation()
                         }
-                    }, h ? null : r().createElement(No, {
+                    }, h ? null : r().createElement(Do, {
                         type: t,
-                        color: g,
+                        color: m,
                         name: o,
                         nodeId: i,
                         isInput: !0,
                         triggerRecalculation: c
                     }), (!v.length || u || _) && r().createElement("label", {
                         "data-flume-component": "port-label",
                         className: _o
-                    }, n || m), u || _ ? null : r().createElement("div", {
+                    }, n || g), u || _ ? null : r().createElement("div", {
                         className: "IoPorts_controls__1dKFt"
                     }, v.map((function(e) {
                         return r().createElement(Eo, ce({}, e, {
                             nodeId: i,
                             portName: o,
                             triggerRecalculation: c,
                             updateNodeConnections: d,
@@ -2397,15 +2397,15 @@
                             allData: a,
                             key: e.name,
                             inputData: p,
                             isMonoControl: 1 === v.length
                         }))
                     }))))
                 },
-                Do = function(e) {
+                No = function(e) {
                     var t = e.label,
                         n = e.name,
                         o = e.nodeId,
                         i = e.type,
                         a = e.inputTypes,
                         s = e.triggerRecalculation,
                         l = a[i] || {},
@@ -2417,68 +2417,68 @@
                         "data-controlless": !0,
                         onDragStart: function(e) {
                             e.preventDefault(), e.stopPropagation()
                         }
                     }, r().createElement("span", {
                         "data-flume-component": "port-label",
                         className: _o
-                    }, t || u), r().createElement(No, {
+                    }, t || u), r().createElement(Do, {
                         type: i,
                         name: n,
                         color: c,
                         nodeId: o,
                         triggerRecalculation: s
                     }))
                 },
-                No = function(e) {
+                Do = function(e) {
                     var t = e.color,
                         n = void 0 === t ? "grey" : t,
                         i = e.name,
                         a = void 0 === i ? "" : i,
                         s = e.type,
                         l = e.isInput,
                         u = e.nodeId,
                         c = e.triggerRecalculation,
                         d = r().useContext(G),
                         _ = r().useContext(te),
                         p = r().useContext(re),
                         h = "" + Rn + p,
                         f = r().useContext(J),
-                        m = r().useState(!1),
-                        g = _e(m, 2),
-                        y = g[0],
-                        E = g[1],
+                        g = r().useState(!1),
+                        m = _e(g, 2),
+                        y = m[0],
+                        E = m[1],
                         v = r().useState({
                             x: 0,
                             y: 0
                         }),
                         x = _e(v, 2),
                         C = x[0],
                         O = x[1],
-                        D = r().useRef(C),
-                        N = r().useRef(),
+                        N = r().useRef(C),
+                        D = r().useRef(),
                         w = r().useRef(),
                         M = r().useRef(),
                         I = function(e) {
                             return 1 / _.scale * e
                         },
                         T = function(e) {
                             var t = document.getElementById(h).getBoundingClientRect();
                             if (l) {
                                 var n = {
                                     x: I(e.clientX - t.x - t.width / 2) + I(_.translate.x),
                                     y: I(e.clientY - t.y - t.height / 2) + I(_.translate.y)
                                 };
-                                M.current.setAttribute("d", ao(D.current, n))
+                                M.current.setAttribute("d", ao(N.current, n))
                             } else {
                                 var o = {
                                     x: I(e.clientX - t.x - t.width / 2) + I(_.translate.x),
                                     y: I(e.clientY - t.y - t.height / 2) + I(_.translate.y)
                                 };
-                                w.current.setAttribute("d", ao(D.current, o))
+                                w.current.setAttribute("d", ao(N.current, o))
                             }
                         },
                         P = (0, o.useContext)(ie),
                         R = function e(t) {
                             var n = !!t.target.dataset.portName;
                             if (l) {
                                 var o = M.current.dataset,
@@ -2494,37 +2494,37 @@
                                         },
                                         output: {
                                             nodeId: _,
                                             portName: p
                                         }
                                     }), n) {
                                     var h = t.target.dataset,
-                                        m = h.portName,
-                                        g = h.nodeId,
+                                        g = h.portName,
+                                        m = h.nodeId,
                                         y = h.portType,
                                         b = h.portTransputType;
-                                    _ !== g && "output" !== b && f[y].acceptTypes.includes(s) && d({
+                                    _ !== m && "output" !== b && f[y].acceptTypes.includes(s) && d({
                                         type: "ADD_CONNECTION",
                                         input: {
-                                            nodeId: g,
-                                            portName: m
+                                            nodeId: m,
+                                            portName: g
                                         },
                                         output: {
                                             nodeId: _,
                                             portName: p
                                         }
                                     })
                                 }
                             } else if (n) {
                                 var v = t.target.dataset,
                                     x = v.portName,
                                     C = v.nodeId,
                                     O = v.portType,
-                                    D = v.portTransputType;
-                                C !== u && "output" !== D && f[O].acceptTypes.includes(s) && (d({
+                                    N = v.portTransputType;
+                                C !== u && "output" !== N && f[O].acceptTypes.includes(s) && (d({
                                     type: "ADD_CONNECTION",
                                     output: {
                                         nodeId: u,
                                         portName: a
                                     },
                                     input: {
                                         nodeId: C,
@@ -2536,47 +2536,47 @@
                         };
                     return r().createElement(r().Fragment, null, r().createElement("div", {
                         style: {
                             zIndex: 999
                         },
                         onMouseDown: function(e) {
                             e.preventDefault(), e.stopPropagation();
-                            var t = N.current.getBoundingClientRect(),
+                            var t = D.current.getBoundingClientRect(),
                                 n = document.getElementById(h).getBoundingClientRect();
                             if (l) {
                                 if (M.current = document.querySelector('[data-input-node-id="' + u + '"][data-input-port-name="' + a + '"]'), M.current) {
                                     M.current.parentNode.style.zIndex = 9999;
                                     var o = io(M.current.dataset.outputNodeId, M.current.dataset.outputPortName, "output"),
                                         r = {
                                             x: I(o.x - n.x + o.width / 2 - n.width / 2) + I(_.translate.x),
                                             y: I(o.y - n.y + o.width / 2 - n.height / 2) + I(_.translate.y)
                                         };
-                                    O(r), D.current = r, E(!0), document.addEventListener("mouseup", R), document.addEventListener("mousemove", T)
+                                    O(r), N.current = r, E(!0), document.addEventListener("mouseup", R), document.addEventListener("mousemove", T)
                                 }
                             } else {
                                 var i = {
                                     x: I(t.x - n.x + t.width / 2 - n.width / 2) + I(_.translate.x),
                                     y: I(t.y - n.y + t.width / 2 - n.height / 2) + I(_.translate.y)
                                 };
-                                O(i), D.current = i, E(!0), document.addEventListener("mouseup", R), document.addEventListener("mousemove", T)
+                                O(i), N.current = i, E(!0), document.addEventListener("mouseup", R), document.addEventListener("mousemove", T)
                             }
                         },
                         className: "IoPorts_port__1_a6J",
                         "data-port-color": n,
                         "data-port-name": a,
                         "data-port-type": s,
                         "data-port-transput-type": l ? "input" : "output",
                         "data-node-id": u,
                         "data-flume-component": "port-handle",
                         onDragStart: function(e) {
                             e.preventDefault(), e.stopPropagation()
                         },
-                        ref: N
+                        ref: D
                     }), y && !l ? r().createElement(b, {
-                        node: document.getElementById("" + An + p)
+                        node: document.getElementById("" + kn + p)
                     }, r().createElement(bo, {
                         from: C,
                         to: C,
                         lineRef: w
                     })) : null)
                 },
                 wo = function(e) {
@@ -2589,129 +2589,129 @@
                         u = e.type,
                         c = e.inputData,
                         d = e.root,
                         _ = e.onDragStart,
                         p = e.renderNodeHeader,
                         h = r().useContext(ie),
                         f = r().useContext(ne),
-                        m = r().useContext(H),
-                        g = r().useContext(G),
+                        g = r().useContext(H),
+                        m = r().useContext(G),
                         y = r().useContext(te),
-                        E = m[u],
+                        E = g[u],
                         b = E.label,
                         v = (E.deletable, E.inputs),
                         x = void 0 === v ? [] : v,
                         C = E.outputs,
                         O = void 0 === C ? [] : C,
-                        D = r().useRef(),
-                        N = r().useState(!1),
-                        w = _e(N, 2),
+                        N = r().useRef(),
+                        D = r().useState(!1),
+                        w = _e(D, 2),
                         M = (w[0], w[1]),
                         I = r().useState({
                             x: 0,
                             y: 0
                         }),
                         T = _e(I, 2),
                         P = (T[0], T[1]),
                         R = function(e) {
                             return 1 / y.scale * e
                         },
-                        A = function() {
+                        k = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                                 t = arguments[1];
                             for (var o in e) {
                                 var r = e[o],
                                     i = !0,
                                     a = !1,
                                     l = void 0;
                                 try {
                                     for (var u, c = r[Symbol.iterator](); !(i = (u = c.next()).done); i = !0) {
                                         var d, _ = u.value,
                                             p = io(n, o, t ? "output" : "input", f),
                                             h = io(_.nodeId, _.portName, t ? "input" : "output", f),
-                                            m = h.width / 2;
+                                            g = h.width / 2;
                                         d = t ? n + o + _.nodeId + _.portName : _.nodeId + _.portName + n + o;
-                                        var g = void 0,
+                                        var m = void 0,
                                             E = f.current.connections[d];
-                                        E ? g = E : (g = document.querySelector('[data-connection-id="' + d + '"]'), f.current.connections[d] = g);
+                                        E ? m = E : (m = document.querySelector('[data-connection-id="' + d + '"]'), f.current.connections[d] = m);
                                         var b = {
-                                                x: R(p.x - s.current.x + m - s.current.width / 2) + R(y.translate.x),
-                                                y: R(p.y - s.current.y + m - s.current.height / 2) + R(y.translate.y)
+                                                x: R(p.x - s.current.x + g - s.current.width / 2) + R(y.translate.x),
+                                                y: R(p.y - s.current.y + g - s.current.height / 2) + R(y.translate.y)
                                             },
                                             v = {
-                                                x: R(h.x - s.current.x + m - s.current.width / 2) + R(y.translate.x),
-                                                y: R(h.y - s.current.y + m - s.current.height / 2) + R(y.translate.y)
+                                                x: R(h.x - s.current.x + g - s.current.width / 2) + R(y.translate.x),
+                                                y: R(h.y - s.current.y + g - s.current.height / 2) + R(y.translate.y)
                                             };
-                                        g.setAttribute("d", ao(b, v))
+                                        m.setAttribute("d", ao(b, v))
                                     }
                                 } catch (e) {
                                     a = !0, l = e
                                 } finally {
                                     try {
                                         !i && c.return && c.return()
                                     } finally {
                                         if (a) throw l
                                     }
                                 }
                             }
                         },
                         S = function() {
-                            l && (A(l.inputs), A(l.outputs, !0))
+                            l && (k(l.inputs), k(l.outputs, !0))
                         },
-                        k = function(e) {
+                        A = function(e) {
                             return e.preventDefault(), e.stopPropagation(), P({
                                 x: e.clientX,
                                 y: e.clientY
                             }), M(!0), !1
                         },
                         L = r().useRef(null);
-                    return h && h.outOptions && h.outOptions((ue(t = {}, "updateNodeConnections_" + n, S), ue(t, "nodeDraggable_" + n, D), ue(t, "startDragDelay_" + n, L), t)), r().createElement(me, {
+                    return h && h.outOptions && h.outOptions((ue(t = {}, "updateNodeConnections_" + n, S), ue(t, "nodeDraggable_" + n, N), ue(t, "startDragDelay_" + n, L), t)), r().createElement(ge, {
                         className: "Node_wrapper__3SmT7",
                         style: {
                             width: o,
                             transform: "translate(" + i + "px, " + a + "px)"
                         },
                         onDragStart: function(e) {
-                            _(), h && h.onNodeStartDrag && h.onNodeStartDrag(n, D.current)
+                            _(), h && h.onNodeStartDrag && h.onNodeStartDrag(n, N.current)
                         },
                         onDrag: function(e) {
                             var t = e.x,
                                 n = e.y;
-                            D.current.style.transform = "translate(" + t + "px," + n + "px)", S()
+                            N.current.style.transform = "translate(" + t + "px," + n + "px)", S()
                         },
                         onDragEnd: function(e, t) {
-                            g(ce({
+                            m(ce({
                                 type: "SET_NODE_COORDINATES"
                             }, t, {
                                 nodeId: n
                             }))
                         },
-                        innerRef: D,
+                        innerRef: N,
                         id: n,
                         "data-node-id": n,
                         "data-flume-component": "node",
                         "data-flume-node-type": E.type,
                         "data-flume-component-is-root": !!d,
-                        onContextMenu: k,
+                        onContextMenu: A,
                         stageState: y,
                         stageRect: s,
                         onMouseDown: function(e) {
-                            h && h.onNodeMouseDown && h.onNodeMouseDown(e, n, D.current)
+                            h && h.onNodeMouseDown && h.onNodeMouseDown(e, n, N.current)
                         },
                         onMouseUp: function(e) {
-                            h && h.onNodeMouseUp && h.onNodeMouseUp(e, n, D.current)
+                            h && h.onNodeMouseUp && h.onNodeMouseUp(e, n, N.current)
                         },
                         startDragDelayRef: L
                     }, p ? p(Mo, E, {
-                        openMenu: k,
+                        openMenu: A,
                         closeMenu: function() {
                             M(!1)
                         },
                         deleteNode: function() {
-                            g({
+                            m({
                                 type: "REMOVE_NODE",
                                 nodeId: n
                             })
                         }
                     }, n) : r().createElement(Mo, null, b), r().createElement(Co, {
                         nodeId: n,
                         inputs: x,
@@ -2817,15 +2817,15 @@
                     blue: "blue",
                     green: "green",
                     grey: "grey",
                     tuple: "tuple",
                     dict: "dict",
                     control: "control"
                 },
-                Ao = function(e) {
+                ko = function(e) {
                     return Object.values(e).reduce((function(e, t) {
                         return e[t.type] = function() {
                             var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                             return {
                                 type: t.type,
                                 name: e.name || t.name,
                                 label: e.label || t.label,
@@ -2861,24 +2861,24 @@
                                 type: e.type,
                                 label: Io(e.label, ""),
                                 description: Io(e.description, ""),
                                 addable: Io(e.addable, !0),
                                 deletable: Io(e.deletable, !0)
                             };
                             if (e.initialWidth && (t.initialWidth = e.initialWidth), void 0 !== e.sortIndex && (t.sortIndex = e.sortIndex), "function" == typeof e.inputs) {
-                                var n = e.inputs(Ao(this.portTypes));
+                                var n = e.inputs(ko(this.portTypes));
                                 if (!Array.isArray(n) && "function" != typeof e.inputs) throw new Error('When providing a function to the "inputs" key, you must return either an array or a function.');
                                 t.inputs = n
                             } else if (void 0 === e.inputs) t.inputs = [];
                             else {
                                 if (!Array.isArray(e.inputs)) throw new Error('Optional key, "inputs" must be an array.');
                                 t.inputs = e.inputs
                             }
                             if ("function" == typeof e.outputs) {
-                                var o = e.outputs(Ao(this.portTypes));
+                                var o = e.outputs(ko(this.portTypes));
                                 if (!Array.isArray(o) && "function" != typeof e.outputs) throw new Error('When providing a function to the "outputs" key, you must return either an array or a function.');
                                 t.outputs = o
                             } else if (void 0 === e.outputs) t.outputs = [];
                             else {
                                 if (void 0 !== e.outputs && !Array.isArray(e.outputs)) throw new Error('Optional key, "outputs" must be an array.');
                                 t.outputs = e.outputs
                             }
@@ -2942,15 +2942,15 @@
                                     i = (r[e], de(r, [e]));
                                 this.portTypes = i
                             } else console.error('Non-existent port type "' + e + '" cannot be removed.');
                             return this
                         }
                     }]), e
                 }(),
-                ko = function(e) {
+                Ao = function(e) {
                     var t = e.x,
                         n = e.y,
                         o = e.onColorPicked,
                         i = e.onRequestClose,
                         a = r().useRef(),
                         s = r().useCallback((function(e) {
                             a.current && !a.current.contains(e.target) && (i(), document.removeEventListener("click", s), document.removeEventListener("contextmenu", s))
@@ -3005,57 +3005,57 @@
                         u = e.text,
                         c = e.stageRect,
                         d = e.onDragStart,
                         _ = e.isNew,
                         p = r().useContext(ie),
                         h = r().useContext(te),
                         f = r().useRef(),
-                        m = r().useRef(),
-                        g = r().useState(!1),
-                        y = _e(g, 2),
+                        g = r().useRef(),
+                        m = r().useState(!1),
+                        y = _e(m, 2),
                         E = y[0],
                         v = y[1],
                         x = r().useState(!1),
                         C = _e(x, 2),
                         O = C[0],
-                        D = C[1],
-                        N = r().useState(!1),
-                        w = _e(N, 2),
+                        N = C[1],
+                        D = r().useState(!1),
+                        w = _e(D, 2),
                         M = (w[0], w[1]),
                         I = r().useState({
                             x: 0,
                             y: 0
                         }),
                         T = _e(I, 2),
                         P = (T[0], T[1]),
                         R = r().useState({
                             x: 0,
                             y: 0
                         }),
-                        A = _e(R, 2),
-                        S = A[0],
-                        k = A[1],
+                        k = _e(R, 2),
+                        S = k[0],
+                        A = k[1],
                         L = r().useRef(!1);
                     r().useEffect((function() {
                         _ && (v(!0), t({
                             type: "REMOVE_COMMENT_NEW",
                             id: n
                         }))
                     }), [_, t, n]);
                     var B, W = r().useRef(null);
                     return r().useEffect((function() {
                         return function() {
                             L.current && p && p.setInputing && (p.setInputing(!1), L.current = !1)
                         }
                     }), []), p && p.outOptions && p.outOptions((ue(B = {}, "nodeDraggable_" + n, f), ue(B, "startDragDelay_" + n, W), ue(B, "commentSetIsPickingColor_" + n, (function(e) {
-                        if (D(e), f.current) {
+                        if (N(e), f.current) {
                             var t = f.current.getBoundingClientRect();
-                            k(t)
+                            A(t)
                         }
-                    })), B)), r().createElement(me, {
+                    })), B)), r().createElement(ge, {
                         innerRef: f,
                         className: "Comment_wrapper__1Pnbd",
                         style: {
                             transform: "translate(" + o + "px," + i + "px)",
                             width: a,
                             height: s,
                             zIndex: E ? 999 : ""
@@ -3117,44 +3117,44 @@
                         },
                         onBlur: function() {
                             v(!1), p && p.setInputing && (p.setInputing(!1), L.current = !1)
                         },
                         placeholder: "Text of the comment...",
                         autoFocus: !0,
                         value: u,
-                        ref: m
+                        ref: g
                     }) : r().createElement("div", {
                         "data-flume-component": "comment-text",
                         "data-comment": !0,
                         className: "Comment_text__Ie2nX"
-                    }, u), r().createElement(me, {
+                    }, u), r().createElement(ge, {
                         className: "Comment_resizeThumb__20KWn",
                         stageState: h,
                         stageRect: c,
                         onDrag: function(e) {
-                            var t = X(e.x - o + 10, 80, 1e4),
-                                n = X(e.y - i + 10, 30, 1e4);
+                            var t = q(e.x - o + 10, 80, 1e4),
+                                n = q(e.y - i + 10, 30, 1e4);
                             f.current.style.width = t + "px", f.current.style.height = n + "px"
                         },
                         onDragEnd: function(e, r) {
-                            var a = X(r.x - o + 10, 80, 1e4),
-                                s = X(r.y - i + 10, 30, 1e4);
+                            var a = q(r.x - o + 10, 80, 1e4),
+                                s = q(r.y - i + 10, 30, 1e4);
                             t({
                                 type: "SET_COMMENT_DIMENSIONS",
                                 id: n,
                                 width: a,
                                 height: s
                             })
                         },
                         "data-flume-component": "comment-resize-handle"
-                    }), O ? r().createElement(b, null, r().createElement(ko, {
+                    }), O ? r().createElement(b, null, r().createElement(Ao, {
                         x: S.x,
                         y: S.y,
                         onRequestClose: function() {
-                            return D(!1)
+                            return N(!1)
                         },
                         onColorPicked: function(e) {
                             t({
                                 type: "SET_COMMENT_COLOR",
                                 id: n,
                                 color: e
                             })
@@ -3210,32 +3210,32 @@
                         u = e.onHeightReceived,
                         c = e.onExitRequested,
                         d = e.onRemoveRequested,
                         _ = r().useState(!1),
                         p = _e(_, 2),
                         h = p[0],
                         f = p[1],
-                        m = r().useRef(),
                         g = r().useRef(),
+                        m = r().useRef(),
                         y = r().useCallback((function() {
-                            f(!0), clearTimeout(g.current)
+                            f(!0), clearTimeout(m.current)
                         }), []),
                         E = r().useCallback((function() {
-                            f(!1), g.current = setTimeout((function() {
+                            f(!1), m.current = setTimeout((function() {
                                 return c(t)
                             }), i)
                         }), [t, i, c]);
                     return r().useLayoutEffect((function() {
-                        var e = m.current.getBoundingClientRect().height;
+                        var e = g.current.getBoundingClientRect().height;
                         u(t, e)
                     }), [u, t]), r().useEffect((function() {
                         return E(), y
                     }), [E, y]), r().createElement("div", {
                         "data-flume-component": "toast",
-                        ref: m,
+                        ref: g,
                         className: "Toaster_toast__3YHVS",
                         "data-type": a,
                         style: {
                             transform: "translateY(-" + l + "px)"
                         },
                         "data-exiting": s,
                         onAnimationEnd: function() {
@@ -3357,15 +3357,15 @@
                                     nodeTypes: t,
                                     portTypes: n,
                                     context: o
                                 })
                             }));
                             var a = Object.values(r).reduce((function(e, r) {
                                 var i = t[r.type],
-                                    a = qo({
+                                    a = Xo({
                                         node: r,
                                         nodeType: i,
                                         portTypes: n,
                                         context: o
                                     }),
                                     s = Object.entries(r.inputData).reduce((function(e, t) {
                                         var n = _e(t, 2),
@@ -3397,27 +3397,27 @@
                         }, {
                             nodeTypes: n,
                             portTypes: o,
                             context: r
                         })), t
                     }), {}))
                 },
-                qo = function(e) {
+                Xo = function(e) {
                     var t = e.node,
                         n = e.nodeType,
                         o = e.portTypes,
                         r = e.context;
                     return (Array.isArray(n.inputs) ? n.inputs : n.inputs(t.inputData, t.connections, r, t.id)).reduce((function(e, t) {
                         var n = o[t.type];
                         return e[t.name || n.name] = (t.controls || n.controls || []).reduce((function(e, t) {
                             return e[t.name] = t.defaultValue, e
                         }), {}), e
                     }), {})
                 },
-                Xo = function(e) {
+                qo = function(e) {
                     var t = [];
                     for (var n in e) t.push(n);
                     var o = !0,
                         r = !1,
                         i = void 0;
                     try {
                         for (var a, s = t[Symbol.iterator](); !(o = (a = s.next()).done); o = !0) {
@@ -3504,16 +3504,16 @@
                             return e
                         };
                     switch (t.type) {
                         case "ADD_CONNECTION":
                             var h = t.input,
                                 f = t.output;
                             if (!e[h.nodeId].connections.inputs[h.portName]) {
-                                var m = "warn" === a || "allow" === a,
-                                    g = function(e, t, n, o) {
+                                var g = "warn" === a || "allow" === a,
+                                    m = function(e, t, n, o) {
                                         var r;
                                         return ce({}, e, (ue(r = {}, t.nodeId, ce({}, e[t.nodeId], {
                                             connections: ce({}, e[t.nodeId].connections, {
                                                 inputs: ce({}, e[t.nodeId].connections.inputs, ue({}, t.portName, [].concat(pe(e[t.nodeId].connections.inputs[t.portName] || []), [{
                                                     nodeId: n.nodeId,
                                                     portName: n.portName
                                                 }])))
@@ -3536,88 +3536,88 @@
                                                     if (u.nodeId === t) {
                                                         n = !0;
                                                         break
                                                     }
                                                     o(u.nodeId)
                                                 }
                                         }(t), n
-                                    }(g, f.nodeId);
-                                return y && !m ? (u({
+                                    }(m, f.nodeId);
+                                return y && !g ? (u({
                                     type: "ADD_TOAST",
                                     title: "Unable to connect",
                                     message: "Connecting these nodes would result in an infinite loop.",
                                     toastType: "warning",
                                     duration: 5e3
                                 }), e) : (y && "warn" === a && u({
                                     type: "ADD_TOAST",
                                     title: "Circular Connection Detected",
                                     message: "Connecting these nodes has created an infinite loop.",
                                     toastType: "warning",
                                     duration: 5e3
-                                }), g)
+                                }), m)
                             }
                             return e;
                         case "REMOVE_CONNECTION":
                             var E = t.input,
                                 b = t.output;
                             return d(E.nodeId, E.portName, "input"), d(b.nodeId, b.portName, "output"), c(E, b), jo(e, E, b);
                         case "DESTROY_TRANSPUT":
                             var v = t.transput,
                                 x = t.transputType,
                                 C = v.nodeId + v.portName + x;
                             delete i.current.ports[C];
                             var O = "input" === x ? "inputs" : "outputs",
-                                D = e[v.nodeId].connections[O][v.portName];
-                            return D && D.length ? D.reduce((function(e, t) {
+                                N = e[v.nodeId].connections[O][v.portName];
+                            return N && N.length ? N.reduce((function(e, t) {
                                 var n = _e("input" === x ? [v, t] : [t, v], 2),
                                     o = n[0],
                                     r = n[1],
                                     a = r.nodeId + r.portName + o.nodeId + o.portName;
                                 return delete i.current.connections[a], so({
                                     id: a
                                 }), jo(e, o, r)
                             }), e) : e;
                         case "ADD_NODE":
-                            var N = t.x,
+                            var D = t.x,
                                 w = t.y,
                                 M = t.nodeType,
                                 I = t.id,
                                 T = t.defaultNode,
                                 P = t.node,
                                 R = void 0 === P ? null : P;
                             if (null == R) {
-                                var A = I || Y(10),
+                                var k = I || Y(10),
                                     S = {
-                                        id: A,
-                                        x: N,
+                                        id: k,
+                                        x: D,
                                         y: w,
                                         type: M,
                                         width: o[M].initialWidth || 200,
                                         connections: {
                                             inputs: {},
                                             outputs: {}
                                         },
                                         inputData: {}
                                     };
-                                return S.inputData = qo({
+                                return S.inputData = Xo({
                                     node: S,
                                     nodeType: o[M],
                                     portTypes: r,
                                     context: s
-                                }), T && (S.defaultNode = !0), o[M].root && (S.root = !0), ce({}, e, ue({}, A, S))
+                                }), T && (S.defaultNode = !0), o[M].root && (S.root = !0), ce({}, e, ue({}, k, S))
                             }
                             return p(ce({}, e, ue({}, R.id, R)), R);
                         case "ADD_NODES":
-                            var k = t.nodes,
+                            var A = t.nodes,
                                 L = e,
                                 B = !0,
                                 W = !1,
                                 K = void 0;
                             try {
-                                for (var U, j = k[Symbol.iterator](); !(B = (U = j.next()).done); B = !0) {
+                                for (var U, j = A[Symbol.iterator](); !(B = (U = j.next()).done); B = !0) {
                                     var V = U.value;
                                     L = ce({}, L, ue({}, V.id, V))
                                 }
                             } catch (e) {
                                 W = !0, K = e
                             } finally {
                                 try {
@@ -3626,20 +3626,20 @@
                                     if (W) throw K
                                 }
                             }
                             var $ = !0,
                                 z = !1,
                                 F = void 0;
                             try {
-                                for (var q, X = k[Symbol.iterator](); !($ = (q = X.next()).done); $ = !0) L = p(L, L[q.value.id])
+                                for (var X, q = A[Symbol.iterator](); !($ = (X = q.next()).done); $ = !0) L = p(L, L[X.value.id])
                             } catch (e) {
                                 z = !0, F = e
                             } finally {
                                 try {
-                                    !$ && X.return && X.return()
+                                    !$ && q.return && q.return()
                                 } finally {
                                     if (z) throw F
                                 }
                             }
                             return L;
                         case "REMOVE_NODE":
                             var Z = t.nodeId;
@@ -3679,43 +3679,43 @@
                                 }
                             }
                             return J;
                         case "HYDRATE_DEFAULT_NODES":
                             var he = ce({}, e);
                             for (var fe in he)
                                 if (he[fe].defaultNode) {
-                                    var me = Y(10),
-                                        ge = he[fe],
-                                        ye = (ge.id, ge.defaultNode, de(ge, ["id", "defaultNode"]));
-                                    he[me] = ce({}, ye, {
-                                        id: me
+                                    var ge = Y(10),
+                                        me = he[fe],
+                                        ye = (me.id, me.defaultNode, de(me, ["id", "defaultNode"]));
+                                    he[ge] = ce({}, ye, {
+                                        id: ge
                                     }), delete he[fe]
                                 } return he;
                         case "SET_PORT_DATA":
                             var Ee = t.nodeId,
                                 be = t.portName,
                                 ve = t.controlName,
                                 xe = t.data,
                                 Ce = t.setValue,
                                 Oe = ce({}, e[Ee].inputData, ue({}, be, ce({}, e[Ee].inputData[be], ue({}, ve, xe))));
                             return Ce && (Oe = Ce(Oe, e[Ee].inputData)), ce({}, e, ue({}, Ee, ce({}, e[Ee], {
                                 inputData: Oe
                             })));
                         case "SET_NODE_COORDINATES":
-                            var De = t.x,
-                                Ne = t.y,
+                            var Ne = t.x,
+                                De = t.y,
                                 we = t.nodeId;
                             return ce({}, e, ue({}, we, ce({}, e[we], {
-                                x: De,
-                                y: Ne
+                                x: Ne,
+                                y: De
                             })));
                         case "CLEAR":
-                            return Xo(e);
+                            return qo(e);
                         case "RE_INIT":
-                            return Xo(e), t.nodes;
+                            return qo(e), t.nodes;
                         case "SET_NODE_WIDTH":
                             var Me = t.nodeId,
                                 Ie = t.width;
                             return ce({}, e, ue({}, Me, ce({}, e[Me], {
                                 width: Ie
                             })));
                         default:
@@ -3872,59 +3872,59 @@
                                 }
                             }));
                         return n.onlyResolveConnected ? a : ce({}, i, a)
                     }
                     return console.error("A root node was not found. The Root Engine requires that exactly one node be marked as the root node."), {}
                 }
             }]);
-            var tr = kn,
+            var tr = An,
                 nr = ie,
                 or = lo,
                 rr = uo,
                 ir = {},
                 ar = function(e, t) {
                     var n = e.comments,
                         i = e.nodes,
                         a = e.nodeTypes,
                         s = void 0 === a ? {} : a,
                         l = e.portTypes,
                         c = void 0 === l ? {} : l,
                         _ = e.defaultNodes,
                         h = void 0 === _ ? [] : _,
                         f = e.context,
-                        m = void 0 === f ? ir : f,
-                        g = e.onChange,
+                        g = void 0 === f ? ir : f,
+                        m = e.onChange,
                         y = e.onCommentsChange,
                         E = e.initialScale,
                         b = e.spaceToPan,
                         v = void 0 !== b && b,
                         x = e.hideComments,
                         C = void 0 !== x && x,
                         O = e.disableComments,
-                        D = void 0 !== O && O,
-                        N = e.disableZoom,
-                        w = void 0 !== N && N,
+                        N = void 0 !== O && O,
+                        D = e.disableZoom,
+                        w = void 0 !== D && D,
                         M = e.disablePan,
                         I = void 0 !== M && M,
                         T = e.circularBehavior,
                         P = e.renderNodeHeader,
                         R = e.debug,
-                        A = (0, o.useContext)(ie),
+                        k = (0, o.useContext)(ie),
                         S = function(e) {
                             var t = d ? p() : null,
                                 n = (0, o.useState)(t),
                                 r = n[0],
                                 i = n[1];
                             return u((function() {
                                 null === r && i(p())
                             }), []), (0, o.useEffect)((function() {
                                 !1 === d && (d = !0)
                             }), []), null != r ? String(r) : void 0
                         }(),
-                        k = r().useRef(new Go),
+                        A = r().useRef(new Go),
                         L = r().useRef(),
                         B = r().useState(),
                         W = _e(B, 2),
                         K = W[0],
                         U = W[1],
                         j = r().useReducer(Ho, []),
                         V = _e(j, 2),
@@ -3933,24 +3933,24 @@
                         F = r().useReducer(function(e, t, n) {
                             return function(o, r) {
                                 return e(o, r, t, n)
                             }
                         }(Yo, {
                             nodeTypes: s,
                             portTypes: c,
-                            cache: k,
+                            cache: A,
                             circularBehavior: T,
-                            context: m,
-                            owner: A
+                            context: g,
+                            owner: k
                         }, U), {}, (function() {
-                            return Fo(i, h, s, c, m)
+                            return Fo(i, h, s, c, g)
                         })),
-                        q = _e(F, 2),
-                        Z = q[0],
-                        ae = q[1],
+                        X = _e(F, 2),
+                        Z = X[0],
+                        ae = X[1],
                         se = r().useReducer(function(e) {
                             return function() {
                                 return function() {
                                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                                         t = arguments[1],
                                         n = arguments[2];
                                     switch (n && n.onCommentsAction && n.onCommentsAction(e, t, Y), t.type) {
@@ -4014,29 +4014,29 @@
                                             }
                                             return ce({}, e);
                                         default:
                                             return e
                                     }
                                 }(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {}, arguments[1], e)
                             }
-                        }(A), n || {}),
+                        }(k), n || {}),
                         le = _e(se, 2),
                         pe = le[0],
                         he = le[1];
                     r().useEffect((function() {
                         ae({
                             type: "HYDRATE_DEFAULT_NODES"
                         })
                     }), []);
                     var fe = r().useState(!0),
-                        me = _e(fe, 2),
-                        ge = me[0],
-                        ye = me[1],
+                        ge = _e(fe, 2),
+                        me = ge[0],
+                        ye = ge[1],
                         Ee = r().useReducer(Jo, {
-                            scale: "number" == typeof E ? X(E, .1, 7) : 1,
+                            scale: "number" == typeof E ? q(E, .1, 7) : 1,
                             translate: {
                                 x: 0,
                                 y: 0
                             }
                         }),
                         be = _e(Ee, 2),
                         ve = be[0],
@@ -4110,74 +4110,74 @@
                                 }
                             }(Z, ve, S)
                         }), [Z, S, ve]),
                         Oe = r().useCallback((function() {
                             L.current = document.getElementById("" + Rn + S).getBoundingClientRect()
                         }), [S]);
                     r().useLayoutEffect((function() {
-                        ge && (Ce(), ye(!1))
-                    }), [ge, Ce]);
-                    var De = r().useCallback((function() {
+                        me && (Ce(), ye(!1))
+                    }), [me, Ce]);
+                    var Ne = r().useCallback((function() {
                         ye(!0)
                     }), []);
                     r().useImperativeHandle(t, (function() {
                         return {
                             getNodes: function() {
                                 return Z
                             },
                             getComments: function() {
                                 return pe
                             }
                         }
                     }));
-                    var Ne = vo(Z);
+                    var De = vo(Z);
                     r().useEffect((function() {
-                        Ne && g && Z !== Ne && g(Z)
-                    }), [Z, Ne, g]);
+                        De && m && Z !== De && m(Z)
+                    }), [Z, De, m]);
                     var we = vo(pe);
                     return r().useEffect((function() {
                         we && y && pe !== we && y(pe)
                     }), [pe, we, y]), r().useEffect((function() {
                         K && (z(K), U(null))
-                    }), [K]), A && A.outOptions && (A.dispatchNodes = ae, A.getInitialNodes = Fo, A.dispatchComments = he, A.outOptions({
+                    }), [K]), k && k.outOptions && (k.dispatchNodes = ae, k.getInitialNodes = Fo, k.dispatchComments = he, k.outOptions({
                         refreshCache: function() {
-                            k.current = new Go
+                            A.current = new Go
                         },
                         recalculateStageRect: Oe,
                         nanoid: Y,
                         editorId: S,
-                        triggerRecalculation: De
+                        triggerRecalculation: Ne
                     })), r().createElement(J.Provider, {
                         value: c
                     }, r().createElement(H.Provider, {
                         value: s
                     }, r().createElement(G.Provider, {
                         value: ae
                     }, r().createElement(Q.Provider, {
-                        value: De
+                        value: Ne
                     }, r().createElement(ee.Provider, {
-                        value: m
+                        value: g
                     }, r().createElement(te.Provider, {
                         value: ve
                     }, r().createElement(ne.Provider, {
-                        value: k
+                        value: A
                     }, r().createElement(re.Provider, {
                         value: S
                     }, r().createElement(oe.Provider, {
                         value: Oe
                     }, r().createElement(Ln, {
                         editorId: S,
                         scale: ve.scale,
                         translate: ve.translate,
                         spaceToPan: v,
                         disablePan: I,
                         disableZoom: w,
                         dispatchStageState: xe,
                         dispatchComments: he,
-                        disableComments: D || C,
+                        disableComments: N || C,
                         stageRef: L,
                         numNodes: Object.keys(Z).length,
                         outerStageChildren: r().createElement(r().Fragment, null, R && r().createElement("div", {
                             className: Qo.debugWrapper
                         }, r().createElement("button", {
                             className: Qo.debugButton,
                             onClick: function() {
@@ -4203,26 +4203,26 @@
                             dispatch: he,
                             onDragStart: Oe,
                             key: e.id
                         }))
                     })), Object.values(Z).map((function(e) {
                         return r().createElement(wo, ce({}, e, {
                             stageRect: L,
-                            onDragEnd: De,
+                            onDragEnd: Ne,
                             onDragStart: Oe,
                             renderNodeHeader: P,
                             key: e.id
                         }))
                     })), r().createElement(Uo, {
                         nodes: Z,
                         editorId: S
                     }), r().createElement("div", {
                         className: Qo.dragWrapper,
-                        id: "" + An + S
-                    })), A && A.refreshNodeBoxShadow())))))))))
+                        id: "" + kn + S
+                    })), k && k.refreshNodeBoxShadow())))))))))
                 };
             ar = r().forwardRef(ar)
         },
         8327: (e, t, n) => {
             "use strict";
             var o = n(5377);
 
@@ -4466,48 +4466,49 @@
                     fill: s
                 })))
             }
         },
         5764: (e, t, n) => {
             "use strict";
             n.d(t, {
-                $4: () => c,
-                Ao: () => p,
-                J8: () => g,
-                Mz: () => y,
+                $4: () => d,
+                Ao: () => h,
+                J8: () => y,
+                Mz: () => E,
                 ZP: () => D,
-                Zo: () => u,
-                bN: () => _,
-                kN: () => l,
-                mN: () => E,
-                tq: () => O,
-                y9: () => b
+                Zo: () => c,
+                bN: () => p,
+                kN: () => u,
+                mN: () => b,
+                tq: () => N,
+                y9: () => v
             });
             var o = n(6037),
                 r = n(6029),
                 i = n.n(r),
                 a = n(6988),
-                s = n(3593);
-            let l = 16,
-                u = 200,
-                c = 1e3,
-                d = {};
+                s = n(3593),
+                l = n(3172);
+            let u = 16,
+                c = 200,
+                d = 1e3,
+                _ = {};
 
-            function _(e, t) {
-                let n = d[e];
+            function p(e, t) {
+                let n = _[e];
                 n && n(t)
             }
 
-            function p(e) {
+            function h(e) {
                 let t = [];
-                for (const n in d) e.editorNodes[n] || t.push(n);
-                for (const e of t) delete d[e]
+                for (const n in _) e.editorNodes[n] || t.push(n);
+                for (const e of t) delete _[e]
             }
-            let h = {},
-                f = {},
+            let f = {},
+                g = {},
                 m = {
                     any: (e, t, n, r) => e.any({
                         label: t,
                         name: n,
                         controls: [o.ZX.text({
                             label: t,
                             name: n,
@@ -4605,37 +4606,37 @@
                             name: n,
                             label: t,
                             options: r
                         })]
                     })
                 };
 
-            function g(e) {
-                return [y("control")(e), y("any")(e, "输出", "out", "None")]
+            function y(e) {
+                return [E("control")(e), E("any")(e, "输出", "out", "None")]
             }
 
-            function y(e) {
+            function E(e) {
                 let t = m[e];
                 return t || (t = m.any), t
             }
 
-            function E(e) {
+            function b(e) {
                 let t, n = -1;
                 for (const o in e) {
                     let e = /v(\d)/g.exec(o);
                     e && (t = Number(e[1]), n < t && (n = t))
                 }
                 return n
             }
 
-            function b(e) {
+            function v(e) {
                 return `v${e}`
             }
 
-            function v(e, t, n, o) {
+            function x(e, t, n, o) {
                 let r = `[data-node-id='${t}'][data-port-name='${n}']`,
                     i = e.querySelector(r);
                 if (!i || !i.parentElement) return !1;
                 let a = i.getAttribute("data-port-type");
                 switch (a) {
                     case "string":
                     case "any": {
@@ -4664,15 +4665,15 @@
                             case "number":
                                 t.value = o ? `${o}` : "0"
                         }
                     }
                 }
             }
 
-            function x(e) {
+            function C(e) {
                 switch (e) {
                     case "dict":
                         return "{}";
                     case "tuple":
                         return "()";
                     case "any":
                         return "None";
@@ -4684,19 +4685,19 @@
                         return "";
                     case "bool":
                     case "boolean":
                         return !1
                 }
             }
 
-            function C(e, t) {
+            function O(e, t) {
                 return `${e}@${t}`
             }
 
-            function O(e) {
+            function N(e) {
                 return /(\S+?)@(\S+)/g.exec(e)
             }
 
             function D() {
                 const e = new o.ik;
                 return e.addPortType({
                     type: "any",
@@ -4758,25 +4759,69 @@
                     controls: [o.ZX.custom({
                         name: "image",
                         label: "image",
                         defaultValue: {
                             urls: [],
                             index: 0
                         },
-                        render: (e, t, n, o, r, a) => {
-                            function s() {
+                        render: (e, t, n, a, s, u) => {
+                            function c() {
                                 n.setShowImgUrls(e.urls), n.setShowImgStartIndex(e.index), n.setShowImg(!0)
                             }
-                            return d[r.nodeId] = e => {
+                            _[s.nodeId] = e => {
                                 t({
                                     urls: e,
                                     index: 0
                                 })
-                            }, i().createElement("div", null, i().createElement("button", {
-                                onClick: s
+                            };
+                            const [d, p] = (0, r.useState)(!1), h = i().useRef(null), f = i().useRef(null), g = i().useRef(!1), m = i().useRef(null), y = i().useRef(null), E = (e, t) => {
+                                const o = f.current,
+                                    r = n.editorOptions.stagetScale,
+                                    i = o.getBoundingClientRect();
+                                let a = (e - i.x) / r,
+                                    s = (t - i.y) / r;
+                                return {
+                                    posX: a,
+                                    posY: s,
+                                    imgPosX: Math.floor(a / (i.width / r) * o.naturalWidth),
+                                    imgPosY: Math.floor(s / (i.height / r) * o.naturalHeight)
+                                }
+                            }, b = e => {
+                                if (!h.current || !f.current) return;
+                                const t = f.current,
+                                    n = h.current;
+                                let {
+                                    posX: o,
+                                    posY: r,
+                                    imgPosX: i,
+                                    imgPosY: a
+                                } = E(e.clientX, e.clientY);
+                                if (n.style.position = "absolute", n.style.left = `${o}px`, n.style.top = `${r}px`, g.current && m.current) {
+                                    let e = E(m.current.x, m.current.y);
+                                    n.innerText = `[${e.imgPosX}, ${e.imgPosY}, ${i}, ${a}]`
+                                } else n.innerText = `[${i}, ${a}]`;
+                                (i < 0 || i >= t.naturalWidth || a < 0 || a >= t.naturalHeight) && p(!1)
+                            }, v = (e, t) => {
+                                if (2 === e.button)
+                                    if (g.current = t, t) m.current = {
+                                        x: e.clientX,
+                                        y: e.clientY
+                                    }, y.current && y.current.setAttribute("d", "");
+                                    else {
+                                        m.current = null;
+                                        const e = h.current;
+                                        navigator.clipboard.writeText(e.innerText).then((() => {
+                                            l.Notification.success(`复制选取到剪切板成功${e.innerText}`)
+                                        })).catch((e => {
+                                            l.Notification.error("复制选取到剪切板错误！")
+                                        }))
+                                    }
+                            };
+                            return i().createElement("div", null, i().createElement("button", {
+                                onClick: c
                             }, "浏览"), i().createElement("button", {
                                 onClick: n => {
                                     let o = (e.index - 1 + e.urls.length) % e.urls.length;
                                     t({
                                         urls: e.urls,
                                         index: o
                                     })
@@ -4785,35 +4830,82 @@
                                 onClick: n => {
                                     let o = (e.index + 1) % e.urls.length;
                                     t({
                                         urls: e.urls,
                                         index: o
                                     })
                                 }
-                            }, "下一个"), i().createElement("span", null, "当前索引:", e.index), i().createElement("img", {
+                            }, "下一个"), i().createElement("span", null, "当前索引:", e.index), i().createElement("div", {
+                                style: {
+                                    position: "relative",
+                                    top: "0px",
+                                    left: "0px"
+                                },
+                                onMouseEnter: e => {
+                                    p(!0), b(e)
+                                },
+                                onMouseMove: e => {
+                                    d && (g.current && (e => {
+                                        if (!y.current) {
+                                            const e = document.createElementNS("http://www.w3.org/2000/svg", "svg");
+                                            e.setAttribute("class", o.oP), e.setAttribute("style", "z-index:100;"), e.setAttribute("viewport", "0 0 ");
+                                            const t = document.createElementNS("http://www.w3.org/2000/svg", "path");
+                                            if (t.setAttribute("stroke", "rgb(185, 186, 189)"), t.setAttribute("stroke-width", "1"), t.setAttribute("stroke-linecap", "round"), t.setAttribute("fill", "rgba(255,255,255,0.2)"), t.setAttribute("d", ""), e.appendChild(t), f.current) {
+                                                let t = f.current;
+                                                t.parentElement && t.parentElement.appendChild(e)
+                                            }
+                                            y.current = t
+                                        }
+                                        if (y.current && m.current) {
+                                            const t = f.current.getBoundingClientRect(),
+                                                o = n.editorOptions.stagetScale;
+                                            let r = m.current,
+                                                i = (r.x - t.x) / o,
+                                                a = (r.y - t.y) / o,
+                                                s = (e.clientX - t.x) / o - i,
+                                                l = (e.clientY - t.y) / o - a;
+                                            y.current.setAttribute("d", `M ${i} ${a} h ${s} v ${l} h ${-s} Z`)
+                                        }
+                                    })(e), b(e))
+                                },
+                                onMouseLeave: e => {
+                                    p(!1)
+                                },
+                                onMouseDown: e => v(e, !0),
+                                onMouseUp: e => v(e, !1)
+                            }, i().createElement("img", {
+                                style: {
+                                    width: "100%",
+                                    height: "100%",
+                                    objectFit: "contain"
+                                },
                                 onLoad: e => {
                                     try {
-                                        n.updateNodeConnections(r.nodeId)
+                                        n.updateNodeConnections(s.nodeId)
                                     } catch (e) {}
                                 },
-                                onDoubleClick: s,
-                                id: "img_" + r.nodeId,
-                                style: {
-                                    width: "100%"
-                                },
+                                onDoubleClick: c,
+                                id: "img_" + s.nodeId,
+                                ref: f,
                                 src: (() => {
                                     "object" != typeof e.urls && (e.urls = [""], e.index = 0, t({
                                         urls: e.urls,
                                         index: 0
                                     }));
                                     let n = e.urls || [],
                                         o = e.index || 0;
                                     if (0 != n.length) return n[o]
                                 })()
-                            }))
+                            }), d && i().createElement("span", {
+                                ref: h,
+                                style: {
+                                    position: "absolute",
+                                    backgroundColor: "white"
+                                }
+                            })))
                         }
                     })]
                 }).addPortType({
                     type: "video",
                     name: "video",
                     label: "视频",
                     color: o.wL.pink,
@@ -4821,15 +4913,15 @@
                     controls: [o.ZX.custom({
                         name: "video",
                         label: "video",
                         defaultValue: {
                             urls: [],
                             index: 0
                         },
-                        render: (e, t, n, o, r, a) => (d[r.nodeId] = e => {
+                        render: (e, t, n, o, r, a) => (_[r.nodeId] = e => {
                             t({
                                 urls: e,
                                 index: 0
                             })
                         }, i().createElement("div", null, i().createElement("button", {
                             onClick: n => {
                                 let o = (e.index - 1 + e.urls.length) % e.urls.length;
@@ -4956,40 +5048,40 @@
                         defaultValue: [],
                         render: (e, t, n, o, r, a) => i().createElement("div", null, i().createElement("button", {
                             onClick: o => {
                                 ! function(e, t, o) {
                                     e.splice(t, 0, o);
                                     let i = n.editorNodes[r.nodeId];
                                     if (i) {
-                                        let e, n = E(i.inputData),
+                                        let e, n = b(i.inputData),
                                             o = i.inputData;
                                         for (let r = n; r >= t; r--) try {
-                                            e = o[b(r)], e ? o[b(r + 1)] = {
-                                                [b(r + 1)]: e[b(r)]
-                                            } : delete o[b(r + 1)]
+                                            e = o[v(r)], e ? o[v(r + 1)] = {
+                                                [v(r + 1)]: e[v(r)]
+                                            } : delete o[v(r + 1)]
                                         } catch (e) {}
                                         try {
-                                            delete o[b(t)]
+                                            delete o[v(t)]
                                         } catch (e) {}
                                         console.log(o)
                                     }
                                 }(e, a.index, a.type), t(e)
                             }
                         }, "添加+"), i().createElement("button", {
                             onClick: o => {
                                 ! function(e, t) {
                                     e.splice(t, 1);
                                     let o = n.editorNodes[r.nodeId];
                                     if (o) {
                                         let e, n = o.inputData,
-                                            r = E(n);
-                                        for (let o = t; o < r; o++) e = n[b(o + 1)], e ? n[b(o)] = {
-                                            [b(o)]: e[b(o + 1)]
-                                        } : delete n[b(o)];
-                                        delete n[b(r)], console.log(n)
+                                            r = b(n);
+                                        for (let o = t; o < r; o++) e = n[v(o + 1)], e ? n[v(o)] = {
+                                            [v(o)]: e[v(o + 1)]
+                                        } : delete n[v(o)];
+                                        delete n[v(r)], console.log(n)
                                     }
                                 }(e, a.index), t(e)
                             }
                         }, "删除-"))
                     })]
                 }).addPortType({
                     type: "dict_editor",
@@ -5181,155 +5273,155 @@
                         }
                     })]
                 }).addNodeType({
                     type: "image",
                     label: "图片显示(show image)",
                     description: "图片显示(show image)",
                     initialWidth: 250,
-                    inputs: e => [y("control")(e), y("string")(e, "url列表", "urls"), e.image({
+                    inputs: e => [E("control")(e), E("string")(e, "url列表", "urls"), e.image({
                         hidePort: !0
                     })],
-                    outputs: g
+                    outputs: y
                 }).addNodeType({
                     type: "video",
                     label: "视频(show video)",
                     description: "视频(show video)",
                     initialWidth: 250,
-                    inputs: e => [y("control")(e), y("string")(e, "url列表", "urls"), e.video({
+                    inputs: e => [E("control")(e), E("string")(e, "url列表", "urls"), e.video({
                         hidePort: !0
                     })],
-                    outputs: g
+                    outputs: y
                 }).addNodeType({
                     type: "any",
                     label: "任意类型(any)",
                     description: "任意类型(any)",
-                    initialWidth: (0, a.cx)("any", l, u, c),
-                    inputs: e => [y("control")(e), y("any")(e, "值", "value", "None")],
-                    outputs: g
+                    initialWidth: (0, a.cx)("any", u, c, d),
+                    inputs: e => [E("control")(e), E("any")(e, "值", "value", "None")],
+                    outputs: y
                 }).addNodeType({
                     type: "tuple",
                     label: "元组(tuple)",
                     description: "元组(tuple)",
                     initialWidth: 250,
                     inputs: e => (t, n, o, r) => {
-                        let i = [y("control")(e), e.tuple_editor()],
+                        let i = [E("control")(e), e.tuple_editor()],
                             a = 0;
                         if (t.tuple_editor && t.tuple_editor.tuple_editor) {
                             for (const n of t.tuple_editor.tuple_editor) {
-                                let t = y(n),
-                                    o = b(a++),
-                                    r = x(n),
+                                let t = E(n),
+                                    o = v(a++),
+                                    r = C(n),
                                     s = t(e, o, o, r);
                                 i.push(s)
                             }
-                            let n = h[r];
+                            let n = f[r];
                             n && n.length == t.tuple_editor.tuple_editor.length || setTimeout((() => {
                                 let e = 0;
                                 for (const n of t.tuple_editor.tuple_editor) {
-                                    let n = b(e++);
-                                    v(o.node, r, n, t[n] ? t[n][n] : null)
+                                    let n = v(e++);
+                                    x(o.node, r, n, t[n] ? t[n][n] : null)
                                 }
-                            })), h[r] = JSON.parse(JSON.stringify(t.tuple_editor.tuple_editor))
+                            })), f[r] = JSON.parse(JSON.stringify(t.tuple_editor.tuple_editor))
                         }
                         return i
                     },
-                    outputs: g
+                    outputs: y
                 }).addNodeType({
                     type: "dict",
                     label: "字典(dict)",
                     description: "字典(dict)",
                     initialWidth: 250,
                     inputs: e => (t, n, o, r) => {
-                        let i = [y("control")(e), e.dict_editor()];
+                        let i = [E("control")(e), e.dict_editor()];
                         if (t.dict_editor && t.dict_editor.dict_editor) {
                             let n, a, s = t.dict_editor.dict_editor,
                                 l = !1,
-                                u = f[r];
+                                u = g[r];
                             for (const t in s) {
                                 n = s[t];
-                                let o = y(n),
-                                    r = x(n);
-                                a = C(t, n);
+                                let o = E(n),
+                                    r = C(n);
+                                a = O(t, n);
                                 let c = o(e, a, a, r);
                                 i.push(c), !u || u[t] && u[t] == n || (l = !0)
                             }
                             if (u && !l)
                                 for (const e in u) s[e] && u[e] == s[e] || (l = !0);
                             u && !l || setTimeout((() => {
-                                for (const e in t.dict_editor.dict_editor) a = C(e, n), v(o.node, r, a, t[a] ? t[a][a] : null)
-                            })), f[r] = JSON.parse(JSON.stringify(t.dict_editor.dict_editor))
+                                for (const e in t.dict_editor.dict_editor) a = O(e, n), x(o.node, r, a, t[a] ? t[a][a] : null)
+                            })), g[r] = JSON.parse(JSON.stringify(t.dict_editor.dict_editor))
                         }
                         return i
                     },
-                    outputs: g
+                    outputs: y
                 }).addNodeType({
                     type: "int",
                     label: "整数(int)",
                     description: "整数(int)",
-                    initialWidth: (0, a.cx)("int", l, u, c),
-                    inputs: e => [y("control")(e), y("str")(e, "值", "value", 0)],
-                    outputs: g
+                    initialWidth: (0, a.cx)("int", u, c, d),
+                    inputs: e => [E("control")(e), E("str")(e, "值", "value", 0)],
+                    outputs: y
                 }).addNodeType({
                     type: "float",
                     label: "浮点数(float)",
                     description: "浮点数(float)",
-                    initialWidth: (0, a.cx)("float", l, u, c),
-                    inputs: e => [y("control")(e), y("str")(e, "值", "value", 0)],
-                    outputs: g
+                    initialWidth: (0, a.cx)("float", u, c, d),
+                    inputs: e => [E("control")(e), E("str")(e, "值", "value", 0)],
+                    outputs: y
                 }).addNodeType({
                     type: "string",
                     label: "文本/字符串(string)",
                     description: "文本/字符串(string)",
                     initialWidth: 500,
-                    inputs: e => [y("control")(e), y("string")(e, " ", "value", 0)],
-                    outputs: g
+                    inputs: e => [E("control")(e), E("string")(e, " ", "value", 0)],
+                    outputs: y
                 }).addNodeType({
                     type: "bool",
                     label: "布尔(bool)(真/假)",
                     description: "布尔(bool)(真/假)",
-                    initialWidth: (0, a.cx)("bool", l, u, c),
-                    inputs: e => [y("control")(e), y("bool")(e, "值", "value", 0)],
-                    outputs: g
+                    initialWidth: (0, a.cx)("bool", u, c, d),
+                    inputs: e => [E("control")(e), E("bool")(e, "值", "value", 0)],
+                    outputs: y
                 }).addNodeType({
                     type: "if",
                     label: "条件判定(if)",
                     description: "条件判定(if)",
-                    initialWidth: (0, a.cx)("if", l, u, c),
-                    inputs: e => [y("bool")(e, "判定", "value", 0), y("any")(e, "真", "true", "None"), y("any")(e, "假", "false", "None")],
-                    outputs: g
+                    initialWidth: (0, a.cx)("if", u, c, d),
+                    inputs: e => [E("bool")(e, "判定", "value", 0), E("any")(e, "真", "true", "None"), E("any")(e, "假", "false", "None")],
+                    outputs: y
                 }).addNodeType({
                     type: "loop",
                     label: "循环(loop)",
                     description: "循环(loop)",
-                    initialWidth: (0, a.cx)("loop", l, u, c),
-                    inputs: e => [y("control")(e), y("bool")(e, "判定", "value", 0), e.control({
+                    initialWidth: (0, a.cx)("loop", u, c, d),
+                    inputs: e => [E("control")(e), E("bool")(e, "判定", "value", 0), e.control({
                         label: "循环",
                         name: "loop"
                     })],
-                    outputs: e => [y("control")(e)]
+                    outputs: e => [E("control")(e)]
                 }).addNodeType({
                     type: "operator",
                     label: "操作符(operator)",
                     description: "操作符(operator)",
-                    initialWidth: (0, a.cx)("operator", l, u, c),
-                    inputs: e => [y("control")(e), e.operator(), y("any")(e, "参数1", "value1", "None"), y("any")(e, "参数2", "value2", "None")],
-                    outputs: g
+                    initialWidth: (0, a.cx)("operator", u, c, d),
+                    inputs: e => [E("control")(e), e.operator(), E("any")(e, "参数1", "value1", "None"), E("any")(e, "参数2", "value2", "None")],
+                    outputs: y
                 }).addNodeType({
                     type: "setvar",
                     label: "设置变量(setvar)",
                     description: "设置变量(setvar)",
-                    initialWidth: (0, a.cx)("设置变量(setvar)", l, u, c),
-                    inputs: e => [y("control")(e), y("any")(e, "变量名", "name", ""), y("any")(e, "值", "value", "None")],
-                    outputs: g
+                    initialWidth: (0, a.cx)("设置变量(setvar)", u, c, d),
+                    inputs: e => [E("control")(e), E("any")(e, "变量名", "name", ""), E("any")(e, "值", "value", "None")],
+                    outputs: y
                 }).addNodeType({
                     type: "start",
                     label: "开始(start)",
                     description: "开始(start)",
-                    initialWidth: (0, a.cx)("开始(start)", l, u, c),
-                    inputs: e => [y("control")(e)],
+                    initialWidth: (0, a.cx)("开始(start)", u, c, d),
+                    inputs: e => [E("control")(e)],
                     outputs: []
                 }), e
             }
         },
         3336: (e, t, n) => {
             "use strict";
             n.d(t, {
@@ -5344,71 +5436,71 @@
                     startIndex: n = 0,
                     maxScale: a = 100,
                     minScale: s = .1
                 } = e, [l, u] = (0, o.useState)(n), c = (0, o.useRef)(null), d = (0, o.useRef)(null), _ = (0, o.useRef)(!1), p = (0, o.useRef)(null);
                 let h = t;
                 Array.isArray(t) || (h = [t]);
                 const f = (0, o.useRef)(1),
-                    m = (0, o.useRef)(f.current),
-                    g = e => {
-                        m.current = f.current, f.current = e, b()
+                    g = (0, o.useRef)(f.current),
+                    m = e => {
+                        g.current = f.current, f.current = e, b()
                     },
                     y = (0, o.useRef)({
                         x: 0,
                         y: 0
                     });
 
                 function E(e) {
                     y.current = e, b()
                 }
 
                 function b() {
                     null != c.current && (c.current.style.transform = `translate(${y.current.x}px, ${y.current.y}px) scale(${f.current})`)
                 }
                 const v = (e, t) => {
-                        if (g(e), null != c.current) {
+                        if (m(e), null != c.current) {
                             const e = c.current.getBoundingClientRect(),
                                 n = t.clientX,
                                 o = t.clientY;
                             let r = n - (e.x + e.width / 2),
                                 i = o - e.y,
-                                a = r - r / m.current * f.current,
-                                s = i - i / m.current * f.current;
+                                a = r - r / g.current * f.current,
+                                s = i - i / g.current * f.current;
                             E({
                                 x: y.current.x + a,
                                 y: y.current.y + s
                             })
                         }
                     },
                     x = e => Math.max(Math.min(e, a), s),
                     C = (0, o.useRef)(!1),
                     O = e => {
                         C.current = e
                     },
-                    D = e => {
+                    N = e => {
                         O(!0);
                         let t = c.current;
                         t.style.cursor = "grabbing";
                         try {
                             t.setPointerCapture(e.pointerId)
                         } catch (e) {}
                     },
-                    N = e => {
+                    D = e => {
                         O(!1);
                         let t = c.current;
                         t.style.cursor = "grab";
                         try {
                             t.releasePointerCapture(e.pointerId)
                         } catch (e) {}
                     },
                     w = () => {
                         null != c.current && null != d.current && (c.current.style.transformOrigin = "50% 0", E({
                             x: 0,
                             y: 0
-                        }), g(1))
+                        }), m(1))
                     },
                     M = h.length,
                     I = e => {
                         u((e => (e - 1 + M) % M))
                     },
                     T = e => {
                         console.log(e), u((e => (e + 1) % M))
@@ -5421,28 +5513,28 @@
                             I();
                             break;
                         case "d":
                         case "ArrowRight":
                             T(e);
                             break;
                         case " ":
-                            D(e);
+                            N(e);
                             break;
                         case "s":
                             _.current = !0;
                             break;
                         case "g":
                             w()
                     }
                 }
 
                 function R(e) {
                     switch (e.stopPropagation(), e.preventDefault(), e.key) {
                         case " ":
-                            N(e);
+                            D(e);
                             break;
                         case "s":
                             _.current = !1, p.current = null
                     }
                 }
                 return r().useEffect((() => (document.addEventListener("keydown", P), document.addEventListener("keyup", R), () => {
                     document.removeEventListener("keydown", P), document.removeEventListener("keyup", R)
@@ -5452,41 +5544,47 @@
                         backgroundColor: "black",
                         width: "100%",
                         height: "100%",
                         display: "flex",
                         justifyContent: "center"
                     },
                     onMouseDown: e => {
-                        e.preventDefault(), D(e)
+                        e.preventDefault(), N(e)
                     },
                     onMouseMove: e => {
                         if (e.preventDefault(), C.current && E({
                                 x: y.current.x + e.movementX,
                                 y: y.current.y + e.movementY
                             }), _.current)
                             if (p.current) {
                                 let t = x(f.current + .01 * e.movementX);
                                 v(t, p.current)
                             } else p.current = e
                     },
                     onMouseUp: e => {
-                        e.preventDefault(), N(e)
+                        e.preventDefault(), D(e)
                     }
-                }, r().createElement("img", {
+                }, r().createElement("div", {
+                    ref: c,
                     onWheel: e => {
                         const t = x(f.current + (e.deltaY < 0 ? .1 : -.1));
                         v(t, e)
+                    }
+                }, r().createElement("img", {
+                    style: {
+                        width: "100%",
+                        height: "100%",
+                        objectFit: "contain"
                     },
                     src: h[l],
                     alt: "Image",
-                    ref: c,
                     onLoad: e => {
                         w()
                     }
-                }), r().createElement("div", {
+                })), r().createElement("div", {
                     style: {
                         position: "absolute",
                         left: 0,
                         top: "calc(50% - 50px)"
                     }
                 }, r().createElement(i.Z, {
                     onClick: I,
@@ -5937,54 +6035,54 @@
                             d(e)
                         };
                         const _ = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(null);
                         this._editorContainerRef = _;
                         const [p, h] = (0, react__WEBPACK_IMPORTED_MODULE_8__.useState)(!1);
                         this._setshowCodeEditor = h;
                         const f = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(null),
-                            [m, g] = (0, react__WEBPACK_IMPORTED_MODULE_8__.useState)(!1);
-                        this._setUseDiffEditor = g;
+                            [g, m] = (0, react__WEBPACK_IMPORTED_MODULE_8__.useState)(!1);
+                        this._setUseDiffEditor = m;
                         const [y, E] = react__WEBPACK_IMPORTED_MODULE_8___default().useState(!1), [b, v] = react__WEBPACK_IMPORTED_MODULE_8___default().useState({
                             x: 0,
                             y: 0
                         }), [x, C] = (0, react__WEBPACK_IMPORTED_MODULE_8__.useState)([]), O = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(null);
                         this._cellIndexInputRef = O, this._kernelStateLabelNodeEditorRef = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(null), this._kernelStateLabelCodeEditorRef = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(null), this._nodeIsDefaultLabelRef = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(null), react__WEBPACK_IMPORTED_MODULE_8___default().useEffect((() => {
                             if (e) this._commonFilterKeys(), this._setshowCodeEditor(!1), this._setShowOutputArea(!1);
                             else {
                                 const e = this.editorOptions.draggableRef;
                                 e.current && e.current.focus(), this.keyEventFilter.clear()
                             }
                         }), [e]);
-                        const D = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(0);
+                        const N = react__WEBPACK_IMPORTED_MODULE_8___default().useRef(0);
                         react__WEBPACK_IMPORTED_MODULE_8___default().useEffect((() => {
                             if (c) {
                                 const e = u.current;
-                                _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ReactWidget.attach(this._outputArea, e, null), e.scrollTop = e.scrollHeight - e.clientHeight, D.current = e.scrollTop
+                                _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ReactWidget.attach(this._outputArea, e, null), e.scrollTop = e.scrollHeight - e.clientHeight, N.current = e.scrollTop
                             }
                             this._onResize()
                         }), [c]), react__WEBPACK_IMPORTED_MODULE_8___default().useEffect((() => {
-                            if (p) this._commonFilterKeys(), this.setShowImg(!1), f.current && (m ? (this._codeDiffEditor = monaco_editor__WEBPACK_IMPORTED_MODULE_11__.editor.createDiffEditor(f.current, {
+                            if (p) this._commonFilterKeys(), this.setShowImg(!1), f.current && (g ? (this._codeDiffEditor = monaco_editor__WEBPACK_IMPORTED_MODULE_11__.editor.createDiffEditor(f.current, {
                                 originalEditable: !0,
                                 automaticLayout: !0,
                                 theme: "vs-dark"
                             }), this._codeDiffEditor.focus()) : (this._codeEditor = monaco_editor__WEBPACK_IMPORTED_MODULE_11__.editor.create(f.current, {
                                 theme: "vs-dark",
                                 language: "python"
                             }), this._codeEditor.focus(), this._codeEditor.onDidChangeModelContent((e => {
                                 var t;
                                 this._onCodeEditorChange(null === (t = this._codeEditor) || void 0 === t ? void 0 : t.getValue(), e)
                             })), this._codeEditor.onContextMenu((e => {
-                                N(e)
+                                D(e)
                             }))));
                             else {
                                 const e = this.editorOptions.draggableRef;
                                 e.current && e.current.focus(), this.keyEventFilter.clear(), this._setShowOutputArea(!1), this._codeDiffEditor && (this._codeDiffEditor = null), this._codeEditor && (this._codeEditor = null)
                             }
                         }), [p]);
-                        const N = e => (e.event.preventDefault(), v({
+                        const D = e => (e.event.preventDefault(), v({
                             x: e.event.posx,
                             y: e.event.posy
                         }), E(!0), !1);
                         react__WEBPACK_IMPORTED_MODULE_8___default().useEffect((() => {
                             if (y) {
                                 const e = this._context.model.cells.length,
                                     t = [];
@@ -6007,15 +6105,15 @@
                         return react__WEBPACK_IMPORTED_MODULE_8___default().createElement(_flume__WEBPACK_IMPORTED_MODULE_7__.BC.Provider, {
                             value: this
                         }, react__WEBPACK_IMPORTED_MODULE_8___default().createElement("div", {
                             ref: l,
                             className: "nd-container",
                             "data-show-image-viewer": e,
                             "data-show-code-editor": p,
-                            "data-use-diff-editor": m,
+                            "data-use-diff-editor": g,
                             "data-inputing": "false"
                         }, c && react__WEBPACK_IMPORTED_MODULE_8___default().createElement("div", {
                             style: {
                                 position: "absolute",
                                 left: "0px",
                                 top: "0px",
                                 backgroundColor: "white",
@@ -6065,15 +6163,15 @@
                             style: {
                                 width: "100%",
                                 height: "calc(100% - 24px)",
                                 overflowY: "scroll"
                             },
                             onScroll: e => {
                                 let t = e.target;
-                                t.scrollTop - D.current < 0 ? this._outputAreaAutoScroll = !1 : this._outputAreaAutoScroll || (this._outputAreaAutoScroll = t.scrollHeight - t.scrollTop < t.clientHeight + 1), D.current = t.scrollTop
+                                t.scrollTop - N.current < 0 ? this._outputAreaAutoScroll = !1 : this._outputAreaAutoScroll || (this._outputAreaAutoScroll = t.scrollHeight - t.scrollTop < t.clientHeight + 1), N.current = t.scrollTop
                             }
                         })), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("div", {
                             ref: _,
                             style: {
                                 position: "absolute",
                                 left: "0px",
                                 top: "0px",
@@ -6164,29 +6262,29 @@
                                 position: "absolute",
                                 right: "0px",
                                 top: "0px",
                                 zIndex: 100,
                                 display: "flex",
                                 alignItems: "center"
                             }
-                        }, m && react__WEBPACK_IMPORTED_MODULE_8___default().createElement(_yesIcon__WEBPACK_IMPORTED_MODULE_17__.Z, {
+                        }, g && react__WEBPACK_IMPORTED_MODULE_8___default().createElement(_yesIcon__WEBPACK_IMPORTED_MODULE_17__.Z, {
                             onClick: () => {
                                 h(!1), this._saveCode && this._saveCode()
                             },
                             width: M,
                             height: M
                         }), react__WEBPACK_IMPORTED_MODULE_8___default().createElement(_runIcon__WEBPACK_IMPORTED_MODULE_18__.Z, {
                             onClick: () => {
                                 this._editorRun()
                             },
                             width: M,
                             height: M
                         }), react__WEBPACK_IMPORTED_MODULE_8___default().createElement(_deleteIcon__WEBPACK_IMPORTED_MODULE_15__.Z, {
                             onClick: () => {
-                                h(!1), g(!1), this._saveCode = null, this._curEditingCellIndex = -1
+                                h(!1), m(!1), this._saveCode = null, this._curEditingCellIndex = -1
                             },
                             width: M,
                             height: M
                         })), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("div", {
                             style: {
                                 position: "absolute",
                                 left: "0px",
@@ -6195,15 +6293,15 @@
                             }
                         }, react__WEBPACK_IMPORTED_MODULE_8___default().createElement("label", {
                             ref: this._kernelStateLabelCodeEditorRef,
                             style: {
                                 height: "100%",
                                 color: "white"
                             }
-                        }, "空闲"), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("br", null), !m && react__WEBPACK_IMPORTED_MODULE_8___default().createElement("span", null, react__WEBPACK_IMPORTED_MODULE_8___default().createElement("label", {
+                        }, "空闲"), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("br", null), !g && react__WEBPACK_IMPORTED_MODULE_8___default().createElement("span", null, react__WEBPACK_IMPORTED_MODULE_8___default().createElement("label", {
                             style: {
                                 height: "100%",
                                 color: "white"
                             }
                         }, "当前索引:"), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("input", {
                             ref: O,
                             type: "number",
@@ -6779,111 +6877,213 @@
                                 detail_level: 1
                             }));
                             if (e && "ok" == e.content.status) {
                                 let t = e.content.data["text/plain"];
                                 t = (0, _utils__WEBPACK_IMPORTED_MODULE_22__.cc)(t);
                                 let n = /Init\ssignature:(.*?)(\(.*\))/g.exec(t);
                                 if (n) {
-                                    let e = this._buildInputPortsFromSignature(n[2]);
+                                    let e = this._buildInputPortsFromSignature(n[2], !0);
                                     node_types = this._buildCommonNodeTypes(node_type_name, e, "class"), this._nodeTypes[node_type_name] = {
                                         type: "class",
                                         node_type_name,
                                         in_ports: e
                                     }
                                 }
                             }
                         }
                     }
                     return node_types
                 }
-                _buildInputPortsFromSignature(signature) {
+                _buildInputPortsFromSignature(signature, isClass = !1) {
                     signature = signature.replace(/->.*/g, ""), signature = signature.trim(), signature = signature.slice(1, signature.length - 1);
-                    let segs = signature.split(","),
-                        in_ports = [],
+                    let in_ports = [],
+                        state = "read_name",
+                        arg_name = "",
                         arg_in_type = "keyword",
-                        starIndex = -1,
-                        gangIndex = -1,
-                        index = 0;
-                    for (let e of segs) "*" == e.trim() && (starIndex = index), "/" == e.trim() && (gangIndex = index), index++; - 1 != starIndex && -1 != gangIndex && starIndex < gangIndex && gangIndex == segs.length - 1 && segs.pop(), index = 0;
-                    for (let seg of segs) {
-                        if (index++, seg = seg.trim(), !seg) continue;
-                        let arg_name = "",
-                            arg_type = "any",
-                            arg_default = "None";
-                        if ("/" != seg)
-                            if ("*" != seg) {
-                                if ("self" != seg || 1 != index) {
-                                    for (;;) {
-                                        let ret = /\*{2}\s*([_\w]+)/g.exec(seg);
-                                        if (ret) {
-                                            try {
-                                                arg_name = "**" + ret[1].trim() + "(dict)"
-                                            } catch (e) {}
-                                            arg_type = "dict";
-                                            break
-                                        }
-                                        if (ret = /\*\s*([_\w]+)/g.exec(seg), ret) {
-                                            try {
-                                                arg_name = "*" + ret[1].trim() + "(tuple)"
-                                            } catch (e) {}
-                                            arg_type = "tuple";
-                                            break
-                                        }
-                                        if (ret = /([_\w]+)\s*(:\s*([_\w]+)){0,1}\s*(=(.*)){0,1}/g.exec(seg), ret) {
-                                            try {
-                                                arg_name = ret[1].trim()
-                                            } catch (e) {}
-                                            try {
-                                                arg_type = ret[3].trim()
-                                            } catch (e) {}
-                                            try {
-                                                for (; ret[5];) {
-                                                    let dvalue = ret[5].trim();
-                                                    if ('"' == dvalue.charAt(0) && '"' == dvalue.charAt(dvalue.length - 1) || "'" == dvalue.charAt(0) && "'" == dvalue.charAt(dvalue.length - 1)) {
-                                                        arg_type = "str", arg_default = eval(dvalue);
-                                                        break
-                                                    }
-                                                    if (ret = /<class(.*)>/g.exec(dvalue), ret) {
-                                                        arg_type = "any", arg_default = dvalue;
-                                                        break
-                                                    }
-                                                    if (ret = /<function(.*?)at/g.exec(dvalue), ret) {
-                                                        arg_type = "any", arg_default = dvalue;
-                                                        break
-                                                    }
-                                                    if (ret = /<built-in function (.*)>/g.exec(dvalue), ret) {
-                                                        arg_type = "any", arg_default = dvalue;
-                                                        break
-                                                    }
-                                                    if (ret = /[\d\.]+/g.exec(dvalue), ret) {
-                                                        arg_type = "int", arg_default = Number(dvalue);
-                                                        break
-                                                    }
-                                                    arg_default = dvalue;
-                                                    break
-                                                }
-                                            } catch (e) {}
-                                            break
-                                        }
+                        arg_type = "any",
+                        arg_default = "None",
+                        stateStack = [],
+                        starFlag = !1;
+
+                    function tryPushPortAndResetState() {
+                        if (starFlag || "/" != arg_name) {
+                            if ("*" == arg_name) arg_in_type = "keyword", starFlag = !0;
+                            else if (isClass && 0 == in_ports.length);
+                            else if (arg_name.length > 0) {
+                                let ret = /\*{2}\s*([_\w]+)/g.exec(arg_name);
+                                if (ret) {
+                                    try {
+                                        arg_name = "**" + ret[1].trim() + "(dict)"
+                                    } catch (e) {}
+                                    arg_type = "dict"
+                                } else if (ret = /\*\s*([_\w]+)/g.exec(arg_name), ret) {
+                                    try {
+                                        arg_name = "*" + ret[1].trim() + "(tuple)"
+                                    } catch (e) {}
+                                    arg_type = "tuple"
+                                }
+                                for (; arg_default;) {
+                                    let dvalue = arg_default.trim();
+                                    if ('"' == dvalue.charAt(0) && '"' == dvalue.charAt(dvalue.length - 1) || "'" == dvalue.charAt(0) && "'" == dvalue.charAt(dvalue.length - 1)) {
+                                        arg_type = "str", arg_default = eval(dvalue);
                                         break
                                     }
-                                    arg_name.length > 0 && in_ports.push({
-                                        arg_name,
-                                        arg_type,
-                                        arg_default,
-                                        arg_in_type
-                                    })
+                                    if (ret = /<class(.*)>/g.exec(dvalue), ret) {
+                                        arg_type = "any", arg_default = dvalue;
+                                        break
+                                    }
+                                    if (ret = /<function(.*?)at/g.exec(dvalue), ret) {
+                                        arg_type = "any", arg_default = dvalue;
+                                        break
+                                    }
+                                    if (ret = /<built-in function (.*)>/g.exec(dvalue), ret) {
+                                        arg_type = "any", arg_default = dvalue;
+                                        break
+                                    }
+                                    if (ret = /^[\d\.]+$/g.exec(dvalue), ret) {
+                                        arg_type = "int", arg_default = Number(dvalue);
+                                        break
+                                    }
+                                    if ("True" == dvalue) {
+                                        arg_type = "boolean", arg_default = !0;
+                                        break
+                                    }
+                                    if ("False" == dvalue) {
+                                        arg_type = "boolean", arg_default = !1;
+                                        break
+                                    }
+                                    arg_default = dvalue;
+                                    break
                                 }
-                            } else arg_in_type = "keyword";
-                        else {
+                                in_ports.push({
+                                    arg_name,
+                                    arg_type,
+                                    arg_default,
+                                    arg_in_type
+                                })
+                            }
+                        } else {
                             arg_in_type = "keyword";
                             for (let e of in_ports) e.arg_in_type = "positional"
                         }
+                        arg_name = "", arg_type = "any", arg_default = "None", state = "read_name"
+                    }
+                    for (const e of signature) switch (state) {
+                        case "read_name":
+                            switch (e) {
+                                case " ":
+                                    continue;
+                                case ":":
+                                    state = "read_type", arg_type = "";
+                                    break;
+                                case "=":
+                                    state = "read_default", arg_default = "";
+                                    break;
+                                case "*":
+                                    0 == arg_name.length ? (arg_type = "tuple", arg_default = "()") : "*" == arg_name && (arg_type = "dict", arg_default = "{}"), arg_name += e;
+                                    break;
+                                case ",":
+                                    tryPushPortAndResetState();
+                                    break;
+                                default:
+                                    arg_name += e
+                            }
+                            break;
+                        case "read_type":
+                            switch (e) {
+                                case " ":
+                                    continue;
+                                case "=":
+                                    state = "read_default", arg_default = "";
+                                    break;
+                                case ",":
+                                    switch (arg_type) {
+                                        case "str":
+                                            arg_default = "";
+                                            break;
+                                        case "int":
+                                        case "float":
+                                            arg_default = 0;
+                                            break;
+                                        case "bool":
+                                            arg_default = !1
+                                    }
+                                    tryPushPortAndResetState();
+                                    break;
+                                default:
+                                    arg_type += e
+                            }
+                            break;
+                        case "read_()":
+                            if (")" === e) {
+                                state = stateStack.pop(), arg_default += e;
+                                continue
+                            }
+                        case "read_[]":
+                            if ("]" === e) {
+                                state = stateStack.pop(), arg_default += e;
+                                continue
+                            }
+                        case "read_{}":
+                            if ("}" === e) {
+                                state = stateStack.pop(), arg_default += e;
+                                continue
+                            }
+                        case "read_default":
+                            switch (e) {
+                                case "'":
+                                    stateStack.push(state), state = "read_''", arg_default += e;
+                                    break;
+                                case '"':
+                                    stateStack.push(state), state = 'read_""', arg_default += e;
+                                    break;
+                                case "(":
+                                    stateStack.push(state), state = "read_()", arg_default += e;
+                                    break;
+                                case "[":
+                                    stateStack.push(state), state = "read_[]", arg_default += e;
+                                    break;
+                                case "{":
+                                    stateStack.push(state), state = "read_{}", arg_default += e;
+                                    break;
+                                case ",":
+                                    "read_default" == state ? tryPushPortAndResetState() : arg_default += e;
+                                    break;
+                                default:
+                                    arg_default += e
+                            }
+                            break;
+                        case "read_zhuangyi":
+                            state = stateStack.pop(), arg_default += e;
+                            break;
+                        case "read_''":
+                            switch (e) {
+                                case "'":
+                                    arg_default += e, state = stateStack.pop();
+                                    break;
+                                case "\\":
+                                    stateStack.push(state), state = "read_zhuangyi", arg_default += e;
+                                    break;
+                                default:
+                                    arg_default += e
+                            }
+                            break;
+                        case 'read_""':
+                            switch (e) {
+                                case '"':
+                                    state = stateStack.pop(), arg_default += e;
+                                    break;
+                                case "\\":
+                                    stateStack.push(state), state = "read_zhuangyi", arg_default += e;
+                                    break;
+                                default:
+                                    arg_default += e
+                            }
                     }
-                    return in_ports
+                    return tryPushPortAndResetState(), in_ports
                 }
                 _buildCommonNodeTypes(e, t, n = "function") {
                     let o = [],
                         r = {
                             type: n + "@" + e,
                             label: e,
                             description: e,
@@ -7500,15 +7700,15 @@
                         output_type: "stream",
                         ...e.content
                     };
                     else if (_jupyterlab_services__WEBPACK_IMPORTED_MODULE_4__.KernelMessage.isErrorMsg(e)) {
                         console.error(e.content.ename), console.error(e.content.evalue);
                         let n = "";
                         for (const t of e.content.traceback) n += t + "\n";
-                        console.error(n), this._setRunningNode(this._runningNodeId, !0), this.refreshNodeBoxShadow(), t = {
+                        console.error(n), _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.Notification.error((0, _utils__WEBPACK_IMPORTED_MODULE_22__.cc)(n)), this._setRunningNode(this._runningNodeId, !0), this.refreshNodeBoxShadow(), t = {
                             output_type: "error",
                             ...e.content
                         }
                     } else if (_jupyterlab_services__WEBPACK_IMPORTED_MODULE_4__.KernelMessage.isExecuteResultMsg(e) || _jupyterlab_services__WEBPACK_IMPORTED_MODULE_4__.KernelMessage.isDisplayDataMsg(e)) console.log(e.content.data), t = {
                         output_type: "execute_result",
                         ...e.content
                     };
@@ -7521,15 +7721,14 @@
                                 ...e.content,
                                 output_type: "display_data"
                             },
                             o = this._outputArea._displayIdMap.get(t);
                         if (o)
                             for (const e of o) this._outputArea.model.set(e, n)
                     }
-                    t && this._outputArea && this._outputArea.model.add(t)
                 }
                 _getOutVarName(e) {
                     return `_${e}_out`.replace(/-/g, "_")
                 }
                 _addRedo(e) {
                     this._redoList.splice(this._redoListIndex, this._redoList.length - this._redoListIndex), this._redoList.push(e), this._redoList.length > this._redoListMaxLength && this._redoList.splice(0, this._redoList.length - this._redoListMaxLength), this._redoListIndex = this._redoList.length
                 }
@@ -7599,16 +7798,16 @@
                     const u = e => e * (1 / a),
                         c = e => e * (1 / l),
                         d = r.x + r.width / 2,
                         _ = r.y + r.height / 2,
                         p = u(this._scaleStartPos.clientX - d + i.x),
                         h = u(this._scaleStartPos.clientY - _ + i.y),
                         f = c(this._scaleStartPos.clientX - d + i.x),
-                        m = c(this._scaleStartPos.clientY - _ + i.y);
-                    this._scaleXDistance = (p - f) * l, this._scaleYDistance = (h - m) * l, n.current.style.transform = `scale(${l})`, o.current.style.transform = `translate(${-i.x-this._scaleXDistance}px, ${-i.y-this._scaleYDistance}px)`
+                        g = c(this._scaleStartPos.clientY - _ + i.y);
+                    this._scaleXDistance = (p - f) * l, this._scaleYDistance = (h - g) * l, n.current.style.transform = `scale(${l})`, o.current.style.transform = `translate(${-i.x-this._scaleXDistance}px, ${-i.y-this._scaleYDistance}px)`
                 }
                 _stopScale() {
                     this.editorOptions.draggableRef.current.style.cursor = "";
                     const e = this.editorOptions.stagetScale,
                         t = this.editorOptions.stagetTranslate;
                     (0, this.editorOptions.dispatchStageState)({
                         type: "SET_TRANSLATE_SCALE",
```

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/remoteEntry.80729a1327f495afa265.js` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/remoteEntry.05ee5c7186d725a070e5.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -123,15 +123,15 @@
         8084: "dda9b009ce099df0bb96",
         8180: "a3d01aa0d2f10b552dd3",
         8401: "d14444e38cb7aa24efdd",
         8424: "3938b0f02a27846d3fcd",
         8670: "e60df217bf8cf5c38364",
         8715: "815f4104f6ed5438c593",
         8719: "e05fefc4bcc2bc7ab0d6",
-        8863: "82c89f078a753cb91d3d",
+        8863: "6ed3cbfeea198a6b6e21",
         8906: "b9ef8e8fbada8f634ff8",
         8946: "e37c54e493ef0fcd3129",
         9343: "68df0c5454cb71b71ac8",
         9398: "e709c53f5309c556391b",
         9400: "af8212185e81be7c179c",
         9537: "5b34dc2ee55a5048c2a8",
         9684: "31d4865e5191437dcb69",
@@ -215,15 +215,15 @@
         8084: "dda9b009ce099df0bb96",
         8180: "a3d01aa0d2f10b552dd3",
         8401: "d14444e38cb7aa24efdd",
         8424: "3938b0f02a27846d3fcd",
         8670: "e60df217bf8cf5c38364",
         8715: "815f4104f6ed5438c593",
         8719: "e05fefc4bcc2bc7ab0d6",
-        8863: "82c89f078a753cb91d3d",
+        8863: "6ed3cbfeea198a6b6e21",
         8906: "b9ef8e8fbada8f634ff8",
         8946: "e37c54e493ef0fcd3129",
         9343: "68df0c5454cb71b71ac8",
         9398: "e709c53f5309c556391b",
         9400: "af8212185e81be7c179c",
         9537: "5b34dc2ee55a5048c2a8",
         9684: "31d4865e5191437dcb69",
@@ -285,15 +285,15 @@
                         (!b || !b.loaded && (!f != !b.eager ? f : t > b.from)) && (c[a] = {
                             get: d,
                             from: t,
                             eager: !!f
                         })
                     },
                     o = [];
-                return "default" === d && (b("jupyterlab_nodeeditor", "1.0.6", (() => Promise.all([E.e(2602), E.e(8863)]).then((() => () => E(8863))))), b("monaco-editor", "0.39.0", (() => Promise.all([E.e(3837), E.e(8)]).then((() => () => E(3837))))), b("react-portal", "4.2.2", (() => Promise.all([E.e(2602), E.e(5600)]).then((() => () => E(5600))))), b("uuid", "9.0.0", (() => E.e(9687).then((() => () => E(9687)))))), e[d] = o.length ? Promise.all(o).then((() => e[d] = 1)) : 1
+                return "default" === d && (b("jupyterlab_nodeeditor", "1.0.7", (() => Promise.all([E.e(2602), E.e(8863)]).then((() => () => E(8863))))), b("monaco-editor", "0.39.0", (() => Promise.all([E.e(3837), E.e(8)]).then((() => () => E(3837))))), b("react-portal", "4.2.2", (() => Promise.all([E.e(2602), E.e(5600)]).then((() => () => E(5600))))), b("uuid", "9.0.0", (() => E.e(9687).then((() => () => E(9687)))))), e[d] = o.length ? Promise.all(o).then((() => e[d] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         E.g.importScripts && (e = E.g.location + "");
         var a = E.g.document;
         if (!e && a && (a.currentScript && (e = a.currentScript.src), !e)) {
```

### Comparing `jupyterlab_nodeeditor-1.0.6/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json` & `jupyterlab_nodeeditor-1.0.7/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/schema/plugin.json` & `jupyterlab_nodeeditor-1.0.7/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/ReRunIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/ReRunIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/arrownIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/arrownIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/clearIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/clearIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/deleteIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/deleteIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/exportIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/exportIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/factory.ts` & `jupyterlab_nodeeditor-1.0.7/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/flumeConfig.tsx` & `jupyterlab_nodeeditor-1.0.7/src/flumeConfig.tsx`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-import { FlumeConfig, Colors, Controls, Node } from '../flume'
+import { FlumeConfig, Colors, Controls, SvgContainerStyle } from '../flume'
 import React, { useState, useCallback } from 'react'
 import { NodeEditorWidget } from './widget'
 import { buildNodeWidth } from './utils'
 import * as monaco from 'monaco-editor';
+import { Notification } from '@jupyterlab/apputils'
 
 export let headerFontsize = 16
 export let nodeMinWidth = 200
 export let nodeMaxWidth = 1000
 
 let image_urls_functions: any = {}
 export function setImageUrls(node_id, urls) {
@@ -415,33 +416,195 @@
                         const onLoad = (e) => {
                             try {
                                 executionContext.updateNodeConnections(portProps.nodeId)
                             } catch (error) {
 
                             }
                         }
+
+                        const [showImagePosition, setImagePosition] = useState(false)
+                        const positionRef = React.useRef(null)
+                        const imageRef = React.useRef(null)
+                        const rectSelect = React.useRef(false)
+                        interface positionRecord {
+                            x: number,
+                            y: number
+                        }
+                        const startPos = React.useRef<null | positionRecord>(null)
+                        const selectRect = React.useRef<null | SVGPathElement>(null)
+
+                        const getMousePos = (clientX, clientY) => {
+                            const imgElement = imageRef.current as unknown as HTMLImageElement
+                            const scale = executionContext.editorOptions["stagetScale"]
+                            const rect = imgElement.getBoundingClientRect()
+                            let posX = (clientX - rect.x) / scale
+                            let posY = (clientY - rect.y) / scale
+                            let imgPosX = Math.floor(posX / (rect.width / scale) * imgElement.naturalWidth)
+                            let imgPosY = Math.floor(posY / (rect.height / scale) * imgElement.naturalHeight)
+                            return { posX, posY, imgPosX, imgPosY }
+                        }
+
+
+                        const updatePostionInfo = (e: React.MouseEvent<HTMLImageElement, MouseEvent>) => {
+                            if (!positionRef.current || !imageRef.current) {
+                                return
+                            }
+                            const imgElement = imageRef.current as unknown as HTMLImageElement
+                            const element = positionRef.current as unknown as HTMLSpanElement
+                            let { posX, posY, imgPosX, imgPosY } = getMousePos(e.clientX, e.clientY)
+
+                            element.style.position = 'absolute'
+                            element.style.left = `${posX}px`
+                            element.style.top = `${posY}px`
+
+                            if (rectSelect.current && startPos.current) {
+                                let startPosData = getMousePos(startPos.current.x, startPos.current.y)
+                                element.innerText = `[${startPosData.imgPosX}, ${startPosData.imgPosY}, ${imgPosX}, ${imgPosY}]`
+                            } else {
+                                element.innerText = `[${imgPosX}, ${imgPosY}]`
+                            }
+
+                            if (imgPosX < 0
+                                || imgPosX >= imgElement.naturalWidth
+                                || imgPosY < 0
+                                || imgPosY >= imgElement.naturalHeight) {
+                                setImagePosition(false)
+                            }
+                        }
+
+                        const updateRectSelct = (e: React.MouseEvent<HTMLImageElement, MouseEvent>) => {
+                            if (!selectRect.current) {
+                                const svg = document.createElementNS("http://www.w3.org/2000/svg", "svg");
+                                svg.setAttribute("class", SvgContainerStyle);
+                                svg.setAttribute("style", "z-index:100;");
+                                svg.setAttribute("viewport", `0 0 `)
+                                const path = document.createElementNS("http://www.w3.org/2000/svg", "path");
+                                path.setAttribute("stroke", "rgb(185, 186, 189)");
+                                path.setAttribute("stroke-width", "1");
+                                path.setAttribute("stroke-linecap", "round");
+                                path.setAttribute("fill", "rgba(255,255,255,0.2)");
+                                path.setAttribute("d", "");
+                                svg.appendChild(path)
+                                if (imageRef.current) {
+                                    let container = imageRef.current as unknown as HTMLImageElement
+                                    if (container.parentElement) {
+                                        container.parentElement.appendChild(svg)
+                                    }
+                                }
+                                selectRect.current = path
+                            }
+
+                            if (selectRect.current && startPos.current) {
+                                const imgElement = imageRef.current as unknown as HTMLImageElement
+                                const rect = imgElement.getBoundingClientRect()
+                                const scale = executionContext.editorOptions["stagetScale"]
+                                let startPosRecord = startPos.current as positionRecord
+                                let startPosX = (startPosRecord.x - rect.x) / scale
+                                let startPosY = (startPosRecord.y - rect.y) / scale
+                                let endPosX = (e.clientX - rect.x) / scale
+                                let endPosY = (e.clientY - rect.y) / scale
+                                let width = endPosX - startPosX
+                                let height = endPosY - startPosY
+                                selectRect.current.setAttribute("d", `M ${startPosX} ${startPosY} h ${width} v ${height} h ${-width} Z`)
+                            }
+                        }
+
+                        const handleOnMouseEnter = (e: React.MouseEvent<HTMLImageElement, MouseEvent>) => {
+                            setImagePosition(true)
+                            updatePostionInfo(e)
+                        }
+
+                        const handleOnMouseMove = (e: React.MouseEvent<HTMLImageElement, MouseEvent>) => {
+                            if (!showImagePosition) {
+                                return
+                            }
+
+                            if (rectSelect.current) {
+                                updateRectSelct(e)
+                            }
+
+                            updatePostionInfo(e)
+                        }
+
+                        const handleOnMouseLeave = (e: React.MouseEvent<HTMLImageElement, MouseEvent>) => {
+                            setImagePosition(false)
+                        }
+
+                        const handleOnMouseDownUP = (e: React.MouseEvent<HTMLDivElement, MouseEvent>, down: boolean) => {
+                            switch (e.button) {
+                                case 2:
+                                    rectSelect.current = down
+                                    if (!down) {
+                                        startPos.current = null
+                                        const element = positionRef.current as unknown as HTMLSpanElement
+                                        navigator.clipboard.writeText(element.innerText).then(() => {
+                                            Notification.success(`复制选取到剪切板成功${element.innerText}`)
+                                        }).catch(reason => {
+                                            Notification.error("复制选取到剪切板错误！")
+                                        })
+                                    } else {
+                                        startPos.current = {
+                                            x: e.clientX,
+                                            y: e.clientY
+                                        }
+                                        if (selectRect.current) {
+                                            selectRect.current.setAttribute('d', "")
+                                        }
+                                    }
+                                    break;
+                            }
+                        }
+
                         return (
                             <div>
                                 <button onClick={showImg}>浏览</button>
                                 <button onClick={e => {
                                     let new_index = (data.index - 1 + data.urls.length) % data.urls.length
                                     onChange({ urls: data.urls, index: new_index })
                                 }}>上一个</button>
                                 <button onClick={e => {
                                     let new_index = (data.index + 1) % data.urls.length
                                     onChange({ urls: data.urls, index: new_index })
                                 }}>下一个</button>
                                 <span>当前索引:{data.index}</span>
-                                <img
-                                    onLoad={onLoad}
-                                    onDoubleClick={showImg}
-                                    id={"img_" + portProps.nodeId}
-                                    style={{ width: "100%" }}
-                                    src={get_url()}
-                                />
+                                <div
+                                    style={{
+                                        position: 'relative',
+                                        top: '0px',
+                                        left: '0px'
+                                    }}
+                                    onMouseEnter={handleOnMouseEnter}
+                                    onMouseMove={handleOnMouseMove}
+                                    onMouseLeave={handleOnMouseLeave}
+                                    onMouseDown={e => handleOnMouseDownUP(e, true)}
+                                    onMouseUp={e => handleOnMouseDownUP(e, false)}
+                                >
+                                    <img
+                                        style={{
+                                            width: '100%',
+                                            height: "100%",
+                                            objectFit: 'contain',
+                                        }}
+                                        onLoad={onLoad}
+                                        onDoubleClick={showImg}
+                                        id={"img_" + portProps.nodeId}
+                                        ref={imageRef}
+                                        src={get_url()}
+                                    />
+                                    {
+                                        showImagePosition && <span
+                                            ref={positionRef}
+                                            style={{
+                                                position: 'absolute',
+                                                backgroundColor: 'white',
+                                            }}
+                                        ></span>
+                                    }
+                                </div>
+
                             </div>
                         )
                     }
                 }),
             ]
         })
         .addPortType({
@@ -1121,22 +1284,22 @@
             description: "开始(start)",
             initialWidth: buildNodeWidth("开始(start)", headerFontsize, nodeMinWidth, nodeMaxWidth),
             inputs: ports => [
                 get_port_func("control")(ports),
             ],
             outputs: [],
         })
-        // .addNodeType({
-        //     type: "function",
-        //     label: "函数(function)",
-        //     description: "函数(function)",
-        //     initialWidth: 500,
-        //     inputs: ports => [
-        //         get_port_func("control")(ports),
-        //         ports.code_editor()
-
-        //     ],
-        //     outputs: [],
-        // })
+    // .addNodeType({
+    //     type: "function",
+    //     label: "函数(function)",
+    //     description: "函数(function)",
+    //     initialWidth: 500,
+    //     inputs: ports => [
+    //         get_port_func("control")(ports),
+    //         ports.code_editor()
+
+    //     ],
+    //     outputs: [],
+    // })
 
     return config
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.6/src/imageViewer.tsx` & `jupyterlab_nodeeditor-1.0.7/src/imageViewer.tsx`

 * *Files 3% similar despite different names*

```diff
@@ -215,28 +215,47 @@
     return (
         <div
             ref={divRef}
             style={{
                 backgroundColor: "black",
                 width: "100%",
                 height: "100%",
-                display:"flex",
-                justifyContent:"center",
+                display: "flex",
+                justifyContent: "center",
             }}
             onMouseDown={handleMouseDown}
             onMouseMove={handleMouseMove}
             onMouseUp={handleMouseUp}
         >
-            <img
-                onWheel={handleWheel}
-                src={urls[index]}
-                alt="Image"
+            <div
                 ref={imgRef}
-                onLoad={handleImageLoad}
-            />
+                onWheel={handleWheel}
+            >
+                <img
+                    style={{
+                        width: '100%',
+                        height: "100%",
+                        objectFit: 'contain',
+                    }}
+                    src={urls[index]}
+                    alt="Image"
+                    onLoad={handleImageLoad}
+                />
+                {/* <svg
+                    width='100%' height='100%'
+                    style={{
+                        position: 'absolute',
+                        top: '0px',
+                        left: '0px'
+                    }}
+                >
+                    <rect height="94" width="148" y="235" x="306" stroke="#000" fill="#7DD8B5" />
+                </svg> */}
+            </div>
+
             <div style={{
                 position: "absolute",
                 left: 0,
                 top: "calc(50% - 50px)"
             }} >
                 <ArrownIcon onClick={preImage} width={"100px"} height={"100px"} />
             </div>
```

### Comparing `jupyterlab_nodeeditor-1.0.6/src/index.ts` & `jupyterlab_nodeeditor-1.0.7/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/lockIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/lockIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/newIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/newIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/runIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/runIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/utils.tsx` & `jupyterlab_nodeeditor-1.0.7/src/utils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/src/widget.tsx` & `jupyterlab_nodeeditor-1.0.7/src/widget.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import {
     Dialog,
     showDialog,
     SessionContextDialogs,
     ReactWidget,
     ICommandPalette,
     showErrorMessage,
+    Notification,
 } from "@jupyterlab/apputils";
 import {
     JupyterFrontEnd,
 } from "@jupyterlab/application"
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { ITranslator, nullTranslator } from '@jupyterlab/translation';
 import { KernelError } from "@jupyterlab/notebook";
@@ -1860,15 +1861,15 @@
                     detail_level: 1
                 })
                 if (ret && ret.content.status == "ok") {
                     let content = ret.content.data['text/plain'] as string
                     content = removeAnsi(content)
                     let execRet = /Init\ssignature:(.*?)(\(.*\))/g.exec(content)
                     if (execRet) {
-                        let in_ports: any[] = this._buildInputPortsFromSignature(execRet[2])
+                        let in_ports: any[] = this._buildInputPortsFromSignature(execRet[2], true)
                         // 2.构建nodeType
                         node_types = this._buildCommonNodeTypes(node_type_name, in_ports, "class")
                         // 3.记录下来
                         this._nodeTypes[node_type_name] = {
                             type: "class",
                             node_type_name,
                             in_ports,
@@ -1877,160 +1878,301 @@
                 }
             } break;
             case "keywork": { } break;
         }
         return node_types
     }
 
-    private _buildInputPortsFromSignature(signature: String) {
+    private _buildInputPortsFromSignature(signature: String, isClass = false) {
         signature = signature.replace(/->.*/g, "")
         signature = signature.trim()
         signature = signature.slice(1, signature.length - 1)
-        // 2.用 ", "分割
-        let segs = signature.split(",")
-        // 3.解析参数和默认值
         let in_ports: any[] = []
-        let arg_in_type = "keyword"
-
-        // 4.检查签名是否同时出现了* 和 /（有时候获取的签名有错误，比如numpy.array的签名）
-        let starIndex = -1
-        let gangIndex = -1
-        let index = 0
-        for (let seg of segs) {
-            if (seg.trim() == "*") {
-                starIndex = index
-            }
-            if (seg.trim() == "/") {
-                gangIndex = index
-            }
-            index++
-        }
-
-        if (starIndex != -1 && gangIndex != -1 && starIndex < gangIndex) {
-            // 如果/在最后面，以前面的*为主
-            if (gangIndex == segs.length - 1) {
-                segs.pop()
-            } else {
-
-            }
-            // 需要重新获取签名
-        }
-
-        index = 0
-        for (let seg of segs) {
-            index++
-            seg = seg.trim()
-            if (!seg) {
-                continue
-            }
-
-            let arg_name: string = ""
-            let arg_type: string = "any"
-            let arg_default: any = "None"
-            if (seg == "/") {
+        // 2.用 ", "分割
+        let state: 'read_name'
+            | 'read_type'
+            | 'read_default'
+            | 'read_zhuangyi'
+            | 'read_()'
+            | 'read_""'
+            | "read_''"
+            | 'read_{}'
+            | 'read_[]'
+            = 'read_name'
+        let arg_name = ''
+        let arg_in_type = 'keyword'
+        let arg_type = 'any'
+        let arg_default: any = 'None'
+        let stateStack: any[] = []
+        let starFlag = false
+        function tryPushPortAndResetState() {
+            if (!starFlag && arg_name == "/") {
                 arg_in_type = "keyword"
                 for (let port of in_ports) {
                     port.arg_in_type = "positional"
                 }
-                continue
-            }
-
-            if (seg == "*") {
+            } else if (arg_name == "*") {
                 arg_in_type = "keyword"
-                continue
-            }
-
-            if (seg == "self" && index == 1) {
-                continue
-            }
-
-            while (true) {
+                starFlag = true
+            } else if (isClass && in_ports.length == 0) {
+            } else if (arg_name.length > 0) {
                 // 判断是否是dict
-                let ret = /\*{2}\s*([_\w]+)/g.exec(seg)
+                let ret = /\*{2}\s*([_\w]+)/g.exec(arg_name)
                 if (ret) {
                     try { arg_name = "**" + ret[1].trim() + "(dict)" } catch (error) { }
                     arg_type = "dict"
-                    break
-                }
-                // 判断是否是tuple
-                ret = /\*\s*([_\w]+)/g.exec(seg)
-                if (ret) {
-                    try { arg_name = "*" + ret[1].trim() + "(tuple)" } catch (error) { }
-                    arg_type = "tuple"
-                    break
+                } else {
+                    // 判断是否是tuple
+                    ret = /\*\s*([_\w]+)/g.exec(arg_name)
+                    if (ret) {
+                        try { arg_name = "*" + ret[1].trim() + "(tuple)" } catch (error) { }
+                        arg_type = "tuple"
+                    }
                 }
 
-                // 正常的类型参数
-                ret = /([_\w]+)\s*(:\s*([_\w]+)){0,1}\s*(=(.*)){0,1}/g.exec(seg)
-                if (ret) {
-                    try { arg_name = ret[1].trim() } catch (error) { }
-                    try { arg_type = ret[3].trim() } catch (error) { }
-                    try {
-                        while (ret[5]) {
-                            let dvalue = ret[5].trim()
-                            // 判断是什么类型
-                            // 字符串
-                            if ((dvalue.charAt(0) == "\"" && dvalue.charAt(dvalue.length - 1) == "\"")
-                                || (dvalue.charAt(0) == "\'" && dvalue.charAt(dvalue.length - 1) == "\'")) {
-                                arg_type = "str"
-                                arg_default = eval(dvalue)
-                                break
-                            }
-                            // class类型 "<class 'matplotlib.figure.Figure'>"
-                            ret = /<class(.*)>/g.exec(dvalue)
-                            if (ret) {
-                                arg_type = "any"
-                                arg_default = dvalue
-                                break
-                            }
+                while (arg_default) {
+                    let dvalue = arg_default.trim()
+                    // 判断是什么类型
+                    // 字符串
+                    if ((dvalue.charAt(0) == "\"" && dvalue.charAt(dvalue.length - 1) == "\"")
+                        || (dvalue.charAt(0) == "\'" && dvalue.charAt(dvalue.length - 1) == "\'")) {
+                        arg_type = "str"
+                        arg_default = eval(dvalue)
+                        break
+                    }
+                    // class类型 "<class 'matplotlib.figure.Figure'>"
+                    ret = /<class(.*)>/g.exec(dvalue)
+                    if (ret) {
+                        arg_type = "any"
+                        arg_default = dvalue
+                        break
+                    }
 
-                            // 普通函数类型
-                            ret = /<function(.*?)at/g.exec(dvalue)
-                            if (ret) {
-                                arg_type = "any"
-                                arg_default = dvalue
-                                break
-                            }
+                    // 普通函数类型
+                    ret = /<function(.*?)at/g.exec(dvalue)
+                    if (ret) {
+                        arg_type = "any"
+                        arg_default = dvalue
+                        break
+                    }
 
-                            // build-in函数： <built-in function imread>
-                            // 目前不知道如何处理
-                            ret = /<built-in function (.*)>/g.exec(dvalue)
-                            if (ret) {
-                                arg_type = "any"
-                                arg_default = dvalue
-                                break
-                            }
+                    // build-in函数： <built-in function imread>
+                    // 目前不知道如何处理
+                    ret = /<built-in function (.*)>/g.exec(dvalue)
+                    if (ret) {
+                        arg_type = "any"
+                        arg_default = dvalue
+                        break
+                    }
 
-                            // 数字类型
-                            ret = /[\d\.]+/g.exec(dvalue)
-                            if (ret) {
-                                arg_type = "int"
-                                arg_default = Number(dvalue)
-                                break
-                            }
+                    // 数字类型
+                    ret = /^[\d\.]+$/g.exec(dvalue)
+                    if (ret) {
+                        arg_type = "int"
+                        arg_default = Number(dvalue)
+                        break
+                    }
 
-                            arg_default = dvalue
-                            break
-                        }
+                    // 布尔类型
+                    if (dvalue == 'True') {
+                        arg_type = "boolean"
+                        arg_default = true
+                        break
+                    }
+
+                    // 布尔类型
+                    if (dvalue == 'False') {
+                        arg_type = "boolean"
+                        arg_default = false
+                        break
+                    }
 
-                    } catch (error) { }
+                    arg_default = dvalue
                     break
                 }
-                break
-            }
-            if (arg_name.length > 0) {
+
                 in_ports.push({
                     arg_name,
                     arg_type,
                     arg_default,
                     arg_in_type
                 })
             }
+            arg_name = ''
+            arg_type = 'any'
+            arg_default = 'None'
+            state = 'read_name'
+        }
+
+        for (const c of signature) {
+            switch (state) {
+                case "read_name": {
+                    switch (c) {
+                        case ' ': continue
+                        case ':': {
+                            state = 'read_type'
+                            arg_type = ''
+                        } break
+                        case '=': {
+                            state = 'read_default'
+                            arg_default = ''
+                        } break
+                        case '*': {
+                            if (arg_name.length == 0) {
+                                arg_type = 'tuple'
+                                arg_default = '()'
+                            } else if (arg_name == '*') {
+                                arg_type = 'dict'
+                                arg_default = '{}'
+                            }
+                            arg_name += c
+                        } break
+                        case ',': {
+                            tryPushPortAndResetState()
+                        } break
+                        default: {
+                            arg_name += c
+                        } break
+                    }
+                } break
+                case 'read_type': {
+                    switch (c) {
+                        case ' ': continue
+                        case '=': {
+                            state = 'read_default'
+                            arg_default = ''
+                        } break
+                        case ',': {
+                            switch (arg_type) {
+                                case 'str':
+                                    arg_default = ''
+                                    break;
+                                case 'int':
+                                    arg_default = 0
+                                    break;
+                                case 'float':
+                                    arg_default = 0
+                                    break;
+                                case 'bool':
+                                    arg_default = false
+                                    break;
+                                default:
+                                    break;
+                            }
+                            tryPushPortAndResetState()
+                        } break
+                        default: {
+                            arg_type += c
+                        } break
+                    }
+                } break
+                case 'read_()': {
+                    switch (c) {
+                        case ')': {
+                            state = stateStack.pop()
+                            arg_default += c
+                        } continue
+                    }
+                }
+                case 'read_[]': {
+                    switch (c) {
+                        case ']': {
+                            state = stateStack.pop()
+                            arg_default += c
+                        } continue
+                    }
+                }
+                case 'read_{}': {
+                    switch (c) {
+                        case '}': {
+                            state = stateStack.pop()
+                            arg_default += c
+                        } continue
+                    }
+                }
+                case 'read_default': {
+                    switch (c) {
+                        case "'": {
+                            stateStack.push(state)
+                            state = "read_''"
+                            arg_default += c
+                        } break
+                        case '"': {
+                            stateStack.push(state)
+                            state = 'read_""'
+                            arg_default += c
+                        } break
+                        case '(': {
+                            stateStack.push(state)
+                            state = 'read_()'
+                            arg_default += c
+                        } break
+                        case '[': {
+                            stateStack.push(state)
+                            state = 'read_[]'
+                            arg_default += c
+                        } break
+                        case '{': {
+                            stateStack.push(state)
+                            state = 'read_{}'
+                            arg_default += c
+                        } break
+                        case ',': {
+                            if (state == 'read_default') {
+                                tryPushPortAndResetState()
+                            } else {
+                                arg_default += c
+                            }
+                        } break
+                        default:
+                            arg_default += c
+                            break;
+                    }
+                } break
+                case 'read_zhuangyi': {
+                    state = stateStack.pop()
+                    arg_default += c
+                } break
+                case "read_''": {
+                    switch (c) {
+                        case "'": {
+                            arg_default += c
+                            state = stateStack.pop()
+                        } break
+                        case '\\': {
+                            stateStack.push(state)
+                            state = 'read_zhuangyi'
+                            arg_default += c
+                        } break
+                        default:
+                            arg_default += c
+                            break;
+                    }
+                } break
+                case 'read_""': {
+                    switch (c) {
+                        case '"': {
+                            state = stateStack.pop()
+                            arg_default += c
+                        } break
+                        case '\\': {
+                            stateStack.push(state)
+                            state = 'read_zhuangyi'
+                            arg_default += c
+                        } break
+                        default:
+                            arg_default += c
+                            break;
+                    }
+                } break
+            }
         }
 
+        tryPushPortAndResetState()
+
         return in_ports
     }
 
     private _buildCommonNodeTypes(node_type_name, in_ports, prefix = "function") {
         let type_name = prefix + "@" + node_type_name
         let node_types: any[] = []
         let nodetype = {
@@ -3108,14 +3250,15 @@
             console.error(msg.content.ename)
             console.error(msg.content.evalue)
             let errMsg = ""
             for (const traceback of msg.content.traceback) {
                 errMsg += traceback + "\n"
             }
             console.error(errMsg)
+            Notification.error(removeAnsi(errMsg))
             this._setRunningNode(this._runningNodeId, true)
             this.refreshNodeBoxShadow()
             outputMsg = {
                 output_type: "error",
                 ...msg.content
             }
         }
@@ -3139,19 +3282,19 @@
             if (targets) {
                 for (const index of targets) {
                     this._outputArea.model.set(index, output);
                 }
             }
         }
 
-        if (outputMsg) {
-            if (this._outputArea) {
-                this._outputArea.model.add(outputMsg)
-            }
-        }
+        // if (outputMsg) {
+        //     if (this._outputArea) {
+        //         this._outputArea.model.add(outputMsg)
+        //     }
+        // }
     }
 
     private _getOutVarName(nodeId) {
         let out_var_name = `_${nodeId}_out`
         return out_var_name.replace(/-/g, "_")
     }
```

### Comparing `jupyterlab_nodeeditor-1.0.6/src/yesIcon.tsx` & `jupyterlab_nodeeditor-1.0.7/src/yesIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/test_ext/1.jpeg` & `jupyterlab_nodeeditor-1.0.7/test_ext/1.jpeg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/test_ext/2.jpeg` & `jupyterlab_nodeeditor-1.0.7/test_ext/2.jpeg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/test_ext/main.ipynb` & `jupyterlab_nodeeditor-1.0.7/test_ext/main.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/test_ext/testlib.ipynb` & `jupyterlab_nodeeditor-1.0.7/test_ext/testlib.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/.gitignore` & `jupyterlab_nodeeditor-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/LICENSE` & `jupyterlab_nodeeditor-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/README.md` & `jupyterlab_nodeeditor-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/pyproject.toml` & `jupyterlab_nodeeditor-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.6/PKG-INFO` & `jupyterlab_nodeeditor-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nodeeditor
-Version: 1.0.6
+Version: 1.0.7
 Summary: 一个节点编辑器
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_nodeeditor
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_nodeeditor/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_nodeeditor.git
 Author-email: l0n0l <cenlan@hotmail.com>
 License: BSD 3-Clause License
```

