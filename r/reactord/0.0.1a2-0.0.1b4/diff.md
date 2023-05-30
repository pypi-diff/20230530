# Comparing `tmp/reactord-0.0.1a2.tar.gz` & `tmp/reactord-0.0.1b4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactord-0.0.1a2.tar", last modified: Fri Jan 20 14:32:13 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

