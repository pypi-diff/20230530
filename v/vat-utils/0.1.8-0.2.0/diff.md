# Comparing `tmp/vat_utils-0.1.8-py2.py3-none-any.whl.zip` & `tmp/vat_utils-0.2.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4407 bytes, number of entries: 9
+Zip file size: 4417 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-18 08:29 vat_utils/__init__.py
 -rw-r--r--  2.0 unx     1140 b- defN 20-Feb-18 08:29 vat_utils/command.py
--rw-r--r--  2.0 unx     5399 b- defN 20-Mar-27 11:02 vat_utils/config.py
+-rw-r--r--  2.0 unx     5520 b- defN 23-May-30 11:24 vat_utils/config.py
 -rw-r--r--  2.0 unx      339 b- defN 20-Feb-18 08:29 vat_utils/misc.py
--rw-r--r--  2.0 unx     1051 b- defN 20-Mar-27 11:09 vat_utils-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      231 b- defN 20-Mar-27 11:09 vat_utils-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 20-Mar-27 11:09 vat_utils-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 20-Mar-27 11:09 vat_utils-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      701 b- defN 20-Mar-27 11:09 vat_utils-0.1.8.dist-info/RECORD
-9 files, 8981 bytes uncompressed, 3201 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     1051 b- defN 23-May-30 11:31 vat_utils-0.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      176 b- defN 23-May-30 11:31 vat_utils-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 11:31 vat_utils-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-30 11:31 vat_utils-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      701 b- defN 23-May-30 11:31 vat_utils-0.2.0.dist-info/RECORD
+9 files, 9047 bytes uncompressed, 3211 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: vat_utils/config.py
 Comment: 
 
 Filename: vat_utils/misc.py
 Comment: 
 
-Filename: vat_utils-0.1.8.dist-info/LICENSE.txt
+Filename: vat_utils-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vat_utils-0.1.8.dist-info/METADATA
+Filename: vat_utils-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: vat_utils-0.1.8.dist-info/WHEEL
+Filename: vat_utils-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: vat_utils-0.1.8.dist-info/top_level.txt
+Filename: vat_utils-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: vat_utils-0.1.8.dist-info/RECORD
+Filename: vat_utils-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vat_utils/config.py

```diff
@@ -98,23 +98,26 @@
 
     def _fetch_root_json_value(self):
         response = self.ssm_client.get_parameter(
             Name=self.config_source,
             WithDecryption=True
         )
         value = response['Parameter']['Value']
-        encoding, payload = re.match(r'^(?:([^:]+):)?([^:]+)$', value).groups()
-        if encoding is None:
-            return json.loads(base64.b64decode(payload).decode())
-        elif encoding == 'b64gz':
-            data = io.BytesIO(base64.b64decode(payload))
-            with gzip.GzipFile(fileobj=data, mode='rb') as gz_data:
-                return json.loads(gz_data.read().decode())
+        if value.startswith("{"):
+            return json.loads(value)
         else:
-            raise ValueError("Invalid parameter value")
+            encoding, payload = re.match(r'^(?:([^:]+):)?([^:]+)$', value).groups()
+            if encoding is None:
+                return json.loads(base64.b64decode(payload).decode())
+            elif encoding == 'b64gz':
+                data = io.BytesIO(base64.b64decode(payload))
+                with gzip.GzipFile(fileobj=data, mode='rb') as gz_data:
+                    return json.loads(gz_data.read().decode())
+            else:
+                raise ValueError("Invalid parameter value")
 
 class S3ConfigClient(BaseJsonConfigClient):
     """
     """
     def __init__(self, config_source, boto3_session=None):
         if boto3_session is not None:
             self.s3_client = boto3_session.client('s3')
```

## Comparing `vat_utils-0.1.8.dist-info/LICENSE.txt` & `vat_utils-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vat_utils-0.1.8.dist-info/RECORD` & `vat_utils-0.2.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 vat_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 vat_utils/command.py,sha256=wa0XtSFgrwwLXbjCT2IROPNJVJuTQxh2ZLQTK9cRZek,1140
-vat_utils/config.py,sha256=t2x_0hJyUaZkipJrtoKCObpcmoVqj4soVpQMtEH4Z_A,5399
+vat_utils/config.py,sha256=c_VC1_s_T-lEXnKY9ZLfMdhfFa7LrcE6iMmpBhjHcYM,5520
 vat_utils/misc.py,sha256=MgumMJdI7orXLy_MYQJKXkYa_zw_AiF4nxXJv_Rt1OM,339
-vat_utils-0.1.8.dist-info/LICENSE.txt,sha256=WL6t3ykTGS4ebVdYrRhGYul5s1XqtT-Tn3P6e6Pt1VQ,1051
-vat_utils-0.1.8.dist-info/METADATA,sha256=5sgERjV_QvpZtqhqlP7OfNPn1LOlni1n122TP4qMtbk,231
-vat_utils-0.1.8.dist-info/WHEEL,sha256=kGT74LWyRUZrL4VgLh6_g12IeVl_9u9ZVhadrgXZUEY,110
-vat_utils-0.1.8.dist-info/top_level.txt,sha256=zvCY2G2Wbh8I2lZKKR9d-7Qc3VhZGzrZhL64okyVang,10
-vat_utils-0.1.8.dist-info/RECORD,,
+vat_utils-0.2.0.dist-info/LICENSE.txt,sha256=WL6t3ykTGS4ebVdYrRhGYul5s1XqtT-Tn3P6e6Pt1VQ,1051
+vat_utils-0.2.0.dist-info/METADATA,sha256=XxHy4SXk3nNmt5Js6akV_P345t-X9fqORFIRj_VEmnA,176
+vat_utils-0.2.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+vat_utils-0.2.0.dist-info/top_level.txt,sha256=zvCY2G2Wbh8I2lZKKR9d-7Qc3VhZGzrZhL64okyVang,10
+vat_utils-0.2.0.dist-info/RECORD,,
```

