# Comparing `tmp/tieba-sign-0.7.0.tar.gz` & `tmp/tieba_sign-0.8.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tieba-sign-0.7.0.tar", last modified: Fri May 21 12:43:21 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

