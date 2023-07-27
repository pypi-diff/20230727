# Comparing `tmp/morm-1.4.3.tar.gz` & `tmp/morm-1.4.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morm-1.4.3.tar", last modified: Wed Jul 21 15:10:13 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

