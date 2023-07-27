# Comparing `tmp/chichicha-1.1.1.2.tar.gz` & `tmp/chichicha-2.1.7.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\chichicha-1.1.1.2.tar", last modified: Thu Jul 27 08:33:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

