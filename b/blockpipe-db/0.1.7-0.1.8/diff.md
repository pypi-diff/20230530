# Comparing `tmp/blockpipe_db-0.1.7.tar.gz` & `tmp/blockpipe_db-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe_db-0.1.7.tar", max compression
+gzip compressed data, was "blockpipe_db-0.1.8.tar", max compression
```

## Comparing `blockpipe_db-0.1.7.tar` & `blockpipe_db-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.7/README.md
--rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.7/blockpipe_db/__init__.py
--rw-r--r--   0        0        0     2223 2023-05-30 10:29:36.385478 blockpipe_db-0.1.7/blockpipe_db/client.py
--rw-r--r--   0        0        0      595 2023-05-30 09:20:34.775341 blockpipe_db-0.1.7/blockpipe_db/msg.py
--rw-r--r--   0        0        0      393 2023-05-30 10:29:43.734545 blockpipe_db-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.8/README.md
+-rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.8/blockpipe_db/__init__.py
+-rw-r--r--   0        0        0     2258 2023-05-30 10:32:23.074881 blockpipe_db-0.1.8/blockpipe_db/client.py
+-rw-r--r--   0        0        0      595 2023-05-30 09:20:34.775341 blockpipe_db-0.1.8/blockpipe_db/msg.py
+-rw-r--r--   0        0        0      393 2023-05-30 10:32:42.773700 blockpipe_db-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.8/PKG-INFO
```

### Comparing `blockpipe_db-0.1.7/blockpipe_db/client.py` & `blockpipe_db-0.1.8/blockpipe_db/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             sz = int.from_bytes(nb, 'big')
             e = buf_read.read_exact(sz)
             v = msgpack.unpackb(e)
             if 'Done' in v:
                 break
             z = v['DataFrame']
             z[2] = '0x'+z[2].hex()
+            z[3] = '0x'+z[3].hex()
             z[6] = '0x'+z[6].hex()
             z[7] = '0x'+z[7].hex()
             z[8] = '0x'+z[8].hex()
             z[9] = '0x'+z[9].hex()
             z[10] = '0x'+z[10].hex()
             z[11] = '0x'+z[11].hex()
             data.append(z)
```

### Comparing `blockpipe_db-0.1.7/blockpipe_db/msg.py` & `blockpipe_db-0.1.8/blockpipe_db/msg.py`

 * *Files identical despite different names*

### Comparing `blockpipe_db-0.1.7/PKG-INFO` & `blockpipe_db-0.1.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockpipe-db
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: thepsint@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

