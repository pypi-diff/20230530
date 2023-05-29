# Comparing `tmp/gravitas-0.0.9.tar.gz` & `tmp/gravitas-0.1.1-pp38-pypy38_pp73-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.0.9.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

