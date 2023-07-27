# Comparing `tmp/xmlib-to-git-1.0.6.tar.gz` & `tmp/xmlib_to_git-1.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlib-to-git-1.0.6.tar", last modified: Thu May  5 15:49:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

