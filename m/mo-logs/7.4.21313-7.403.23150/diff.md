# Comparing `tmp/mo-logs-7.4.21313.tar.gz` & `tmp/mo_logs-7.403.23150-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo-logs-7.4.21313.tar", last modified: Tue Nov  9 12:27:12 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

