# Comparing `tmp/byquant-0.5.2.tar.gz` & `tmp/byquant-0.5.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byquant-0.5.2.tar", last modified: Tue May 16 08:07:22 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

