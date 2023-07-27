# Comparing `tmp/chichicha-1.0.16.tar.gz` & `tmp/chichicha-2.1.7.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chichicha-1.0.16.tar", last modified: Thu Oct 13 09:47:28 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

