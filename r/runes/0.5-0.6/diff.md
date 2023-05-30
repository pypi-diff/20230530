# Comparing `tmp/runes-0.5.tar.gz` & `tmp/runes-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-0.5.tar", last modified: Wed Jun 22 04:03:18 2022, max compression
+gzip compressed data, was "runes-0.6.tar", last modified: Tue May 30 02:36:38 2023, max compression
```

## Comparing `runes-0.5.tar` & `runes-0.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 rusty     (1000) rusty     (1000)        0 2022-06-22 04:03:18.820399 runes-0.5/
--rw-rw-r--   0 rusty     (1000) rusty     (1000)     7466 2022-06-22 04:03:18.820399 runes-0.5/PKG-INFO
--rw-rw-r--   0 rusty     (1000) rusty     (1000)     7177 2022-06-22 04:00:53.000000 runes-0.5/README.md
-drwxrwxr-x   0 rusty     (1000) rusty     (1000)        0 2022-06-22 04:03:18.820399 runes-0.5/runes/
--rw-rw-r--   0 rusty     (1000) rusty     (1000)      351 2022-06-22 04:01:39.000000 runes-0.5/runes/__init__.py
--rw-rw-r--   0 rusty     (1000) rusty     (1000)    17453 2022-06-22 04:00:53.000000 runes-0.5/runes/runes.py
-drwxrwxr-x   0 rusty     (1000) rusty     (1000)        0 2022-06-22 04:03:18.820399 runes-0.5/runes.egg-info/
--rw-rw-r--   0 rusty     (1000) rusty     (1000)     7466 2022-06-22 04:03:18.000000 runes-0.5/runes.egg-info/PKG-INFO
--rw-rw-r--   0 rusty     (1000) rusty     (1000)      219 2022-06-22 04:03:18.000000 runes-0.5/runes.egg-info/SOURCES.txt
--rw-rw-r--   0 rusty     (1000) rusty     (1000)        1 2022-06-22 04:03:18.000000 runes-0.5/runes.egg-info/dependency_links.txt
--rw-rw-r--   0 rusty     (1000) rusty     (1000)        7 2022-06-22 04:03:18.000000 runes-0.5/runes.egg-info/requires.txt
--rw-rw-r--   0 rusty     (1000) rusty     (1000)        6 2022-06-22 04:03:18.000000 runes-0.5/runes.egg-info/top_level.txt
--rw-rw-r--   0 rusty     (1000) rusty     (1000)        1 2021-07-30 01:51:57.000000 runes-0.5/runes.egg-info/zip-safe
--rw-rw-r--   0 rusty     (1000) rusty     (1000)       38 2022-06-22 04:03:18.820399 runes-0.5/setup.cfg
--rw-rw-r--   0 rusty     (1000) rusty     (1000)     1218 2021-08-03 04:05:21.000000 runes-0.5/setup.py
+drwxrwxr-x   0 rusty     (1000) rusty     (1000)        0 2023-05-30 02:36:38.427871 runes-0.6/
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)     7464 2023-05-30 02:36:38.427871 runes-0.6/PKG-INFO
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)     7195 2023-05-30 02:29:12.000000 runes-0.6/README.md
+drwxrwxr-x   0 rusty     (1000) rusty     (1000)        0 2023-05-30 02:36:38.427871 runes-0.6/runes/
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)      351 2023-05-30 02:36:12.000000 runes-0.6/runes/__init__.py
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)    17377 2023-05-30 02:29:12.000000 runes-0.6/runes/runes.py
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)     4342 2023-05-30 02:28:59.000000 runes-0.6/runes/sha256.py
+drwxrwxr-x   0 rusty     (1000) rusty     (1000)        0 2023-05-30 02:36:38.427871 runes-0.6/runes.egg-info/
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)     7464 2023-05-30 02:36:38.000000 runes-0.6/runes.egg-info/PKG-INFO
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)      249 2023-05-30 02:36:38.000000 runes-0.6/runes.egg-info/SOURCES.txt
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)        1 2023-05-30 02:36:38.000000 runes-0.6/runes.egg-info/dependency_links.txt
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)        6 2023-05-30 02:36:38.000000 runes-0.6/runes.egg-info/top_level.txt
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)        1 2021-07-30 01:51:57.000000 runes-0.6/runes.egg-info/zip-safe
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)       38 2023-05-30 02:36:38.427871 runes-0.6/setup.cfg
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)     1075 2023-05-30 02:29:02.000000 runes-0.6/setup.py
+drwxrwxr-x   0 rusty     (1000) rusty     (1000)        0 2023-05-30 02:36:38.427871 runes-0.6/tests/
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)    15018 2023-05-30 02:28:59.000000 runes-0.6/tests/test_runes.py
+-rw-rw-r--   0 rusty     (1000) rusty     (1000)    11618 2023-05-30 02:29:12.000000 runes-0.6/tests/test_vectors.py
```

### Comparing `runes-0.5/PKG-INFO` & `runes-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: runes
-Version: 0.5
+Version: 0.6
 Summary: Simple Cookies You Can Extend (similar to Macaroons)
 Home-page: http://github.com/rustyrussell/runes
 Author: Rusty Russell
 Author-email: rusty@rustcorp.com.au
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Runes - Simple Cookies You Can Extend (similar to Macaroons)
 
 https://research.google/pubs/pub41892/ is a paper called "Macaroons:
 Cookies with Contextual Caveats for Decentralized Authorization in the
 Cloud".  It has one good idea, some extended ideas nobody implements,
@@ -34,15 +33,17 @@
 one of which can pass.
 
 The form of each alternative is a simple string:
 
     ALTERNATIVE := FIELDNAME CONDITION VALUE
 
 `FIELDNAME` contains only UTF-8 characters, exclusive of
-! " # $ % & ' ( ) * +, - . / : ;  ? @ [ \ ] ^ _ \` { | } ~ (C's ispunct()).
+! " # $ % & ' ( ) * + , - . / : ;  ? @ [ \ ] ^ \` { | } ~ < = > 
+
+(C's ispunct(), minus `_`).
 These can appear inside a `VALUE`, but `&`, `|` and `\\` must be escaped with `\` (escaping is legal for any character, but unnecessary).
 
 
 `CONDITION` is one of the following values:
 * `!`: Pass if field is missing (value ignored)
 * `=`: Pass if exists and exactly equals
 * `/`: Pass if exists and is not exactly equal
@@ -211,9 +212,7 @@
 
 
 ## Author
 
 Rusty Russell wrote it; but I blame @roasbeef for raving about them
 long enough at LnConf that I actually read the paper.  It only took me
 18 months to find a day to implement them.
-
-
```

### Comparing `runes-0.5/README.md` & `runes-0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 one of which can pass.
 
 The form of each alternative is a simple string:
 
     ALTERNATIVE := FIELDNAME CONDITION VALUE
 
 `FIELDNAME` contains only UTF-8 characters, exclusive of
-! " # $ % & ' ( ) * +, - . / : ;  ? @ [ \ ] ^ _ \` { | } ~ (C's ispunct()).
+! " # $ % & ' ( ) * + , - . / : ;  ? @ [ \ ] ^ \` { | } ~ < = > 
+
+(C's ispunct(), minus `_`).
 These can appear inside a `VALUE`, but `&`, `|` and `\\` must be escaped with `\` (escaping is legal for any character, but unnecessary).
 
 
 `CONDITION` is one of the following values:
 * `!`: Pass if field is missing (value ignored)
 * `=`: Pass if exists and exactly equals
 * `/`: Pass if exists and is not exactly equal
```

### Comparing `runes-0.5/runes/runes.py` & `runes-0.6/runes/runes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import base64
 import copy
 import hashlib
 import re
-# We can't use the hashlib one, since we need midstate access :(
-import sha256  # type: ignore
-import string
 from typing import Dict, List, Sequence, Optional, Tuple, Any, Union
-
+from .sha256 import sha256
 
 def padlen_64(x: int):
     """Amount which will increase x until it's divisible evenly by 64"""
     return (64 - (x % 64)) % 64
 
 
 def end_shastream(length: int):
     """Simulate an SHA-256 ending pad (1 bit, zero bad, 64-bit length)"""
     padlen = padlen_64(length + 1 + 8)
     return bytes([0x80]) + bytes(padlen) + int.to_bytes(length * 8, 8, 'big')
 
 
 class Alternative(object):
+    SEPARATORS=set('!"#$%&\'()*+,-./:;?@[\\]^`{|}~<=>')
     """One of possibly several conditions which could be met"""
     def __init__(self, field: str, cond: str, value: str, allow_idfield: bool = False):
-        if any([c in string.punctuation for c in field]):
+        if any([c in self.SEPARATORS for c in field]):
             raise ValueError("field not valid")
         if cond not in ('!', '=', '/', '^', '$', '~', '<', '>', '}', '{', '#'):
             raise ValueError("cond not valid")
         if field == '':
             if not allow_idfield:
                 raise ValueError("unique_id field not valid here")
             if cond != '=':
@@ -129,15 +127,15 @@
     def decode(cls, encstr: str, allow_idfield: bool = False) -> Tuple['Alternative', str]:
         """Pull an Alternative from encoded string, return remainder"""
         cond = None
         end_off = 0
 
         # Swallow field up to conditiona
         while end_off < len(encstr):
-            if encstr[end_off] in string.punctuation:
+            if encstr[end_off] in cls.SEPARATORS:
                 cond = encstr[end_off]
                 break
             end_off += 1
         if cond is None:
             raise ValueError('{} does not contain any operator'
                              .format(encstr))
         field = encstr[:end_off]
@@ -158,15 +156,15 @@
 
         return cls(field, cond, value, allow_idfield), encstr[end_off:]
 
     @classmethod
     def from_str(cls, encstr: str) -> 'Alternative':
         """Turns this user-readable string into an Alternative (no escaping)"""
         encstr = re.sub(r'\s+', '', encstr)
-        parts = re.split('([' + string.punctuation + '])', encstr, maxsplit=1)
+        parts = re.split('([' + ''.join(re.escape(s) for s in cls.SEPARATORS) + '])', encstr, maxsplit=1)
         return cls(parts[0], parts[1], parts[2])
 
     def __eq__(self, other) -> bool:
         return (self.field == other.field
                 and self.value == other.value
                 and self.cond == other.cond)
 
@@ -248,16 +246,17 @@
                  restrictions: Sequence[Restriction] = []):
         """Convenient constructor: adds unique_id, version and any other restrictions"""
         assert isinstance(unique_id, (int, str, type(None)))
         assert isinstance(version, (int, str, type(None)))
         self.restrictions: List[Restriction] = []
 
         # Replace with real shastate (aka authcode)
-        self.shaobj = sha256.sha256()
-        self.shaobj.state = (authbase, 64)
+        self.shaobj = sha256()
+        self.shaobj._counter = 64
+        self.shaobj.set_midstate(authbase)
 
         # If they provide a unique_id, it goes first.
         if unique_id is not None:
             self.add_restriction(Restriction.unique_id(unique_id, version))
 
         for r in restrictions:
             self.add_restriction(r)
@@ -267,26 +266,26 @@
                       authcode: bytes,
                       restrictions: Sequence[Restriction]):
         """Alternate constructor when authcode already calculated with these restrictions"""
         ret = cls(authcode)
         ret.restrictions = list(restrictions)
 
         # SHA state needs to simply be updated to cover this length.
-        runelength = ret.shaobj.state[1]
+        runelength = ret.shaobj._counter
         for r in ret.restrictions:
             runelength += len(r.encode())
             runelength += padlen_64(runelength)
 
-        ret.shaobj.state = (ret.shaobj.state[0], runelength)
+        ret.shaobj._counter = runelength
         return ret
 
     def add_restriction(self, restriction: Restriction) -> None:
         self.restrictions.append(restriction)
         self.shaobj.update(bytes(restriction.encode(), encoding='utf8'))
-        self.shaobj.update(end_shastream(self.shaobj.state[1]))
+        self.shaobj.update(end_shastream(self.shaobj._counter))
 
     def are_restrictions_met(self, values: Dict[str, Any]) -> Tuple[bool, str]:
         """Tests the restrictions against the values dict given.  Normally
         values are treated strings, but < and > conditions only work
         if they're actually integers.
 
         Returns (True, '') if everything is good.  Otherwise, returns
@@ -296,15 +295,15 @@
         for r in self.restrictions:
             reasons = r.test(values)
             if reasons is not None:
                 return False, reasons
         return True, ''
 
     def authcode(self) -> bytes:
-        return self.shaobj.state[0]
+        return self.shaobj.midstate()
 
     def to_str(self) -> str:
         return (self.authcode().hex()
                 + ':'
                 + '&'.join([r.encode() for r in self.restrictions]))
 
     def to_base64(self) -> str:
@@ -332,27 +331,27 @@
     @classmethod
     def from_base64(cls, b64str: str) -> 'Rune':
         binstr = base64.urlsafe_b64decode(b64str)
         return cls.from_str(binstr[:32].hex() + ':' + binstr[32:].decode('utf8'))
 
     def __eq__(self, other) -> bool:
         return (self.restrictions == other.restrictions
-                and self.shaobj.state == other.shaobj.state)
+                and self.shaobj == other.shaobj)
 
     def copy(self) -> 'Rune':
         """Perform a shallow copy"""
         return self.__copy__()
 
     def __copy__(self) -> 'Rune':
         # You don't want to share the shaobj!
-        return self.from_authcode(self.shaobj.state[0], self.restrictions)
+        return self.from_authcode(self.shaobj.midstate(), self.restrictions)
 
     def __deepcopy__(self, memo=None) -> 'Rune':
         """sha256.sha256 doesn't implement pickle"""
-        return self.from_authcode(self.shaobj.state[0], copy.deepcopy(self.restrictions))
+        return self.from_authcode(self.shaobj.midstate(), copy.deepcopy(self.restrictions))
 
 
 class MasterRune(Rune):
     """This is where the server creates the Rune; it's recommended you
 give each rune a unique id (often a persistent counter) (with an
 optional version), which gets included as an empty-fieldname field.
 
@@ -365,15 +364,15 @@
         # If they provide a unique_id, it goes first.
         if unique_id is not None:
             restrictions = [Restriction.unique_id(unique_id, version)] + list(restrictions)
 
         self.restrictions = []
         # Everyone assumes that seed secret takes 1 block only
         assert len(seedsecret) + 1 + 8 <= 64
-        self.shaobj = sha256.sha256()
+        self.shaobj = sha256()
         self.shaobj.update(seedsecret + end_shastream(len(seedsecret)))
         for r in restrictions:
             self.add_restriction(r)
 
         # For fast calc using hashlib
         self.shabase = hashlib.sha256()
         self.shabase.update(seedsecret)
@@ -383,24 +382,23 @@
         """Perform a shallow copy"""
         return self.__copy__()
 
     def __copy__(self) -> 'MasterRune':
         # Create dummy so we can populate it (we don't store secret)
         ret = MasterRune(bytes())
         ret.restrictions = self.restrictions.copy()
-        ret.shaobj.state = self.shaobj.state
+        ret.shaobj = self.shaobj.copy()
         ret.shabase = self.shabase
         ret.seclen = self.seclen
         return ret
 
     def __deepcopy__(self, memo=None) -> 'MasterRune':
-        """sha256.sha256 doesn't implement pickle"""
         ret = MasterRune(bytes())
         ret.restrictions = copy.deepcopy(self.restrictions)
-        ret.shaobj.state = self.shaobj.state
+        ret.shaobj = self.shaobj.copy()
         ret.shabase = self.shabase
         ret.seclen = self.seclen
         return ret
 
     def is_rune_authorized(self, other: Rune) -> bool:
         """This is faster than adding the restrictions one-by-one and checking
         the final authcode (but equivalent)"""
```

### Comparing `runes-0.5/runes.egg-info/PKG-INFO` & `runes-0.6/runes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: runes
-Version: 0.5
+Version: 0.6
 Summary: Simple Cookies You Can Extend (similar to Macaroons)
 Home-page: http://github.com/rustyrussell/runes
 Author: Rusty Russell
 Author-email: rusty@rustcorp.com.au
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # Runes - Simple Cookies You Can Extend (similar to Macaroons)
 
 https://research.google/pubs/pub41892/ is a paper called "Macaroons:
 Cookies with Contextual Caveats for Decentralized Authorization in the
 Cloud".  It has one good idea, some extended ideas nobody implements,
@@ -34,15 +33,17 @@
 one of which can pass.
 
 The form of each alternative is a simple string:
 
     ALTERNATIVE := FIELDNAME CONDITION VALUE
 
 `FIELDNAME` contains only UTF-8 characters, exclusive of
-! " # $ % & ' ( ) * +, - . / : ;  ? @ [ \ ] ^ _ \` { | } ~ (C's ispunct()).
+! " # $ % & ' ( ) * + , - . / : ;  ? @ [ \ ] ^ \` { | } ~ < = > 
+
+(C's ispunct(), minus `_`).
 These can appear inside a `VALUE`, but `&`, `|` and `\\` must be escaped with `\` (escaping is legal for any character, but unnecessary).
 
 
 `CONDITION` is one of the following values:
 * `!`: Pass if field is missing (value ignored)
 * `=`: Pass if exists and exactly equals
 * `/`: Pass if exists and is not exactly equal
@@ -211,9 +212,7 @@
 
 
 ## Author
 
 Rusty Russell wrote it; but I blame @roasbeef for raving about them
 long enough at LnConf that I actually read the paper.  It only took me
 18 months to find a day to implement them.
-
-
```

