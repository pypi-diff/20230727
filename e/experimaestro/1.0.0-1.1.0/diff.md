# Comparing `tmp/experimaestro-1.0.0.zip` & `tmp/experimaestro-1.1.0.zip`

## zipinfo {}

```diff
@@ -1,249 +1,250 @@
-Zip file size: 5169797 bytes, number of entries: 247
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/app/
--rw-r--r--  2.0 unx      646 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/requirements.txt
--rw-r--r--  2.0 unx     2130 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/setup.cfg
--rw-r--r--  2.0 unx      236 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/pytest.ini
--rw-r--r--  2.0 unx      991 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/mkdocs.yml
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/.gitmodules
--rw-r--r--  2.0 unx     7470 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/PKG-INFO
--rw-r--r--  2.0 unx     3585 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/CHANGELOG.md
--rw-r--r--  2.0 unx      182 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/.gitignore
--rw-r--r--  2.0 unx      232 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/MANIFEST.in
--rw-r--r--  2.0 unx      511 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/.flake8
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/LICENSE
--rw-r--r--  2.0 unx       33 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/.prettierignore
--rw-r--r--  2.0 unx     3045 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/README.md
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/setup.py
--rw-r--r--  2.0 unx      348 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/pyproject.toml
--rw-r--r--  2.0 unx      287 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/tox.ini
--rw-r--r--  2.0 unx      355 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/.readthedocs.yml
--rw-r--r--  2.0 unx      567 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/.pre-commit-config.yaml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/docs/launchers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/docs/experiments/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/docs/connectors/
--rw-r--r--  2.0 unx       33 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/requirements.txt
--rw-r--r--  2.0 unx      701 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/faq.md
--rw-r--r--  2.0 unx      269 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/configuration.md
--rw-r--r--  2.0 unx     1938 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/index.md
--rw-r--r--  2.0 unx     2036 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/documenting.md
--rw-r--r--  2.0 unx      827 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/cli.md
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/changelog.md
--rw-r--r--  2.0 unx     1024 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/serialization.md
--rw-r--r--  2.0 unx       18 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/tutorial.md
--rw-r--r--  2.0 unx      744 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/concepts.md
--rw-r--r--  2.0 unx      675 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/jupyter.md
--rw-r--r--  2.0 unx     5712 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/launchers/index.md
--rw-r--r--  2.0 unx     3879 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/experiments/task.md
--rw-r--r--  2.0 unx     7818 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/experiments/config.md
--rw-r--r--  2.0 unx     6433 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/experiments/overview.md
--rw-r--r--  2.0 unx     4317 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/experiments/plan.md
--rw-r--r--  2.0 unx       60 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/docs/connectors/index.md
--rw-r--r--  2.0 unx      597 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/scripts/longtask.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/launcherfinder/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/mkdocs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tools/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/sphinx/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/launchers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/core/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/connectors/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/scheduler/
--rw-r--r--  2.0 unx     4455 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/run.py
--rw-r--r--  2.0 unx      285 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/mypy.py
--rw-r--r--  2.0 unx     5775 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/filter.py
--rw-r--r--  2.0 unx      160 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/version.py
--rw-r--r--  2.0 unx     3605 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/rpyc.py
--rw-r--r--  2.0 unx     1785 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/typingutils.py
--rw-r--r--  2.0 unx     1230 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/generators.py
--rw-r--r--  2.0 unx     8343 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/annotations.py
--rw-r--r--  2.0 unx     1490 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/ipc.py
--rw-r--r--  2.0 unx      638 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/xpmutils.py
--rw-r--r--  2.0 unx      696 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/checkers.py
--rw-r--r--  2.0 unx    14681 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tokens.py
--rw-r--r--  2.0 unx     1011 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/settings.py
--rw-r--r--  2.0 unx      171 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/compat.py
--rw-r--r--  2.0 unx     8710 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/notifications.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/huggingface.py
--rw-r--r--  2.0 unx     1477 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/locking.py
--rw-r--r--  2.0 unx     1465 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/__init__.py
--rw-r--r--  2.0 unx     2390 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/click.py
--rw-r--r--  2.0 unx    13915 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/__main__.py
--rw-r--r--  2.0 unx     4235 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/scriptbuilder.py
--rw-r--r--  2.0 unx     9463 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/commandline.py
--rw-r--r--  2.0 unx      499 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/taskglobals.py
--rw-r--r--  2.0 unx     6140 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launcherfinder/specs.py
--rw-r--r--  2.0 unx     1020 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launcherfinder/base.py
--rw-r--r--  2.0 unx     7878 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launcherfinder/registry.py
--rw-r--r--  2.0 unx      148 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launcherfinder/__init__.py
--rw-r--r--  2.0 unx     2129 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launcherfinder/parser.py
--rw-r--r--  2.0 unx       66 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/mkdocs/style.css
--rw-r--r--  2.0 unx      263 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/mkdocs/annotations.py
--rw-r--r--  2.0 unx    16716 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/mkdocs/base.py
--rw-r--r--  2.0 unx       34 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/mkdocs/__init__.py
--rw-r--r--  2.0 unx     1481 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/mkdocs/metaloader.py
--rw-r--r--  2.0 unx     3516 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tools/jobs.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tools/__init__.py
--rw-r--r--  2.0 unx     3309 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tools/diff.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/sphinx/static/
--rw-r--r--  2.0 unx     9560 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/sphinx/__init__.py
--rw-r--r--  2.0 unx      294 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/sphinx/static/experimaestro.css
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/
--rw-r--r--  2.0 unx    10854 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/server/__init__.py
--rw-r--r--  2.0 unx      706 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/index.html
--rw-r--r--  2.0 unx   156236 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
--rw-r--r--  2.0 unx   397728 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/b48ad290d0335879a92b.ttf
--rw-r--r--  2.0 unx  3822921 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/index.js.map
--rw-r--r--  2.0 unx   206260 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/5d681e2edae8c60630db.woff
--rw-r--r--  2.0 unx   528999 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/index.css.map
--rw-r--r--  2.0 unx   376002 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/index.css
--rw-r--r--  2.0 unx   182028 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/f882956fd323fd322f31.woff
--rw-r--r--  2.0 unx  3649207 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/index.js
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/manifest.json
--rw-r--r--  2.0 unx   107460 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/e1a247a5ef41e1975742.woff2
--rw-r--r--  2.0 unx      511 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/login.html
--rw-r--r--  2.0 unx   155276 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
--rw-r--r--  2.0 unx   215704 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
--rw-r--r--  2.0 unx   150472 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/66104b766c3d0462b3c5.woff2
--rw-r--r--  2.0 unx   164912 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
--rw-r--r--  2.0 unx     3870 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/favicon.ico
--rw-r--r--  2.0 unx   135984 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
--rw-r--r--  2.0 unx   339600 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
--rw-r--r--  2.0 unx   186112 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/f9ee61fab3c11e2f3ed3.ttf
--rw-r--r--  2.0 unx   173620 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
--rw-r--r--  2.0 unx    62048 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/abf801b7acb6705a15ad.ttf
--rw-r--r--  2.0 unx   128352 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
--rw-r--r--  2.0 unx    25096 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/server/data/639d2000c1ece92eaec8.woff2
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/launchers/slurm/
--rw-r--r--  2.0 unx     1967 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launchers/direct.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launchers/oar.py
--rw-r--r--  2.0 unx     2525 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launchers/__init__.py
--rw-r--r--  2.0 unx    12747 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launchers/slurm/base.py
--rw-r--r--  2.0 unx    19130 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launchers/slurm/configuration.py
--rw-r--r--  2.0 unx       41 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launchers/slurm/__init__.py
--rw-r--r--  2.0 unx      818 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/launchers/slurm/cli.py
--rw-r--r--  2.0 unx     5620 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/arguments.py
--rw-r--r--  2.0 unx    18984 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/types.py
--rw-r--r--  2.0 unx    58915 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/objects.py
--rw-r--r--  2.0 unx     7355 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/objects.pyi
--rw-r--r--  2.0 unx     2479 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/context.py
--rw-r--r--  2.0 unx      493 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/__init__.py
--rw-r--r--  2.0 unx     1197 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/core/serializers.py
--rw-r--r--  2.0 unx     1006 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/utils/resources.py
--rw-r--r--  2.0 unx     6766 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/utils/yaml.py
--rw-r--r--  2.0 unx      793 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/utils/settings.py
--rw-r--r--  2.0 unx     2394 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/utils/jobs.py
--rw-r--r--  2.0 unx      601 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/utils/asyncio.py
--rw-r--r--  2.0 unx     2434 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/utils/__init__.py
--rw-r--r--  2.0 unx     2183 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/utils/jupyter.py
--rw-r--r--  2.0 unx     8206 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/connectors/ssh.py
--rw-r--r--  2.0 unx     5461 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/connectors/__init__.py
--rw-r--r--  2.0 unx     5760 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/connectors/local.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/launchers/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/tasks/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/connectors/
--rw-r--r--  2.0 unx     3081 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_snippets.py
--rw-r--r--  2.0 unx     1837 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_objects.py
--rw-r--r--  2.0 unx      477 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/task_tokens.py
--rw-r--r--  2.0 unx     4016 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/restart.py
--rw-r--r--  2.0 unx      695 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/conftest.py
--rw-r--r--  2.0 unx      781 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_outputs.py
--rw-r--r--  2.0 unx     9099 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_tasks.py
--rw-r--r--  2.0 unx      979 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_ssh.py
--rw-r--r--  2.0 unx     4339 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_validation.py
--rw-r--r--  2.0 unx     1502 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_serializers.py
--rw-r--r--  2.0 unx    12285 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_identifier.py
--rw-r--r--  2.0 unx     2964 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_findlauncher.py
--rw-r--r--  2.0 unx     1701 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/token_reschedule.py
--rw-r--r--  2.0 unx      780 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_forward.py
--rw-r--r--  2.0 unx     6405 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_param.py
--rw-r--r--  2.0 unx     1975 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_tags.py
--rw-r--r--  2.0 unx     2005 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_dependencies.py
--rw-r--r--  2.0 unx      295 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/restart_main.py
--rw-r--r--  2.0 unx     3805 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/utils.py
--rw-r--r--  2.0 unx     7826 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_tokens.py
--rw-r--r--  2.0 unx     1540 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_instance.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/__init__.py
--rw-r--r--  2.0 unx     7580 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_progress.py
--rw-r--r--  2.0 unx      414 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/definitions_types.py
--rw-r--r--  2.0 unx      403 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_checkers.py
--rw-r--r--  2.0 unx     1257 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/test_types.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/launchers/config_slurm/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/
--rw-r--r--  2.0 unx      717 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/test_local.py
--rw-r--r--  2.0 unx     2534 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/test_slurm.py
--rw-r--r--  2.0 unx     2468 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/common.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/__init__.py
--rw-r--r--  2.0 unx     2497 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/config_slurm/__init__.py
--rwxr-xr-x  2.0 unx      639 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/sacct
--rwxr-xr-x  2.0 unx     1177 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/sbatch
--rw-r--r--  2.0 unx      477 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/test.py
--rw-r--r--  2.0 unx     1851 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/tasks/all.py
--rw-r--r--  2.0 unx      153 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/tasks/foreign.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/tasks/__init__.py
--rw-r--r--  2.0 unx      407 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/scripts/notifyandwait.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/scripts/waitforfile.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro/tests/connectors/bin/
--rw-r--r--  2.0 unx     1204 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/connectors/test_local.py
--rw-r--r--  2.0 unx      702 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/connectors/utils.py
--rw-r--r--  2.0 unx       21 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/tests/connectors/bin/executable.py
--rw-r--r--  2.0 unx     1994 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/scheduler/dependencies.py
--rw-r--r--  2.0 unx     1820 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/scheduler/services.py
--rw-r--r--  2.0 unx     1731 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/scheduler/workspace.py
--rw-r--r--  2.0 unx     2393 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/scheduler/environment.py
--rw-r--r--  2.0 unx    29179 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/scheduler/base.py
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/src/experimaestro/scheduler/__init__.py
--rw-r--r--  2.0 unx     7470 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/not-zip-safe
--rw-r--r--  2.0 unx       14 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/top_level.txt
--rw-r--r--  2.0 unx     7039 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx      414 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      591 b- defN 23-Jul-23 15:59 experimaestro-1.0.0/src/experimaestro.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/app/xp/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/app/public/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/app/src/
--rw-r--r--  2.0 unx      536 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/tsconfig.json
--rw-r--r--  2.0 unx     1955 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/CHANGELOG.md
--rw-r--r--  2.0 unx      324 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/.gitignore
--rw-r--r--  2.0 unx     2319 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/package.json
--rw-r--r--  2.0 unx   127144 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/README.md
--rw-r--r--  2.0 unx   785936 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/package-lock.json
--rw-r--r--  2.0 unx      314 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/.nolluprc.js
--rw-r--r--  2.0 unx     9556 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/webpack.config.ts
--rw-r--r--  2.0 unx      930 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/postcss.config.js
--rw-r--r--  2.0 unx     5061 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/xp/run.py
--rw-r--r--  2.0 unx      706 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/public/index.html
--rw-r--r--  2.0 unx      318 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/public/manifest.json
--rw-r--r--  2.0 unx      511 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/public/login.html
--rw-r--r--  2.0 unx     3870 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/public/favicon.ico
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/app/src/theme/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-23 15:59 experimaestro-1.0.0/app/src/ui/
--rw-r--r--  2.0 unx   130132 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/logo.png
--rw-r--r--  2.0 unx      682 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/index.tsx
--rw-r--r--  2.0 unx     1461 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/client.ts
--rw-r--r--  2.0 unx     1155 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/Services.tsx
--rw-r--r--  2.0 unx     3656 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/Tasks.tsx
--rw-r--r--  2.0 unx      102 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/index.css
--rw-r--r--  2.0 unx      621 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/clipboard.ts
--rw-r--r--  2.0 unx     1614 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/TaskJobs.tsx
--rw-r--r--  2.0 unx       13 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/Experiments.tsx
--rw-r--r--  2.0 unx   495919 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/logo.pxm
--rw-r--r--  2.0 unx     3255 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/reducers.ts
--rw-r--r--  2.0 unx      918 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/store.ts
--rw-r--r--  2.0 unx     2845 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/TaskDetail.tsx
--rw-r--r--  2.0 unx     1368 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/App.tsx
--rw-r--r--  2.0 unx     1583 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/theme/theme.scss
--rw-r--r--  2.0 unx     3400 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/theme/_jobs.scss
--rw-r--r--  2.0 unx     3629 b- defN 23-Jul-23 15:58 experimaestro-1.0.0/app/src/ui/messages.tsx
-247 files, 13320556 bytes uncompressed, 5125839 bytes compressed:  61.5%
+Zip file size: 5170939 bytes, number of entries: 248
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/app/
+-rw-r--r--  2.0 unx      646 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/requirements.txt
+-rw-r--r--  2.0 unx     2130 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/setup.cfg
+-rw-r--r--  2.0 unx      236 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/pytest.ini
+-rw-r--r--  2.0 unx      991 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/mkdocs.yml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/.gitmodules
+-rw-r--r--  2.0 unx     7604 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/PKG-INFO
+-rw-r--r--  2.0 unx     3719 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/CHANGELOG.md
+-rw-r--r--  2.0 unx      182 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/.gitignore
+-rw-r--r--  2.0 unx      232 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/MANIFEST.in
+-rw-r--r--  2.0 unx      511 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/.flake8
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/LICENSE
+-rw-r--r--  2.0 unx       33 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/.prettierignore
+-rw-r--r--  2.0 unx     3045 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/README.md
+-rw-r--r--  2.0 unx       38 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/setup.py
+-rw-r--r--  2.0 unx      348 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/pyproject.toml
+-rw-r--r--  2.0 unx      287 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/tox.ini
+-rw-r--r--  2.0 unx      355 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/.readthedocs.yml
+-rw-r--r--  2.0 unx      567 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/.pre-commit-config.yaml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/docs/launchers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/docs/experiments/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/docs/connectors/
+-rw-r--r--  2.0 unx       33 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/requirements.txt
+-rw-r--r--  2.0 unx      701 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/faq.md
+-rw-r--r--  2.0 unx      269 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/configuration.md
+-rw-r--r--  2.0 unx     1938 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/index.md
+-rw-r--r--  2.0 unx     2036 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/documenting.md
+-rw-r--r--  2.0 unx      827 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/cli.md
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/changelog.md
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/serialization.md
+-rw-r--r--  2.0 unx       18 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/tutorial.md
+-rw-r--r--  2.0 unx      744 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/concepts.md
+-rw-r--r--  2.0 unx      675 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/jupyter.md
+-rw-r--r--  2.0 unx     5712 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/launchers/index.md
+-rw-r--r--  2.0 unx     3879 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/experiments/task.md
+-rw-r--r--  2.0 unx     7818 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/experiments/config.md
+-rw-r--r--  2.0 unx     6433 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/experiments/overview.md
+-rw-r--r--  2.0 unx     4317 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/experiments/plan.md
+-rw-r--r--  2.0 unx       60 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/docs/connectors/index.md
+-rw-r--r--  2.0 unx      597 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/scripts/longtask.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/launcherfinder/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/mkdocs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tools/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/sphinx/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/launchers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/core/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/connectors/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/scheduler/
+-rw-r--r--  2.0 unx     4455 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/run.py
+-rw-r--r--  2.0 unx      285 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/mypy.py
+-rw-r--r--  2.0 unx     5794 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/filter.py
+-rw-r--r--  2.0 unx      160 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/version.py
+-rw-r--r--  2.0 unx     3605 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/rpyc.py
+-rw-r--r--  2.0 unx     1785 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/typingutils.py
+-rw-r--r--  2.0 unx     1230 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/generators.py
+-rw-r--r--  2.0 unx     8343 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/annotations.py
+-rw-r--r--  2.0 unx     1490 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/ipc.py
+-rw-r--r--  2.0 unx      638 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/xpmutils.py
+-rw-r--r--  2.0 unx      696 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/checkers.py
+-rw-r--r--  2.0 unx    14681 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tokens.py
+-rw-r--r--  2.0 unx     1011 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/settings.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/compat.py
+-rw-r--r--  2.0 unx     8710 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/notifications.py
+-rw-r--r--  2.0 unx     2956 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/huggingface.py
+-rw-r--r--  2.0 unx     1477 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/locking.py
+-rw-r--r--  2.0 unx     1465 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/__init__.py
+-rw-r--r--  2.0 unx     2390 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/click.py
+-rw-r--r--  2.0 unx    13373 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/__main__.py
+-rw-r--r--  2.0 unx     4235 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/scriptbuilder.py
+-rw-r--r--  2.0 unx     9463 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/commandline.py
+-rw-r--r--  2.0 unx      499 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/taskglobals.py
+-rw-r--r--  2.0 unx     6140 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launcherfinder/specs.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launcherfinder/base.py
+-rw-r--r--  2.0 unx     7878 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launcherfinder/registry.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launcherfinder/__init__.py
+-rw-r--r--  2.0 unx     2129 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launcherfinder/parser.py
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/mkdocs/style.css
+-rw-r--r--  2.0 unx      263 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/mkdocs/annotations.py
+-rw-r--r--  2.0 unx    16716 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/mkdocs/base.py
+-rw-r--r--  2.0 unx       34 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/mkdocs/__init__.py
+-rw-r--r--  2.0 unx     1481 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/mkdocs/metaloader.py
+-rw-r--r--  2.0 unx     3516 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tools/jobs.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tools/__init__.py
+-rw-r--r--  2.0 unx     2166 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tools/documentation.py
+-rw-r--r--  2.0 unx     3309 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tools/diff.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/sphinx/static/
+-rw-r--r--  2.0 unx     9560 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/sphinx/__init__.py
+-rw-r--r--  2.0 unx      294 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/sphinx/static/experimaestro.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/
+-rw-r--r--  2.0 unx    10854 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/server/__init__.py
+-rw-r--r--  2.0 unx      706 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/index.html
+-rw-r--r--  2.0 unx   156236 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
+-rw-r--r--  2.0 unx   397728 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/b48ad290d0335879a92b.ttf
+-rw-r--r--  2.0 unx  3822921 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/index.js.map
+-rw-r--r--  2.0 unx   206260 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/5d681e2edae8c60630db.woff
+-rw-r--r--  2.0 unx   528999 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/index.css.map
+-rw-r--r--  2.0 unx   376002 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/index.css
+-rw-r--r--  2.0 unx   182028 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/f882956fd323fd322f31.woff
+-rw-r--r--  2.0 unx  3649207 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/index.js
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/manifest.json
+-rw-r--r--  2.0 unx   107460 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/e1a247a5ef41e1975742.woff2
+-rw-r--r--  2.0 unx      511 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/login.html
+-rw-r--r--  2.0 unx   155276 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
+-rw-r--r--  2.0 unx   215704 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
+-rw-r--r--  2.0 unx   150472 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/66104b766c3d0462b3c5.woff2
+-rw-r--r--  2.0 unx   164912 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
+-rw-r--r--  2.0 unx     3870 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/favicon.ico
+-rw-r--r--  2.0 unx   135984 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
+-rw-r--r--  2.0 unx   339600 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
+-rw-r--r--  2.0 unx   186112 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/f9ee61fab3c11e2f3ed3.ttf
+-rw-r--r--  2.0 unx   173620 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
+-rw-r--r--  2.0 unx    62048 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/abf801b7acb6705a15ad.ttf
+-rw-r--r--  2.0 unx   128352 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
+-rw-r--r--  2.0 unx    25096 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/server/data/639d2000c1ece92eaec8.woff2
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/launchers/slurm/
+-rw-r--r--  2.0 unx     1967 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launchers/direct.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launchers/oar.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launchers/__init__.py
+-rw-r--r--  2.0 unx    12747 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launchers/slurm/base.py
+-rw-r--r--  2.0 unx    19130 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launchers/slurm/configuration.py
+-rw-r--r--  2.0 unx       41 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launchers/slurm/__init__.py
+-rw-r--r--  2.0 unx      818 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/launchers/slurm/cli.py
+-rw-r--r--  2.0 unx     5620 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/arguments.py
+-rw-r--r--  2.0 unx    19141 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/types.py
+-rw-r--r--  2.0 unx    58915 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/objects.py
+-rw-r--r--  2.0 unx     7355 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/objects.pyi
+-rw-r--r--  2.0 unx     2479 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/context.py
+-rw-r--r--  2.0 unx      493 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/__init__.py
+-rw-r--r--  2.0 unx     1197 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/core/serializers.py
+-rw-r--r--  2.0 unx     1006 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/utils/resources.py
+-rw-r--r--  2.0 unx     6766 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/utils/yaml.py
+-rw-r--r--  2.0 unx      793 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/utils/settings.py
+-rw-r--r--  2.0 unx     2394 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/utils/jobs.py
+-rw-r--r--  2.0 unx      601 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/utils/asyncio.py
+-rw-r--r--  2.0 unx     2434 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/utils/__init__.py
+-rw-r--r--  2.0 unx     2183 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/utils/jupyter.py
+-rw-r--r--  2.0 unx     8206 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/connectors/ssh.py
+-rw-r--r--  2.0 unx     5461 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/connectors/__init__.py
+-rw-r--r--  2.0 unx     5760 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/connectors/local.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/launchers/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/tasks/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/connectors/
+-rw-r--r--  2.0 unx     3081 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_snippets.py
+-rw-r--r--  2.0 unx     1837 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_objects.py
+-rw-r--r--  2.0 unx      477 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/task_tokens.py
+-rw-r--r--  2.0 unx     4016 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/restart.py
+-rw-r--r--  2.0 unx      695 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/conftest.py
+-rw-r--r--  2.0 unx      781 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_outputs.py
+-rw-r--r--  2.0 unx     9099 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_tasks.py
+-rw-r--r--  2.0 unx      979 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_ssh.py
+-rw-r--r--  2.0 unx     4339 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_validation.py
+-rw-r--r--  2.0 unx     1502 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_serializers.py
+-rw-r--r--  2.0 unx    12285 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_identifier.py
+-rw-r--r--  2.0 unx     2964 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_findlauncher.py
+-rw-r--r--  2.0 unx     1701 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/token_reschedule.py
+-rw-r--r--  2.0 unx      780 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_forward.py
+-rw-r--r--  2.0 unx     6405 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_param.py
+-rw-r--r--  2.0 unx     1975 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_tags.py
+-rw-r--r--  2.0 unx     2005 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_dependencies.py
+-rw-r--r--  2.0 unx      295 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/restart_main.py
+-rw-r--r--  2.0 unx     3805 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/utils.py
+-rw-r--r--  2.0 unx     7826 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_tokens.py
+-rw-r--r--  2.0 unx     1540 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_instance.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/__init__.py
+-rw-r--r--  2.0 unx     7580 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_progress.py
+-rw-r--r--  2.0 unx      414 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/definitions_types.py
+-rw-r--r--  2.0 unx      403 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_checkers.py
+-rw-r--r--  2.0 unx     1257 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/test_types.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/launchers/config_slurm/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/
+-rw-r--r--  2.0 unx      717 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/test_local.py
+-rw-r--r--  2.0 unx     2534 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/test_slurm.py
+-rw-r--r--  2.0 unx     2468 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/common.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/__init__.py
+-rw-r--r--  2.0 unx     2497 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/config_slurm/__init__.py
+-rwxr-xr-x  2.0 unx      639 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/sacct
+-rwxr-xr-x  2.0 unx     1177 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/sbatch
+-rw-r--r--  2.0 unx      477 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/test.py
+-rw-r--r--  2.0 unx     1851 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/tasks/all.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/tasks/foreign.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/tasks/__init__.py
+-rw-r--r--  2.0 unx      407 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/scripts/notifyandwait.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/scripts/waitforfile.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro/tests/connectors/bin/
+-rw-r--r--  2.0 unx     1204 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/connectors/test_local.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/connectors/utils.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/tests/connectors/bin/executable.py
+-rw-r--r--  2.0 unx     1994 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/scheduler/dependencies.py
+-rw-r--r--  2.0 unx     1820 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/scheduler/services.py
+-rw-r--r--  2.0 unx     1731 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/scheduler/workspace.py
+-rw-r--r--  2.0 unx     2393 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/scheduler/environment.py
+-rw-r--r--  2.0 unx    29179 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/scheduler/base.py
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/src/experimaestro/scheduler/__init__.py
+-rw-r--r--  2.0 unx     7604 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx       14 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     7080 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      414 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      591 b- defN 23-Jul-27 12:09 experimaestro-1.1.0/src/experimaestro.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/app/xp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/app/public/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/app/src/
+-rw-r--r--  2.0 unx      536 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/tsconfig.json
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/CHANGELOG.md
+-rw-r--r--  2.0 unx      324 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/.gitignore
+-rw-r--r--  2.0 unx     2319 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/package.json
+-rw-r--r--  2.0 unx   127144 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/README.md
+-rw-r--r--  2.0 unx   785936 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/package-lock.json
+-rw-r--r--  2.0 unx      314 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/.nolluprc.js
+-rw-r--r--  2.0 unx     9556 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/webpack.config.ts
+-rw-r--r--  2.0 unx      930 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/postcss.config.js
+-rw-r--r--  2.0 unx     5061 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/xp/run.py
+-rw-r--r--  2.0 unx      706 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/public/index.html
+-rw-r--r--  2.0 unx      318 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/public/manifest.json
+-rw-r--r--  2.0 unx      511 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/public/login.html
+-rw-r--r--  2.0 unx     3870 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/public/favicon.ico
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/app/src/theme/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jul-27 12:09 experimaestro-1.1.0/app/src/ui/
+-rw-r--r--  2.0 unx   130132 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/logo.png
+-rw-r--r--  2.0 unx      682 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/index.tsx
+-rw-r--r--  2.0 unx     1461 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/client.ts
+-rw-r--r--  2.0 unx     1155 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/Services.tsx
+-rw-r--r--  2.0 unx     3656 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/Tasks.tsx
+-rw-r--r--  2.0 unx      102 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/index.css
+-rw-r--r--  2.0 unx      621 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/clipboard.ts
+-rw-r--r--  2.0 unx     1614 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/TaskJobs.tsx
+-rw-r--r--  2.0 unx       13 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/Experiments.tsx
+-rw-r--r--  2.0 unx   495919 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/logo.pxm
+-rw-r--r--  2.0 unx     3255 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/reducers.ts
+-rw-r--r--  2.0 unx      918 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/store.ts
+-rw-r--r--  2.0 unx     2845 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/TaskDetail.tsx
+-rw-r--r--  2.0 unx     1368 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/App.tsx
+-rw-r--r--  2.0 unx     1583 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/theme/theme.scss
+-rw-r--r--  2.0 unx     3400 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/theme/_jobs.scss
+-rw-r--r--  2.0 unx     3629 b- defN 23-Jul-27 12:08 experimaestro-1.1.0/app/src/ui/messages.tsx
+248 files, 13322799 bytes uncompressed, 5126785 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,742 +1,745 @@
-Filename: experimaestro-1.0.0/
+Filename: experimaestro-1.1.0/
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/
+Filename: experimaestro-1.1.0/docs/
 Comment: 
 
-Filename: experimaestro-1.0.0/scripts/
+Filename: experimaestro-1.1.0/scripts/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/
+Filename: experimaestro-1.1.0/src/
 Comment: 
 
-Filename: experimaestro-1.0.0/app/
+Filename: experimaestro-1.1.0/app/
 Comment: 
 
-Filename: experimaestro-1.0.0/requirements.txt
+Filename: experimaestro-1.1.0/requirements.txt
 Comment: 
 
-Filename: experimaestro-1.0.0/setup.cfg
+Filename: experimaestro-1.1.0/setup.cfg
 Comment: 
 
-Filename: experimaestro-1.0.0/pytest.ini
+Filename: experimaestro-1.1.0/pytest.ini
 Comment: 
 
-Filename: experimaestro-1.0.0/mkdocs.yml
+Filename: experimaestro-1.1.0/mkdocs.yml
 Comment: 
 
-Filename: experimaestro-1.0.0/.gitmodules
+Filename: experimaestro-1.1.0/.gitmodules
 Comment: 
 
-Filename: experimaestro-1.0.0/PKG-INFO
+Filename: experimaestro-1.1.0/PKG-INFO
 Comment: 
 
-Filename: experimaestro-1.0.0/CHANGELOG.md
+Filename: experimaestro-1.1.0/CHANGELOG.md
 Comment: 
 
-Filename: experimaestro-1.0.0/.gitignore
+Filename: experimaestro-1.1.0/.gitignore
 Comment: 
 
-Filename: experimaestro-1.0.0/MANIFEST.in
+Filename: experimaestro-1.1.0/MANIFEST.in
 Comment: 
 
-Filename: experimaestro-1.0.0/.flake8
+Filename: experimaestro-1.1.0/.flake8
 Comment: 
 
-Filename: experimaestro-1.0.0/LICENSE
+Filename: experimaestro-1.1.0/LICENSE
 Comment: 
 
-Filename: experimaestro-1.0.0/.prettierignore
+Filename: experimaestro-1.1.0/.prettierignore
 Comment: 
 
-Filename: experimaestro-1.0.0/README.md
+Filename: experimaestro-1.1.0/README.md
 Comment: 
 
-Filename: experimaestro-1.0.0/setup.py
+Filename: experimaestro-1.1.0/setup.py
 Comment: 
 
-Filename: experimaestro-1.0.0/pyproject.toml
+Filename: experimaestro-1.1.0/pyproject.toml
 Comment: 
 
-Filename: experimaestro-1.0.0/tox.ini
+Filename: experimaestro-1.1.0/tox.ini
 Comment: 
 
-Filename: experimaestro-1.0.0/.readthedocs.yml
+Filename: experimaestro-1.1.0/.readthedocs.yml
 Comment: 
 
-Filename: experimaestro-1.0.0/.pre-commit-config.yaml
+Filename: experimaestro-1.1.0/.pre-commit-config.yaml
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/launchers/
+Filename: experimaestro-1.1.0/docs/launchers/
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/experiments/
+Filename: experimaestro-1.1.0/docs/experiments/
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/connectors/
+Filename: experimaestro-1.1.0/docs/connectors/
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/requirements.txt
+Filename: experimaestro-1.1.0/docs/requirements.txt
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/faq.md
+Filename: experimaestro-1.1.0/docs/faq.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/configuration.md
+Filename: experimaestro-1.1.0/docs/configuration.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/index.md
+Filename: experimaestro-1.1.0/docs/index.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/documenting.md
+Filename: experimaestro-1.1.0/docs/documenting.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/cli.md
+Filename: experimaestro-1.1.0/docs/cli.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/changelog.md
+Filename: experimaestro-1.1.0/docs/changelog.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/serialization.md
+Filename: experimaestro-1.1.0/docs/serialization.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/tutorial.md
+Filename: experimaestro-1.1.0/docs/tutorial.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/concepts.md
+Filename: experimaestro-1.1.0/docs/concepts.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/jupyter.md
+Filename: experimaestro-1.1.0/docs/jupyter.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/launchers/index.md
+Filename: experimaestro-1.1.0/docs/launchers/index.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/experiments/task.md
+Filename: experimaestro-1.1.0/docs/experiments/task.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/experiments/config.md
+Filename: experimaestro-1.1.0/docs/experiments/config.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/experiments/overview.md
+Filename: experimaestro-1.1.0/docs/experiments/overview.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/experiments/plan.md
+Filename: experimaestro-1.1.0/docs/experiments/plan.md
 Comment: 
 
-Filename: experimaestro-1.0.0/docs/connectors/index.md
+Filename: experimaestro-1.1.0/docs/connectors/index.md
 Comment: 
 
-Filename: experimaestro-1.0.0/scripts/longtask.py
+Filename: experimaestro-1.1.0/scripts/longtask.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/
+Filename: experimaestro-1.1.0/src/experimaestro/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launcherfinder/
+Filename: experimaestro-1.1.0/src/experimaestro/launcherfinder/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/mkdocs/
+Filename: experimaestro-1.1.0/src/experimaestro/mkdocs/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tools/
+Filename: experimaestro-1.1.0/src/experimaestro/tools/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/sphinx/
+Filename: experimaestro-1.1.0/src/experimaestro/sphinx/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/
+Filename: experimaestro-1.1.0/src/experimaestro/server/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/
+Filename: experimaestro-1.1.0/src/experimaestro/core/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/
+Filename: experimaestro-1.1.0/src/experimaestro/utils/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/connectors/
+Filename: experimaestro-1.1.0/src/experimaestro/connectors/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/
+Filename: experimaestro-1.1.0/src/experimaestro/tests/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scheduler/
+Filename: experimaestro-1.1.0/src/experimaestro/scheduler/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/run.py
+Filename: experimaestro-1.1.0/src/experimaestro/run.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/mypy.py
+Filename: experimaestro-1.1.0/src/experimaestro/mypy.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/filter.py
+Filename: experimaestro-1.1.0/src/experimaestro/filter.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/version.py
+Filename: experimaestro-1.1.0/src/experimaestro/version.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/rpyc.py
+Filename: experimaestro-1.1.0/src/experimaestro/rpyc.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/typingutils.py
+Filename: experimaestro-1.1.0/src/experimaestro/typingutils.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/generators.py
+Filename: experimaestro-1.1.0/src/experimaestro/generators.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/annotations.py
+Filename: experimaestro-1.1.0/src/experimaestro/annotations.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/ipc.py
+Filename: experimaestro-1.1.0/src/experimaestro/ipc.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/xpmutils.py
+Filename: experimaestro-1.1.0/src/experimaestro/xpmutils.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/checkers.py
+Filename: experimaestro-1.1.0/src/experimaestro/checkers.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tokens.py
+Filename: experimaestro-1.1.0/src/experimaestro/tokens.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/settings.py
+Filename: experimaestro-1.1.0/src/experimaestro/settings.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/compat.py
+Filename: experimaestro-1.1.0/src/experimaestro/compat.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/notifications.py
+Filename: experimaestro-1.1.0/src/experimaestro/notifications.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/huggingface.py
+Filename: experimaestro-1.1.0/src/experimaestro/huggingface.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/locking.py
+Filename: experimaestro-1.1.0/src/experimaestro/locking.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/click.py
+Filename: experimaestro-1.1.0/src/experimaestro/click.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/__main__.py
+Filename: experimaestro-1.1.0/src/experimaestro/__main__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scriptbuilder.py
+Filename: experimaestro-1.1.0/src/experimaestro/scriptbuilder.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/commandline.py
+Filename: experimaestro-1.1.0/src/experimaestro/commandline.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/taskglobals.py
+Filename: experimaestro-1.1.0/src/experimaestro/taskglobals.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launcherfinder/specs.py
+Filename: experimaestro-1.1.0/src/experimaestro/launcherfinder/specs.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launcherfinder/base.py
+Filename: experimaestro-1.1.0/src/experimaestro/launcherfinder/base.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launcherfinder/registry.py
+Filename: experimaestro-1.1.0/src/experimaestro/launcherfinder/registry.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launcherfinder/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/launcherfinder/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launcherfinder/parser.py
+Filename: experimaestro-1.1.0/src/experimaestro/launcherfinder/parser.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/mkdocs/style.css
+Filename: experimaestro-1.1.0/src/experimaestro/mkdocs/style.css
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/mkdocs/annotations.py
+Filename: experimaestro-1.1.0/src/experimaestro/mkdocs/annotations.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/mkdocs/base.py
+Filename: experimaestro-1.1.0/src/experimaestro/mkdocs/base.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/mkdocs/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/mkdocs/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/mkdocs/metaloader.py
+Filename: experimaestro-1.1.0/src/experimaestro/mkdocs/metaloader.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tools/jobs.py
+Filename: experimaestro-1.1.0/src/experimaestro/tools/jobs.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tools/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/tools/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tools/diff.py
+Filename: experimaestro-1.1.0/src/experimaestro/tools/documentation.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/sphinx/static/
+Filename: experimaestro-1.1.0/src/experimaestro/tools/diff.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/sphinx/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/sphinx/static/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/sphinx/static/experimaestro.css
+Filename: experimaestro-1.1.0/src/experimaestro/sphinx/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/
+Filename: experimaestro-1.1.0/src/experimaestro/sphinx/static/experimaestro.css
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/index.html
+Filename: experimaestro-1.1.0/src/experimaestro/server/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/index.html
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/b48ad290d0335879a92b.ttf
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/3a4004a46a653d4b2166.woff
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/index.js.map
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/b48ad290d0335879a92b.ttf
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/5d681e2edae8c60630db.woff
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/index.js.map
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/index.css.map
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/5d681e2edae8c60630db.woff
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/index.css
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/index.css.map
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/f882956fd323fd322f31.woff
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/index.css
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/index.js
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/f882956fd323fd322f31.woff
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/manifest.json
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/index.js
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/e1a247a5ef41e1975742.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/manifest.json
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/login.html
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/e1a247a5ef41e1975742.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/login.html
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/66104b766c3d0462b3c5.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/66104b766c3d0462b3c5.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/favicon.ico
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/4d73cb90e394b34b7670.woff
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/favicon.ico
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/f9ee61fab3c11e2f3ed3.ttf
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/3baa5b8f3469222b822d.woff
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/f9ee61fab3c11e2f3ed3.ttf
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/abf801b7acb6705a15ad.ttf
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/c380809fd3677d7d6903.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/abf801b7acb6705a15ad.ttf
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/server/data/639d2000c1ece92eaec8.woff2
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/0c35d18bf06992036b69.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/slurm/
+Filename: experimaestro-1.1.0/src/experimaestro/server/data/639d2000c1ece92eaec8.woff2
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/direct.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/slurm/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/oar.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/direct.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/oar.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/slurm/base.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/slurm/configuration.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/slurm/base.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/slurm/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/slurm/configuration.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/launchers/slurm/cli.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/slurm/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/arguments.py
+Filename: experimaestro-1.1.0/src/experimaestro/launchers/slurm/cli.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/types.py
+Filename: experimaestro-1.1.0/src/experimaestro/core/arguments.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/objects.py
+Filename: experimaestro-1.1.0/src/experimaestro/core/types.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/objects.pyi
+Filename: experimaestro-1.1.0/src/experimaestro/core/objects.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/context.py
+Filename: experimaestro-1.1.0/src/experimaestro/core/objects.pyi
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/utils.py
+Filename: experimaestro-1.1.0/src/experimaestro/core/context.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/core/utils.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/core/serializers.py
+Filename: experimaestro-1.1.0/src/experimaestro/core/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/resources.py
+Filename: experimaestro-1.1.0/src/experimaestro/core/serializers.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/yaml.py
+Filename: experimaestro-1.1.0/src/experimaestro/utils/resources.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/settings.py
+Filename: experimaestro-1.1.0/src/experimaestro/utils/yaml.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/jobs.py
+Filename: experimaestro-1.1.0/src/experimaestro/utils/settings.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/asyncio.py
+Filename: experimaestro-1.1.0/src/experimaestro/utils/jobs.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/utils/asyncio.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/utils/jupyter.py
+Filename: experimaestro-1.1.0/src/experimaestro/utils/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/connectors/ssh.py
+Filename: experimaestro-1.1.0/src/experimaestro/utils/jupyter.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/connectors/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/connectors/ssh.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/connectors/local.py
+Filename: experimaestro-1.1.0/src/experimaestro/connectors/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/
+Filename: experimaestro-1.1.0/src/experimaestro/connectors/local.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/tasks/
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/scripts/
+Filename: experimaestro-1.1.0/src/experimaestro/tests/tasks/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/connectors/
+Filename: experimaestro-1.1.0/src/experimaestro/tests/scripts/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_snippets.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/connectors/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_objects.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_snippets.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/task_tokens.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_objects.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/restart.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/task_tokens.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/conftest.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/restart.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_outputs.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/conftest.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_tasks.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_outputs.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_ssh.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_tasks.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_validation.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_ssh.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_serializers.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_validation.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_identifier.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_serializers.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_findlauncher.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_identifier.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/token_reschedule.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_findlauncher.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_forward.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/token_reschedule.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_param.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_forward.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_tags.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_param.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_dependencies.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_tags.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/restart_main.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_dependencies.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/utils.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/restart_main.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_tokens.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/utils.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_instance.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_tokens.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_instance.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_progress.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/definitions_types.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_progress.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_checkers.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/definitions_types.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/test_types.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_checkers.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/config_slurm/
+Filename: experimaestro-1.1.0/src/experimaestro/tests/test_types.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/config_slurm/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/test_local.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/test_slurm.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/test_local.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/common.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/test_slurm.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/common.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/config_slurm/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/config_slurm/launchers.yaml
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/sacct
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/config_slurm/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/sbatch
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/sacct
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/test.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/sbatch
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/tasks/all.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/test.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/tasks/foreign.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/tasks/all.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/tasks/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/tasks/foreign.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/scripts/notifyandwait.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/tasks/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/scripts/waitforfile.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/scripts/notifyandwait.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/connectors/bin/
+Filename: experimaestro-1.1.0/src/experimaestro/tests/scripts/waitforfile.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/connectors/test_local.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/connectors/bin/
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/connectors/utils.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/connectors/test_local.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/tests/connectors/bin/executable.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/connectors/utils.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scheduler/dependencies.py
+Filename: experimaestro-1.1.0/src/experimaestro/tests/connectors/bin/executable.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scheduler/services.py
+Filename: experimaestro-1.1.0/src/experimaestro/scheduler/dependencies.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scheduler/workspace.py
+Filename: experimaestro-1.1.0/src/experimaestro/scheduler/services.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scheduler/environment.py
+Filename: experimaestro-1.1.0/src/experimaestro/scheduler/workspace.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scheduler/base.py
+Filename: experimaestro-1.1.0/src/experimaestro/scheduler/environment.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro/scheduler/__init__.py
+Filename: experimaestro-1.1.0/src/experimaestro/scheduler/base.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/PKG-INFO
+Filename: experimaestro-1.1.0/src/experimaestro/scheduler/__init__.py
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/not-zip-safe
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/PKG-INFO
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/top_level.txt
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/not-zip-safe
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/SOURCES.txt
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/top_level.txt
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/requires.txt
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/SOURCES.txt
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/dependency_links.txt
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/requires.txt
 Comment: 
 
-Filename: experimaestro-1.0.0/src/experimaestro.egg-info/entry_points.txt
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/dependency_links.txt
 Comment: 
 
-Filename: experimaestro-1.0.0/app/xp/
+Filename: experimaestro-1.1.0/src/experimaestro.egg-info/entry_points.txt
 Comment: 
 
-Filename: experimaestro-1.0.0/app/public/
+Filename: experimaestro-1.1.0/app/xp/
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/
+Filename: experimaestro-1.1.0/app/public/
 Comment: 
 
-Filename: experimaestro-1.0.0/app/tsconfig.json
+Filename: experimaestro-1.1.0/app/src/
 Comment: 
 
-Filename: experimaestro-1.0.0/app/CHANGELOG.md
+Filename: experimaestro-1.1.0/app/tsconfig.json
 Comment: 
 
-Filename: experimaestro-1.0.0/app/.gitignore
+Filename: experimaestro-1.1.0/app/CHANGELOG.md
 Comment: 
 
-Filename: experimaestro-1.0.0/app/package.json
+Filename: experimaestro-1.1.0/app/.gitignore
 Comment: 
 
-Filename: experimaestro-1.0.0/app/README.md
+Filename: experimaestro-1.1.0/app/package.json
 Comment: 
 
-Filename: experimaestro-1.0.0/app/package-lock.json
+Filename: experimaestro-1.1.0/app/README.md
 Comment: 
 
-Filename: experimaestro-1.0.0/app/.nolluprc.js
+Filename: experimaestro-1.1.0/app/package-lock.json
 Comment: 
 
-Filename: experimaestro-1.0.0/app/webpack.config.ts
+Filename: experimaestro-1.1.0/app/.nolluprc.js
 Comment: 
 
-Filename: experimaestro-1.0.0/app/postcss.config.js
+Filename: experimaestro-1.1.0/app/webpack.config.ts
 Comment: 
 
-Filename: experimaestro-1.0.0/app/xp/run.py
+Filename: experimaestro-1.1.0/app/postcss.config.js
 Comment: 
 
-Filename: experimaestro-1.0.0/app/public/index.html
+Filename: experimaestro-1.1.0/app/xp/run.py
 Comment: 
 
-Filename: experimaestro-1.0.0/app/public/manifest.json
+Filename: experimaestro-1.1.0/app/public/index.html
 Comment: 
 
-Filename: experimaestro-1.0.0/app/public/login.html
+Filename: experimaestro-1.1.0/app/public/manifest.json
 Comment: 
 
-Filename: experimaestro-1.0.0/app/public/favicon.ico
+Filename: experimaestro-1.1.0/app/public/login.html
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/theme/
+Filename: experimaestro-1.1.0/app/public/favicon.ico
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/ui/
+Filename: experimaestro-1.1.0/app/src/theme/
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/logo.png
+Filename: experimaestro-1.1.0/app/src/ui/
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/index.tsx
+Filename: experimaestro-1.1.0/app/src/logo.png
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/client.ts
+Filename: experimaestro-1.1.0/app/src/index.tsx
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/Services.tsx
+Filename: experimaestro-1.1.0/app/src/client.ts
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/Tasks.tsx
+Filename: experimaestro-1.1.0/app/src/Services.tsx
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/index.css
+Filename: experimaestro-1.1.0/app/src/Tasks.tsx
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/clipboard.ts
+Filename: experimaestro-1.1.0/app/src/index.css
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/TaskJobs.tsx
+Filename: experimaestro-1.1.0/app/src/clipboard.ts
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/Experiments.tsx
+Filename: experimaestro-1.1.0/app/src/TaskJobs.tsx
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/logo.pxm
+Filename: experimaestro-1.1.0/app/src/Experiments.tsx
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/reducers.ts
+Filename: experimaestro-1.1.0/app/src/logo.pxm
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/store.ts
+Filename: experimaestro-1.1.0/app/src/reducers.ts
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/TaskDetail.tsx
+Filename: experimaestro-1.1.0/app/src/store.ts
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/App.tsx
+Filename: experimaestro-1.1.0/app/src/TaskDetail.tsx
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/theme/theme.scss
+Filename: experimaestro-1.1.0/app/src/App.tsx
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/theme/_jobs.scss
+Filename: experimaestro-1.1.0/app/src/theme/theme.scss
 Comment: 
 
-Filename: experimaestro-1.0.0/app/src/ui/messages.tsx
+Filename: experimaestro-1.1.0/app/src/theme/_jobs.scss
+Comment: 
+
+Filename: experimaestro-1.1.0/app/src/ui/messages.tsx
 Comment: 
 
 Zip file comment:
```

## Comparing `experimaestro-1.0.0/requirements.txt` & `experimaestro-1.1.0/requirements.txt`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/setup.cfg` & `experimaestro-1.1.0/setup.cfg`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/mkdocs.yml` & `experimaestro-1.1.0/mkdocs.yml`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/PKG-INFO` & `experimaestro-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimaestro
-Version: 1.0.0
+Version: 1.1.0
 Summary: "Experimaestro is a computer science experiment manager"
 Home-page: https://github.com/experimaestro/experimaestro-python
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 License: GPL-3
 Keywords: experiment manager
 Platform: any
@@ -123,14 +123,21 @@
 
 if __name__ == "__main__":
     cli()
 ```
 
 which can be launched with `python test.py /tmp/helloworld-workdir`
 
+## 1.1.0 (2023-07-27)
+
+### Feat
+
+- Generic documentation checker (for use in automated tests)
+- improved check documentation command
+
 ## 1.0.0 (2023-07-23)
 
 ### Feat
 
 - List experiments
 - **documentation**: Checks for undocumented configuration objects in a package
```

## Comparing `experimaestro-1.0.0/CHANGELOG.md` & `experimaestro-1.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 1.1.0 (2023-07-27)
+
+### Feat
+
+- Generic documentation checker (for use in automated tests)
+- improved check documentation command
+
 ## 1.0.0 (2023-07-23)
 
 ### Feat
 
 - List experiments
 - **documentation**: Checks for undocumented configuration objects in a package
```

## Comparing `experimaestro-1.0.0/LICENSE` & `experimaestro-1.1.0/LICENSE`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/README.md` & `experimaestro-1.1.0/README.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/.pre-commit-config.yaml` & `experimaestro-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/faq.md` & `experimaestro-1.1.0/docs/faq.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/index.md` & `experimaestro-1.1.0/docs/index.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/documenting.md` & `experimaestro-1.1.0/docs/documenting.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/cli.md` & `experimaestro-1.1.0/docs/cli.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/serialization.md` & `experimaestro-1.1.0/docs/serialization.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/concepts.md` & `experimaestro-1.1.0/docs/concepts.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/jupyter.md` & `experimaestro-1.1.0/docs/jupyter.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/launchers/index.md` & `experimaestro-1.1.0/docs/launchers/index.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/experiments/task.md` & `experimaestro-1.1.0/docs/experiments/task.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/experiments/config.md` & `experimaestro-1.1.0/docs/experiments/config.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/experiments/overview.md` & `experimaestro-1.1.0/docs/experiments/overview.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/docs/experiments/plan.md` & `experimaestro-1.1.0/docs/experiments/plan.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/scripts/longtask.py` & `experimaestro-1.1.0/scripts/longtask.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/run.py` & `experimaestro-1.1.0/src/experimaestro/run.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/filter.py` & `experimaestro-1.1.0/src/experimaestro/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     def __init__(self, values):
         (self.varname,) = values
 
     def get(self, info: JobInformation):
         if self.varname == "@state":
             return info.state.name if info.state else None
 
+        if self.varname == "@name":
+            return str(info.path.parent.name)
+
         return info.tags.get(self.varname, None)
 
     def __repr__(self):
         return f"""VAR<{self.varname}>"""
 
 
 class BaseInExpr:
@@ -132,16 +135,14 @@
         self.operator, self.y = tokens
         self.x = None
 
     def filter(self, information: JobInformation):
         if self.operator == "and":
             return self.y.filter(information) and self.x.filter(information)
 
-        print(self.y.filter(information), "OR", self.x.filter(information))
-
         return self.y.filter(information) or self.x.filter(information)
 
     @staticmethod
     def summary(tokens):
         if len(tokens) == 1:
             return tokens[0]
         v = tokens[1]
@@ -168,15 +169,15 @@
 l = pp.Literal
 
 lpar, rpar, lbra, rbra, eq, comma, pipe, tilde = map(pp.Suppress, "()[]=,|~")
 quotedString = pp.QuotedString('"', unquoteResults=True) | pp.QuotedString(
     "'", unquoteResults=True
 )
 
-var = l("@state") | pp.Word(pp.alphas)
+var = l("@state") | l("@name") | pp.Word(pp.alphas)
 var.setParseAction(VarExpr)
 
 regexExpr = var + tilde + quotedString
 regexExpr.setParseAction(RegexExpr)
 
 varQuotedString = quotedString
 varQuotedString.setParseAction(ConstantString)
```

## Comparing `experimaestro-1.0.0/src/experimaestro/rpyc.py` & `experimaestro-1.1.0/src/experimaestro/rpyc.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/typingutils.py` & `experimaestro-1.1.0/src/experimaestro/typingutils.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/generators.py` & `experimaestro-1.1.0/src/experimaestro/generators.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/annotations.py` & `experimaestro-1.1.0/src/experimaestro/annotations.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/ipc.py` & `experimaestro-1.1.0/src/experimaestro/ipc.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/xpmutils.py` & `experimaestro-1.1.0/src/experimaestro/xpmutils.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/checkers.py` & `experimaestro-1.1.0/src/experimaestro/checkers.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tokens.py` & `experimaestro-1.1.0/src/experimaestro/tokens.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/settings.py` & `experimaestro-1.1.0/src/experimaestro/settings.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/notifications.py` & `experimaestro-1.1.0/src/experimaestro/notifications.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/huggingface.py` & `experimaestro-1.1.0/src/experimaestro/huggingface.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/locking.py` & `experimaestro-1.1.0/src/experimaestro/locking.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/__init__.py` & `experimaestro-1.1.0/src/experimaestro/__init__.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/click.py` & `experimaestro-1.1.0/src/experimaestro/click.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/__main__.py` & `experimaestro-1.1.0/src/experimaestro/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -189,15 +189,29 @@
     filter: str,
     tags: bool,
     ready: bool,
     kill: bool,
     clean: bool,
     force: bool,
 ):
-    """Job control: list, kill and clean"""
+    """Job control: list, kill and clean
+
+    The job filter is a boolean expression where tags (alphanumeric)
+    and special job information (@state for job state, @name for job full
+    name) can be compared to a given value (using '~' for regex matching,
+    '=', 'not in', or 'in')
+
+    For instance,
+
+    model = "bm25" and mode in ["a", b"] and @state = "RUNNING"
+
+    selects jobs where the tag model is "bm25", the tag mode is either
+    "a" or "b", and the state is running.
+
+    """
     for p in (path / "xp").glob("*"):
         if experiment and p.name != experiment:
             continue
 
         from .filter import createFilter, JobInformation
         from experimaestro.scheduler import JobState
 
@@ -326,64 +340,35 @@
             if show_all:
                 show(key, prefix="[not orphan] ")
             found += 1
 
     print(f"{found} jobs are not orphans")
 
 
+def arg_split(ctx, param, value):
+    # split columns by ',' and remove whitespace
+    return set(c.strip() for c in value.split(","))
+
+
+@click.option("--skip", default=set(), callback=arg_split)
 @click.argument("package", type=str)
 @click.argument("objects", type=Path)
 @cli.command()
-def check_documentation(objects, package):
+def check_documentation(objects, package, skip):
     """Check that all the configuration and tasks are documented within a
     package, relying on the sphinx objects.inv file"""
-    import pkgutil
-    import sphobjinv
-    import inspect
-    from experimaestro import Config
-    from importlib import import_module
-
-    def process(mod: ModuleType, configurations: Set):
-        ok = True
-        for info in pkgutil.iter_modules(mod.__path__, prefix=f"{mod.__name__}."):
-            try:
-                logging.info("Processing %s...", info.name)
-                mod = info.module_finder.find_module(info.name).load_module(info.name)
-                configurations.update(
-                    x
-                    for x in mod.__dict__.values()
-                    if inspect.isclass(x) and issubclass(x, Config)
-                )
-            except Exception:
-                logging.exception("Error while loading %s", info.name)
-                cprint(f"{info.name} module could not be loaded", "red")
-
-                ok = False
-
-            # Process sub-modules
-            if info.ispkg:
-                ok = process(mod, configurations) & ok
-
-        return ok
-
-    logging.info("Loading objects.inv")
-
-    inv = sphobjinv.Inventory(objects)
-    documented = set(
-        obj.name
-        for obj in inv.objects
-        if obj.domain == "py" and obj.role == "xpmconfig"
-    )
-
-    configurations = set()
-    ok = process(import_module(package), configurations)
-    for configuration in configurations:
-        name = f"{configuration.__module__}.{configuration.__qualname__}"
-        if name.startswith(f"{package}.") and name not in documented:
-            cprint(f"{name} is not documented", "red")
+    from experimaestro.tools.documentation import documented_from_objects, undocumented
+
+    documented = documented_from_objects(objects)
+    ok, configs = undocumented(package, documented, skip)
+    for config in configs:
+        cprint(f"{config.__module__}.{config.__qualname__}", "red")
+
+    if not ok or configs:
+        sys.exit(1)
 
 
 @click.option("--config", type=Path, help="Show size of each folder")
 @click.argument("spec", type=str)
 @cli.command()
 def find_launchers(config: Optional[Path], spec: str):
     """Find launchers matching a specification"""
```

## Comparing `experimaestro-1.0.0/src/experimaestro/scriptbuilder.py` & `experimaestro-1.1.0/src/experimaestro/scriptbuilder.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/commandline.py` & `experimaestro-1.1.0/src/experimaestro/commandline.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launcherfinder/specs.py` & `experimaestro-1.1.0/src/experimaestro/launcherfinder/specs.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launcherfinder/base.py` & `experimaestro-1.1.0/src/experimaestro/launcherfinder/base.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launcherfinder/registry.py` & `experimaestro-1.1.0/src/experimaestro/launcherfinder/registry.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launcherfinder/parser.py` & `experimaestro-1.1.0/src/experimaestro/launcherfinder/parser.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/mkdocs/base.py` & `experimaestro-1.1.0/src/experimaestro/mkdocs/base.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/mkdocs/metaloader.py` & `experimaestro-1.1.0/src/experimaestro/mkdocs/metaloader.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tools/jobs.py` & `experimaestro-1.1.0/src/experimaestro/tools/jobs.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tools/diff.py` & `experimaestro-1.1.0/src/experimaestro/tools/diff.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/sphinx/__init__.py` & `experimaestro-1.1.0/src/experimaestro/sphinx/__init__.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/__init__.py` & `experimaestro-1.1.0/src/experimaestro/server/__init__.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/index.html` & `experimaestro-1.1.0/src/experimaestro/server/data/index.html`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/3a4004a46a653d4b2166.woff` & `experimaestro-1.1.0/src/experimaestro/server/data/3a4004a46a653d4b2166.woff`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/b48ad290d0335879a92b.ttf` & `experimaestro-1.1.0/src/experimaestro/server/data/b48ad290d0335879a92b.ttf`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/index.js.map` & `experimaestro-1.1.0/src/experimaestro/server/data/index.js.map`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/5d681e2edae8c60630db.woff` & `experimaestro-1.1.0/src/experimaestro/server/data/5d681e2edae8c60630db.woff`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/index.css.map` & `experimaestro-1.1.0/src/experimaestro/server/data/index.css.map`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/index.css` & `experimaestro-1.1.0/src/experimaestro/server/data/index.css`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/f882956fd323fd322f31.woff` & `experimaestro-1.1.0/src/experimaestro/server/data/f882956fd323fd322f31.woff`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/index.js` & `experimaestro-1.1.0/src/experimaestro/server/data/index.js`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/e1a247a5ef41e1975742.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/e1a247a5ef41e1975742.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/6f420cf17cc0d7676fad.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/4ef4218c522f1eb6b5b1.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/66104b766c3d0462b3c5.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/66104b766c3d0462b3c5.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/4d73cb90e394b34b7670.woff` & `experimaestro-1.1.0/src/experimaestro/server/data/4d73cb90e394b34b7670.woff`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/favicon.ico` & `experimaestro-1.1.0/src/experimaestro/server/data/favicon.ico`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/219aa9140e099e6c72ed.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/3baa5b8f3469222b822d.woff` & `experimaestro-1.1.0/src/experimaestro/server/data/3baa5b8f3469222b822d.woff`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/f9ee61fab3c11e2f3ed3.ttf` & `experimaestro-1.1.0/src/experimaestro/server/data/f9ee61fab3c11e2f3ed3.ttf`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/c380809fd3677d7d6903.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/c380809fd3677d7d6903.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/abf801b7acb6705a15ad.ttf` & `experimaestro-1.1.0/src/experimaestro/server/data/abf801b7acb6705a15ad.ttf`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/0c35d18bf06992036b69.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/0c35d18bf06992036b69.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/server/data/639d2000c1ece92eaec8.woff2` & `experimaestro-1.1.0/src/experimaestro/server/data/639d2000c1ece92eaec8.woff2`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launchers/direct.py` & `experimaestro-1.1.0/src/experimaestro/launchers/direct.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launchers/__init__.py` & `experimaestro-1.1.0/src/experimaestro/launchers/__init__.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launchers/slurm/base.py` & `experimaestro-1.1.0/src/experimaestro/launchers/slurm/base.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launchers/slurm/configuration.py` & `experimaestro-1.1.0/src/experimaestro/launchers/slurm/configuration.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/launchers/slurm/cli.py` & `experimaestro-1.1.0/src/experimaestro/launchers/slurm/cli.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/core/arguments.py` & `experimaestro-1.1.0/src/experimaestro/core/arguments.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/core/types.py` & `experimaestro-1.1.0/src/experimaestro/core/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,15 +251,17 @@
         __configbases__ = tuple(
             s.__getxpmtype__().configtype
             for s in tp.__bases__
             if issubclass(s, Config) and (s is not Config)
         ) or (TypeConfig,)
 
         *tp_qual, tp_name = self.basetype.__qualname__.split(".")
-        self.configtype = type(f"{tp_name}_XPMConfig", __configbases__ + (self.basetype,), {})
+        self.configtype = type(
+            f"{tp_name}_XPMConfig", __configbases__ + (self.basetype,), {}
+        )
         self.configtype.__qualname__ = ".".join(tp_qual + [self.configtype.__name__])
         self.configtype.__module__ = tp.__module__
 
         # Create the type-specific object class
         # (now, the same as basetype - but in the future, remove references)
         self.objecttype = self.basetype  # type: type
         self.basetype._ = self.configtype
@@ -307,15 +309,15 @@
             return
         self.__initialized__ = True
 
         from .objects import Task
 
         # Get the module
         module = inspect.getmodule(self.originaltype)
-        if getattr(module, '__file__', None) is None:
+        if getattr(module, "__file__", None) is None:
             self._file = None
         else:
             self._file = Path(inspect.getfile(self.originaltype)).absolute()
         self._module = module.__name__
         self._package = module.__package__
 
         # The class of the object
@@ -414,14 +416,19 @@
         # Uses the parent identifier (and saves the deprecated one for path updates)
         self._deprecated_identifier = self.identifier
         parent = self.basetype.__bases__[0].__getxpmtype__()
         self.identifier = parent.identifier
         self._deprecated = True
 
     @property
+    def deprecated(self) -> bool:
+        """Returns true if this type is deprecated"""
+        return self._deprecated
+
+    @property
     def description(self) -> str:
         self.__parsedoc__()
         return self._description
 
     @property
     def title(self) -> Dict[str, Argument]:
         self.__parsedoc__()
```

## Comparing `experimaestro-1.0.0/src/experimaestro/core/objects.py` & `experimaestro-1.1.0/src/experimaestro/core/objects.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/core/objects.pyi` & `experimaestro-1.1.0/src/experimaestro/core/objects.pyi`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/core/context.py` & `experimaestro-1.1.0/src/experimaestro/core/context.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/core/serializers.py` & `experimaestro-1.1.0/src/experimaestro/core/serializers.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/utils/resources.py` & `experimaestro-1.1.0/src/experimaestro/utils/resources.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/utils/yaml.py` & `experimaestro-1.1.0/src/experimaestro/utils/yaml.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/utils/settings.py` & `experimaestro-1.1.0/src/experimaestro/utils/settings.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/utils/jobs.py` & `experimaestro-1.1.0/src/experimaestro/utils/jobs.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/utils/asyncio.py` & `experimaestro-1.1.0/src/experimaestro/utils/asyncio.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/utils/__init__.py` & `experimaestro-1.1.0/src/experimaestro/utils/__init__.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/utils/jupyter.py` & `experimaestro-1.1.0/src/experimaestro/utils/jupyter.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/connectors/ssh.py` & `experimaestro-1.1.0/src/experimaestro/connectors/ssh.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/connectors/__init__.py` & `experimaestro-1.1.0/src/experimaestro/connectors/__init__.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/connectors/local.py` & `experimaestro-1.1.0/src/experimaestro/connectors/local.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_snippets.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_snippets.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_objects.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_objects.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/restart.py` & `experimaestro-1.1.0/src/experimaestro/tests/restart.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/conftest.py` & `experimaestro-1.1.0/src/experimaestro/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_outputs.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_outputs.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_tasks.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_tasks.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_ssh.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_ssh.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_validation.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_validation.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_serializers.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_serializers.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_identifier.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_identifier.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_findlauncher.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_findlauncher.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/token_reschedule.py` & `experimaestro-1.1.0/src/experimaestro/tests/token_reschedule.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_forward.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_forward.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_param.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_param.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_tags.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_tags.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_dependencies.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_dependencies.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/utils.py` & `experimaestro-1.1.0/src/experimaestro/tests/utils.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_tokens.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_tokens.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_instance.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_instance.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_progress.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_progress.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/test_types.py` & `experimaestro-1.1.0/src/experimaestro/tests/test_types.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/launchers/test_local.py` & `experimaestro-1.1.0/src/experimaestro/tests/launchers/test_local.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/launchers/test_slurm.py` & `experimaestro-1.1.0/src/experimaestro/tests/launchers/test_slurm.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/launchers/common.py` & `experimaestro-1.1.0/src/experimaestro/tests/launchers/common.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/launchers/config_slurm/launchers.yaml` & `experimaestro-1.1.0/src/experimaestro/tests/launchers/config_slurm/launchers.yaml`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/sacct` & `experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/sacct`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/launchers/bin/sbatch` & `experimaestro-1.1.0/src/experimaestro/tests/launchers/bin/sbatch`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/tasks/all.py` & `experimaestro-1.1.0/src/experimaestro/tests/tasks/all.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/connectors/test_local.py` & `experimaestro-1.1.0/src/experimaestro/tests/connectors/test_local.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/tests/connectors/utils.py` & `experimaestro-1.1.0/src/experimaestro/tests/connectors/utils.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/scheduler/dependencies.py` & `experimaestro-1.1.0/src/experimaestro/scheduler/dependencies.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/scheduler/services.py` & `experimaestro-1.1.0/src/experimaestro/scheduler/services.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/scheduler/workspace.py` & `experimaestro-1.1.0/src/experimaestro/scheduler/workspace.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/scheduler/environment.py` & `experimaestro-1.1.0/src/experimaestro/scheduler/environment.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro/scheduler/base.py` & `experimaestro-1.1.0/src/experimaestro/scheduler/base.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/src/experimaestro.egg-info/PKG-INFO` & `experimaestro-1.1.0/src/experimaestro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimaestro
-Version: 1.0.0
+Version: 1.1.0
 Summary: "Experimaestro is a computer science experiment manager"
 Home-page: https://github.com/experimaestro/experimaestro-python
 Author: Benjamin Piwowarski
 Author-email: benjamin@piwowarski.fr
 License: GPL-3
 Keywords: experiment manager
 Platform: any
@@ -123,14 +123,21 @@
 
 if __name__ == "__main__":
     cli()
 ```
 
 which can be launched with `python test.py /tmp/helloworld-workdir`
 
+## 1.1.0 (2023-07-27)
+
+### Feat
+
+- Generic documentation checker (for use in automated tests)
+- improved check documentation command
+
 ## 1.0.0 (2023-07-23)
 
 ### Feat
 
 - List experiments
 - **documentation**: Checks for undocumented configuration objects in a package
```

## Comparing `experimaestro-1.0.0/src/experimaestro.egg-info/SOURCES.txt` & `experimaestro-1.1.0/src/experimaestro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 src/experimaestro/tests/scripts/notifyandwait.py
 src/experimaestro/tests/scripts/waitforfile.py
 src/experimaestro/tests/tasks/__init__.py
 src/experimaestro/tests/tasks/all.py
 src/experimaestro/tests/tasks/foreign.py
 src/experimaestro/tools/__init__.py
 src/experimaestro/tools/diff.py
+src/experimaestro/tools/documentation.py
 src/experimaestro/tools/jobs.py
 src/experimaestro/utils/__init__.py
 src/experimaestro/utils/asyncio.py
 src/experimaestro/utils/jobs.py
 src/experimaestro/utils/jupyter.py
 src/experimaestro/utils/resources.py
 src/experimaestro/utils/settings.py
```

## Comparing `experimaestro-1.0.0/src/experimaestro.egg-info/entry_points.txt` & `experimaestro-1.1.0/src/experimaestro.egg-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/tsconfig.json` & `experimaestro-1.1.0/app/tsconfig.json`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/CHANGELOG.md` & `experimaestro-1.1.0/app/CHANGELOG.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/package.json` & `experimaestro-1.1.0/app/package.json`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/README.md` & `experimaestro-1.1.0/app/README.md`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/package-lock.json` & `experimaestro-1.1.0/app/package-lock.json`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/webpack.config.ts` & `experimaestro-1.1.0/app/webpack.config.ts`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/postcss.config.js` & `experimaestro-1.1.0/app/postcss.config.js`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/xp/run.py` & `experimaestro-1.1.0/app/xp/run.py`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/public/index.html` & `experimaestro-1.1.0/app/public/index.html`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/public/favicon.ico` & `experimaestro-1.1.0/app/public/favicon.ico`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/logo.png` & `experimaestro-1.1.0/app/src/logo.png`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/index.tsx` & `experimaestro-1.1.0/app/src/index.tsx`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/client.ts` & `experimaestro-1.1.0/app/src/client.ts`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/Services.tsx` & `experimaestro-1.1.0/app/src/Services.tsx`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/Tasks.tsx` & `experimaestro-1.1.0/app/src/Tasks.tsx`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/clipboard.ts` & `experimaestro-1.1.0/app/src/clipboard.ts`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/TaskJobs.tsx` & `experimaestro-1.1.0/app/src/TaskJobs.tsx`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/logo.pxm` & `experimaestro-1.1.0/app/src/logo.pxm`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/reducers.ts` & `experimaestro-1.1.0/app/src/reducers.ts`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/store.ts` & `experimaestro-1.1.0/app/src/store.ts`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/TaskDetail.tsx` & `experimaestro-1.1.0/app/src/TaskDetail.tsx`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/App.tsx` & `experimaestro-1.1.0/app/src/App.tsx`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/theme/theme.scss` & `experimaestro-1.1.0/app/src/theme/theme.scss`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/theme/_jobs.scss` & `experimaestro-1.1.0/app/src/theme/_jobs.scss`

 * *Files identical despite different names*

## Comparing `experimaestro-1.0.0/app/src/ui/messages.tsx` & `experimaestro-1.1.0/app/src/ui/messages.tsx`

 * *Files identical despite different names*

