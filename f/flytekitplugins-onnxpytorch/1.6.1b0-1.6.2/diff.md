# Comparing `tmp/flytekitplugins-onnxpytorch-1.6.1b0.tar.gz` & `tmp/flytekitplugins_onnxpytorch-1.6.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxpytorch-1.6.1b0.tar", last modified: Mon May 15 22:07:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

