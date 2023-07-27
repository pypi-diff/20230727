# Comparing `tmp/abstract_gui-0.0.41.tar.gz` & `tmp/abstract_gui-0.0.42-py3.11.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.41.tar", last modified: Wed May 31 14:40:01 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

