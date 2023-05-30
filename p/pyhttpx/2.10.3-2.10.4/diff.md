# Comparing `tmp/pyhttpx-2.10.3.tar.gz` & `tmp/pyhttpx-2.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhttpx-2.10.3.tar", last modified: Wed May 24 03:33:25 2023, max compression
+gzip compressed data, was "dist\pyhttpx-2.10.4.tar", last modified: Tue May 30 00:26:17 2023, max compression
```

## Comparing `pyhttpx-2.10.3.tar` & `pyhttpx-2.10.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/
--rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.3/LICENSE
--rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.3/MANIFEST.in
--rw-rw-rw-   0        0        0      339 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/PKG-INFO
--rw-rw-rw-   0        0        0     3197 2023-05-23 13:16:49.000000 pyhttpx-2.10.3/README.md
--rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/
--rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.3/pyhttpx/__init__.py
--rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/__version__.py
--rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/compat.py
--rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.3/pyhttpx/exception.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/__init__.py
--rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/aes.py
--rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_aead.py
--rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_block.py
--rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/ciphers.py
--rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/ecc.py
--rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/hkdf.py
--rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/kx_algs.py
--rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/prf.py
--rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/extensions.py
--rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/fields.py
--rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/handshake.py
--rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/keyexchange.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/linux/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/linux/__init__.py
--rw-rw-rw-   0        0        0    10488 2023-05-23 13:31:03.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/pyaiossl.py
--rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/pyssl.py
--rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/socks.py
--rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/suites.py
--rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/tls_context.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/window/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.3/pyhttpx/layers/tls/window/__init__.py
--rw-rw-rw-   0        0        0     9302 2023-03-08 03:35:13.000000 pyhttpx-2.10.3/pyhttpx/models.py
--rw-rw-rw-   0        0        0    16930 2023-05-24 03:33:07.000000 pyhttpx-2.10.3/pyhttpx/session.py
--rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.3/pyhttpx/utils.py
--rw-rw-rw-   0        0        0     8230 2023-05-23 13:39:01.000000 pyhttpx-2.10.3/pyhttpx/websocket.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/pyhttpx.egg-info/
--rw-rw-rw-   0        0        0      339 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.3/pyhttpx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-24 03:33:24.000000 pyhttpx-2.10.3/pyhttpx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/setup.cfg
--rw-rw-rw-   0        0        0     1576 2023-05-24 03:33:22.000000 pyhttpx-2.10.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:33:25.000000 pyhttpx-2.10.3/tests/
--rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.3/tests/__init__.py
--rw-rw-rw-   0        0        0     1197 2023-05-23 13:57:49.000000 pyhttpx-2.10.3/tests/requestTest.py
--rw-rw-rw-   0        0        0     1931 2023-05-23 13:43:36.000000 pyhttpx-2.10.3/tests/websocketTest.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/
+-rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.4/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      339 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3197 2023-05-23 13:16:49.000000 pyhttpx-2.10.4/README.md
+-rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx/
+-rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.4/pyhttpx/__init__.py
+-rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/__version__.py
+-rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/compat.py
+-rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.4/pyhttpx/exception.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx/layers/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/aes.py
+-rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/cipher_aead.py
+-rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/cipher_block.py
+-rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/ciphers.py
+-rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/ecc.py
+-rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/hkdf.py
+-rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/kx_algs.py
+-rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/prf.py
+-rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/extensions.py
+-rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/fields.py
+-rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/handshake.py
+-rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/keyexchange.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/linux/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/linux/__init__.py
+-rw-rw-rw-   0        0        0    10351 2023-05-29 10:31:50.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/pyaiossl.py
+-rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/pyssl.py
+-rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/socks.py
+-rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/suites.py
+-rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/tls_context.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/window/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.4/pyhttpx/layers/tls/window/__init__.py
+-rw-rw-rw-   0        0        0     9276 2023-05-26 09:23:48.000000 pyhttpx-2.10.4/pyhttpx/models.py
+-rw-rw-rw-   0        0        0    16930 2023-05-27 06:13:47.000000 pyhttpx-2.10.4/pyhttpx/session.py
+-rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.4/pyhttpx/utils.py
+-rw-rw-rw-   0        0        0     8142 2023-05-30 00:24:03.000000 pyhttpx-2.10.4/pyhttpx/websocket.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.4/pyhttpx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/pyhttpx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-05-30 00:26:13.000000 pyhttpx-2.10.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:26:17.000000 pyhttpx-2.10.4/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.4/tests/__init__.py
+-rw-rw-rw-   0        0        0     1133 2023-05-29 03:40:20.000000 pyhttpx-2.10.4/tests/requestTest.py
+-rw-rw-rw-   0        0        0     1882 2023-05-29 10:30:29.000000 pyhttpx-2.10.4/tests/websocketTest.py
```

### Comparing `pyhttpx-2.10.3/LICENSE` & `pyhttpx-2.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/README.md` & `pyhttpx-2.10.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/exception.py` & `pyhttpx-2.10.4/pyhttpx/exception.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/aes.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/chacha20_poly1305.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_aead.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/cipher_aead.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/cipher_block.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/cipher_block.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/ecc.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/hkdf.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/kx_algs.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/kx_algs.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/crypto/prf.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/crypto/prf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/extensions.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/extensions.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/handshake.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/handshake.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/keyexchange.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/keyexchange.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/pyaiossl.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/pyaiossl.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,49 +158,40 @@
         self.writer.write(self.write_buff)
         self.cache = b''
         self.plaintext_reader = b''
 
     async def recv(self, size=4096):
 
         s = await self.reader.read(size)
-        if not s:
-            return None
+        if size > 0 and s == b'':
+            raise ConnectionClosed('server closed')
 
         s = self.cache + s
         self.cache = b''
-
-        # 会存在读取长度不足而返回空字符,而不是收到fin
-        exc_alert = False
         while s and len(s) >= 5:
 
             handshake_type = struct.unpack('!B', s[:1])[0]
             length = struct.unpack('!H', s[3:5])[0]
             flowtext = s[5:5 + length]
 
             if len(flowtext) < length:
                 self.cache = s[:]
                 break
 
             s = s[5 + length:]
             if handshake_type == 0x17:
                 p = self.tls_cxt.decrypt(flowtext, b'\x17')
                 self.plaintext_reader += p
-
-
             elif handshake_type == 0x15:
                 self.isclosed = True
-                exc_alert = True
                 raise ConnectionClosed('server closed')
 
-        b = self.plaintext_reader
+        p = self.plaintext_reader
         self.plaintext_reader = b''
-        if exc_alert:
-            b = None
-        return b
-
+        return p
 
 
 PROTOCOL_TLSv1_2 = b'\x03\x03'
 def default_context():
     return SSLContext(PROTOCOL_TLSv1_2)
```

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/pyssl.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/pyssl.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/socks.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/socks.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/suites.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/suites.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/layers/tls/tls_context.py` & `pyhttpx-2.10.4/pyhttpx/layers/tls/tls_context.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/models.py` & `pyhttpx-2.10.4/pyhttpx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
         return self._content
 
     @property
     def text(self):
         return self.content.decode(encoding=self.encoding)
 
-    @property
+
     def json(self):
         return json.loads(self.text)
 
     def __repr__(self):
         template = '<Response status_code={status_code}>'
         return  template.format(status_code=self.status_code)
 
@@ -305,15 +305,15 @@
 
         return self._content
 
     @property
     def text(self):
         return self.content.decode(encoding=self.encoding)
 
-    @property
+
     def json(self):
         return json.loads(self.text)
 
     def __repr__(self):
         template = '<Response status_code={status_code}>'
         return  template.format(status_code=self.status_code)
```

### Comparing `pyhttpx-2.10.3/pyhttpx/session.py` & `pyhttpx-2.10.4/pyhttpx/session.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/utils.py` & `pyhttpx-2.10.4/pyhttpx/utils.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/pyhttpx/websocket.py` & `pyhttpx-2.10.4/pyhttpx/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from urllib.parse import urlparse
 import socket
 
 from pyhttpx.layers.tls.pyaiossl import SSLContext,PROTOCOL_TLSv1_2
 from pyhttpx.exception import (
     SwitchingProtocolError,
     SecWebSocketKeyError,
-    WebSocketClosed
+    WebSocketClosed,
+    ConnectionClosed
 )
 
 DEFAULT_HEADERS = {
         'Accept-Encoding': 'gzip, deflate, br',
         'Accept-Language': 'zh,zh-CN;q=0.9,en;q=0.8',
         'Cache-Control': 'no-cache',
         'Pragma': 'no-cache',
@@ -165,28 +166,25 @@
             s += m
             s += struct.pack('!Q', len(data))
 
         else:
             raise OverflowError('data length more than 64 byte')
 
         mask_key = os.urandom(4)
-
         s += mask_key
         for i in range(len(data)):
             n = ord(data[i]) ^ (mask_key[i % 4])
             s += struct.pack('!B', n)
 
-
         await self.sock.sendall(s)
 
     async def flush(self ,data):
         self.cache_buffer += data
     async def handle(self):
 
-        #self.cache_buffer += data
         if len(self.cache_buffer) < 2:
             return
 
         frame_head = self.cache_buffer[0]
         FIN = frame_head >> 7
         opcode = frame_head & 0b1111
         payload_len = self.cache_buffer[1] & 0b1111111
@@ -210,14 +208,16 @@
 
 
         while len(msg) < msg_len:
             #数据长度不足,缓存中的数据还属于当前帧,继续读取
             d = await self.sock.recv(msg_len)
             msg += d
 
+        self.cache_buffer += msg[msg_len:]
+        msg = msg[:msg_len]
         if per_message_compressed:
             msg = zlib.decompressobj(-zlib.MAX_WBITS).decompress(msg)
 
         if opcode == 0x00:
             self.reader_buffer += msg
         elif opcode == 0x01:
             self.reader_buffer += msg
@@ -250,21 +250,18 @@
             #握手过程产生的缓存数据
             result = await self.handle()
 
             if result:
                 return result
             try:
                 data = await self.sock.recv(2 ** 14)
-            except ConnectionResetError:
+            except Exception:
                 self.open = False
                 raise WebSocketClosed('webscoket Closed')
             else:
-                if data is None:
-                    self.open = False
-                    raise WebSocketClosed('webscoket Closed')
                 await self.flush(data)
 
 
     async def loop_ping(self):
         while 1:
             s = os.urandom(4).decode('latin1')
             await self.send(s,binary=True, opc=0x09)
```

### Comparing `pyhttpx-2.10.3/pyhttpx.egg-info/SOURCES.txt` & `pyhttpx-2.10.4/pyhttpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.3/setup.py` & `pyhttpx-2.10.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sys.exit(errno)
 
 
 
 packages = find_packages()
 setup(
     name = "pyhttpx",
-    version = "2.10.3",
+    version = "2.10.4",
     keywords = ["pip", "pyhttpx"],
     description = "HTTP library.",
     long_description = "HTTP library, TLS supported version：tls1.2/tls1.3, HTTP supported version: http1.1/http2",
     license = "MIT Licence",
 
     url = "https://github.com/zero3301/pyhttpx",
     author = "3301",
```

### Comparing `pyhttpx-2.10.3/tests/requestTest.py` & `pyhttpx-2.10.4/tests/requestTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 }
 
 
 def main():
     sess = pyhttpx.HttpSession(http2=False,
                                browser_type='chrome',
-                               shuffle_extension_protocol=True
                                )
 
     url='https://tls.peet.ws/api/all'
     #url = 'https://httpbin.org/ip'
     proxies = {
         'https': 'http://username:password@host:port'
     }
```

### Comparing `pyhttpx-2.10.3/tests/websocketTest.py` & `pyhttpx-2.10.4/tests/websocketTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,51 +11,55 @@
 from pyhttpx import WebSocketClient
 
 class WSS:
     def __init__(self,url=None, headers=None, loop=None):
         self.url = url
         self.headers = headers
         self.loop = loop
-        self.ja3 = '771,19018-4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,0-23-65281-10-11-35-16-5-13-18-51-45-43-27-17513,27242-29-23-24,0'
+        self.ja3 = '771,19018-4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,23-0-65281-10-11-35-16-5-13-18-51-45-43-27-17513,27242-29-23-24,0'
 
     async def connect(self):
 
         self.sock = await WebSocketClient(url=self.url,
                                           headers=self.headers,
                                           loop=self.loop,
-                                          ja3=self.ja3
                                           ).connect()
 
         print('连接成功...')
     async def send(self):
-        await self.sock.send('666')
-        pass
+
+        await self.sock.send('3301')
+
 
     async def recv(self):
         while 1:
             r = await self.sock.recv()
             print(r)
+
 def main():
     loop = asyncio.get_event_loop()
     url = 'wss://www.python-spider.com/api/challenge62'
     headers = {
         'Host': 'www.python-spider.com',
         'Connection': 'Upgrade',
         'Pragma': 'no-cache',
         'Cache-Control': 'no-cache',
-        'Origin': 'www.python-spider.com',
+        'Origin': 'https://www.python-spider.com',
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
         'Upgrade': 'websocket',
         'Sec-WebSocket-Version': '13',
         'Accept-Encoding': 'gzip, deflate, br',
         'Accept-Language': 'zh,zh-CN;q=0.9,en;q=0.8',
         'Sec-WebSocket-Extensions': 'permessage-deflate; client_max_window_bits',
 
 }
+
     wss = WSS(url, headers, loop)
     loop.run_until_complete(wss.connect())
     loop.create_task(wss.send())
     loop.create_task(wss.recv())
     loop.run_forever()
 
 if __name__ == '__main__':
     main()
+
+
```

