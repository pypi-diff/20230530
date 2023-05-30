# Comparing `tmp/fastapi_tryton-0.2.0.tar.gz` & `tmp/fastapi_tryton-0.2.1-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_tryton-0.2.0.tar", last modified: Tue Jan 10 21:24:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

