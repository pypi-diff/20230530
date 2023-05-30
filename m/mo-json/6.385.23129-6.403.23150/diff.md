# Comparing `tmp/mo_json-6.385.23129-py2.py3-none-any.whl.zip` & `tmp/mo_json-6.403.23150-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 31569 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat    13208 b- defN 23-Apr-14 10:26 mo_json/__init__.py
+Zip file size: 31606 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat    13329 b- defN 23-May-30 00:28 mo_json/__init__.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-14 10:26 mo_json/decoder.py
 -rw-rw-rw-  2.0 fat    15429 b- defN 23-Apr-14 10:26 mo_json/encoder.py
 -rw-rw-rw-  2.0 fat    16185 b- defN 23-Apr-14 10:26 mo_json/stream.py
 -rw-rw-rw-  2.0 fat    17835 b- defN 23-May-04 10:50 mo_json/typed_encoder.py
 -rw-rw-rw-  2.0 fat     2896 b- defN 23-May-04 10:50 mo_json/typed_object.py
 -rw-rw-rw-  2.0 fat    10240 b- defN 23-Apr-30 12:14 mo_json/types.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-May-09 23:31 mo_json-6.385.23129.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11595 b- defN 23-May-09 23:31 mo_json-6.385.23129.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-09 23:31 mo_json-6.385.23129.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-09 23:31 mo_json-6.385.23129.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      956 b- defN 23-May-09 23:31 mo_json-6.385.23129.dist-info/RECORD
-12 files, 105500 bytes uncompressed, 29987 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11595 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      956 b- defN 23-May-30 00:28 mo_json-6.403.23150.dist-info/RECORD
+12 files, 105621 bytes uncompressed, 30024 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: mo_json/typed_object.py
 Comment: 
 
 Filename: mo_json/types.py
 Comment: 
 
-Filename: mo_json-6.385.23129.dist-info/LICENSE
+Filename: mo_json-6.403.23150.dist-info/LICENSE
 Comment: 
 
-Filename: mo_json-6.385.23129.dist-info/METADATA
+Filename: mo_json-6.403.23150.dist-info/METADATA
 Comment: 
 
-Filename: mo_json-6.385.23129.dist-info/WHEEL
+Filename: mo_json-6.403.23150.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json-6.385.23129.dist-info/top_level.txt
+Filename: mo_json-6.403.23150.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json-6.385.23129.dist-info/RECORD
+Filename: mo_json-6.403.23150.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_json/__init__.py

```diff
@@ -7,36 +7,39 @@
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 import math
 from datetime import timedelta, timezone
 
 from hjson import loads as hjson2value
+
 from mo_dots import (
     Data,
     FlatList,
     Null,
     SLOT,
     to_data,
     leaves_to_data,
     null_types,
 )
 from mo_dots.objects import DataObject
-from mo_logs import Except, Log, strings
-from mo_logs.strings import expand_template
-from mo_times import Date, Duration
-
 from mo_future import (
     integer_types,
     is_binary,
     is_text,
 )
+from mo_imports import delay_import
 from mo_json.types import *
+from mo_logs import Except, strings
+from mo_logs.strings import expand_template
+from mo_times import Duration
 
-FIND_LOOPS = False
+logger = delay_import("mo_logs.logger")
+
+FIND_LOOPS = True  # FIND LOOPS IN DATA STRUCTURES
 SNAP_TO_BASE_10 = False  # Identify floats near a round base10 value (has 000 or 999) and shorten
 CAN_NOT_DECODE_JSON = "Can not decode JSON"
 
 
 true, false, null = True, False, None
 
 _get = object.__getattribute__
@@ -86,17 +89,15 @@
             return sign + (digits[: 1 + int_exp] + "." + digits[1 + int_exp :].rstrip("0")).rstrip(".")
         elif -4 < int_exp:
             digits = ("0" * (-int_exp)) + digits
             return sign + (digits[:1] + "." + digits[1:].rstrip("0")).rstrip(".")
         else:
             return sign + digits[0] + "." + (digits[1:].rstrip("0") or "0") + "e" + text(int_exp)
     except Exception as e:
-        from mo_logs import Log
-
-        Log.error("not expected", e)
+        logger.error("not expected", e)
 
 
 def _snap_to_base_10(mantissa):
     # TODO: https://lists.nongnu.org/archive/html/gcl-devel/2012-10/pdfkieTlklRzN.pdf
     digits = mantissa.replace(".", "")
     if SNAP_TO_BASE_10:
         f9 = strings.find(digits, "999")
@@ -149,15 +150,15 @@
     return _scrub(value, set(), [], scrub_text=scrub_text, scrub_number=scrub_number)
 
 
 def _scrub(value, is_done, stack, scrub_text, scrub_number):
     if FIND_LOOPS:
         _id = id(value)
         if _id in stack and type(_id).__name__ not in ["int"]:
-            Log.error("loop in JSON")
+            logger.error("loop in JSON")
         stack = stack + [_id]
     type_ = value.__class__
 
     if type_ in null_types:
         return None
     elif type_ is text:
         return scrub_text(value)
@@ -182,31 +183,31 @@
     elif type_ is Decimal:
         return scrub_number(value)
     elif type_ is Data:
         return _scrub(_get(value, SLOT), is_done, stack, scrub_text, scrub_number)
     elif is_data(value):
         _id = id(value)
         if _id in is_done:
-            Log.warning("possible loop in structure detected")
+            # logger.warning("possible loop in structure detected")
             return '"<LOOP IN STRUCTURE>"'
         is_done.add(_id)
-
-        output = {}
-        for k, v in value.items():
-            if is_text(k):
-                pass
-            elif is_binary(k):
-                k = k.decode("utf8")
-            else:
-                Log.error("keys must be strings")
-            v = _scrub(v, is_done, stack, scrub_text, scrub_number)
-            if v != None or is_data(v):
-                output[k] = v
-
-        is_done.discard(_id)
+        try:
+            output = {}
+            for k, v in value.items():
+                if is_text(k):
+                    pass
+                elif is_binary(k):
+                    k = k.decode("utf8")
+                else:
+                    logger.error("keys must be strings")
+                v = _scrub(v, is_done, stack, scrub_text, scrub_number)
+                if v != None or is_data(v):
+                    output[k] = v
+        finally:
+            is_done.discard(_id)
         return output
     elif type_ in (tuple, list, FlatList):
         output = []
         for v in value:
             v = _scrub(v, is_done, stack, scrub_text, scrub_number)
             output.append(v)
         return output  # if output else None
@@ -224,20 +225,20 @@
             j = value.__json__()
             if is_text(j):
                 data = json_decoder(j)
             else:
                 data = json_decoder("".join(j))
             return _scrub(data, is_done, stack, scrub_text, scrub_number)
         except Exception as cause:
-            Log.error("problem with calling __json__()", cause)
+            logger.error("problem with calling __json__()", cause)
     elif hasattr(value, "__data__"):
         try:
             return _scrub(value.__data__(), is_done, stack, scrub_text, scrub_number)
         except Exception as cause:
-            Log.error("problem with calling __data__()", cause)
+            logger.error("problem with calling __data__()", cause)
     elif hasattr(value, "co_code") or hasattr(value, "f_locals"):
         return None
     elif hasattr(value, "__iter__"):
         output = []
         for v in value:
             v = _scrub(v, is_done, stack, scrub_text, scrub_number)
             output.append(v)
@@ -260,27 +261,27 @@
     :return:
     """
     if FIND_LOOPS:
         obj = scrub(obj, scrub_text=_keep_whitespace if keep_whitespace else trim_whitespace)
     try:
         json = json_encoder(obj, pretty=pretty)
         if json == None:
-            Log.note(
+            logger.note(
                 str(type(obj)) + " is not valid{{type}}JSON", type=" (pretty) " if pretty else " ",
             )
-            Log.error("Not valid JSON: " + str(obj) + " of type " + str(type(obj)))
+            logger.error("Not valid JSON: " + str(obj) + " of type " + str(type(obj)))
         return json
     except Exception as e:
         e = Except.wrap(e)
         try:
             json = pypy_json_encode(obj)
             return json
         except Exception:
             pass
-        Log.error("Can not encode into JSON: {{value}}", value=text(repr(obj)), cause=e)
+        logger.error("Can not encode into JSON: {{value}}", value=text(repr(obj)), cause=e)
 
 
 def remove_line_comment(line):
     mode = 0  # 0=code, 1=inside_string, 2=escaping
     for i, c in enumerate(line):
         if c == '"':
             if mode == 0:
@@ -335,15 +336,15 @@
             e += 1
             expecting[e] = "]"
             i += 1
         elif c in "]}":
             if expecting[e] == c:
                 e -= 1
             else:
-                Log.error("invalid JSON")
+                logger.error("invalid JSON")
             i += 1
         else:
             i += 1
 
 
 def json2value(json_string, params=Null, flexible=False, leaves=False):
     """
@@ -351,15 +352,15 @@
     :param params: STANDARD JSON PARAMS
     :param flexible: REMOVE COMMENTS
     :param leaves: ASSUME JSON KEYS ARE DOT-DELIMITED
     :return: Python value
     """
     json_string = text(json_string)
     if not is_text(json_string) and json_string.__class__.__name__ != "FileString":
-        Log.error("only unicode json accepted")
+        logger.error("only unicode json accepted")
 
     try:
         if params:
             # LOOKUP REFERENCES
             json_string = expand_template(json_string, params)
 
         if flexible:
@@ -372,15 +373,15 @@
 
         return value
 
     except Exception as e:
         e = Except.wrap(e)
 
         if not json_string.strip():
-            Log.error("JSON string is only whitespace")
+            logger.error("JSON string is only whitespace")
 
         c = e
         while c.cause and "Expecting '" in c.cause and "' delimiter: line" in c.cause:
             c = c.cause
 
         if "Expecting '" in c and "' delimiter: line" in c:
             line_index = int(strings.between(c.message, " line ", " column ")) - 1
@@ -392,25 +393,25 @@
             else:
                 sample = line
                 pointer = (" " * column) + "^"
 
             if len(sample) > 43:
                 sample = sample[:43] + "..."
 
-            Log.error(
+            logger.error(
                 CAN_NOT_DECODE_JSON + " at:\n\t{{sample}}\n\t{{pointer}}\n", sample=sample, pointer=pointer,
             )
 
         base_str = strings.limit(json_string, 1000).encode("utf8")
         hexx_str = bytes2hex(base_str, " ")
         try:
             char_str = " " + "  ".join((chr(c) if c >= 32 else ".") for c in base_str)
         except Exception as cause:
             char_str = " "
-        Log.error(
+        logger.error(
             CAN_NOT_DECODE_JSON + ":\n{{char_str}}\n{{hexx_str}}\n", char_str=char_str, hexx_str=hexx_str, cause=e,
         )
 
 
 def bytes2hex(value, separator=" "):
     return separator.join("{:02X}".format(x) for x in value)
 
@@ -430,20 +431,16 @@
             else:
                 diff = value - DATETIME_EPOCH.replace(tzinfo=None)
             return diff.total_seconds()
         elif isinstance(value, date):
             diff = value - DATE_EPOCH
             return diff.total_seconds()
         else:
-            from mo_logs import Log
-
-            Log.error(
+            logger.error(
                 "Can not convert {{value}} of type {{type}}", value=value, type=value.__class__,
             )
     except Exception as e:
-        from mo_logs import Log
-
-        Log.error("Can not convert {{value}}", value=value, cause=e)
+        logger.error("Can not convert {{value}}", value=value, cause=e)
 
 
 from mo_json.decoder import json_decoder
 from mo_json.encoder import json_encoder, pypy_json_encode
```

## Comparing `mo_json-6.385.23129.dist-info/LICENSE` & `mo_json-6.403.23150.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_json-6.385.23129.dist-info/METADATA` & `mo_json-6.403.23150.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.385.23129
+Version: 6.403.23150
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: mo-dots (==9.376.23121)
-Requires-Dist: mo-future (==7.340.23006)
-Requires-Dist: mo-logs (==7.385.23129)
-Requires-Dist: mo-times (==5.385.23129)
+Requires-Dist: mo-dots (==9.401.23144)
+Requires-Dist: mo-future (==7.401.23144)
+Requires-Dist: mo-logs (==7.403.23150)
+Requires-Dist: mo-times (==5.403.23150)
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 
 # More JSON Tools
```

## Comparing `mo_json-6.385.23129.dist-info/RECORD` & `mo_json-6.403.23150.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-mo_json/__init__.py,sha256=u8xZL00hAoeMsFwimj6TjfHuzTaiKjsqW6Vm8fXquV0,13208
+mo_json/__init__.py,sha256=tfCrE8yLs0ESbkwwfbOeAh34-s6oc8HmBKMNt2Kr7e0,13329
 mo_json/decoder.py,sha256=iCE9aa_bwOCD6iDk461ywcHIBMJye-YIicGM6ILMlBk,313
 mo_json/encoder.py,sha256=PH8y_YEz9TSNhm1QJy2eW1PKUSPE2GdZwtHkASb18Js,15429
 mo_json/stream.py,sha256=DRbMb3IwpyW1s2J-Udws1wjCVCbaXGiXAa_7Ao9W4tI,16185
 mo_json/typed_encoder.py,sha256=ZLYbbeqgVbllDmxmQ4v83EM48w9hfdYnjK9q1R8mU0k,17835
 mo_json/typed_object.py,sha256=BAFhhVEdzsOIW6ZBEPlgaak7AnKr8UBIZzwxyGAsJGo,2896
 mo_json/types.py,sha256=VSLHgpQ8KF1iTXuqV0XTZILaLO28AGSrab_wdFLgo48,10240
-mo_json-6.385.23129.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_json-6.385.23129.dist-info/METADATA,sha256=S3PAfbUHReQzs6aQ6PKetIJybeJV9N2f-taO32HIqKM,11595
-mo_json-6.385.23129.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_json-6.385.23129.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
-mo_json-6.385.23129.dist-info/RECORD,,
+mo_json-6.403.23150.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_json-6.403.23150.dist-info/METADATA,sha256=PqFASI79Fe4Xm0CUCL7zp3pKpuCNxuZKqOfh1oUCqwo,11595
+mo_json-6.403.23150.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_json-6.403.23150.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
+mo_json-6.403.23150.dist-info/RECORD,,
```

