# Comparing `tmp/pragzip-0.5.0.tar.gz` & `tmp/pragzip-0.6.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pragzip-0.5.0.tar", last modified: Sun Jan 29 10:33:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

