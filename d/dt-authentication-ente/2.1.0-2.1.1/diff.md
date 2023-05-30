# Comparing `tmp/dt-authentication-ente-2.1.0.tar.gz` & `tmp/dt-authentication-ente-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-authentication-ente-2.1.0.tar", last modified: Fri May 12 04:20:00 2023, max compression
+gzip compressed data, was "dt-authentication-ente-2.1.1.tar", last modified: Tue May 30 05:45:56 2023, max compression
```

## Comparing `dt-authentication-ente-2.1.0.tar` & `dt-authentication-ente-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.0/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.0/README.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2299 2023-05-07 18:37:07.000000 dt-authentication-ente-2.1.0/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.485245 dt-authentication-ente-2.1.0/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.485245 dt-authentication-ente-2.1.0/src/dt_authentication/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      153 2023-05-12 04:19:55.000000 dt-authentication-ente-2.1.0/src/dt_authentication/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2545 2023-05-12 03:53:49.000000 dt-authentication-ente-2.1.0/src/dt_authentication/cli.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2023-05-07 18:35:09.000000 dt-authentication-ente-2.1.0/src/dt_authentication/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.1.0/src/dt_authentication/scope.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    10981 2023-05-12 04:00:36.000000 dt-authentication-ente-2.1.0/src/dt_authentication/token.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-07 07:29:27.000000 dt-authentication-ente-2.1.0/src/dt_authentication/utils.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-12 04:20:00.489246 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      127 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       13 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-05-12 04:20:00.000000 dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.1/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.1.1/README.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2374 2023-05-23 13:18:48.000000 dt-authentication-ente-2.1.1/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:55.999044 dt-authentication-ente-2.1.1/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:55.999044 dt-authentication-ente-2.1.1/src/dt_authentication/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      253 2023-05-30 05:45:54.000000 dt-authentication-ente-2.1.1/src/dt_authentication/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3659 2023-05-30 05:44:24.000000 dt-authentication-ente-2.1.1/src/dt_authentication/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      482 2023-05-22 20:16:11.000000 dt-authentication-ente-2.1.1/src/dt_authentication/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.1.1/src/dt_authentication/scope.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    13360 2023-05-30 05:44:24.000000 dt-authentication-ente-2.1.1/src/dt_authentication/token.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-22 20:52:39.000000 dt-authentication-ente-2.1.1/src/dt_authentication/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-30 05:45:56.003044 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      179 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       22 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-05-30 05:45:55.000000 dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/top_level.txt
```

### Comparing `dt-authentication-ente-2.1.0/setup.py` & `dt-authentication-ente-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 # The requirements here must be broad.
 # dependencies_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'dependencies.txt')
 # with open(dependencies_file, 'rt') as fin:
 #     dependencies = list(filter(lambda line: not line.startswith('#'), fin.read().splitlines()))
 
 install_requires = [
     'base58',
-    'ecdsa'
+    'ecdsa',
+    'requests'
 ]
 tests_require = []
 
 # compile description
 underline = '=' * (len(package_name) + len(short_description) + 2)
 description = """
 {name}: {short}
@@ -54,14 +55,15 @@
 
 {long}
 """.format(name=package_name, short=short_description, long=full_description, underline=underline)
 
 console_scripts = [
     "dt-tokens-generate = dt_authentication.cli:cli_generate",
     "dt-tokens-verify = dt_authentication.cli:cli_verify",
+    "dt-tokens-keygen = dt_authentication.cli:cli_keygen",
 ]
 
 # setup package
 setup(
     name=package_name,
     author=maintainer,
     author_email=maintainer_email,
```

### Comparing `dt-authentication-ente-2.1.0/src/dt_authentication/cli.py` & `dt-authentication-ente-2.1.1/src/dt_authentication/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import argparse
 import datetime
 import logging
 import sys
+import tempfile
 
 # noinspection PyProtectedMember
-from ecdsa import SigningKey
+from ecdsa import SigningKey, VerifyingKey
 from future import builtins
 
 from dt_authentication import DuckietownToken, InvalidToken
+from dt_authentication.utils import get_or_create_key_pair
 
 logging.basicConfig()
 logger = logging.getLogger("duckietown-tokens ")
 logger.setLevel(logging.INFO)
 
 __all__ = ["cli_verify", "cli_generate"]
 
@@ -30,33 +32,30 @@
         try:
             token = DuckietownToken.from_string(token_s)
         except InvalidToken:
             msg = "Invalid token format."
             logger.error(msg)
             sys.exit(1)
 
-        if token.expired:
-            msg = f"This token has expired on {token.expiration}"
-            logger.error(msg)
-            sys.exit(2)
-
         _print_token_info(token)
         sys.exit(0)
     except Exception as e:
         logger.error(str(e))
         sys.exit(3)
 
 
 def cli_generate(args=None):
     parser = argparse.ArgumentParser()
     parser.add_argument("--uid", type=int, help="ID to sign")
     parser.add_argument("--key", type=str, help="Path to signing key")
-    parser.add_argument("--ndays", type=int, default=365, help="Number of days for validity")
+    parser.add_argument("--ndays", type=int, default=0, help="Number of days for validity")
     parser.add_argument("--nhours", type=int, default=0, help="Number of hours for validity")
     parser.add_argument("--nminutes", type=int, default=0, help="Number of minutes for validity")
+    parser.add_argument("--renewable", action="store_true", default=False, help="Make a renewable token")
+    parser.add_argument("--scope", type=str, default=None, help="Scope as compact comma-separated list")
 
     args = parser.parse_args(args=args)
 
     if args.key is None:
         msg = "Please supply --key "
         raise Exception(msg)
     if args.uid is None:
@@ -71,28 +70,60 @@
     # generate token
     token: DuckietownToken = DuckietownToken.generate(
         key=sk,
         user_id=args.uid,
         days=args.ndays,
         hours=args.nhours,
         minutes=args.nminutes,
-        scope=None,
+        scope=args.scope.split(",") if args.scope else None,
+        renewable=args.renewable
     )
     _print_token_info(token)
 
 
+def cli_keygen(args=None):
+    parser = argparse.ArgumentParser()
+    parser.add_argument("--version", type=str, default="dt2", help="Version of the token")
+    parser.add_argument("--out", type=str, default=None, help="Directory where to write the keys "
+                                                              "(default: print only)")
+    args = parser.parse_args(args=args)
+    # create keys
+    if args.out:
+        sk, vk = get_or_create_key_pair(args.version, args.out)
+    else:
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            sk, vk = get_or_create_key_pair(args.version, tmp_dir)
+    _print_keys(sk, vk)
+
+
+def _print_keys(sk: SigningKey, vk: VerifyingKey):
+    print(f"""
+SigningKey:
+===========
+
+{sk.to_pem().decode()}
+
+
+Verifying Key:
+==============
+
+{vk.to_pem().decode()}
+""")
+
+
 def _print_token_info(token: DuckietownToken):
     exp_info: str = "expired" if token.expired else \
-        f"in {(token.expiration - datetime.datetime.now()).days} days"
+        f"in {token.expiration and (token.expiration - datetime.datetime.utcnow()).days} days"
     print(f"""
 Payload:
 --------
 {token.payload_as_json(sort_keys=True, indent=4).strip("{}")}
 
 Expiration:
 --------\n
+    Expired: {'Yes' if token.expired else 'No'}
     {token.expiration}    -    ({exp_info})
 
 Token:
 --------\n
     {token.as_string()}
     """)
```

### Comparing `dt-authentication-ente-2.1.0/src/dt_authentication/scope.py` & `dt-authentication-ente-2.1.1/src/dt_authentication/scope.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.0/src/dt_authentication/token.py` & `dt-authentication-ente-2.1.1/src/dt_authentication/token.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import copy
 import datetime
 import json
+import os
 from typing import Dict, Union, List, Optional
 
+import requests
 from base58 import b58decode, b58encode
 # noinspection PyProtectedMember
 from ecdsa import NIST192p
 from ecdsa.keys import VerifyingKey, BadSignatureError, SigningKey
 
-from .exceptions import InvalidToken, ExpiredToken
+from .exceptions import InvalidToken, ExpiredToken, GenericException, NotARenewableToken
 from .scope import Scope
 
 PUBLIC_KEYS = {
     # dt1 was introduced in 2017
     "dt1": """-----BEGIN PUBLIC KEY-----
 MEkwEwYHKoZIzj0CAQYIKoZIzj0DAQEDMgAEQr/8RJmJZT+Bh1YMb1aqc2ao5teE
 ixOeCMGTO79Dbvw5dGmHJLYyNPwnKkWayyJS
@@ -37,14 +39,17 @@
 }
 DEFAULT_VERSION = "dt2"
 
 
 ScopeList = List[Union[Scope, str]]
 DEFAULT_SCOPE = [Scope(action="auth")]
 
+TOKEN_RENEW_ONLINE_HOST = os.environ.get("DT_TOKEN_RENEW_HOST", "hub.duckietown.com")
+TOKEN_RENEW_ONLINE_URL = f"https://{TOKEN_RENEW_ONLINE_HOST}/api/v1/auth/token/renew"
+
 
 class DuckietownToken(object):
     """
     Class modeling a Duckietown Token.
 
     Args:
         payload:    The token's payload as a dictionary.
@@ -136,15 +141,15 @@
     def expired(self) -> bool:
         """ Whether the token is already expired """
         exp: Optional[datetime.date] = self.expiration
         if exp is None:
             # never-expiring tokens
             return False
         # compare now() with token expiration date
-        return exp < datetime.datetime.now()
+        return exp < datetime.datetime.utcnow()
 
     def as_string(self) -> str:
         """
         Returns the Duckietown Token string.
         """
         # encode payload into JSON
         payload_json: str = self.payload_as_json()
@@ -163,33 +168,86 @@
         # encode payload into JSON
         payload = copy.deepcopy(self._payload)
         payload["scope"] = scope
         return json.dumps(payload, sort_keys=sort_keys, **kwargs)
 
     def grants(self, action: str, resource: Optional[str] = None, identifier: Optional[str] = None,
                service: Optional[str] = None) -> bool:
+        """
+        Checks whether this token grants the given scope.
+
+        :param action:      Action of the scope to check for
+        :param resource:    Resource of the scope to check for
+        :param identifier:  Resource identifier of the scope to check for
+        :param service:     Service of the scope to check for
+        :return:            'True' if this token grants this scope, 'False' otherwise.
+        """
         for s in self.scope:
             if s.grants(action, resource, identifier, service):
                 return True
         return False
 
-    def renew(self, key: SigningKey):
+    def renew(self, key: Optional[SigningKey] = None, in_place: bool = False) -> 'DuckietownToken':
+        """
+        Renews this token using the given signing key or by reaching out to the remote Duckietown auth
+        service if no keys are given.
+
+        :param key:         (Optional) Signing key to use to sign the new token.
+        :param in_place:    Update this very instance with the new token.
+        :return:            A new token with the same scope and duration of the old one.
+        """
         # make sure the token is renewable
         if not self.renewable:
-            raise ValueError("This token is not renewable")
-        # generate new token
-        return self.generate(
-            key,
-            self.uid,
-            minutes=self.duration,
-            renewable=True,
-            data=self.data,
-            scope=self.scope,
-            version=self.version,
-        )
+            raise NotARenewableToken()
+
+        if key is not None:
+            # generate new token with the given key
+            new: DuckietownToken = self.generate(
+                key,
+                self.uid,
+                minutes=self.duration,
+                renewable=True,
+                data=self.data,
+                scope=self.scope,
+                version=self.version,
+            )
+        else:
+            # request new token
+            try:
+                response = requests.get(
+                    url=TOKEN_RENEW_ONLINE_URL,
+                    headers={
+                        "Authorization": f"Token {self.as_string()}"
+                    }
+                ).json()
+            except requests.RequestException as e:
+                raise e
+            except requests.JSONDecodeError as e:
+                raise e
+            # ---
+            if not response["success"]:
+                raise GenericException(response["messages"])
+            # parse new token
+            new: DuckietownToken = DuckietownToken.from_string(response["result"]["token"])
+        # apply in-place edits
+        if in_place:
+            # copy token content
+            self.copy_from(new)
+        # ---
+        return new
+
+    def copy_from(self, other: 'DuckietownToken'):
+        """
+        Turns this instance into an exact copy of the given token.
+
+        :param other:   The token to duplicate.
+        """
+        self._version = other._version
+        self._payload = other._payload
+        self._signature = other._signature
 
     @staticmethod
     def from_string(s: str, vk: Optional[VerifyingKey] = None, allow_expired: bool = True) \
             -> 'DuckietownToken':
         """
         Decodes a Duckietown Token string into an instance of
         :py:class:`dt_authentication.DuckietownToken`.
@@ -252,15 +310,15 @@
                  # metadata
                  version: str = DEFAULT_VERSION) -> 'DuckietownToken':
         # get supported fields for version
         fields = SUPPORTED_FIELDS[version]
         # compute expiration date
         exp = None
         if (days + hours + minutes) > 0:
-            now = datetime.datetime.now()
+            now = datetime.datetime.utcnow()
             delta = datetime.timedelta(days=days, hours=hours, minutes=minutes)
             exp = (now + delta).strftime(DATETIME_FORMAT[version])
         # initialize payload
         payload = {
             "uid": user_id,
             "exp": exp
         }
```

### Comparing `dt-authentication-ente-2.1.0/src/dt_authentication/utils.py` & `dt-authentication-ente-2.1.1/src/dt_authentication/utils.py`

 * *Files identical despite different names*

### Comparing `dt-authentication-ente-2.1.0/src/dt_authentication_ente.egg-info/SOURCES.txt` & `dt-authentication-ente-2.1.1/src/dt_authentication_ente.egg-info/SOURCES.txt`

 * *Files identical despite different names*

