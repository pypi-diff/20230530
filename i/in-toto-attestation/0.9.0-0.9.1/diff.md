# Comparing `tmp/in_toto_attestation-0.9.0.tar.gz` & `tmp/in_toto_attestation-0.9.1.tar.gz`

## Comparing `in_toto_attestation-0.9.0.tar` & `in_toto_attestation-0.9.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/in_toto_attestation/__init__.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/in_toto_attestation/predicates/vsa/v0/vsa_pb2.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/in_toto_attestation/v1/resource_descriptor_pb2.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/in_toto_attestation/v1/statement_pb2.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/README.md
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/in_toto_attestation/__init__.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/in_toto_attestation/predicates/link/v0/link_pb2.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/in_toto_attestation/predicates/vsa/v0/vsa_pb2.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/in_toto_attestation/v1/resource_descriptor_pb2.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/in_toto_attestation/v1/statement_pb2.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/.gitignore
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/README.md
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 in_toto_attestation-0.9.1/PKG-INFO
```

### Comparing `in_toto_attestation-0.9.0/in_toto_attestation/predicates/vsa/v0/vsa_pb2.py` & `in_toto_attestation-0.9.1/in_toto_attestation/predicates/vsa/v0/vsa_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/in_toto_attestation/predicates/vsa/v0/vsa.proto\x12\x1ein_toto_attestation.predicates\x1a\x1fgoogle/protobuf/timestamp.proto\"\xf9\x07\n\x13VerificationSummary\x12N\n\x08verifier\x18\x01 \x01(\x0b\x32<.in_toto_attestation.predicates.VerificationSummary.Verifier\x12?\n\x0ctimeVerified\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\rtime_verified\x12!\n\x0bresourceUri\x18\x03 \x01(\tR\x0cresource_uri\x12J\n\x06policy\x18\x04 \x01(\x0b\x32:.in_toto_attestation.predicates.VerificationSummary.Policy\x12s\n\x11inputAttestations\x18\x05 \x03(\x0b\x32\x44.in_toto_attestation.predicates.VerificationSummary.InputAttestationR\x12input_attestations\x12/\n\x12verificationResult\x18\x06 \x01(\tR\x13verification_result\x12!\n\x0bpolicyLevel\x18\x07 \x01(\tR\x0cpolicy_level\x12v\n\x10\x64\x65pendencyLevels\x18\x08 \x03(\x0b\x32I.in_toto_attestation.predicates.VerificationSummary.DependencyLevelsEntryR\x11\x64\x65pendency_levels\x1a\x16\n\x08Verifier\x12\n\n\x02id\x18\x01 \x01(\t\x1a\x9c\x01\n\x06Policy\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12V\n\x06\x64igest\x18\x02 \x03(\x0b\x32\x46.in_toto_attestation.predicates.VerificationSummary.Policy.DigestEntry\x1a-\n\x0b\x44igestEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xb0\x01\n\x10InputAttestation\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12`\n\x06\x64igest\x18\x02 \x03(\x0b\x32P.in_toto_attestation.predicates.VerificationSummary.InputAttestation.DigestEntry\x1a-\n\x0b\x44igestEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x37\n\x15\x44\x65pendencyLevelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\x42\x35Z3github.com/in-toto/attestation/go/predicates/vsa/v0b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/in_toto_attestation/predicates/vsa/v0/vsa.proto\x12%in_toto_attestation.predicates.vsa.v0\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa3\x08\n\x13VerificationSummary\x12U\n\x08verifier\x18\x01 \x01(\x0b\x32\x43.in_toto_attestation.predicates.vsa.v0.VerificationSummary.Verifier\x12?\n\x0ctimeVerified\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\rtime_verified\x12!\n\x0bresourceUri\x18\x03 \x01(\tR\x0cresource_uri\x12Q\n\x06policy\x18\x04 \x01(\x0b\x32\x41.in_toto_attestation.predicates.vsa.v0.VerificationSummary.Policy\x12z\n\x11inputAttestations\x18\x05 \x03(\x0b\x32K.in_toto_attestation.predicates.vsa.v0.VerificationSummary.InputAttestationR\x12input_attestations\x12/\n\x12verificationResult\x18\x06 \x01(\tR\x13verification_result\x12!\n\x0bpolicyLevel\x18\x07 \x01(\tR\x0cpolicy_level\x12}\n\x10\x64\x65pendencyLevels\x18\x08 \x03(\x0b\x32P.in_toto_attestation.predicates.vsa.v0.VerificationSummary.DependencyLevelsEntryR\x11\x64\x65pendency_levels\x1a\x16\n\x08Verifier\x12\n\n\x02id\x18\x01 \x01(\t\x1a\xa3\x01\n\x06Policy\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12]\n\x06\x64igest\x18\x02 \x03(\x0b\x32M.in_toto_attestation.predicates.vsa.v0.VerificationSummary.Policy.DigestEntry\x1a-\n\x0b\x44igestEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\xb7\x01\n\x10InputAttestation\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12g\n\x06\x64igest\x18\x02 \x03(\x0b\x32W.in_toto_attestation.predicates.vsa.v0.VerificationSummary.InputAttestation.DigestEntry\x1a-\n\x0b\x44igestEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x37\n\x15\x44\x65pendencyLevelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\x42\x65\n.io.github.intoto.attestation.predicates.vsa.v0Z3github.com/in-toto/attestation/go/predicates/vsa/v0b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'in_toto_attestation.predicates.vsa.v0.vsa_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z3github.com/in-toto/attestation/go/predicates/vsa/v0'
+  DESCRIPTOR._serialized_options = b'\n.io.github.intoto.attestation.predicates.vsa.v0Z3github.com/in-toto/attestation/go/predicates/vsa/v0'
   _VERIFICATIONSUMMARY_POLICY_DIGESTENTRY._options = None
   _VERIFICATIONSUMMARY_POLICY_DIGESTENTRY._serialized_options = b'8\001'
   _VERIFICATIONSUMMARY_INPUTATTESTATION_DIGESTENTRY._options = None
   _VERIFICATIONSUMMARY_INPUTATTESTATION_DIGESTENTRY._serialized_options = b'8\001'
   _VERIFICATIONSUMMARY_DEPENDENCYLEVELSENTRY._options = None
   _VERIFICATIONSUMMARY_DEPENDENCYLEVELSENTRY._serialized_options = b'8\001'
-  _VERIFICATIONSUMMARY._serialized_start=117
-  _VERIFICATIONSUMMARY._serialized_end=1134
-  _VERIFICATIONSUMMARY_VERIFIER._serialized_start=717
-  _VERIFICATIONSUMMARY_VERIFIER._serialized_end=739
-  _VERIFICATIONSUMMARY_POLICY._serialized_start=742
-  _VERIFICATIONSUMMARY_POLICY._serialized_end=898
-  _VERIFICATIONSUMMARY_POLICY_DIGESTENTRY._serialized_start=853
-  _VERIFICATIONSUMMARY_POLICY_DIGESTENTRY._serialized_end=898
-  _VERIFICATIONSUMMARY_INPUTATTESTATION._serialized_start=901
-  _VERIFICATIONSUMMARY_INPUTATTESTATION._serialized_end=1077
-  _VERIFICATIONSUMMARY_INPUTATTESTATION_DIGESTENTRY._serialized_start=853
-  _VERIFICATIONSUMMARY_INPUTATTESTATION_DIGESTENTRY._serialized_end=898
-  _VERIFICATIONSUMMARY_DEPENDENCYLEVELSENTRY._serialized_start=1079
-  _VERIFICATIONSUMMARY_DEPENDENCYLEVELSENTRY._serialized_end=1134
+  _VERIFICATIONSUMMARY._serialized_start=124
+  _VERIFICATIONSUMMARY._serialized_end=1183
+  _VERIFICATIONSUMMARY_VERIFIER._serialized_start=752
+  _VERIFICATIONSUMMARY_VERIFIER._serialized_end=774
+  _VERIFICATIONSUMMARY_POLICY._serialized_start=777
+  _VERIFICATIONSUMMARY_POLICY._serialized_end=940
+  _VERIFICATIONSUMMARY_POLICY_DIGESTENTRY._serialized_start=895
+  _VERIFICATIONSUMMARY_POLICY_DIGESTENTRY._serialized_end=940
+  _VERIFICATIONSUMMARY_INPUTATTESTATION._serialized_start=943
+  _VERIFICATIONSUMMARY_INPUTATTESTATION._serialized_end=1126
+  _VERIFICATIONSUMMARY_INPUTATTESTATION_DIGESTENTRY._serialized_start=895
+  _VERIFICATIONSUMMARY_INPUTATTESTATION_DIGESTENTRY._serialized_end=940
+  _VERIFICATIONSUMMARY_DEPENDENCYLEVELSENTRY._serialized_start=1128
+  _VERIFICATIONSUMMARY_DEPENDENCYLEVELSENTRY._serialized_end=1183
 # @@protoc_insertion_point(module_scope)
```

### Comparing `in_toto_attestation-0.9.0/in_toto_attestation/v1/resource_descriptor_pb2.py` & `in_toto_attestation-0.9.1/in_toto_attestation/v1/resource_descriptor_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0in_toto_attestation/v1/resource_descriptor.proto\x12\x16in_toto_attestation.v1\x1a\x1cgoogle/protobuf/struct.proto\"\x83\x03\n\x12ResourceDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x46\n\x06\x64igest\x18\x03 \x03(\x0b\x32\x36.in_toto_attestation.v1.ResourceDescriptor.DigestEntry\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\x0c\x12\x18\n\x10\x64ownloadLocation\x18\x05 \x01(\t\x12\x11\n\tmediaType\x18\x06 \x01(\t\x12P\n\x0b\x61nnotations\x18\x07 \x03(\x0b\x32;.in_toto_attestation.v1.ResourceDescriptor.AnnotationsEntry\x1a-\n\x0b\x44igestEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aK\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct:\x02\x38\x01\x42&Z$github.com/in-toto/attestation/go/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0in_toto_attestation/v1/resource_descriptor.proto\x12\x16in_toto_attestation.v1\x1a\x1cgoogle/protobuf/struct.proto\"\x83\x03\n\x12ResourceDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x46\n\x06\x64igest\x18\x03 \x03(\x0b\x32\x36.in_toto_attestation.v1.ResourceDescriptor.DigestEntry\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\x0c\x12\x18\n\x10\x64ownloadLocation\x18\x05 \x01(\t\x12\x11\n\tmediaType\x18\x06 \x01(\t\x12P\n\x0b\x61nnotations\x18\x07 \x03(\x0b\x32;.in_toto_attestation.v1.ResourceDescriptor.AnnotationsEntry\x1a-\n\x0b\x44igestEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1aK\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct:\x02\x38\x01\x42G\n\x1fio.github.intoto.attestation.v1Z$github.com/in-toto/attestation/go/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'in_toto_attestation.v1.resource_descriptor_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z$github.com/in-toto/attestation/go/v1'
+  DESCRIPTOR._serialized_options = b'\n\037io.github.intoto.attestation.v1Z$github.com/in-toto/attestation/go/v1'
   _RESOURCEDESCRIPTOR_DIGESTENTRY._options = None
   _RESOURCEDESCRIPTOR_DIGESTENTRY._serialized_options = b'8\001'
   _RESOURCEDESCRIPTOR_ANNOTATIONSENTRY._options = None
   _RESOURCEDESCRIPTOR_ANNOTATIONSENTRY._serialized_options = b'8\001'
   _RESOURCEDESCRIPTOR._serialized_start=107
   _RESOURCEDESCRIPTOR._serialized_end=494
   _RESOURCEDESCRIPTOR_DIGESTENTRY._serialized_start=372
```

### Comparing `in_toto_attestation-0.9.0/in_toto_attestation/v1/statement_pb2.py` & `in_toto_attestation-0.9.1/in_toto_attestation/v1/statement_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,26 +8,21 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from in_toto_attestation.v1 import resource_descriptor_pb2 as in__toto__attestation_dot_v1_dot_resource__descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&in_toto_attestation/v1/statement.proto\x12\x16in_toto_attestation.v1\x1a\x1cgoogle/protobuf/struct.proto\"\xaf\x02\n\tStatement\x12\x13\n\x04type\x18\x01 \x01(\tR\x05_type\x12:\n\x07subject\x18\x02 \x03(\x0b\x32).in_toto_attestation.v1.Statement.Subject\x12\x15\n\rpredicateType\x18\x03 \x01(\t\x12*\n\tpredicate\x18\x04 \x01(\x0b\x32\x17.google.protobuf.Struct\x1a\x8d\x01\n\x07Subject\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x45\n\x06\x64igest\x18\x02 \x03(\x0b\x32\x35.in_toto_attestation.v1.Statement.Subject.DigestEntry\x1a-\n\x0b\x44igestEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42&Z$github.com/in-toto/attestation/go/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&in_toto_attestation/v1/statement.proto\x12\x16in_toto_attestation.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x30in_toto_attestation/v1/resource_descriptor.proto\"\xa0\x01\n\tStatement\x12\x13\n\x04type\x18\x01 \x01(\tR\x05_type\x12;\n\x07subject\x18\x02 \x03(\x0b\x32*.in_toto_attestation.v1.ResourceDescriptor\x12\x15\n\rpredicateType\x18\x03 \x01(\t\x12*\n\tpredicate\x18\x04 \x01(\x0b\x32\x17.google.protobuf.StructBG\n\x1fio.github.intoto.attestation.v1Z$github.com/in-toto/attestation/go/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'in_toto_attestation.v1.statement_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z$github.com/in-toto/attestation/go/v1'
-  _STATEMENT_SUBJECT_DIGESTENTRY._options = None
-  _STATEMENT_SUBJECT_DIGESTENTRY._serialized_options = b'8\001'
-  _STATEMENT._serialized_start=97
-  _STATEMENT._serialized_end=400
-  _STATEMENT_SUBJECT._serialized_start=259
-  _STATEMENT_SUBJECT._serialized_end=400
-  _STATEMENT_SUBJECT_DIGESTENTRY._serialized_start=355
-  _STATEMENT_SUBJECT_DIGESTENTRY._serialized_end=400
+  DESCRIPTOR._serialized_options = b'\n\037io.github.intoto.attestation.v1Z$github.com/in-toto/attestation/go/v1'
+  _STATEMENT._serialized_start=147
+  _STATEMENT._serialized_end=307
 # @@protoc_insertion_point(module_scope)
```

### Comparing `in_toto_attestation-0.9.0/pyproject.toml` & `in_toto_attestation-0.9.1/pyproject.toml`

 * *Files identical despite different names*

