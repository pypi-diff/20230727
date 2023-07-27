# Comparing `tmp/javatools-1.5.0.tar.gz` & `tmp/javatools-1.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/javatools-1.5.0.tar", last modified: Sun Jun 21 11:04:41 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

