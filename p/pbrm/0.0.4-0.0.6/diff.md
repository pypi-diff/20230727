# Comparing `tmp/pbrm-0.0.4.tar.gz` & `tmp/pbrm-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbrm-0.0.4.tar", last modified: Fri Mar 31 13:40:05 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

