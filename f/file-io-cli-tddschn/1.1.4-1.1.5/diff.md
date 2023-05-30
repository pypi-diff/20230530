# Comparing `tmp/file_io_cli_tddschn-1.1.4.tar.gz` & `tmp/file_io_cli_tddschn-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_io_cli_tddschn-1.1.4.tar", max compression
+gzip compressed data, was "file_io_cli_tddschn-1.1.5.tar", max compression
```

## Comparing `file_io_cli_tddschn-1.1.4.tar` & `file_io_cli_tddschn-1.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.4/LICENSE
--rw-r--r--   0        0        0     1084 2023-05-29 11:15:29.791564 file_io_cli_tddschn-1.1.4/LICENSE.txt
--rw-r--r--   0        0        0     3342 2023-05-29 11:18:30.561155 file_io_cli_tddschn-1.1.4/README.md
--rw-r--r--   0        0        0      147 2023-05-29 16:14:33.520804 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/__init__.py
--rw-r--r--   0        0        0    11960 2023-05-29 16:12:39.264811 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/cli.py
--rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/config.py
--rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/utils.py
--rw-r--r--   0        0        0     1168 2023-05-29 16:14:33.517821 file_io_cli_tddschn-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.5/LICENSE
+-rw-r--r--   0        0        0     1084 2023-05-29 11:15:29.791564 file_io_cli_tddschn-1.1.5/LICENSE.txt
+-rw-r--r--   0        0        0     3342 2023-05-29 11:18:30.561155 file_io_cli_tddschn-1.1.5/README.md
+-rw-r--r--   0        0        0      147 2023-05-30 03:26:50.936217 file_io_cli_tddschn-1.1.5/file_io_cli_tddschn/__init__.py
+-rw-r--r--   0        0        0    11953 2023-05-30 03:26:14.609001 file_io_cli_tddschn-1.1.5/file_io_cli_tddschn/cli.py
+-rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.5/file_io_cli_tddschn/config.py
+-rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.5/file_io_cli_tddschn/utils.py
+-rw-r--r--   0        0        0     1168 2023-05-30 03:26:50.933890 file_io_cli_tddschn-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.5/PKG-INFO
```

### Comparing `file_io_cli_tddschn-1.1.4/LICENSE` & `file_io_cli_tddschn-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.4/LICENSE.txt` & `file_io_cli_tddschn-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.4/README.md` & `file_io_cli_tddschn-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.4/file_io_cli_tddschn/cli.py` & `file_io_cli_tddschn-1.1.5/file_io_cli_tddschn/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 disposition += '; filename="{}"'.format(self.filename)
             headers['Content-Disposition'] = disposition
 
         if 'Content-Type' not in headers:
             headers['Content-Type'] = 'application/octet-stream'
 
         self.headers = b'\r\n'.join(
-            '{}: {}'.format(k, v).encode('ascii') for k, v in headers.items()
+            '{}: {}'.format(k, v).encode() for k, v in headers.items()
         )
 
     def compute_size(self, include_final_boundary=True):
         pos = self.fp.tell()
         self.fp.seek(0, os.SEEK_END)
         size = self.fp.tell()
         self.fp.seek(pos)
```

### Comparing `file_io_cli_tddschn-1.1.4/pyproject.toml` & `file_io_cli_tddschn-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "file.io-cli-tddschn"
-version = "1.1.4"
+version = "1.1.5"
 description = "Command-line tool to upload files to https://file.io"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 # packages = [{ include = "file_io_cli.py" }]
 packages = [{ include = "file_io_cli_tddschn" }]
 homepage = "https://github.com/tddschn/file.io-cli-tddschn"
```

### Comparing `file_io_cli_tddschn-1.1.4/PKG-INFO` & `file_io_cli_tddschn-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-io-cli-tddschn
-Version: 1.1.4
+Version: 1.1.5
 Summary: Command-line tool to upload files to https://file.io
 Home-page: https://github.com/tddschn/file.io-cli-tddschn
 License: MIT
 Keywords: file.io,utility,uploader,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

