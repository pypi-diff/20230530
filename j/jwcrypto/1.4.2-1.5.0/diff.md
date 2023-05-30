# Comparing `tmp/jwcrypto-1.4.2.tar.gz` & `tmp/jwcrypto-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwcrypto-1.4.2.tar", last modified: Thu Sep 15 13:01:52 2022, max compression
+gzip compressed data, was "jwcrypto-1.5.0.tar", last modified: Tue May 30 17:45:13 2023, max compression
```

## Comparing `jwcrypto-1.4.2.tar` & `jwcrypto-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 13:01:52.656641 jwcrypto-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-09-15 13:01:52.656641 jwcrypto-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 13:01:52.656641 jwcrypto-1.4.2/jwcrypto/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6170 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    32838 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/jwa.py
--rw-r--r--   0 runner    (1001) docker     (121)    23966 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/jwe.py
--rw-r--r--   0 runner    (1001) docker     (121)    49291 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/jwk.py
--rw-r--r--   0 runner    (1001) docker     (121)    27351 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/jws.py
--rw-r--r--   0 runner    (1001) docker     (121)    25882 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/jwt.py
--rw-r--r--   0 runner    (1001) docker     (121)    52210 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/tests-cookbook.py
--rw-r--r--   0 runner    (1001) docker     (121)    94294 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/jwcrypto/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 13:01:52.656641 jwcrypto-1.4.2/jwcrypto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-09-15 13:01:52.000000 jwcrypto-1.4.2/jwcrypto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-15 13:01:52.000000 jwcrypto-1.4.2/jwcrypto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 13:01:52.000000 jwcrypto-1.4.2/jwcrypto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-09-15 13:01:52.000000 jwcrypto-1.4.2/jwcrypto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-15 13:01:52.000000 jwcrypto-1.4.2/jwcrypto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-09-15 13:01:52.656641 jwcrypto-1.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1410 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-09-15 13:01:22.000000 jwcrypto-1.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:45:13.820392 jwcrypto-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-30 17:45:13.820392 jwcrypto-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:45:13.820392 jwcrypto-1.5.0/jwcrypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34492 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/jwa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23966 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/jwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50323 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27352 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52211 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/tests-cookbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98343 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/jwcrypto/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:45:13.820392 jwcrypto-1.5.0/jwcrypto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-30 17:45:13.000000 jwcrypto-1.5.0/jwcrypto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-30 17:45:13.000000 jwcrypto-1.5.0/jwcrypto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:45:13.000000 jwcrypto-1.5.0/jwcrypto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 17:45:13.000000 jwcrypto-1.5.0/jwcrypto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 17:45:13.000000 jwcrypto-1.5.0/jwcrypto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-30 17:45:13.820392 jwcrypto-1.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-30 17:44:53.000000 jwcrypto-1.5.0/tox.ini
```

### Comparing `jwcrypto-1.4.2/LICENSE` & `jwcrypto-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jwcrypto-1.4.2/PKG-INFO` & `jwcrypto-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwcrypto
-Version: 1.4.2
+Version: 1.5.0
 Summary: Implementation of JOSE Web standards
 Home-page: https://github.com/latchset/jwcrypto
 Maintainer: JWCrypto Project Contributors
 Maintainer-email: simo@redhat.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jwcrypto-1.4.2/README.md` & `jwcrypto-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jwcrypto-1.4.2/jwcrypto/common.py` & `jwcrypto-1.5.0/jwcrypto/common.py`

 * *Files identical despite different names*

### Comparing `jwcrypto-1.4.2/jwcrypto/jwa.py` & `jwcrypto-1.5.0/jwcrypto/jwa.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,26 +40,34 @@
     @abstractmethod
     def description(self):
         """A short description"""
 
     @property
     @abstractmethod
     def keysize(self):
-        """The actual/recommended/minimum key size"""
+        """The algorithm key size"""
 
     @property
     @abstractmethod
     def algorithm_usage_location(self):
         """One of 'alg', 'enc' or 'JWK'"""
 
     @property
     @abstractmethod
     def algorithm_use(self):
         """One of 'sig', 'kex', 'enc'"""
 
+    @property
+    def input_keysize(self):
+        """The input key size"""
+        try:
+            return self.wrap_key_size
+        except AttributeError:
+            return self.keysize
+
 
 def _bitsize(x):
     return len(x) * 8
 
 
 def _inbytes(x):
     return x // 8
@@ -391,15 +399,15 @@
         # always generate a random cek so we spend roughly the
         # same time as in the exception side of the branch
         cek = _randombits(bitsize)
         try:
             cek = super(_Rsa15, self).unwrap(key, bitsize, ek, headers)
             # always raise so we always run through the exception handling
             # code in all cases
-            raise Exception('Dummy')
+            raise ValueError('Dummy')
         except Exception:  # pylint: disable=broad-except
             return cek
 
 
 class _RsaOaep(_RSA, JWAAlgorithm):
 
     name = 'RSA-OAEP'
@@ -890,20 +898,23 @@
         return m[:_inbytes(self.keysize)]
 
     # RFC 7518 - 5.2.2
     def encrypt(self, k, a, m):
         """ Encrypt according to the selected encryption and hashing
         functions.
 
-        :param k: Encryption key (optional)
+        :param k: Encryption key
         :param a: Additional Authentication Data
         :param m: Plaintext
 
         Returns a dictionary with the computed data.
         """
+        if len(k) != _inbytes(self.wrap_key_size):
+            raise ValueError("Invalid input key size")
+
         hkey = k[:_inbytes(self.keysize)]
         ekey = k[_inbytes(self.keysize):]
 
         # encrypt
         iv = _randombits(self.blocksize)
         cipher = Cipher(algorithms.AES(ekey), modes.CBC(iv),
                         backend=self.backend)
@@ -916,22 +927,25 @@
         t = self._mac(hkey, a, iv, e)
 
         return (iv, e, t)
 
     def decrypt(self, k, a, iv, e, t):
         """ Decrypt according to the selected encryption and hashing
         functions.
-        :param k: Encryption key (optional)
+        :param k: Encryption key
         :param a: Additional Authenticated Data
         :param iv: Initialization Vector
         :param e: Ciphertext
         :param t: Authentication Tag
 
         Returns plaintext or raises an error
         """
+        if len(k) != _inbytes(self.wrap_key_size):
+            raise ValueError("Invalid input key size")
+
         hkey = k[:_inbytes(self.keysize)]
         dkey = k[_inbytes(self.keysize):]
 
         # verify mac
         if not constant_time.bytes_eq(t, self._mac(hkey, a, iv, e)):
             raise InvalidSignature('Failed to verify MAC')
 
@@ -986,18 +1000,18 @@
 
     def __init__(self):
         self.backend = default_backend()
         self.wrap_key_size = self.keysize
 
     # RFC 7518 - 5.3
     def encrypt(self, k, a, m):
-        """ Encrypt accoriding to the selected encryption and hashing
+        """ Encrypt according to the selected encryption and hashing
         functions.
 
-        :param k: Encryption key (optional)
+        :param k: Encryption key
         :param a: Additional Authentication Data
         :param m: Plaintext
 
         Returns a dictionary with the computed data.
         """
         iv = _randombits(96)
         cipher = Cipher(algorithms.AES(k), modes.GCM(iv),
@@ -1005,17 +1019,17 @@
         encryptor = cipher.encryptor()
         encryptor.authenticate_additional_data(a)
         e = encryptor.update(m) + encryptor.finalize()
 
         return (iv, e, encryptor.tag)
 
     def decrypt(self, k, a, iv, e, t):
-        """ Decrypt accoriding to the selected encryption and hashing
+        """ Decrypt according to the selected encryption and hashing
         functions.
-        :param k: Encryption key (optional)
+        :param k: Encryption key
         :param a: Additional Authenticated Data
         :param iv: Initialization Vector
         :param e: Ciphertext
         :param t: Authentication Tag
 
         Returns plaintext or raises an error
         """
@@ -1049,14 +1063,62 @@
     name = 'A256GCM'
     description = "AES GCM using 256-bit key"
     keysize = 256
     algorithm_usage_location = 'enc'
     algorithm_use = 'enc'
 
 
+class _BP256R1(_RawEC, JWAAlgorithm):
+
+    name = "BP256R1"
+    description = (
+        "ECDSA using Brainpool256R1 curve and SHA-256"
+        " (unregistered, custom-defined in breach"
+        " of IETF rules by gematik GmbH)"
+    )
+    keysize = 256
+    algorithm_usage_location = 'alg'
+    algorithm_use = 'sig'
+
+    def __init__(self):
+        super(_BP256R1, self).__init__('BP-256', hashes.SHA256())
+
+
+class _BP384R1(_RawEC, JWAAlgorithm):
+
+    name = "BP384R1"
+    description = (
+        "ECDSA using Brainpool384R1 curve and SHA-384"
+        " (unregistered, custom-defined in breach"
+        " of IETF rules by gematik GmbH)"
+    )
+    keysize = 384
+    algorithm_usage_location = 'alg'
+    algorithm_use = 'sig'
+
+    def __init__(self):
+        super(_BP384R1, self).__init__('BP-384', hashes.SHA384())
+
+
+class _BP512R1(_RawEC, JWAAlgorithm):
+
+    name = "BP512R1"
+    description = (
+        "ECDSA using Brainpool512R1 curve and SHA-512"
+        " (unregistered, custom-defined in breach"
+        " of IETF rules by gematik GmbH)"
+    )
+    keysize = 512
+    algorithm_usage_location = 'alg'
+    algorithm_use = 'sig'
+
+    def __init__(self):
+        super(_BP512R1, self).__init__('BP-512', hashes.SHA512())
+
+
 class JWA:
     """JWA Signing Algorithms.
 
     This class provides access to all JWA algorithms.
     """
 
     algorithms_registry = {
@@ -1093,15 +1155,18 @@
         'PBES2-HS384+A192KW': _Pbes2Hs384A192Kw,
         'PBES2-HS512+A256KW': _Pbes2Hs512A256Kw,
         'A128CBC-HS256': _A128CbcHs256,
         'A192CBC-HS384': _A192CbcHs384,
         'A256CBC-HS512': _A256CbcHs512,
         'A128GCM': _A128Gcm,
         'A192GCM': _A192Gcm,
-        'A256GCM': _A256Gcm
+        'A256GCM': _A256Gcm,
+        'BP256R1': _BP256R1,
+        'BP384R1': _BP384R1,
+        'BP512R1': _BP512R1
     }
 
     @classmethod
     def instantiate_alg(cls, name, use=None):
         alg = cls.algorithms_registry[name]
         if use is not None and alg.algorithm_use != use:
             raise KeyError
```

### Comparing `jwcrypto-1.4.2/jwcrypto/jwe.py` & `jwcrypto-1.5.0/jwcrypto/jwe.py`

 * *Files identical despite different names*

### Comparing `jwcrypto-1.4.2/jwcrypto/jwk.py` & `jwcrypto-1.5.0/jwcrypto/jwk.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,25 @@
 JWKEllipticCurveRegistry = {'P-256': 'P-256 curve',
                             'P-384': 'P-384 curve',
                             'P-521': 'P-521 curve',
                             'secp256k1': 'SECG secp256k1 curve',
                             'Ed25519': 'Ed25519 signature algorithm key pairs',
                             'Ed448': 'Ed448 signature algorithm key pairs',
                             'X25519': 'X25519 function key pairs',
-                            'X448': 'X448 function key pairs'}
+                            'X448': 'X448 function key pairs',
+                            'BP-256': 'BrainpoolP256R1 curve'
+                                    ' (unregistered, custom-defined in breach'
+                                    ' of IETF rules by gematik GmbH)',
+                            'BP-384': 'BrainpoolP384R1 curve'
+                                    ' (unregistered, custom-defined in breach'
+                                    ' of IETF rules by gematik GmbH)',
+                            'BP-512': 'BrainpoolP512R1 curve'
+                                    ' (unregistered, custom-defined in breach'
+                                    ' of IETF rules by gematik GmbH)'
+                            }
 """Registry of allowed Elliptic Curves"""
 
 # RFC 7517 - 8.2
 JWKUseRegistry = {'sig': 'Digital Signature or MAC',
                   'enc': 'Encryption'}
 """Registry of allowed uses"""
 
@@ -182,15 +192,18 @@
                          'deriveKey': 'Derive key',
                          'deriveBits': 'Derive bits not to be used as a key'}
 """Registry of allowed operations"""
 
 JWKpycaCurveMap = {'secp256r1': 'P-256',
                    'secp384r1': 'P-384',
                    'secp521r1': 'P-521',
-                   'secp256k1': 'secp256k1'}
+                   'secp256k1': 'secp256k1',
+                   'brainpoolP256r1': 'BP-256',
+                   'brainpoolP384r1': 'BP-384',
+                   'brainpoolP512r1': 'BP-512'}
 
 IANANamedInformationHashAlgorithmRegistry = {
     'sha-256': hashes.SHA256(),
     'sha-256-128': None,
     'sha-256-120': None,
     'sha-256-96': None,
     'sha-256-64': None,
@@ -313,15 +326,15 @@
          * OKP: crv(str) (one of Ed25519, Ed448, X25519, X448)
 
         Deprecated:
         Alternatively if the 'generate' parameter is provided with a
         valid key type as value then a new key will be generated according
         to the defaults or provided key strength options (type specific).
 
-        :param \**kwargs: parameters (otional).
+        :param \**kwargs: parameters (optional).
 
         :raises InvalidJWKType: if the key type is invalid
         :raises InvalidJWKValue: if incorrect or inconsistent parameters
             are provided.
         """
         super(JWK, self).__init__()
         self._cache_pub_k = None
@@ -360,15 +373,15 @@
             size = params.pop('size')
         elif 'alg' in params:
             try:
                 from jwcrypto.jwa import JWA
                 alg = JWA.instantiate_alg(params['alg'])
             except KeyError as e:
                 raise ValueError("Invalid 'alg' parameter") from e
-            size = alg.keysize
+            size = alg.input_keysize
         return size
 
     def _generate_oct(self, params):
         size = self._get_gen_size(params, 128)
         key = os.urandom(size // 8)
         params['kty'] = 'oct'
         params['k'] = base64url_encode(key)
@@ -449,14 +462,20 @@
             return ec.SECP256R1()
         elif cname == 'P-384':
             return ec.SECP384R1()
         elif cname == 'P-521':
             return ec.SECP521R1()
         elif cname == 'secp256k1':
             return ec.SECP256K1()
+        elif cname == 'BP-256':
+            return ec.BrainpoolP256R1()
+        elif cname == 'BP-384':
+            return ec.BrainpoolP384R1()
+        elif cname == 'BP-512':
+            return ec.BrainpoolP512R1()
         elif cname in _OKP_CURVES_TABLE:
             return _OKP_CURVES_TABLE[cname]
         else:
             raise InvalidJWKValue('Unknown Curve Name [%s]' % (name))
 
     def _generate_EC(self, params):
         curve = 'P-256'
```

### Comparing `jwcrypto-1.4.2/jwcrypto/jws.py` & `jwcrypto-1.5.0/jwcrypto/jws.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     def _verify(self, alg, key, payload, signature, protected, header=None):
         p = {}
         # verify it is a valid JSON object and decode
         if protected is not None:
             p = json_decode(protected)
             if not isinstance(p, dict):
                 raise InvalidJWSSignature('Invalid Protected header')
-        # merge heders, and verify there are no duplicates
+        # merge headers, and verify there are no duplicates
         if header:
             if not isinstance(header, dict):
                 raise InvalidJWSSignature('Invalid Unprotected header')
 
         # Merge and check (critical) headers
         chk_hdrs = self._merge_check_headers(p, header)
         for hdr in chk_hdrs:
@@ -320,15 +320,15 @@
     def _get_obj_payload(self, obj, dp):
         op = obj.get('payload')
         if dp is not None:
             if op is None or len(op) == 0:
                 return dp
             else:
                 raise InvalidJWSOperation('Object Payload present but'
-                                          ' Deatched Payload provided')
+                                          ' Detached Payload provided')
         return op
 
     def verify(self, key, alg=None, detached_payload=None):
         """Verifies a JWS token.
 
         :param key: A (:class:`jwcrypto.jwk.JWK`) verification or
          a (:class:`jwcrypto.jwk.JWKSet`) that contains a key indexed by the
```

### Comparing `jwcrypto-1.4.2/jwcrypto/jwt.py` & `jwcrypto-1.5.0/jwcrypto/jwt.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,16 @@
         self._add_time_claim('iat', claims, now)
         self._add_jti_claim(claims)
 
     def _check_string_claim(self, name, claims):
         if name not in claims or claims[name] is None:
             return
         if not isinstance(claims[name], str):
-            raise JWTInvalidClaimFormat("Claim %s is not a StringOrURI type")
+            raise JWTInvalidClaimFormat(
+                "Claim %s is not a StringOrURI type" % (name, ))
 
     def _check_array_or_string_claim(self, name, claims):
         if name not in claims or claims[name] is None:
             return
         if isinstance(claims[name], list):
             if any(not isinstance(claim, str) for claim in claims):
                 raise JWTInvalidClaimFormat(
```

### Comparing `jwcrypto-1.4.2/jwcrypto/tests-cookbook.py` & `jwcrypto-1.5.0/jwcrypto/tests-cookbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -1097,15 +1097,15 @@
     "tag": JWE_Authentication_Tag_5_12_4}
 
 # 5.13 - A256GCMKW not implemented yet
 
 
 # In general we can't compare ciphertexts with the reference because
 # either the algorithms use random nonces to authenticate the ciphertext
-# or we randomly genrate the nonce when we create the JWe.
+# or we randomly generate the nonce when we create the JWe.
 # To double check implementation we encrypt/decrypt our own input and then
 # decrypt the reference and check it against the given plaintext
 class Cookbook08JWETests(unittest.TestCase):
 
     def test_5_1_encryption(self):
         plaintext = Payload_plaintext_5
         protected = base64url_decode(JWE_Protected_Header_5_1_4)
```

### Comparing `jwcrypto-1.4.2/jwcrypto/tests.py` & `jwcrypto-1.5.0/jwcrypto/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -290,15 +290,74 @@
         },
         {
             "kty": "EC",
             "crv": "P-256K",
             "x": "Ss6na3mcci8Ud4lQrjaB_T40sfKApEcl2RLIWOJdjow",
             "y": "7l9qIKtKPW6oEiOYBt7r22Sm0mtFJU-yBkkvMvpscd8",
             "d": "GYhU2vrYGZrjLZn71Xniqm54Mi53xiYtaTLawzaf9dA"
+        }
+    ]
+}
+
+PublicKeys_brainpool = {
+    "keys": [
+        {
+            "kty": "EC",
+            "crv": "BP-256",
+            "x": "mpkJ29_CYAD0mzQ_MsrbjFMFYtcc9Oxpro37Fa4cLfI",
+            "y": "iBfhNHk0cI73agNpjbKW62dvuVxn7kxp1Sm8oDnzHl8",
+        },
+        {
+            "kty": "EC",
+            "crv": "BP-384",
+            "x": ("WZanneaC2Hi3xslA4znJv7otyEdV5dTPzNUvBjBXPM"
+                  "ytf4mRY9JaAITdItjvUTAh"),
+            "y": ("KNLRTNdvUg66aB_TVW4POZkE3q8S0YoQrCzYUrExRDe"
+                  "_BXikkqIama-GYQ3UBOQL"),
+        },
+        {
+            "kty": "EC",
+            "crv": "BP-512",
+            "x": ("aQXpvz7DH9OK5eFNO9dY3BdPY1v0-8Rg9KC322PY1Jy"
+                  "BJq3EhT0uR_-tgbL2E_aGP6k56lF1xIOOtQxo8zziGA"),
+            "y": ("l9XLHHncigOPr5Tvnj_mVzBFv6i7rdBQrLTq3RXZlCC"
+                  "_f_q6L2o79K9IrN_J2wWxAfS8ekuGPGlHZUzK-3D9sA"),
+        }
+    ]
+}
+
+PrivateKeys_brainpool = {
+    "keys": [
+        {
+            "kty": "EC",
+            "crv": "BP-256",
+            "x": "mpkJ29_CYAD0mzQ_MsrbjFMFYtcc9Oxpro37Fa4cLfI",
+            "y": "iBfhNHk0cI73agNpjbKW62dvuVxn7kxp1Sm8oDnzHl8",
+            "d": "KdKRgq0WEM97BQw3jpW_fTOep6fn-Samv4DfDNb-4s4"
         },
+        {
+            "kty": "EC",
+            "crv": "BP-384",
+            "x": ("WZanneaC2Hi3xslA4znJv7otyEdV5dTPzNUvBjBXPM"
+                  "ytf4mRY9JaAITdItjvUTAh"),
+            "y": ("KNLRTNdvUg66aB_TVW4POZkE3q8S0YoQrCzYUrExRDe"
+                  "_BXikkqIama-GYQ3UBOQL"),
+            "d": ("B5WeRV0-RztAPAhRbphSAUrsIzy-eSfWGSM5FxOQGlJ"
+                  "cq-ECLA_-SIlH7NdWIEJY")
+        },
+        {
+            "kty": "EC",
+            "crv": "BP-512",
+            "x": ("aQXpvz7DH9OK5eFNO9dY3BdPY1v0-8Rg9KC322PY1Jy"
+                  "BJq3EhT0uR_-tgbL2E_aGP6k56lF1xIOOtQxo8zziGA"),
+            "y": ("l9XLHHncigOPr5Tvnj_mVzBFv6i7rdBQrLTq3RXZlCC"
+                  "_f_q6L2o79K9IrN_J2wWxAfS8ekuGPGlHZUzK-3D9sA"),
+            "d": ("F_LJ9rebAjOtxoMUfngIywYsnJlZNjy3gxNAEvHjSkL"
+                  "m6RUUdLXDwc50EMp0LeTh1ku039D5kldK3S9Xi0yKZA")
+        }
     ]
 }
 
 Ed25519PrivatePEM = b"""-----BEGIN PRIVATE KEY-----
 MC4CAQAwBQYDK2VwBCIEIEh4ImJiiZgSNg9J9I+Z5toHKh6LDO2MCbSYNZTkMXDU
 -----END PRIVATE KEY-----
 """
@@ -368,27 +427,45 @@
         key = jwk.JWK.generate(kty='oct', size=128)
         e = jwe.JWE('test', '{"alg":"A128KW","enc":"A128GCM"}')
         e.add_recipient(key)
         enc = e.serialize()
         e.deserialize(enc, key)
         self.assertEqual(e.payload.decode('utf-8'), 'test')
 
+        # also test key generation with input_keysize != keysize
+        key = jwk.JWK.generate(kty='oct', alg="A128CBC-HS256")
+        self.assertEqual(len(base64url_decode(key['k'])), 32)
+        e = jwe.JWE('test', '{"alg":"A256KW","enc":"A128CBC-HS256"}')
+        e.add_recipient(key)
+        enc = e.serialize()
+        e.deserialize(enc, key)
+        self.assertEqual(e.payload.decode('utf-8'), 'test')
+
     def test_generate_EC_key(self):
         # Backwards compat curve
         key = jwk.JWK.generate(kty='EC', curve='P-256')
         key.get_op_key('verify', 'P-256')
         # New param
         key = jwk.JWK.generate(kty='EC', crv='P-521')
         key.get_op_key('verify', 'P-521')
         # New param prevails
         key = jwk.JWK.generate(kty='EC', curve='P-256', crv='P-521')
         key.get_op_key('verify', 'P-521')
         # New secp256k curve
         key = jwk.JWK.generate(kty='EC', curve='secp256k1')
         key.get_op_key('verify', 'secp256k1')
+        # Brainpool256R1 curve
+        key = jwk.JWK.generate(kty='EC', crv='BP-256')
+        key.get_op_key('verify', 'BP-256')
+        # Brainpool384R1 curve
+        key = jwk.JWK.generate(kty='EC', crv='BP-384')
+        key.get_op_key('verify', 'BP-384')
+        # Brainpool256R1 curve
+        key = jwk.JWK.generate(kty='EC', crv='BP-512')
+        key.get_op_key('verify', 'BP-512')
 
     def test_generate_OKP_keys(self):
         for crv in jwk.ImplementedOkpCurves:
             key = jwk.JWK.generate(kty='OKP', crv=crv)
             self.assertEqual(key['crv'], crv)
 
     def test_import_pyca_keys(self):
@@ -424,25 +501,25 @@
         k2 = ks2.get_key(RSAPrivateKey['kid'])
         self.assertEqual(k1, k2)
         self.assertEqual(k1['d'], RSAPrivateKey['d'])
         # test class method import too
         ks3 = jwk.JWKSet.from_json(ks.export())
         self.assertEqual(len(ks), len(ks3))
 
-        # Test key set with mutiple keys
+        # Test key set with multiple keys
         ksm = jwk.JWKSet.from_json(json_encode(PrivateKeys))
         num = 0
         for item in ksm:
             self.assertTrue(isinstance(item, jwk.JWK))
             self.assertTrue(item in ksm)
             num += 1
         self.assertEqual(num, len(PrivateKeys['keys']))
 
     def test_jwkset_get_keys(self):
-        # Test key set with mutiple keys
+        # Test key set with multiple keys
         ksm = jwk.JWKSet.from_json(json_encode(PrivateKeys))
         k1 = jwk.JWK.from_json(json_encode(PrivateKeys['keys'][0]))
         kwargs = RSAPrivateKey.copy()
         kwargs['kid'] = '1'
         k2 = jwk.JWK(**kwargs)
         self.assertEqual(k1, ksm.get_key('1'))
         self.assertIsNone(ksm.get_key('not-there'))
@@ -572,14 +649,24 @@
             jwk.JWK(**key)
 
     def test_create_priKeys_secp256k1(self):
         keylist = PrivateKeys_secp256k1['keys']
         for key in keylist:
             jwk.JWK(**key)
 
+    def test_create_pubKeys_brainpool(self):
+        keylist = PublicKeys_brainpool['keys']
+        for key in keylist:
+            jwk.JWK(**key)
+
+    def test_create_priKeys_brainpool(self):
+        keylist = PrivateKeys_brainpool['keys']
+        for key in keylist:
+            jwk.JWK(**key)
+
     def test_thumbprint_eddsa(self):
         for i in range(0, len(PublicKeys_EdDsa['keys'])):
             k = jwk.JWK(**PublicKeys_EdDsa['keys'][i])
             self.assertEqual(
                 k.thumbprint(),
                 PublicKeys_EdDsa['thumbprints'][i])
 
@@ -877,15 +964,15 @@
         s.verify(decsig)
         # ECDSA signatures are always different every time
         # they are generated unlike RSA or symmetric ones
         if test['key']['kty'] != 'EC':
             self.assertEqual(decsig, test['signature'])
         else:
             # Check we can verify the test signature independently
-            # this is so taht we can test the ECDSA agaist a known
+            # this is so that we can test the ECDSA against a known
             # good signature
             s.verify(test['signature'])
 
     def test_A1(self):
         self.check_sign(A1_example)
 
     def test_A2(self):
@@ -922,15 +1009,15 @@
     def test_A7(self):
         s = jws.JWS(A6_example['payload'])
         s.deserialize(A7_example, A6_example['key2'])
 
     def test_E(self):
         s = jws.JWS(A6_example['payload'])
         with self.assertRaises(jws.InvalidJWSSignature):
-            jws.InvalidJWSSignature(s.deserialize, E_negative)
+            s.deserialize(E_negative)
             s.verify(None)
 
     def test_customhdr_jws(self):
         # Test pass header check
         def jws_chk1(jwobj):
             return jwobj.jose_header['custom1'] == 'custom_val'
 
@@ -983,14 +1070,39 @@
         jws_test.add_signature(key, None, json_encode({"alg": "ES256K"}), None)
         jws_test_serialization_compact = jws_test.serialize(compact=True)
         jws_verify = jws.JWS()
         jws_verify.deserialize(jws_test_serialization_compact)
         jws_verify.verify(key.public())
         self.assertEqual(jws_verify.payload, payload)
 
+    def test_brainpool_signing_and_verification(self):
+        for key_data in PrivateKeys_brainpool['keys']:
+            key = jwk.JWK(**key_data)
+            payload = bytes(bytearray(A1_payload))
+            jws_test = jws.JWS(payload)
+
+            curve_name = key.get('crv')
+            if curve_name == "BP-256":
+                alg = "BP256R1"
+            elif curve_name == "BP-384":
+                alg = "BP384R1"
+            else:
+                alg = "BP512R1"
+
+            jws_test.allowed_algs = [alg]
+            jws_test.add_signature(key, None, json_encode({"alg": alg}), None)
+            jws_test_serialization_compact = jws_test.serialize(compact=True)
+
+            jws_verify = jws.JWS()
+            jws_verify.allowed_algs = [alg]
+            jws_verify.deserialize(jws_test_serialization_compact)
+            jws_verify.verify(key.public())
+
+            self.assertEqual(jws_verify.payload, payload)
+
     def test_jws_issue_224(self):
         key = jwk.JWK().generate(kty='oct')
 
         # Test Empty payload is supported for creating and verifying signatures
         s = jws.JWS(payload='')
         s.add_signature(key, None, json_encode({"alg": "HS256"}))
         o1 = s.serialize(compact=True)
@@ -1779,15 +1891,15 @@
         key.key_ops = None
 
         token = jwt.JWT(header={"alg": "A256KW", "enc": "A256GCM"},
                         claims=claims)
         token.make_encrypted_token(key)
         enctok = token.serialize()
 
-        # test workaroud for older applications
+        # test workaround for older applications
         jwt.JWT_expect_type = False
         jwt.JWT(jwt=enctok, key=key)
         jwt.JWT_expect_type = True
 
         token.validate(key)
         token.expected_type = "JWE"
         token.validate(key)
```

### Comparing `jwcrypto-1.4.2/jwcrypto.egg-info/PKG-INFO` & `jwcrypto-1.5.0/jwcrypto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwcrypto
-Version: 1.4.2
+Version: 1.5.0
 Summary: Implementation of JOSE Web standards
 Home-page: https://github.com/latchset/jwcrypto
 Maintainer: JWCrypto Project Contributors
 Maintainer-email: simo@redhat.com
 License: LGPLv3+
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `jwcrypto-1.4.2/setup.py` & `jwcrypto-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
         'Programming Language :: Python :: 3.10',
         'Intended Audience :: Developers',
         'Topic :: Security',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     data_files = [('share/doc/jwcrypto', ['LICENSE', 'README.md'])],
     install_requires = [
-        'cryptography >= 2.3',
+        'cryptography >= 3.4',
         'deprecated',
     ],
     python_requires = '>= 3.6',
 )
```

### Comparing `jwcrypto-1.4.2/tox.ini` & `jwcrypto-1.5.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -54,14 +54,21 @@
 basepython = python3.10
 changedir = docs/source
 deps =
     sphinx
 commands =
     sphinx-build -v -W -b doctest -d {envtmpdir}/doctrees . {envtmpdir}/doctest
 
+[testenv:codespell]
+basepython = python3.10
+deps =
+    codespell
+commands =
+    codespell --ignore-words-list="ser,ect" jwcrypto
+
 [pytest]
 python_files = jwcrypto/test*.py
 
 [flake8]
 exclude = .tox,*.egg,dist,build,docs/source
 show-source = true
 max-line-length = 79
```

