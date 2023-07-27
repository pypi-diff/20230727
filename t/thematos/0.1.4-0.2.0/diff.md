# Comparing `tmp/thematos-0.1.4.tar.gz` & `tmp/thematos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thematos-0.1.4.tar", max compression
+gzip compressed data, was "thematos-0.2.0.tar", max compression
```

## Comparing `thematos-0.1.4.tar` & `thematos-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,12 @@
--rw-r--r--   0        0        0     1071 2023-04-25 23:56:45.162489 thematos-0.1.4/LICENSE
--rw-r--r--   0        0        0     3479 2023-04-25 23:56:45.162489 thematos-0.1.4/README.md
--rw-r--r--   0        0        0     2848 2023-04-25 23:57:20.862580 thematos-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      176 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/__cli__.py
--rw-r--r--   0        0        0      817 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/__init__.py
--rw-r--r--   0        0        0       21 2023-04-25 23:57:20.802580 thematos-0.1.4/src/thematos/_version.py
--rw-r--r--   0        0        0        0 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/__init__.py
--rw-r--r--   0        0        0      196 2023-04-25 23:57:20.802580 thematos-0.1.4/src/thematos/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-25 23:56:45.162489 thematos-0.1.4/src/thematos/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/conf/task/__init__.yaml
--rw-r--r--   0        0        0      197 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/project.toml
--rw-r--r--   0        0        0        0 2023-04-25 23:56:45.166489 thematos-0.1.4/src/thematos/py.typed
--rw-r--r--   0        0        0     4120 1970-01-01 00:00:00.000000 thematos-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-27 09:00:53.178073 thematos-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2112 2023-07-27 09:00:53.178073 thematos-0.2.0/README.md
+-rw-r--r--   0        0        0     2879 2023-07-27 09:01:19.226149 thematos-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-27 09:01:19.186149 thematos-0.2.0/src/thematos/_version.py
+-rw-r--r--   0        0        0        0 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/conf/__init__.py
+-rw-r--r--   0        0        0      179 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/conf/about/thematos.yaml
+-rw-r--r--   0        0        0        0 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/conf/topic/__init__.yaml
+-rw-r--r--   0        0        0      197 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/project.toml
+-rw-r--r--   0        0        0        0 2023-07-27 09:00:53.178073 thematos-0.2.0/src/thematos/py.typed
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 thematos-0.2.0/PKG-INFO
```

### Comparing `thematos-0.1.4/LICENSE` & `thematos-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thematos-0.1.4/pyproject.toml` & `thematos-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 [tool.poetry]
 name = "thematos"
-version = "0.1.4"
+version = "0.2.0"
 description = "A Python Library for Topic Modeling"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://thematos.entelecheia.ai"
 repository = "https://github.com/entelecheia/thematos"
 readme = "README.md"
 packages = [{ include = "thematos", from = "src" }]
 
 [tool.poetry.scripts]
 thematos = 'thematos.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.15"
+click = "^8.1.3"
+hyfi = "^1.11.0"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
-black = "^23.1.0"
+black = ">=23.0.0,<=23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
+
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
@@ -70,30 +77,29 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/thematos/_version.py:__version__"
-version_pattern = 'src/thematos/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
 commit_version_number = true # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
+build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

