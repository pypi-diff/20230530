# Comparing `tmp/quanturf-8.6.3.tar.gz` & `tmp/quanturf-8.6.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanturf-8.6.3.tar", last modified: Mon May 29 14:43:10 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

