# Comparing `tmp/mrgrain.cdk-esbuild-4.1.9.tar.gz` & `tmp/mrgrain.cdk-esbuild-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrgrain.cdk-esbuild-4.1.9.tar", last modified: Thu Jun 15 05:05:11 2023, max compression
+gzip compressed data, was "mrgrain.cdk-esbuild-4.2.0.tar", last modified: Wed Jul 26 23:52:47 2023, max compression
```

## Comparing `mrgrain.cdk-esbuild-4.1.9.tar` & `mrgrain.cdk-esbuild-4.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:05:11.227147 mrgrain.cdk-esbuild-4.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-06-15 05:05:11.227147 mrgrain.cdk-esbuild-4.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18595 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 05:05:11.227147 mrgrain.cdk-esbuild-4.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:05:11.223147 mrgrain.cdk-esbuild-4.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:05:11.223147 mrgrain.cdk-esbuild-4.1.9/src/mrgrain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:05:11.227147 mrgrain.cdk-esbuild-4.1.9/src/mrgrain/cdk_esbuild/
--rw-r--r--   0 runner    (1001) docker     (123)   393083 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain/cdk_esbuild/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:05:11.227147 mrgrain.cdk-esbuild-4.1.9/src/mrgrain/cdk_esbuild/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain/cdk_esbuild/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81279 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.1.9.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:04:54.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain/cdk_esbuild/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 05:05:11.223147 mrgrain.cdk-esbuild-4.1.9/src/mrgrain.cdk_esbuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19553 2023-06-15 05:05:11.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 05:05:11.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 05:05:11.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-15 05:05:11.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain.cdk_esbuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 05:05:11.000000 mrgrain.cdk-esbuild-4.1.9/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.226481 mrgrain.cdk-esbuild-4.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.226481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)   411762 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.230481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82716 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/_jsii/cdk-esbuild@4.2.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:52:34.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 23:52:47.226481 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 23:52:47.000000 mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/top_level.txt
```

### Comparing `mrgrain.cdk-esbuild-4.1.9/LICENSE` & `mrgrain.cdk-esbuild-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mrgrain.cdk-esbuild-4.1.9/PKG-INFO` & `mrgrain.cdk-esbuild-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.1.9
+Version: 4.2.0
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -293,18 +293,18 @@
 
 A custom implementation can be provided by implementing `IBuildProvider` or `ITransformProvider`:
 
 ```python
 @jsii.implements(IBuildProvider)
 @jsii.implements(ITransformProvider)
 class CustomEsbuild:
-    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         pass
 
-    def transform_sync(self, code, *, tsconfigRaw=None, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def transform_sync(self, code, *, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         # custom implementation goes here, return transformed code
         return "transformed code"
 
 # These will use the custom implementation
 TypeScriptCode("src/handler.ts",
     build_provider=CustomEsbuild()
 )
```

### Comparing `mrgrain.cdk-esbuild-4.1.9/README.md` & `mrgrain.cdk-esbuild-4.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -269,18 +269,18 @@
 
 A custom implementation can be provided by implementing `IBuildProvider` or `ITransformProvider`:
 
 ```python
 @jsii.implements(IBuildProvider)
 @jsii.implements(ITransformProvider)
 class CustomEsbuild:
-    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         pass
 
-    def transform_sync(self, code, *, tsconfigRaw=None, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def transform_sync(self, code, *, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         # custom implementation goes here, return transformed code
         return "transformed code"
 
 # These will use the custom implementation
 TypeScriptCode("src/handler.ts",
     build_provider=CustomEsbuild()
 )
```

### Comparing `mrgrain.cdk-esbuild-4.1.9/setup.py` & `mrgrain.cdk-esbuild-4.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "mrgrain.cdk-esbuild",
-    "version": "4.1.9",
+    "version": "4.2.0",
     "description": "CDK constructs for esbuild, an extremely fast JavaScript bundler",
     "license": "MIT",
     "url": "https://github.com/mrgrain/cdk-esbuild",
     "long_description_content_type": "text/markdown",
     "author": "Moritz Kornher<mail@moritzkornher.de>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "mrgrain.cdk_esbuild",
         "mrgrain.cdk_esbuild._jsii"
     ],
     "package_data": {
         "mrgrain.cdk_esbuild._jsii": [
-            "cdk-esbuild@4.1.9.jsii.tgz"
+            "cdk-esbuild@4.2.0.jsii.tgz"
         ],
         "mrgrain.cdk_esbuild": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.12.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.83.0, <2.0.0",
+        "jsii>=1.85.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `mrgrain.cdk-esbuild-4.1.9/src/mrgrain/cdk_esbuild/__init__.py` & `mrgrain.cdk-esbuild-4.2.0/src/mrgrain/cdk_esbuild/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,18 +270,18 @@
 
 A custom implementation can be provided by implementing `IBuildProvider` or `ITransformProvider`:
 
 ```python
 @jsii.implements(IBuildProvider)
 @jsii.implements(ITransformProvider)
 class CustomEsbuild:
-    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         pass
 
-    def transform_sync(self, code, *, tsconfigRaw=None, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def transform_sync(self, code, *, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         # custom implementation goes here, return transformed code
         return "transformed code"
 
 # These will use the custom implementation
 TypeScriptCode("src/handler.ts",
     build_provider=CustomEsbuild()
 )
@@ -437,14 +437,15 @@
         "bundle": "bundle",
         "charset": "charset",
         "chunk_names": "chunkNames",
         "color": "color",
         "conditions": "conditions",
         "define": "define",
         "drop": "drop",
+        "drop_labels": "dropLabels",
         "entry_names": "entryNames",
         "external": "external",
         "footer": "footer",
         "format": "format",
         "global_name": "globalName",
         "ignore_annotations": "ignoreAnnotations",
         "inject": "inject",
@@ -452,14 +453,15 @@
         "jsx_dev": "jsxDev",
         "jsx_factory": "jsxFactory",
         "jsx_fragment": "jsxFragment",
         "jsx_import_source": "jsxImportSource",
         "jsx_side_effects": "jsxSideEffects",
         "keep_names": "keepNames",
         "legal_comments": "legalComments",
+        "line_limit": "lineLimit",
         "loader": "loader",
         "log_level": "logLevel",
         "log_limit": "logLimit",
         "log_override": "logOverride",
         "main_fields": "mainFields",
         "mangle_cache": "mangleCache",
         "mangle_props": "mangleProps",
@@ -485,14 +487,15 @@
         "source_root": "sourceRoot",
         "sources_content": "sourcesContent",
         "splitting": "splitting",
         "supported": "supported",
         "target": "target",
         "tree_shaking": "treeShaking",
         "tsconfig": "tsconfig",
+        "tsconfig_raw": "tsconfigRaw",
         "write": "write",
     },
 )
 class BuildOptions:
     def __init__(
         self,
         *,
@@ -504,14 +507,15 @@
         bundle: typing.Optional[builtins.bool] = None,
         charset: typing.Optional[builtins.str] = None,
         chunk_names: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         conditions: typing.Optional[typing.Sequence[builtins.str]] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         entry_names: typing.Optional[builtins.str] = None,
         external: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         inject: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -519,14 +523,15 @@
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         main_fields: typing.Optional[typing.Sequence[builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
@@ -552,14 +557,15 @@
         source_root: typing.Optional[builtins.str] = None,
         sources_content: typing.Optional[builtins.bool] = None,
         splitting: typing.Optional[builtins.bool] = None,
         supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
         target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         tree_shaking: typing.Optional[builtins.bool] = None,
         tsconfig: typing.Optional[builtins.str] = None,
+        tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union["TsconfigOptions", typing.Dict[builtins.str, typing.Any]]]] = None,
         write: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param abs_working_dir: Documentation: https://esbuild.github.io/api/#working-directory.
         :param alias: Documentation: https://esbuild.github.io/api/#alias.
         :param allow_overwrite: Documentation: https://esbuild.github.io/api/#allow-overwrite.
         :param asset_names: Documentation: https://esbuild.github.io/api/#asset-names.
@@ -567,14 +573,15 @@
         :param bundle: Documentation: https://esbuild.github.io/api/#bundle.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param chunk_names: Documentation: https://esbuild.github.io/api/#chunk-names.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param conditions: Documentation: https://esbuild.github.io/api/#conditions.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
         :param entry_names: Documentation: https://esbuild.github.io/api/#entry-names.
         :param external: Documentation: https://esbuild.github.io/api/#external.
         :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param inject: Documentation: https://esbuild.github.io/api/#inject.
@@ -582,14 +589,15 @@
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
         :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param main_fields: Documentation: https://esbuild.github.io/api/#main-fields.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
@@ -615,14 +623,15 @@
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param splitting: Documentation: https://esbuild.github.io/api/#splitting.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
         :param tsconfig: Documentation: https://esbuild.github.io/api/#tsconfig.
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         :param write: Documentation: https://esbuild.github.io/api/#write.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf3dbfe8b02ff3b7a13b707799738cc16cd402c4e3086f60eb8f86814c6b2680)
             check_type(argname="argument abs_working_dir", value=abs_working_dir, expected_type=type_hints["abs_working_dir"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument allow_overwrite", value=allow_overwrite, expected_type=type_hints["allow_overwrite"])
@@ -631,14 +640,15 @@
             check_type(argname="argument bundle", value=bundle, expected_type=type_hints["bundle"])
             check_type(argname="argument charset", value=charset, expected_type=type_hints["charset"])
             check_type(argname="argument chunk_names", value=chunk_names, expected_type=type_hints["chunk_names"])
             check_type(argname="argument color", value=color, expected_type=type_hints["color"])
             check_type(argname="argument conditions", value=conditions, expected_type=type_hints["conditions"])
             check_type(argname="argument define", value=define, expected_type=type_hints["define"])
             check_type(argname="argument drop", value=drop, expected_type=type_hints["drop"])
+            check_type(argname="argument drop_labels", value=drop_labels, expected_type=type_hints["drop_labels"])
             check_type(argname="argument entry_names", value=entry_names, expected_type=type_hints["entry_names"])
             check_type(argname="argument external", value=external, expected_type=type_hints["external"])
             check_type(argname="argument footer", value=footer, expected_type=type_hints["footer"])
             check_type(argname="argument format", value=format, expected_type=type_hints["format"])
             check_type(argname="argument global_name", value=global_name, expected_type=type_hints["global_name"])
             check_type(argname="argument ignore_annotations", value=ignore_annotations, expected_type=type_hints["ignore_annotations"])
             check_type(argname="argument inject", value=inject, expected_type=type_hints["inject"])
@@ -646,14 +656,15 @@
             check_type(argname="argument jsx_dev", value=jsx_dev, expected_type=type_hints["jsx_dev"])
             check_type(argname="argument jsx_factory", value=jsx_factory, expected_type=type_hints["jsx_factory"])
             check_type(argname="argument jsx_fragment", value=jsx_fragment, expected_type=type_hints["jsx_fragment"])
             check_type(argname="argument jsx_import_source", value=jsx_import_source, expected_type=type_hints["jsx_import_source"])
             check_type(argname="argument jsx_side_effects", value=jsx_side_effects, expected_type=type_hints["jsx_side_effects"])
             check_type(argname="argument keep_names", value=keep_names, expected_type=type_hints["keep_names"])
             check_type(argname="argument legal_comments", value=legal_comments, expected_type=type_hints["legal_comments"])
+            check_type(argname="argument line_limit", value=line_limit, expected_type=type_hints["line_limit"])
             check_type(argname="argument loader", value=loader, expected_type=type_hints["loader"])
             check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
             check_type(argname="argument log_limit", value=log_limit, expected_type=type_hints["log_limit"])
             check_type(argname="argument log_override", value=log_override, expected_type=type_hints["log_override"])
             check_type(argname="argument main_fields", value=main_fields, expected_type=type_hints["main_fields"])
             check_type(argname="argument mangle_cache", value=mangle_cache, expected_type=type_hints["mangle_cache"])
             check_type(argname="argument mangle_props", value=mangle_props, expected_type=type_hints["mangle_props"])
@@ -679,14 +690,15 @@
             check_type(argname="argument source_root", value=source_root, expected_type=type_hints["source_root"])
             check_type(argname="argument sources_content", value=sources_content, expected_type=type_hints["sources_content"])
             check_type(argname="argument splitting", value=splitting, expected_type=type_hints["splitting"])
             check_type(argname="argument supported", value=supported, expected_type=type_hints["supported"])
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
             check_type(argname="argument tree_shaking", value=tree_shaking, expected_type=type_hints["tree_shaking"])
             check_type(argname="argument tsconfig", value=tsconfig, expected_type=type_hints["tsconfig"])
+            check_type(argname="argument tsconfig_raw", value=tsconfig_raw, expected_type=type_hints["tsconfig_raw"])
             check_type(argname="argument write", value=write, expected_type=type_hints["write"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if abs_working_dir is not None:
             self._values["abs_working_dir"] = abs_working_dir
         if alias is not None:
             self._values["alias"] = alias
         if allow_overwrite is not None:
@@ -705,14 +717,16 @@
             self._values["color"] = color
         if conditions is not None:
             self._values["conditions"] = conditions
         if define is not None:
             self._values["define"] = define
         if drop is not None:
             self._values["drop"] = drop
+        if drop_labels is not None:
+            self._values["drop_labels"] = drop_labels
         if entry_names is not None:
             self._values["entry_names"] = entry_names
         if external is not None:
             self._values["external"] = external
         if footer is not None:
             self._values["footer"] = footer
         if format is not None:
@@ -735,14 +749,16 @@
             self._values["jsx_import_source"] = jsx_import_source
         if jsx_side_effects is not None:
             self._values["jsx_side_effects"] = jsx_side_effects
         if keep_names is not None:
             self._values["keep_names"] = keep_names
         if legal_comments is not None:
             self._values["legal_comments"] = legal_comments
+        if line_limit is not None:
+            self._values["line_limit"] = line_limit
         if loader is not None:
             self._values["loader"] = loader
         if log_level is not None:
             self._values["log_level"] = log_level
         if log_limit is not None:
             self._values["log_limit"] = log_limit
         if log_override is not None:
@@ -801,14 +817,16 @@
             self._values["supported"] = supported
         if target is not None:
             self._values["target"] = target
         if tree_shaking is not None:
             self._values["tree_shaking"] = tree_shaking
         if tsconfig is not None:
             self._values["tsconfig"] = tsconfig
+        if tsconfig_raw is not None:
+            self._values["tsconfig_raw"] = tsconfig_raw
         if write is not None:
             self._values["write"] = write
 
     @builtins.property
     def abs_working_dir(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#working-directory.'''
         result = self._values.get("abs_working_dir")
@@ -877,14 +895,20 @@
     @builtins.property
     def drop(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#drop.'''
         result = self._values.get("drop")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def drop_labels(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Documentation: https://esbuild.github.io/api/#drop-labels.'''
+        result = self._values.get("drop_labels")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def entry_names(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#entry-names.'''
         result = self._values.get("entry_names")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def external(self) -> typing.Optional[typing.List[builtins.str]]:
@@ -967,14 +991,20 @@
     @builtins.property
     def legal_comments(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#legal-comments.'''
         result = self._values.get("legal_comments")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def line_limit(self) -> typing.Optional[jsii.Number]:
+        '''Documentation: https://esbuild.github.io/api/#line-limit.'''
+        result = self._values.get("line_limit")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def loader(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#loader.'''
         result = self._values.get("loader")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def log_level(self) -> typing.Optional[builtins.str]:
@@ -1173,14 +1203,22 @@
     @builtins.property
     def tsconfig(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#tsconfig.'''
         result = self._values.get("tsconfig")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def tsconfig_raw(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, "TsconfigOptions"]]:
+        '''Documentation: https://esbuild.github.io/api/#tsconfig-raw.'''
+        result = self._values.get("tsconfig_raw")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, "TsconfigOptions"]], result)
+
+    @builtins.property
     def write(self) -> typing.Optional[builtins.bool]:
         '''Documentation: https://esbuild.github.io/api/#write.'''
         result = self._values.get("write")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -1379,82 +1417,183 @@
         )
 
 
 @jsii.data_type(
     jsii_type="@mrgrain/cdk-esbuild.CompilerOptions",
     jsii_struct_bases=[],
     name_mapping={
+        "always_strict": "alwaysStrict",
+        "base_url": "baseUrl",
+        "experimental_decorators": "experimentalDecorators",
         "imports_not_used_as_values": "importsNotUsedAsValues",
+        "jsx": "jsx",
         "jsx_factory": "jsxFactory",
         "jsx_fragment_factory": "jsxFragmentFactory",
+        "jsx_import_source": "jsxImportSource",
+        "paths": "paths",
         "preserve_value_imports": "preserveValueImports",
+        "strict": "strict",
+        "target": "target",
         "use_define_for_class_fields": "useDefineForClassFields",
+        "verbatim_module_syntax": "verbatimModuleSyntax",
     },
 )
 class CompilerOptions:
     def __init__(
         self,
         *,
+        always_strict: typing.Optional[builtins.bool] = None,
+        base_url: typing.Optional[builtins.bool] = None,
+        experimental_decorators: typing.Optional[builtins.bool] = None,
         imports_not_used_as_values: typing.Optional[builtins.str] = None,
+        jsx: typing.Optional[builtins.str] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment_factory: typing.Optional[builtins.str] = None,
+        jsx_import_source: typing.Optional[builtins.str] = None,
+        paths: typing.Optional[typing.Mapping[builtins.str, typing.Sequence[builtins.str]]] = None,
         preserve_value_imports: typing.Optional[builtins.bool] = None,
+        strict: typing.Optional[builtins.bool] = None,
+        target: typing.Optional[builtins.str] = None,
         use_define_for_class_fields: typing.Optional[builtins.bool] = None,
+        verbatim_module_syntax: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
+        :param always_strict: 
+        :param base_url: 
+        :param experimental_decorators: 
         :param imports_not_used_as_values: 
+        :param jsx: 
         :param jsx_factory: 
         :param jsx_fragment_factory: 
+        :param jsx_import_source: 
+        :param paths: 
         :param preserve_value_imports: 
+        :param strict: 
+        :param target: 
         :param use_define_for_class_fields: 
+        :param verbatim_module_syntax: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9b682d31bc71983a448565f5ef0a021abb3aeaf127a6dab66c921bef47f98592)
+            check_type(argname="argument always_strict", value=always_strict, expected_type=type_hints["always_strict"])
+            check_type(argname="argument base_url", value=base_url, expected_type=type_hints["base_url"])
+            check_type(argname="argument experimental_decorators", value=experimental_decorators, expected_type=type_hints["experimental_decorators"])
             check_type(argname="argument imports_not_used_as_values", value=imports_not_used_as_values, expected_type=type_hints["imports_not_used_as_values"])
+            check_type(argname="argument jsx", value=jsx, expected_type=type_hints["jsx"])
             check_type(argname="argument jsx_factory", value=jsx_factory, expected_type=type_hints["jsx_factory"])
             check_type(argname="argument jsx_fragment_factory", value=jsx_fragment_factory, expected_type=type_hints["jsx_fragment_factory"])
+            check_type(argname="argument jsx_import_source", value=jsx_import_source, expected_type=type_hints["jsx_import_source"])
+            check_type(argname="argument paths", value=paths, expected_type=type_hints["paths"])
             check_type(argname="argument preserve_value_imports", value=preserve_value_imports, expected_type=type_hints["preserve_value_imports"])
+            check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
+            check_type(argname="argument target", value=target, expected_type=type_hints["target"])
             check_type(argname="argument use_define_for_class_fields", value=use_define_for_class_fields, expected_type=type_hints["use_define_for_class_fields"])
+            check_type(argname="argument verbatim_module_syntax", value=verbatim_module_syntax, expected_type=type_hints["verbatim_module_syntax"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if always_strict is not None:
+            self._values["always_strict"] = always_strict
+        if base_url is not None:
+            self._values["base_url"] = base_url
+        if experimental_decorators is not None:
+            self._values["experimental_decorators"] = experimental_decorators
         if imports_not_used_as_values is not None:
             self._values["imports_not_used_as_values"] = imports_not_used_as_values
+        if jsx is not None:
+            self._values["jsx"] = jsx
         if jsx_factory is not None:
             self._values["jsx_factory"] = jsx_factory
         if jsx_fragment_factory is not None:
             self._values["jsx_fragment_factory"] = jsx_fragment_factory
+        if jsx_import_source is not None:
+            self._values["jsx_import_source"] = jsx_import_source
+        if paths is not None:
+            self._values["paths"] = paths
         if preserve_value_imports is not None:
             self._values["preserve_value_imports"] = preserve_value_imports
+        if strict is not None:
+            self._values["strict"] = strict
+        if target is not None:
+            self._values["target"] = target
         if use_define_for_class_fields is not None:
             self._values["use_define_for_class_fields"] = use_define_for_class_fields
+        if verbatim_module_syntax is not None:
+            self._values["verbatim_module_syntax"] = verbatim_module_syntax
+
+    @builtins.property
+    def always_strict(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("always_strict")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def base_url(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("base_url")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def experimental_decorators(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("experimental_decorators")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def imports_not_used_as_values(self) -> typing.Optional[builtins.str]:
         result = self._values.get("imports_not_used_as_values")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def jsx(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("jsx")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def jsx_factory(self) -> typing.Optional[builtins.str]:
         result = self._values.get("jsx_factory")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def jsx_fragment_factory(self) -> typing.Optional[builtins.str]:
         result = self._values.get("jsx_fragment_factory")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def jsx_import_source(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("jsx_import_source")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def paths(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.List[builtins.str]]]:
+        result = self._values.get("paths")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.List[builtins.str]]], result)
+
+    @builtins.property
     def preserve_value_imports(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("preserve_value_imports")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def strict(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("strict")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def target(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("target")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def use_define_for_class_fields(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("use_define_for_class_fields")
         return typing.cast(typing.Optional[builtins.bool], result)
 
+    @builtins.property
+    def verbatim_module_syntax(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("verbatim_module_syntax")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -1882,14 +2021,15 @@
         bundle: typing.Optional[builtins.bool] = None,
         charset: typing.Optional[builtins.str] = None,
         chunk_names: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         conditions: typing.Optional[typing.Sequence[builtins.str]] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         entry_names: typing.Optional[builtins.str] = None,
         external: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         inject: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -1897,14 +2037,15 @@
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         main_fields: typing.Optional[typing.Sequence[builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
@@ -1930,14 +2071,15 @@
         source_root: typing.Optional[builtins.str] = None,
         sources_content: typing.Optional[builtins.bool] = None,
         splitting: typing.Optional[builtins.bool] = None,
         supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
         target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         tree_shaking: typing.Optional[builtins.bool] = None,
         tsconfig: typing.Optional[builtins.str] = None,
+        tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union["TsconfigOptions", typing.Dict[builtins.str, typing.Any]]]] = None,
         write: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''A method implementing the code build.
 
         During synth time, the method will receive all computed ``BuildOptions`` from the bundler.
 
         It MUST implement any output options to integrate correctly and MAY use any other options.
@@ -1952,14 +2094,15 @@
         :param bundle: Documentation: https://esbuild.github.io/api/#bundle.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param chunk_names: Documentation: https://esbuild.github.io/api/#chunk-names.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param conditions: Documentation: https://esbuild.github.io/api/#conditions.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
         :param entry_names: Documentation: https://esbuild.github.io/api/#entry-names.
         :param external: Documentation: https://esbuild.github.io/api/#external.
         :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param inject: Documentation: https://esbuild.github.io/api/#inject.
@@ -1967,14 +2110,15 @@
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
         :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param main_fields: Documentation: https://esbuild.github.io/api/#main-fields.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
@@ -2000,14 +2144,15 @@
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param splitting: Documentation: https://esbuild.github.io/api/#splitting.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
         :param tsconfig: Documentation: https://esbuild.github.io/api/#tsconfig.
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         :param write: Documentation: https://esbuild.github.io/api/#write.
 
         :throws: ``esbuild.BuildFailure``
         '''
         ...
 
 
@@ -2029,14 +2174,15 @@
         bundle: typing.Optional[builtins.bool] = None,
         charset: typing.Optional[builtins.str] = None,
         chunk_names: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         conditions: typing.Optional[typing.Sequence[builtins.str]] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         entry_names: typing.Optional[builtins.str] = None,
         external: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         inject: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -2044,14 +2190,15 @@
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         main_fields: typing.Optional[typing.Sequence[builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
@@ -2077,14 +2224,15 @@
         source_root: typing.Optional[builtins.str] = None,
         sources_content: typing.Optional[builtins.bool] = None,
         splitting: typing.Optional[builtins.bool] = None,
         supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
         target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         tree_shaking: typing.Optional[builtins.bool] = None,
         tsconfig: typing.Optional[builtins.str] = None,
+        tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union["TsconfigOptions", typing.Dict[builtins.str, typing.Any]]]] = None,
         write: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''A method implementing the code build.
 
         During synth time, the method will receive all computed ``BuildOptions`` from the bundler.
 
         It MUST implement any output options to integrate correctly and MAY use any other options.
@@ -2099,14 +2247,15 @@
         :param bundle: Documentation: https://esbuild.github.io/api/#bundle.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param chunk_names: Documentation: https://esbuild.github.io/api/#chunk-names.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param conditions: Documentation: https://esbuild.github.io/api/#conditions.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
         :param entry_names: Documentation: https://esbuild.github.io/api/#entry-names.
         :param external: Documentation: https://esbuild.github.io/api/#external.
         :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param inject: Documentation: https://esbuild.github.io/api/#inject.
@@ -2114,14 +2263,15 @@
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
         :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param main_fields: Documentation: https://esbuild.github.io/api/#main-fields.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
@@ -2147,14 +2297,15 @@
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param splitting: Documentation: https://esbuild.github.io/api/#splitting.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
         :param tsconfig: Documentation: https://esbuild.github.io/api/#tsconfig.
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         :param write: Documentation: https://esbuild.github.io/api/#write.
 
         :throws: ``esbuild.BuildFailure``
         '''
         options = ProviderBuildOptions(
             entry_points=entry_points,
             abs_working_dir=abs_working_dir,
@@ -2165,14 +2316,15 @@
             bundle=bundle,
             charset=charset,
             chunk_names=chunk_names,
             color=color,
             conditions=conditions,
             define=define,
             drop=drop,
+            drop_labels=drop_labels,
             entry_names=entry_names,
             external=external,
             footer=footer,
             format=format,
             global_name=global_name,
             ignore_annotations=ignore_annotations,
             inject=inject,
@@ -2180,14 +2332,15 @@
             jsx_dev=jsx_dev,
             jsx_factory=jsx_factory,
             jsx_fragment=jsx_fragment,
             jsx_import_source=jsx_import_source,
             jsx_side_effects=jsx_side_effects,
             keep_names=keep_names,
             legal_comments=legal_comments,
+            line_limit=line_limit,
             loader=loader,
             log_level=log_level,
             log_limit=log_limit,
             log_override=log_override,
             main_fields=main_fields,
             mangle_cache=mangle_cache,
             mangle_props=mangle_props,
@@ -2213,14 +2366,15 @@
             source_root=source_root,
             sources_content=sources_content,
             splitting=splitting,
             supported=supported,
             target=target,
             tree_shaking=tree_shaking,
             tsconfig=tsconfig,
+            tsconfig_raw=tsconfig_raw,
             write=write,
         )
 
         return typing.cast(None, jsii.invoke(self, "buildSync", [options]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IBuildProvider).__jsii_proxy_class__ = lambda : _IBuildProviderProxy
@@ -2236,26 +2390,28 @@
         input: builtins.str,
         *,
         banner: typing.Optional[builtins.str] = None,
         charset: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[builtins.str] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         jsx: typing.Optional[builtins.str] = None,
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[builtins.str] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
         mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -2280,53 +2436,55 @@
         During synth time, the method will receive the inline code and all computed ``TransformOptions`` from the bundler.
 
         MUST return the transformed code as a string to integrate correctly.
         It MAY use these options to do so.
         On failure, it SHOULD print any warnings & errors to stderr and throw a ``TransformFailure`` to inform the bundler.
 
         :param input: -
-        :param banner: 
+        :param banner: Documentation: https://esbuild.github.io/api/#banner.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
-        :param footer: 
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
+        :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param jsx: Documentation: https://esbuild.github.io/api/#jsx.
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
-        :param loader: 
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
+        :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_quoted: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param minify: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_identifiers: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_syntax: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_whitespace: Documentation: https://esbuild.github.io/api/#minify.
         :param platform: Documentation: https://esbuild.github.io/api/#platform.
         :param pure: Documentation: https://esbuild.github.io/api/#pure.
         :param reserve_props: Documentation: https://esbuild.github.io/api/#mangle-props.
-        :param sourcefile: 
+        :param sourcefile: Documentation: https://esbuild.github.io/api/#sourcefile.
         :param sourcemap: Documentation: https://esbuild.github.io/api/#sourcemap.
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
-        :param tsconfig_raw: 
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
 
         :throws: ``esbuild.TransformFailure``
         '''
         ...
 
 
 class _ITransformProviderProxy:
@@ -2340,26 +2498,28 @@
         input: builtins.str,
         *,
         banner: typing.Optional[builtins.str] = None,
         charset: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[builtins.str] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         jsx: typing.Optional[builtins.str] = None,
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[builtins.str] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
         mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -2384,77 +2544,81 @@
         During synth time, the method will receive the inline code and all computed ``TransformOptions`` from the bundler.
 
         MUST return the transformed code as a string to integrate correctly.
         It MAY use these options to do so.
         On failure, it SHOULD print any warnings & errors to stderr and throw a ``TransformFailure`` to inform the bundler.
 
         :param input: -
-        :param banner: 
+        :param banner: Documentation: https://esbuild.github.io/api/#banner.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
-        :param footer: 
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
+        :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param jsx: Documentation: https://esbuild.github.io/api/#jsx.
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
-        :param loader: 
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
+        :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_quoted: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param minify: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_identifiers: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_syntax: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_whitespace: Documentation: https://esbuild.github.io/api/#minify.
         :param platform: Documentation: https://esbuild.github.io/api/#platform.
         :param pure: Documentation: https://esbuild.github.io/api/#pure.
         :param reserve_props: Documentation: https://esbuild.github.io/api/#mangle-props.
-        :param sourcefile: 
+        :param sourcefile: Documentation: https://esbuild.github.io/api/#sourcefile.
         :param sourcemap: Documentation: https://esbuild.github.io/api/#sourcemap.
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
-        :param tsconfig_raw: 
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
 
         :throws: ``esbuild.TransformFailure``
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b273d64922e32225c024bddb7c08e70f30648e2537ff966572dee3fd5267a11d)
             check_type(argname="argument input", value=input, expected_type=type_hints["input"])
         options = ProviderTransformOptions(
             banner=banner,
             charset=charset,
             color=color,
             define=define,
             drop=drop,
+            drop_labels=drop_labels,
             footer=footer,
             format=format,
             global_name=global_name,
             ignore_annotations=ignore_annotations,
             jsx=jsx,
             jsx_dev=jsx_dev,
             jsx_factory=jsx_factory,
             jsx_fragment=jsx_fragment,
             jsx_import_source=jsx_import_source,
             jsx_side_effects=jsx_side_effects,
             keep_names=keep_names,
             legal_comments=legal_comments,
+            line_limit=line_limit,
             loader=loader,
             log_level=log_level,
             log_limit=log_limit,
             log_override=log_override,
             mangle_cache=mangle_cache,
             mangle_props=mangle_props,
             mangle_quoted=mangle_quoted,
@@ -3019,14 +3183,15 @@
         "bundle": "bundle",
         "charset": "charset",
         "chunk_names": "chunkNames",
         "color": "color",
         "conditions": "conditions",
         "define": "define",
         "drop": "drop",
+        "drop_labels": "dropLabels",
         "entry_names": "entryNames",
         "external": "external",
         "footer": "footer",
         "format": "format",
         "global_name": "globalName",
         "ignore_annotations": "ignoreAnnotations",
         "inject": "inject",
@@ -3034,14 +3199,15 @@
         "jsx_dev": "jsxDev",
         "jsx_factory": "jsxFactory",
         "jsx_fragment": "jsxFragment",
         "jsx_import_source": "jsxImportSource",
         "jsx_side_effects": "jsxSideEffects",
         "keep_names": "keepNames",
         "legal_comments": "legalComments",
+        "line_limit": "lineLimit",
         "loader": "loader",
         "log_level": "logLevel",
         "log_limit": "logLimit",
         "log_override": "logOverride",
         "main_fields": "mainFields",
         "mangle_cache": "mangleCache",
         "mangle_props": "mangleProps",
@@ -3067,14 +3233,15 @@
         "source_root": "sourceRoot",
         "sources_content": "sourcesContent",
         "splitting": "splitting",
         "supported": "supported",
         "target": "target",
         "tree_shaking": "treeShaking",
         "tsconfig": "tsconfig",
+        "tsconfig_raw": "tsconfigRaw",
         "write": "write",
         "entry_points": "entryPoints",
     },
 )
 class ProviderBuildOptions(BuildOptions):
     def __init__(
         self,
@@ -3087,14 +3254,15 @@
         bundle: typing.Optional[builtins.bool] = None,
         charset: typing.Optional[builtins.str] = None,
         chunk_names: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         conditions: typing.Optional[typing.Sequence[builtins.str]] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         entry_names: typing.Optional[builtins.str] = None,
         external: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         inject: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -3102,14 +3270,15 @@
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         main_fields: typing.Optional[typing.Sequence[builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
@@ -3135,14 +3304,15 @@
         source_root: typing.Optional[builtins.str] = None,
         sources_content: typing.Optional[builtins.bool] = None,
         splitting: typing.Optional[builtins.bool] = None,
         supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
         target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         tree_shaking: typing.Optional[builtins.bool] = None,
         tsconfig: typing.Optional[builtins.str] = None,
+        tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union["TsconfigOptions", typing.Dict[builtins.str, typing.Any]]]] = None,
         write: typing.Optional[builtins.bool] = None,
         entry_points: typing.Optional[typing.Union[typing.Sequence[builtins.str], typing.Mapping[builtins.str, builtins.str]]] = None,
     ) -> None:
         '''
         :param abs_working_dir: Documentation: https://esbuild.github.io/api/#working-directory.
         :param alias: Documentation: https://esbuild.github.io/api/#alias.
         :param allow_overwrite: Documentation: https://esbuild.github.io/api/#allow-overwrite.
@@ -3151,14 +3321,15 @@
         :param bundle: Documentation: https://esbuild.github.io/api/#bundle.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param chunk_names: Documentation: https://esbuild.github.io/api/#chunk-names.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param conditions: Documentation: https://esbuild.github.io/api/#conditions.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
         :param entry_names: Documentation: https://esbuild.github.io/api/#entry-names.
         :param external: Documentation: https://esbuild.github.io/api/#external.
         :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param inject: Documentation: https://esbuild.github.io/api/#inject.
@@ -3166,14 +3337,15 @@
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
         :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param main_fields: Documentation: https://esbuild.github.io/api/#main-fields.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
@@ -3199,14 +3371,15 @@
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param splitting: Documentation: https://esbuild.github.io/api/#splitting.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
         :param tsconfig: Documentation: https://esbuild.github.io/api/#tsconfig.
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         :param write: Documentation: https://esbuild.github.io/api/#write.
         :param entry_points: Documentation: https://esbuild.github.io/api/#entry-points.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b78e7efccee59986fec35d76ced509c566ac34900b09d44551f2407cbf1cff4b)
             check_type(argname="argument abs_working_dir", value=abs_working_dir, expected_type=type_hints["abs_working_dir"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
@@ -3216,14 +3389,15 @@
             check_type(argname="argument bundle", value=bundle, expected_type=type_hints["bundle"])
             check_type(argname="argument charset", value=charset, expected_type=type_hints["charset"])
             check_type(argname="argument chunk_names", value=chunk_names, expected_type=type_hints["chunk_names"])
             check_type(argname="argument color", value=color, expected_type=type_hints["color"])
             check_type(argname="argument conditions", value=conditions, expected_type=type_hints["conditions"])
             check_type(argname="argument define", value=define, expected_type=type_hints["define"])
             check_type(argname="argument drop", value=drop, expected_type=type_hints["drop"])
+            check_type(argname="argument drop_labels", value=drop_labels, expected_type=type_hints["drop_labels"])
             check_type(argname="argument entry_names", value=entry_names, expected_type=type_hints["entry_names"])
             check_type(argname="argument external", value=external, expected_type=type_hints["external"])
             check_type(argname="argument footer", value=footer, expected_type=type_hints["footer"])
             check_type(argname="argument format", value=format, expected_type=type_hints["format"])
             check_type(argname="argument global_name", value=global_name, expected_type=type_hints["global_name"])
             check_type(argname="argument ignore_annotations", value=ignore_annotations, expected_type=type_hints["ignore_annotations"])
             check_type(argname="argument inject", value=inject, expected_type=type_hints["inject"])
@@ -3231,14 +3405,15 @@
             check_type(argname="argument jsx_dev", value=jsx_dev, expected_type=type_hints["jsx_dev"])
             check_type(argname="argument jsx_factory", value=jsx_factory, expected_type=type_hints["jsx_factory"])
             check_type(argname="argument jsx_fragment", value=jsx_fragment, expected_type=type_hints["jsx_fragment"])
             check_type(argname="argument jsx_import_source", value=jsx_import_source, expected_type=type_hints["jsx_import_source"])
             check_type(argname="argument jsx_side_effects", value=jsx_side_effects, expected_type=type_hints["jsx_side_effects"])
             check_type(argname="argument keep_names", value=keep_names, expected_type=type_hints["keep_names"])
             check_type(argname="argument legal_comments", value=legal_comments, expected_type=type_hints["legal_comments"])
+            check_type(argname="argument line_limit", value=line_limit, expected_type=type_hints["line_limit"])
             check_type(argname="argument loader", value=loader, expected_type=type_hints["loader"])
             check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
             check_type(argname="argument log_limit", value=log_limit, expected_type=type_hints["log_limit"])
             check_type(argname="argument log_override", value=log_override, expected_type=type_hints["log_override"])
             check_type(argname="argument main_fields", value=main_fields, expected_type=type_hints["main_fields"])
             check_type(argname="argument mangle_cache", value=mangle_cache, expected_type=type_hints["mangle_cache"])
             check_type(argname="argument mangle_props", value=mangle_props, expected_type=type_hints["mangle_props"])
@@ -3264,14 +3439,15 @@
             check_type(argname="argument source_root", value=source_root, expected_type=type_hints["source_root"])
             check_type(argname="argument sources_content", value=sources_content, expected_type=type_hints["sources_content"])
             check_type(argname="argument splitting", value=splitting, expected_type=type_hints["splitting"])
             check_type(argname="argument supported", value=supported, expected_type=type_hints["supported"])
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
             check_type(argname="argument tree_shaking", value=tree_shaking, expected_type=type_hints["tree_shaking"])
             check_type(argname="argument tsconfig", value=tsconfig, expected_type=type_hints["tsconfig"])
+            check_type(argname="argument tsconfig_raw", value=tsconfig_raw, expected_type=type_hints["tsconfig_raw"])
             check_type(argname="argument write", value=write, expected_type=type_hints["write"])
             check_type(argname="argument entry_points", value=entry_points, expected_type=type_hints["entry_points"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if abs_working_dir is not None:
             self._values["abs_working_dir"] = abs_working_dir
         if alias is not None:
             self._values["alias"] = alias
@@ -3291,14 +3467,16 @@
             self._values["color"] = color
         if conditions is not None:
             self._values["conditions"] = conditions
         if define is not None:
             self._values["define"] = define
         if drop is not None:
             self._values["drop"] = drop
+        if drop_labels is not None:
+            self._values["drop_labels"] = drop_labels
         if entry_names is not None:
             self._values["entry_names"] = entry_names
         if external is not None:
             self._values["external"] = external
         if footer is not None:
             self._values["footer"] = footer
         if format is not None:
@@ -3321,14 +3499,16 @@
             self._values["jsx_import_source"] = jsx_import_source
         if jsx_side_effects is not None:
             self._values["jsx_side_effects"] = jsx_side_effects
         if keep_names is not None:
             self._values["keep_names"] = keep_names
         if legal_comments is not None:
             self._values["legal_comments"] = legal_comments
+        if line_limit is not None:
+            self._values["line_limit"] = line_limit
         if loader is not None:
             self._values["loader"] = loader
         if log_level is not None:
             self._values["log_level"] = log_level
         if log_limit is not None:
             self._values["log_limit"] = log_limit
         if log_override is not None:
@@ -3387,14 +3567,16 @@
             self._values["supported"] = supported
         if target is not None:
             self._values["target"] = target
         if tree_shaking is not None:
             self._values["tree_shaking"] = tree_shaking
         if tsconfig is not None:
             self._values["tsconfig"] = tsconfig
+        if tsconfig_raw is not None:
+            self._values["tsconfig_raw"] = tsconfig_raw
         if write is not None:
             self._values["write"] = write
         if entry_points is not None:
             self._values["entry_points"] = entry_points
 
     @builtins.property
     def abs_working_dir(self) -> typing.Optional[builtins.str]:
@@ -3465,14 +3647,20 @@
     @builtins.property
     def drop(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#drop.'''
         result = self._values.get("drop")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def drop_labels(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Documentation: https://esbuild.github.io/api/#drop-labels.'''
+        result = self._values.get("drop_labels")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def entry_names(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#entry-names.'''
         result = self._values.get("entry_names")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def external(self) -> typing.Optional[typing.List[builtins.str]]:
@@ -3555,14 +3743,20 @@
     @builtins.property
     def legal_comments(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#legal-comments.'''
         result = self._values.get("legal_comments")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def line_limit(self) -> typing.Optional[jsii.Number]:
+        '''Documentation: https://esbuild.github.io/api/#line-limit.'''
+        result = self._values.get("line_limit")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def loader(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#loader.'''
         result = self._values.get("loader")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def log_level(self) -> typing.Optional[builtins.str]:
@@ -3761,14 +3955,22 @@
     @builtins.property
     def tsconfig(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#tsconfig.'''
         result = self._values.get("tsconfig")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def tsconfig_raw(
+        self,
+    ) -> typing.Optional[typing.Union[builtins.str, "TsconfigOptions"]]:
+        '''Documentation: https://esbuild.github.io/api/#tsconfig-raw.'''
+        result = self._values.get("tsconfig_raw")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, "TsconfigOptions"]], result)
+
+    @builtins.property
     def write(self) -> typing.Optional[builtins.bool]:
         '''Documentation: https://esbuild.github.io/api/#write.'''
         result = self._values.get("write")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def entry_points(
@@ -3795,26 +3997,28 @@
     jsii_struct_bases=[],
     name_mapping={
         "banner": "banner",
         "charset": "charset",
         "color": "color",
         "define": "define",
         "drop": "drop",
+        "drop_labels": "dropLabels",
         "footer": "footer",
         "format": "format",
         "global_name": "globalName",
         "ignore_annotations": "ignoreAnnotations",
         "jsx": "jsx",
         "jsx_dev": "jsxDev",
         "jsx_factory": "jsxFactory",
         "jsx_fragment": "jsxFragment",
         "jsx_import_source": "jsxImportSource",
         "jsx_side_effects": "jsxSideEffects",
         "keep_names": "keepNames",
         "legal_comments": "legalComments",
+        "line_limit": "lineLimit",
         "loader": "loader",
         "log_level": "logLevel",
         "log_limit": "logLimit",
         "log_override": "logOverride",
         "mangle_cache": "mangleCache",
         "mangle_props": "mangleProps",
         "mangle_quoted": "mangleQuoted",
@@ -3840,26 +4044,28 @@
         self,
         *,
         banner: typing.Optional[builtins.str] = None,
         charset: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[builtins.str] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         jsx: typing.Optional[builtins.str] = None,
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[builtins.str] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
         mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -3876,73 +4082,77 @@
         sources_content: typing.Optional[builtins.bool] = None,
         supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
         target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         tree_shaking: typing.Optional[builtins.bool] = None,
         tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union["TsconfigOptions", typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
-        :param banner: 
+        :param banner: Documentation: https://esbuild.github.io/api/#banner.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
-        :param footer: 
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
+        :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param jsx: Documentation: https://esbuild.github.io/api/#jsx.
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
-        :param loader: 
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
+        :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_quoted: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param minify: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_identifiers: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_syntax: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_whitespace: Documentation: https://esbuild.github.io/api/#minify.
         :param platform: Documentation: https://esbuild.github.io/api/#platform.
         :param pure: Documentation: https://esbuild.github.io/api/#pure.
         :param reserve_props: Documentation: https://esbuild.github.io/api/#mangle-props.
-        :param sourcefile: 
+        :param sourcefile: Documentation: https://esbuild.github.io/api/#sourcefile.
         :param sourcemap: Documentation: https://esbuild.github.io/api/#sourcemap.
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
-        :param tsconfig_raw: 
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6c37248db4a858f2f46ff70ce7ec32f72b189492c09c9e26fc3552cb219fbd47)
             check_type(argname="argument banner", value=banner, expected_type=type_hints["banner"])
             check_type(argname="argument charset", value=charset, expected_type=type_hints["charset"])
             check_type(argname="argument color", value=color, expected_type=type_hints["color"])
             check_type(argname="argument define", value=define, expected_type=type_hints["define"])
             check_type(argname="argument drop", value=drop, expected_type=type_hints["drop"])
+            check_type(argname="argument drop_labels", value=drop_labels, expected_type=type_hints["drop_labels"])
             check_type(argname="argument footer", value=footer, expected_type=type_hints["footer"])
             check_type(argname="argument format", value=format, expected_type=type_hints["format"])
             check_type(argname="argument global_name", value=global_name, expected_type=type_hints["global_name"])
             check_type(argname="argument ignore_annotations", value=ignore_annotations, expected_type=type_hints["ignore_annotations"])
             check_type(argname="argument jsx", value=jsx, expected_type=type_hints["jsx"])
             check_type(argname="argument jsx_dev", value=jsx_dev, expected_type=type_hints["jsx_dev"])
             check_type(argname="argument jsx_factory", value=jsx_factory, expected_type=type_hints["jsx_factory"])
             check_type(argname="argument jsx_fragment", value=jsx_fragment, expected_type=type_hints["jsx_fragment"])
             check_type(argname="argument jsx_import_source", value=jsx_import_source, expected_type=type_hints["jsx_import_source"])
             check_type(argname="argument jsx_side_effects", value=jsx_side_effects, expected_type=type_hints["jsx_side_effects"])
             check_type(argname="argument keep_names", value=keep_names, expected_type=type_hints["keep_names"])
             check_type(argname="argument legal_comments", value=legal_comments, expected_type=type_hints["legal_comments"])
+            check_type(argname="argument line_limit", value=line_limit, expected_type=type_hints["line_limit"])
             check_type(argname="argument loader", value=loader, expected_type=type_hints["loader"])
             check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
             check_type(argname="argument log_limit", value=log_limit, expected_type=type_hints["log_limit"])
             check_type(argname="argument log_override", value=log_override, expected_type=type_hints["log_override"])
             check_type(argname="argument mangle_cache", value=mangle_cache, expected_type=type_hints["mangle_cache"])
             check_type(argname="argument mangle_props", value=mangle_props, expected_type=type_hints["mangle_props"])
             check_type(argname="argument mangle_quoted", value=mangle_quoted, expected_type=type_hints["mangle_quoted"])
@@ -3968,14 +4178,16 @@
             self._values["charset"] = charset
         if color is not None:
             self._values["color"] = color
         if define is not None:
             self._values["define"] = define
         if drop is not None:
             self._values["drop"] = drop
+        if drop_labels is not None:
+            self._values["drop_labels"] = drop_labels
         if footer is not None:
             self._values["footer"] = footer
         if format is not None:
             self._values["format"] = format
         if global_name is not None:
             self._values["global_name"] = global_name
         if ignore_annotations is not None:
@@ -3992,14 +4204,16 @@
             self._values["jsx_import_source"] = jsx_import_source
         if jsx_side_effects is not None:
             self._values["jsx_side_effects"] = jsx_side_effects
         if keep_names is not None:
             self._values["keep_names"] = keep_names
         if legal_comments is not None:
             self._values["legal_comments"] = legal_comments
+        if line_limit is not None:
+            self._values["line_limit"] = line_limit
         if loader is not None:
             self._values["loader"] = loader
         if log_level is not None:
             self._values["log_level"] = log_level
         if log_limit is not None:
             self._values["log_limit"] = log_limit
         if log_override is not None:
@@ -4039,14 +4253,15 @@
         if tree_shaking is not None:
             self._values["tree_shaking"] = tree_shaking
         if tsconfig_raw is not None:
             self._values["tsconfig_raw"] = tsconfig_raw
 
     @builtins.property
     def banner(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#banner.'''
         result = self._values.get("banner")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def charset(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#charset.'''
         result = self._values.get("charset")
@@ -4067,15 +4282,22 @@
     @builtins.property
     def drop(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#drop.'''
         result = self._values.get("drop")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def drop_labels(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Documentation: https://esbuild.github.io/api/#drop-labels.'''
+        result = self._values.get("drop_labels")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def footer(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#footer.'''
         result = self._values.get("footer")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def format(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#format.'''
         result = self._values.get("format")
@@ -4138,15 +4360,22 @@
     @builtins.property
     def legal_comments(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#legal-comments.'''
         result = self._values.get("legal_comments")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def line_limit(self) -> typing.Optional[jsii.Number]:
+        '''Documentation: https://esbuild.github.io/api/#line-limit.'''
+        result = self._values.get("line_limit")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def loader(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#loader.'''
         result = self._values.get("loader")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def log_level(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#log-level.'''
         result = self._values.get("log_level")
@@ -4226,14 +4455,15 @@
     def reserve_props(self) -> typing.Any:
         '''Documentation: https://esbuild.github.io/api/#mangle-props.'''
         result = self._values.get("reserve_props")
         return typing.cast(typing.Any, result)
 
     @builtins.property
     def sourcefile(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#sourcefile.'''
         result = self._values.get("sourcefile")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sourcemap(self) -> typing.Optional[typing.Union[builtins.bool, builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#sourcemap.'''
         result = self._values.get("sourcemap")
@@ -4271,14 +4501,15 @@
         result = self._values.get("tree_shaking")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def tsconfig_raw(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, "TsconfigOptions"]]:
+        '''Documentation: https://esbuild.github.io/api/#tsconfig-raw.'''
         result = self._values.get("tsconfig_raw")
         return typing.cast(typing.Optional[typing.Union[builtins.str, "TsconfigOptions"]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -5063,14 +5294,15 @@
         bundle: typing.Optional[builtins.bool] = None,
         charset: typing.Optional[builtins.str] = None,
         chunk_names: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         conditions: typing.Optional[typing.Sequence[builtins.str]] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         entry_names: typing.Optional[builtins.str] = None,
         external: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         inject: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -5078,14 +5310,15 @@
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         main_fields: typing.Optional[typing.Sequence[builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
@@ -5111,14 +5344,15 @@
         source_root: typing.Optional[builtins.str] = None,
         sources_content: typing.Optional[builtins.bool] = None,
         splitting: typing.Optional[builtins.bool] = None,
         supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
         target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         tree_shaking: typing.Optional[builtins.bool] = None,
         tsconfig: typing.Optional[builtins.str] = None,
+        tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union[TsconfigOptions, typing.Dict[builtins.str, typing.Any]]]] = None,
         write: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''A method implementing the code build.
 
         During synth time, the method will receive all computed ``BuildOptions`` from the bundler.
 
         It MUST implement any output options to integrate correctly and MAY use any other options.
@@ -5133,14 +5367,15 @@
         :param bundle: Documentation: https://esbuild.github.io/api/#bundle.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param chunk_names: Documentation: https://esbuild.github.io/api/#chunk-names.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param conditions: Documentation: https://esbuild.github.io/api/#conditions.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
         :param entry_names: Documentation: https://esbuild.github.io/api/#entry-names.
         :param external: Documentation: https://esbuild.github.io/api/#external.
         :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param inject: Documentation: https://esbuild.github.io/api/#inject.
@@ -5148,14 +5383,15 @@
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
         :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param main_fields: Documentation: https://esbuild.github.io/api/#main-fields.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
@@ -5181,14 +5417,15 @@
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param splitting: Documentation: https://esbuild.github.io/api/#splitting.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
         :param tsconfig: Documentation: https://esbuild.github.io/api/#tsconfig.
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         :param write: Documentation: https://esbuild.github.io/api/#write.
         '''
         options = ProviderBuildOptions(
             entry_points=entry_points,
             abs_working_dir=abs_working_dir,
             alias=alias,
             allow_overwrite=allow_overwrite,
@@ -5197,14 +5434,15 @@
             bundle=bundle,
             charset=charset,
             chunk_names=chunk_names,
             color=color,
             conditions=conditions,
             define=define,
             drop=drop,
+            drop_labels=drop_labels,
             entry_names=entry_names,
             external=external,
             footer=footer,
             format=format,
             global_name=global_name,
             ignore_annotations=ignore_annotations,
             inject=inject,
@@ -5212,14 +5450,15 @@
             jsx_dev=jsx_dev,
             jsx_factory=jsx_factory,
             jsx_fragment=jsx_fragment,
             jsx_import_source=jsx_import_source,
             jsx_side_effects=jsx_side_effects,
             keep_names=keep_names,
             legal_comments=legal_comments,
+            line_limit=line_limit,
             loader=loader,
             log_level=log_level,
             log_limit=log_limit,
             log_override=log_override,
             main_fields=main_fields,
             mangle_cache=mangle_cache,
             mangle_props=mangle_props,
@@ -5245,14 +5484,15 @@
             source_root=source_root,
             sources_content=sources_content,
             splitting=splitting,
             supported=supported,
             target=target,
             tree_shaking=tree_shaking,
             tsconfig=tsconfig,
+            tsconfig_raw=tsconfig_raw,
             write=write,
         )
 
         return typing.cast(None, jsii.invoke(self, "buildSync", [options]))
 
     @jsii.member(jsii_name="transformSync")
     def transform_sync(
@@ -5260,26 +5500,28 @@
         input: builtins.str,
         *,
         banner: typing.Optional[builtins.str] = None,
         charset: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[builtins.str] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         jsx: typing.Optional[builtins.str] = None,
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[builtins.str] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
         mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -5304,75 +5546,79 @@
         During synth time, the method will receive the inline code and all computed ``TransformOptions`` from the bundler.
 
         MUST return the transformed code as a string to integrate correctly.
         It MAY use these options to do so.
         On failure, it SHOULD print any warnings & errors to stderr and throw a ``TransformFailure`` to inform the bundler.
 
         :param input: -
-        :param banner: 
+        :param banner: Documentation: https://esbuild.github.io/api/#banner.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
-        :param footer: 
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
+        :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param jsx: Documentation: https://esbuild.github.io/api/#jsx.
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
-        :param loader: 
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
+        :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_quoted: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param minify: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_identifiers: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_syntax: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_whitespace: Documentation: https://esbuild.github.io/api/#minify.
         :param platform: Documentation: https://esbuild.github.io/api/#platform.
         :param pure: Documentation: https://esbuild.github.io/api/#pure.
         :param reserve_props: Documentation: https://esbuild.github.io/api/#mangle-props.
-        :param sourcefile: 
+        :param sourcefile: Documentation: https://esbuild.github.io/api/#sourcefile.
         :param sourcemap: Documentation: https://esbuild.github.io/api/#sourcemap.
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
-        :param tsconfig_raw: 
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4518845e9c0cd47623e425def75422413186f9fae8d2e5056f61f917f5d888e4)
             check_type(argname="argument input", value=input, expected_type=type_hints["input"])
         options = ProviderTransformOptions(
             banner=banner,
             charset=charset,
             color=color,
             define=define,
             drop=drop,
+            drop_labels=drop_labels,
             footer=footer,
             format=format,
             global_name=global_name,
             ignore_annotations=ignore_annotations,
             jsx=jsx,
             jsx_dev=jsx_dev,
             jsx_factory=jsx_factory,
             jsx_fragment=jsx_fragment,
             jsx_import_source=jsx_import_source,
             jsx_side_effects=jsx_side_effects,
             keep_names=keep_names,
             legal_comments=legal_comments,
+            line_limit=line_limit,
             loader=loader,
             log_level=log_level,
             log_limit=log_limit,
             log_override=log_override,
             mangle_cache=mangle_cache,
             mangle_props=mangle_props,
             mangle_quoted=mangle_quoted,
@@ -5421,26 +5667,28 @@
     jsii_struct_bases=[TransformOptions],
     name_mapping={
         "banner": "banner",
         "charset": "charset",
         "color": "color",
         "define": "define",
         "drop": "drop",
+        "drop_labels": "dropLabels",
         "footer": "footer",
         "format": "format",
         "global_name": "globalName",
         "ignore_annotations": "ignoreAnnotations",
         "jsx": "jsx",
         "jsx_dev": "jsxDev",
         "jsx_factory": "jsxFactory",
         "jsx_fragment": "jsxFragment",
         "jsx_import_source": "jsxImportSource",
         "jsx_side_effects": "jsxSideEffects",
         "keep_names": "keepNames",
         "legal_comments": "legalComments",
+        "line_limit": "lineLimit",
         "loader": "loader",
         "log_level": "logLevel",
         "log_limit": "logLimit",
         "log_override": "logOverride",
         "mangle_cache": "mangleCache",
         "mangle_props": "mangleProps",
         "mangle_quoted": "mangleQuoted",
@@ -5466,26 +5714,28 @@
         self,
         *,
         banner: typing.Optional[builtins.str] = None,
         charset: typing.Optional[builtins.str] = None,
         color: typing.Optional[builtins.bool] = None,
         define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+        drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
         footer: typing.Optional[builtins.str] = None,
         format: typing.Optional[builtins.str] = None,
         global_name: typing.Optional[builtins.str] = None,
         ignore_annotations: typing.Optional[builtins.bool] = None,
         jsx: typing.Optional[builtins.str] = None,
         jsx_dev: typing.Optional[builtins.bool] = None,
         jsx_factory: typing.Optional[builtins.str] = None,
         jsx_fragment: typing.Optional[builtins.str] = None,
         jsx_import_source: typing.Optional[builtins.str] = None,
         jsx_side_effects: typing.Optional[builtins.bool] = None,
         keep_names: typing.Optional[builtins.bool] = None,
         legal_comments: typing.Optional[builtins.str] = None,
+        line_limit: typing.Optional[jsii.Number] = None,
         loader: typing.Optional[builtins.str] = None,
         log_level: typing.Optional[builtins.str] = None,
         log_limit: typing.Optional[jsii.Number] = None,
         log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
         mangle_props: typing.Any = None,
         mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -5502,73 +5752,77 @@
         sources_content: typing.Optional[builtins.bool] = None,
         supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
         target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
         tree_shaking: typing.Optional[builtins.bool] = None,
         tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union[TsconfigOptions, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
-        :param banner: 
+        :param banner: Documentation: https://esbuild.github.io/api/#banner.
         :param charset: Documentation: https://esbuild.github.io/api/#charset.
         :param color: Documentation: https://esbuild.github.io/api/#color.
         :param define: Documentation: https://esbuild.github.io/api/#define.
         :param drop: Documentation: https://esbuild.github.io/api/#drop.
-        :param footer: 
+        :param drop_labels: Documentation: https://esbuild.github.io/api/#drop-labels.
+        :param footer: Documentation: https://esbuild.github.io/api/#footer.
         :param format: Documentation: https://esbuild.github.io/api/#format.
         :param global_name: Documentation: https://esbuild.github.io/api/#global-name.
         :param ignore_annotations: Documentation: https://esbuild.github.io/api/#ignore-annotations.
         :param jsx: Documentation: https://esbuild.github.io/api/#jsx.
         :param jsx_dev: Documentation: https://esbuild.github.io/api/#jsx-development.
         :param jsx_factory: Documentation: https://esbuild.github.io/api/#jsx-factory.
         :param jsx_fragment: Documentation: https://esbuild.github.io/api/#jsx-fragment.
         :param jsx_import_source: Documentation: https://esbuild.github.io/api/#jsx-import-source.
         :param jsx_side_effects: Documentation: https://esbuild.github.io/api/#jsx-side-effects.
         :param keep_names: Documentation: https://esbuild.github.io/api/#keep-names.
         :param legal_comments: Documentation: https://esbuild.github.io/api/#legal-comments.
-        :param loader: 
+        :param line_limit: Documentation: https://esbuild.github.io/api/#line-limit.
+        :param loader: Documentation: https://esbuild.github.io/api/#loader.
         :param log_level: Documentation: https://esbuild.github.io/api/#log-level.
         :param log_limit: Documentation: https://esbuild.github.io/api/#log-limit.
         :param log_override: Documentation: https://esbuild.github.io/api/#log-override.
         :param mangle_cache: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_props: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param mangle_quoted: Documentation: https://esbuild.github.io/api/#mangle-props.
         :param minify: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_identifiers: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_syntax: Documentation: https://esbuild.github.io/api/#minify.
         :param minify_whitespace: Documentation: https://esbuild.github.io/api/#minify.
         :param platform: Documentation: https://esbuild.github.io/api/#platform.
         :param pure: Documentation: https://esbuild.github.io/api/#pure.
         :param reserve_props: Documentation: https://esbuild.github.io/api/#mangle-props.
-        :param sourcefile: 
+        :param sourcefile: Documentation: https://esbuild.github.io/api/#sourcefile.
         :param sourcemap: Documentation: https://esbuild.github.io/api/#sourcemap.
         :param source_root: Documentation: https://esbuild.github.io/api/#source-root.
         :param sources_content: Documentation: https://esbuild.github.io/api/#sources-content.
         :param supported: Documentation: https://esbuild.github.io/api/#supported.
         :param target: Documentation: https://esbuild.github.io/api/#target.
         :param tree_shaking: Documentation: https://esbuild.github.io/api/#tree-shaking.
-        :param tsconfig_raw: 
+        :param tsconfig_raw: Documentation: https://esbuild.github.io/api/#tsconfig-raw.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__884b5e431e012b418b1076d2d6b7d3430be27ad832de2bbd7bbc2412d2ae6999)
             check_type(argname="argument banner", value=banner, expected_type=type_hints["banner"])
             check_type(argname="argument charset", value=charset, expected_type=type_hints["charset"])
             check_type(argname="argument color", value=color, expected_type=type_hints["color"])
             check_type(argname="argument define", value=define, expected_type=type_hints["define"])
             check_type(argname="argument drop", value=drop, expected_type=type_hints["drop"])
+            check_type(argname="argument drop_labels", value=drop_labels, expected_type=type_hints["drop_labels"])
             check_type(argname="argument footer", value=footer, expected_type=type_hints["footer"])
             check_type(argname="argument format", value=format, expected_type=type_hints["format"])
             check_type(argname="argument global_name", value=global_name, expected_type=type_hints["global_name"])
             check_type(argname="argument ignore_annotations", value=ignore_annotations, expected_type=type_hints["ignore_annotations"])
             check_type(argname="argument jsx", value=jsx, expected_type=type_hints["jsx"])
             check_type(argname="argument jsx_dev", value=jsx_dev, expected_type=type_hints["jsx_dev"])
             check_type(argname="argument jsx_factory", value=jsx_factory, expected_type=type_hints["jsx_factory"])
             check_type(argname="argument jsx_fragment", value=jsx_fragment, expected_type=type_hints["jsx_fragment"])
             check_type(argname="argument jsx_import_source", value=jsx_import_source, expected_type=type_hints["jsx_import_source"])
             check_type(argname="argument jsx_side_effects", value=jsx_side_effects, expected_type=type_hints["jsx_side_effects"])
             check_type(argname="argument keep_names", value=keep_names, expected_type=type_hints["keep_names"])
             check_type(argname="argument legal_comments", value=legal_comments, expected_type=type_hints["legal_comments"])
+            check_type(argname="argument line_limit", value=line_limit, expected_type=type_hints["line_limit"])
             check_type(argname="argument loader", value=loader, expected_type=type_hints["loader"])
             check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
             check_type(argname="argument log_limit", value=log_limit, expected_type=type_hints["log_limit"])
             check_type(argname="argument log_override", value=log_override, expected_type=type_hints["log_override"])
             check_type(argname="argument mangle_cache", value=mangle_cache, expected_type=type_hints["mangle_cache"])
             check_type(argname="argument mangle_props", value=mangle_props, expected_type=type_hints["mangle_props"])
             check_type(argname="argument mangle_quoted", value=mangle_quoted, expected_type=type_hints["mangle_quoted"])
@@ -5594,14 +5848,16 @@
             self._values["charset"] = charset
         if color is not None:
             self._values["color"] = color
         if define is not None:
             self._values["define"] = define
         if drop is not None:
             self._values["drop"] = drop
+        if drop_labels is not None:
+            self._values["drop_labels"] = drop_labels
         if footer is not None:
             self._values["footer"] = footer
         if format is not None:
             self._values["format"] = format
         if global_name is not None:
             self._values["global_name"] = global_name
         if ignore_annotations is not None:
@@ -5618,14 +5874,16 @@
             self._values["jsx_import_source"] = jsx_import_source
         if jsx_side_effects is not None:
             self._values["jsx_side_effects"] = jsx_side_effects
         if keep_names is not None:
             self._values["keep_names"] = keep_names
         if legal_comments is not None:
             self._values["legal_comments"] = legal_comments
+        if line_limit is not None:
+            self._values["line_limit"] = line_limit
         if loader is not None:
             self._values["loader"] = loader
         if log_level is not None:
             self._values["log_level"] = log_level
         if log_limit is not None:
             self._values["log_limit"] = log_limit
         if log_override is not None:
@@ -5665,14 +5923,15 @@
         if tree_shaking is not None:
             self._values["tree_shaking"] = tree_shaking
         if tsconfig_raw is not None:
             self._values["tsconfig_raw"] = tsconfig_raw
 
     @builtins.property
     def banner(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#banner.'''
         result = self._values.get("banner")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def charset(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#charset.'''
         result = self._values.get("charset")
@@ -5693,15 +5952,22 @@
     @builtins.property
     def drop(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#drop.'''
         result = self._values.get("drop")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
+    def drop_labels(self) -> typing.Optional[typing.List[builtins.str]]:
+        '''Documentation: https://esbuild.github.io/api/#drop-labels.'''
+        result = self._values.get("drop_labels")
+        return typing.cast(typing.Optional[typing.List[builtins.str]], result)
+
+    @builtins.property
     def footer(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#footer.'''
         result = self._values.get("footer")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def format(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#format.'''
         result = self._values.get("format")
@@ -5764,15 +6030,22 @@
     @builtins.property
     def legal_comments(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#legal-comments.'''
         result = self._values.get("legal_comments")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def line_limit(self) -> typing.Optional[jsii.Number]:
+        '''Documentation: https://esbuild.github.io/api/#line-limit.'''
+        result = self._values.get("line_limit")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def loader(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#loader.'''
         result = self._values.get("loader")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def log_level(self) -> typing.Optional[builtins.str]:
         '''Documentation: https://esbuild.github.io/api/#log-level.'''
         result = self._values.get("log_level")
@@ -5852,14 +6125,15 @@
     def reserve_props(self) -> typing.Any:
         '''Documentation: https://esbuild.github.io/api/#mangle-props.'''
         result = self._values.get("reserve_props")
         return typing.cast(typing.Any, result)
 
     @builtins.property
     def sourcefile(self) -> typing.Optional[builtins.str]:
+        '''Documentation: https://esbuild.github.io/api/#sourcefile.'''
         result = self._values.get("sourcefile")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sourcemap(self) -> typing.Optional[typing.Union[builtins.bool, builtins.str]]:
         '''Documentation: https://esbuild.github.io/api/#sourcemap.'''
         result = self._values.get("sourcemap")
@@ -5897,14 +6171,15 @@
         result = self._values.get("tree_shaking")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def tsconfig_raw(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, TsconfigOptions]]:
+        '''Documentation: https://esbuild.github.io/api/#tsconfig-raw.'''
         result = self._values.get("tsconfig_raw")
         return typing.cast(typing.Optional[typing.Union[builtins.str, TsconfigOptions]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -5962,14 +6237,15 @@
     bundle: typing.Optional[builtins.bool] = None,
     charset: typing.Optional[builtins.str] = None,
     chunk_names: typing.Optional[builtins.str] = None,
     color: typing.Optional[builtins.bool] = None,
     conditions: typing.Optional[typing.Sequence[builtins.str]] = None,
     define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+    drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     entry_names: typing.Optional[builtins.str] = None,
     external: typing.Optional[typing.Sequence[builtins.str]] = None,
     footer: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     format: typing.Optional[builtins.str] = None,
     global_name: typing.Optional[builtins.str] = None,
     ignore_annotations: typing.Optional[builtins.bool] = None,
     inject: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -5977,14 +6253,15 @@
     jsx_dev: typing.Optional[builtins.bool] = None,
     jsx_factory: typing.Optional[builtins.str] = None,
     jsx_fragment: typing.Optional[builtins.str] = None,
     jsx_import_source: typing.Optional[builtins.str] = None,
     jsx_side_effects: typing.Optional[builtins.bool] = None,
     keep_names: typing.Optional[builtins.bool] = None,
     legal_comments: typing.Optional[builtins.str] = None,
+    line_limit: typing.Optional[jsii.Number] = None,
     loader: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     log_level: typing.Optional[builtins.str] = None,
     log_limit: typing.Optional[jsii.Number] = None,
     log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     main_fields: typing.Optional[typing.Sequence[builtins.str]] = None,
     mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
     mangle_props: typing.Any = None,
@@ -6010,14 +6287,15 @@
     source_root: typing.Optional[builtins.str] = None,
     sources_content: typing.Optional[builtins.bool] = None,
     splitting: typing.Optional[builtins.bool] = None,
     supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
     target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
     tree_shaking: typing.Optional[builtins.bool] = None,
     tsconfig: typing.Optional[builtins.str] = None,
+    tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union[TsconfigOptions, typing.Dict[builtins.str, typing.Any]]]] = None,
     write: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f9873d08db3203496e0d96907173153080076971ae0098d003ebff0ccaffdb97(
     *,
@@ -6035,19 +6313,28 @@
     s3_location: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.Location, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9b682d31bc71983a448565f5ef0a021abb3aeaf127a6dab66c921bef47f98592(
     *,
+    always_strict: typing.Optional[builtins.bool] = None,
+    base_url: typing.Optional[builtins.bool] = None,
+    experimental_decorators: typing.Optional[builtins.bool] = None,
     imports_not_used_as_values: typing.Optional[builtins.str] = None,
+    jsx: typing.Optional[builtins.str] = None,
     jsx_factory: typing.Optional[builtins.str] = None,
     jsx_fragment_factory: typing.Optional[builtins.str] = None,
+    jsx_import_source: typing.Optional[builtins.str] = None,
+    paths: typing.Optional[typing.Mapping[builtins.str, typing.Sequence[builtins.str]]] = None,
     preserve_value_imports: typing.Optional[builtins.bool] = None,
+    strict: typing.Optional[builtins.bool] = None,
+    target: typing.Optional[builtins.str] = None,
     use_define_for_class_fields: typing.Optional[builtins.bool] = None,
+    verbatim_module_syntax: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__17ececb4940ec6eae1c73365c13ad8bd754b062cb59e54a4e520ed5b39927f70(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
@@ -6128,26 +6415,28 @@
     input: builtins.str,
     *,
     banner: typing.Optional[builtins.str] = None,
     charset: typing.Optional[builtins.str] = None,
     color: typing.Optional[builtins.bool] = None,
     define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+    drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     footer: typing.Optional[builtins.str] = None,
     format: typing.Optional[builtins.str] = None,
     global_name: typing.Optional[builtins.str] = None,
     ignore_annotations: typing.Optional[builtins.bool] = None,
     jsx: typing.Optional[builtins.str] = None,
     jsx_dev: typing.Optional[builtins.bool] = None,
     jsx_factory: typing.Optional[builtins.str] = None,
     jsx_fragment: typing.Optional[builtins.str] = None,
     jsx_import_source: typing.Optional[builtins.str] = None,
     jsx_side_effects: typing.Optional[builtins.bool] = None,
     keep_names: typing.Optional[builtins.bool] = None,
     legal_comments: typing.Optional[builtins.str] = None,
+    line_limit: typing.Optional[jsii.Number] = None,
     loader: typing.Optional[builtins.str] = None,
     log_level: typing.Optional[builtins.str] = None,
     log_limit: typing.Optional[jsii.Number] = None,
     log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
     mangle_props: typing.Any = None,
     mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -6297,14 +6586,15 @@
     bundle: typing.Optional[builtins.bool] = None,
     charset: typing.Optional[builtins.str] = None,
     chunk_names: typing.Optional[builtins.str] = None,
     color: typing.Optional[builtins.bool] = None,
     conditions: typing.Optional[typing.Sequence[builtins.str]] = None,
     define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+    drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     entry_names: typing.Optional[builtins.str] = None,
     external: typing.Optional[typing.Sequence[builtins.str]] = None,
     footer: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     format: typing.Optional[builtins.str] = None,
     global_name: typing.Optional[builtins.str] = None,
     ignore_annotations: typing.Optional[builtins.bool] = None,
     inject: typing.Optional[typing.Sequence[builtins.str]] = None,
@@ -6312,14 +6602,15 @@
     jsx_dev: typing.Optional[builtins.bool] = None,
     jsx_factory: typing.Optional[builtins.str] = None,
     jsx_fragment: typing.Optional[builtins.str] = None,
     jsx_import_source: typing.Optional[builtins.str] = None,
     jsx_side_effects: typing.Optional[builtins.bool] = None,
     keep_names: typing.Optional[builtins.bool] = None,
     legal_comments: typing.Optional[builtins.str] = None,
+    line_limit: typing.Optional[jsii.Number] = None,
     loader: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     log_level: typing.Optional[builtins.str] = None,
     log_limit: typing.Optional[jsii.Number] = None,
     log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     main_fields: typing.Optional[typing.Sequence[builtins.str]] = None,
     mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
     mangle_props: typing.Any = None,
@@ -6345,39 +6636,42 @@
     source_root: typing.Optional[builtins.str] = None,
     sources_content: typing.Optional[builtins.bool] = None,
     splitting: typing.Optional[builtins.bool] = None,
     supported: typing.Optional[typing.Mapping[builtins.str, builtins.bool]] = None,
     target: typing.Optional[typing.Union[builtins.str, typing.Sequence[builtins.str]]] = None,
     tree_shaking: typing.Optional[builtins.bool] = None,
     tsconfig: typing.Optional[builtins.str] = None,
+    tsconfig_raw: typing.Optional[typing.Union[builtins.str, typing.Union[TsconfigOptions, typing.Dict[builtins.str, typing.Any]]]] = None,
     write: typing.Optional[builtins.bool] = None,
     entry_points: typing.Optional[typing.Union[typing.Sequence[builtins.str], typing.Mapping[builtins.str, builtins.str]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__6c37248db4a858f2f46ff70ce7ec32f72b189492c09c9e26fc3552cb219fbd47(
     *,
     banner: typing.Optional[builtins.str] = None,
     charset: typing.Optional[builtins.str] = None,
     color: typing.Optional[builtins.bool] = None,
     define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+    drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     footer: typing.Optional[builtins.str] = None,
     format: typing.Optional[builtins.str] = None,
     global_name: typing.Optional[builtins.str] = None,
     ignore_annotations: typing.Optional[builtins.bool] = None,
     jsx: typing.Optional[builtins.str] = None,
     jsx_dev: typing.Optional[builtins.bool] = None,
     jsx_factory: typing.Optional[builtins.str] = None,
     jsx_fragment: typing.Optional[builtins.str] = None,
     jsx_import_source: typing.Optional[builtins.str] = None,
     jsx_side_effects: typing.Optional[builtins.bool] = None,
     keep_names: typing.Optional[builtins.bool] = None,
     legal_comments: typing.Optional[builtins.str] = None,
+    line_limit: typing.Optional[jsii.Number] = None,
     loader: typing.Optional[builtins.str] = None,
     log_level: typing.Optional[builtins.str] = None,
     log_limit: typing.Optional[jsii.Number] = None,
     log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
     mangle_props: typing.Any = None,
     mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -6535,26 +6829,28 @@
     input: builtins.str,
     *,
     banner: typing.Optional[builtins.str] = None,
     charset: typing.Optional[builtins.str] = None,
     color: typing.Optional[builtins.bool] = None,
     define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+    drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     footer: typing.Optional[builtins.str] = None,
     format: typing.Optional[builtins.str] = None,
     global_name: typing.Optional[builtins.str] = None,
     ignore_annotations: typing.Optional[builtins.bool] = None,
     jsx: typing.Optional[builtins.str] = None,
     jsx_dev: typing.Optional[builtins.bool] = None,
     jsx_factory: typing.Optional[builtins.str] = None,
     jsx_fragment: typing.Optional[builtins.str] = None,
     jsx_import_source: typing.Optional[builtins.str] = None,
     jsx_side_effects: typing.Optional[builtins.bool] = None,
     keep_names: typing.Optional[builtins.bool] = None,
     legal_comments: typing.Optional[builtins.str] = None,
+    line_limit: typing.Optional[jsii.Number] = None,
     loader: typing.Optional[builtins.str] = None,
     log_level: typing.Optional[builtins.str] = None,
     log_limit: typing.Optional[jsii.Number] = None,
     log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
     mangle_props: typing.Any = None,
     mangle_quoted: typing.Optional[builtins.bool] = None,
@@ -6580,26 +6876,28 @@
 def _typecheckingstub__884b5e431e012b418b1076d2d6b7d3430be27ad832de2bbd7bbc2412d2ae6999(
     *,
     banner: typing.Optional[builtins.str] = None,
     charset: typing.Optional[builtins.str] = None,
     color: typing.Optional[builtins.bool] = None,
     define: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     drop: typing.Optional[typing.Sequence[builtins.str]] = None,
+    drop_labels: typing.Optional[typing.Sequence[builtins.str]] = None,
     footer: typing.Optional[builtins.str] = None,
     format: typing.Optional[builtins.str] = None,
     global_name: typing.Optional[builtins.str] = None,
     ignore_annotations: typing.Optional[builtins.bool] = None,
     jsx: typing.Optional[builtins.str] = None,
     jsx_dev: typing.Optional[builtins.bool] = None,
     jsx_factory: typing.Optional[builtins.str] = None,
     jsx_fragment: typing.Optional[builtins.str] = None,
     jsx_import_source: typing.Optional[builtins.str] = None,
     jsx_side_effects: typing.Optional[builtins.bool] = None,
     keep_names: typing.Optional[builtins.bool] = None,
     legal_comments: typing.Optional[builtins.str] = None,
+    line_limit: typing.Optional[jsii.Number] = None,
     loader: typing.Optional[builtins.str] = None,
     log_level: typing.Optional[builtins.str] = None,
     log_limit: typing.Optional[jsii.Number] = None,
     log_override: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     mangle_cache: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, builtins.bool]]] = None,
     mangle_props: typing.Any = None,
     mangle_quoted: typing.Optional[builtins.bool] = None,
```

### Comparing `mrgrain.cdk-esbuild-4.1.9/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO` & `mrgrain.cdk-esbuild-4.2.0/src/mrgrain.cdk_esbuild.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrgrain.cdk-esbuild
-Version: 4.1.9
+Version: 4.2.0
 Summary: CDK constructs for esbuild, an extremely fast JavaScript bundler
 Home-page: https://github.com/mrgrain/cdk-esbuild
 Author: Moritz Kornher<mail@moritzkornher.de>
 License: MIT
 Project-URL: Source, https://github.com/mrgrain/cdk-esbuild
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -293,18 +293,18 @@
 
 A custom implementation can be provided by implementing `IBuildProvider` or `ITransformProvider`:
 
 ```python
 @jsii.implements(IBuildProvider)
 @jsii.implements(ITransformProvider)
 class CustomEsbuild:
-    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def build_sync(self, *, bundle=None, splitting=None, preserveSymlinks=None, outfile=None, metafile=None, outdir=None, outbase=None, external=None, packages=None, alias=None, loader=None, resolveExtensions=None, mainFields=None, conditions=None, write=None, allowOverwrite=None, tsconfig=None, outExtension=None, publicPath=None, entryNames=None, chunkNames=None, assetNames=None, inject=None, banner=None, footer=None, absWorkingDir=None, nodePaths=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         pass
 
-    def transform_sync(self, code, *, tsconfigRaw=None, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None):
+    def transform_sync(self, code, *, sourcefile=None, loader=None, banner=None, footer=None, sourcemap=None, legalComments=None, sourceRoot=None, sourcesContent=None, format=None, globalName=None, target=None, supported=None, platform=None, mangleProps=None, reserveProps=None, mangleQuoted=None, mangleCache=None, drop=None, dropLabels=None, minify=None, minifyWhitespace=None, minifyIdentifiers=None, minifySyntax=None, lineLimit=None, charset=None, treeShaking=None, ignoreAnnotations=None, jsx=None, jsxFactory=None, jsxFragment=None, jsxImportSource=None, jsxDev=None, jsxSideEffects=None, define=None, pure=None, keepNames=None, color=None, logLevel=None, logLimit=None, logOverride=None, tsconfigRaw=None):
         # custom implementation goes here, return transformed code
         return "transformed code"
 
 # These will use the custom implementation
 TypeScriptCode("src/handler.ts",
     build_provider=CustomEsbuild()
 )
```

