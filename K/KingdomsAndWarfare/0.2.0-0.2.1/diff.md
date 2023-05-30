# Comparing `tmp/KingdomsAndWarfare-0.2.0.tar.gz` & `tmp/KingdomsAndWarfare-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KingdomsAndWarfare-0.2.0.tar", last modified: Tue May 30 05:13:29 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

