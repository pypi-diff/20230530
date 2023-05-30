# Comparing `tmp/icpp_free-2.3.0-py3-none-any.whl.zip` & `tmp/icpp_free-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,29 @@
-Zip file size: 204209 bytes, number of entries: 203
+Zip file size: 205136 bytes, number of entries: 204
 -rw-rw-r--  2.0 unx      747 b- defN 23-Apr-29 11:50 icpp/__init__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-May-19 20:47 icpp/__main__.py
--rw-rw-r--  2.0 unx     1053 b- defN 23-May-19 20:58 icpp/commands_build_native.py
+-rw-rw-r--  2.0 unx     1053 b- defN 23-May-30 13:46 icpp/commands_build_native.py
 -rw-rw-r--  2.0 unx     5433 b- defN 23-May-19 20:47 icpp/commands_build_wasm.py
 -rw-rw-r--  2.0 unx     1122 b- defN 23-Apr-29 11:50 icpp/commands_get.py
 -rw-rw-r--  2.0 unx      753 b- defN 23-Apr-29 11:50 icpp/commands_init.py
 -rw-rw-r--  2.0 unx     3584 b- defN 23-Apr-29 11:50 icpp/commands_install_wasi_sdk.py
--rw-rw-r--  2.0 unx     5138 b- defN 23-Apr-29 17:59 icpp/config_default.py
--rw-rw-r--  2.0 unx     2488 b- defN 23-May-19 20:58 icpp/conftest_base.py
+-rw-rw-r--  2.0 unx     9612 b- defN 23-May-30 13:46 icpp/config_default.py
+-rw-rw-r--  2.0 unx     2488 b- defN 23-May-30 13:46 icpp/conftest_base.py
 -rw-rw-r--  2.0 unx     2944 b- defN 23-May-19 20:47 icpp/decorators.py
 -rw-rw-r--  2.0 unx     3776 b- defN 23-May-12 19:56 icpp/icpp_toml.py
 -rw-rw-r--  2.0 unx      670 b- defN 23-May-19 20:47 icpp/options_build.py
--rw-rw-r--  2.0 unx      925 b- defN 23-May-19 20:58 icpp/options_main.py
--rw-rw-r--  2.0 unx      879 b- defN 23-May-19 20:58 icpp/pro.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-May-30 13:46 icpp/options_main.py
+-rw-rw-r--  2.0 unx      879 b- defN 23-May-30 13:46 icpp/pro.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Apr-29 11:50 icpp/py.typed
 -rw-rw-r--  2.0 unx     5280 b- defN 23-May-10 21:24 icpp/run_shell_cmd.py
--rw-rw-r--  2.0 unx     1463 b- defN 23-May-19 20:58 icpp/smoketest.py
--rw-rw-r--  2.0 unx      322 b- defN 23-May-19 20:58 icpp/version.py
+-rw-rw-r--  2.0 unx     1463 b- defN 23-May-30 13:46 icpp/smoketest.py
+-rw-rw-r--  2.0 unx      322 b- defN 23-May-30 13:46 icpp/version.py
 -rw-rw-r--  2.0 unx      272 b- defN 23-Apr-29 11:50 icpp/version_wasi_sdk.py
 -rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 11:50 icpp/canisters/greet/README.md
+-rwxrwxr-x  2.0 unx      774 b- defN 23-May-30 13:55 icpp/canisters/greet/demo.sh
 -rw-r--r--  2.0 unx      269 b- defN 23-Apr-29 11:50 icpp/canisters/greet/dfx.json
 -rw-r--r--  2.0 unx      474 b- defN 23-Apr-29 11:50 icpp/canisters/greet/icpp.toml
 -rw-rw-r--  2.0 unx     2061 b- defN 23-May-19 20:47 icpp/canisters/greet/native/main.cpp
 -rw-rw-r--  2.0 unx      137 b- defN 23-May-19 20:47 icpp/canisters/greet/native/main.h
 -rw-rw-r--  2.0 unx     3022 b- defN 23-May-19 20:47 icpp/canisters/greet/src/greet.cpp
 -rw-r--r--  2.0 unx      469 b- defN 23-May-19 20:47 icpp/canisters/greet/src/greet.did
 -rw-r--r--  2.0 unx      354 b- defN 23-May-19 20:47 icpp/canisters/greet/src/greet.h
@@ -100,15 +101,15 @@
 -rw-rw-r--  2.0 unx      825 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat8.h
 -rw-rw-r--  2.0 unx     2926 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_principal.cpp
 -rw-rw-r--  2.0 unx      880 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_principal.h
 -rw-rw-r--  2.0 unx     2925 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_text.cpp
 -rw-rw-r--  2.0 unx      853 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_text.h
 -rw-rw-r--  2.0 unx      148 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_prim.cpp
 -rw-rw-r--  2.0 unx      484 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_prim.h
--rw-r--r--  2.0 unx     9545 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_principal.cpp
+-rw-r--r--  2.0 unx     9697 b- defN 23-May-30 13:46 icpp/ic/candid/candid_type_principal.cpp
 -rw-rw-r--  2.0 unx     1819 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_principal.h
 -rw-rw-r--  2.0 unx    10646 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_record.cpp
 -rw-rw-r--  2.0 unx     1206 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_record.h
 -rw-rw-r--  2.0 unx     1045 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_reserved.cpp
 -rw-rw-r--  2.0 unx      434 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_reserved.h
 -rw-rw-r--  2.0 unx     2579 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_table.cpp
 -rw-rw-r--  2.0 unx      676 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_table.h
@@ -148,22 +149,22 @@
 -rw-r--r--  2.0 unx      752 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_principal.h
 -rw-r--r--  2.0 unx     2724 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_text.cpp
 -rw-r--r--  2.0 unx      727 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_text.h
 -rw-rw-r--  2.0 unx    15454 b- defN 23-May-19 20:47 icpp/ic/candid/vec_bytes.cpp
 -rw-rw-r--  2.0 unx     7774 b- defN 23-May-19 20:47 icpp/ic/candid/vec_bytes.h
 -rw-rw-r--  2.0 unx     3407 b- defN 23-Apr-29 11:50 icpp/ic/ic0/ic0.h
 -rw-r--r--  2.0 unx      110 b- defN 23-Apr-29 11:50 icpp/ic/ic0mock/global.h
--rw-r--r--  2.0 unx     3288 b- defN 23-May-19 20:58 icpp/ic/ic0mock/ic0.cpp
+-rw-r--r--  2.0 unx     3288 b- defN 23-May-30 13:46 icpp/ic/ic0mock/ic0.cpp
 -rw-rw-r--  2.0 unx     2091 b- defN 23-Apr-29 11:50 icpp/ic/ic0mock/ic0.h
--rw-r--r--  2.0 unx     1372 b- defN 23-May-19 20:58 icpp/ic/ic0mock/mock_ic.cpp
+-rw-r--r--  2.0 unx     1372 b- defN 23-May-30 13:46 icpp/ic/ic0mock/mock_ic.cpp
 -rw-rw-r--  2.0 unx     1495 b- defN 23-May-01 15:09 icpp/ic/ic0mock/mock_ic.h
--rw-rw-r--  2.0 unx     5969 b- defN 23-May-19 20:47 icpp/ic/icapi/ic_api.cpp
+-rw-rw-r--  2.0 unx     6185 b- defN 23-May-30 13:46 icpp/ic/icapi/ic_api.cpp
 -rw-rw-r--  2.0 unx     2106 b- defN 23-May-19 20:47 icpp/ic/icapi/ic_api.h
 -rw-r--r--  2.0 unx      463 b- defN 23-Apr-29 11:50 icpp/ic/icapi/wasm_symbol.h
--rw-r--r--  2.0 unx      754 b- defN 23-May-19 20:58 icpp/ic/pro/pro.cpp
+-rw-r--r--  2.0 unx      754 b- defN 23-May-30 13:46 icpp/ic/pro/pro.cpp
 -rw-r--r--  2.0 unx      393 b- defN 23-Apr-29 17:59 icpp/ic/pro/pro.h
 -rw-rw-r--  2.0 unx     1155 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/LICENSE
 -rw-rw-r--  2.0 unx     3933 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_crockford.hpp
 -rw-rw-r--  2.0 unx     1366 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_default_crockford.hpp
 -rw-rw-r--  2.0 unx     1342 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_default_hex.hpp
 -rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_default_rfc4648.hpp
 -rw-rw-r--  2.0 unx     3090 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_hex.hpp
@@ -192,14 +193,14 @@
 -rw-r--r--  2.0 unx     1736 b- defN 23-Apr-29 11:50 icpp/ic/vendors/hash-library/crc32.h
 -rw-r--r--  2.0 unx     1758 b- defN 23-Apr-29 11:50 icpp/ic/vendors/hash-library/readme.md
 -rw-rw-r--  2.0 unx     1370 b- defN 23-Apr-29 11:50 icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c
 -rw-rw-r--  2.0 unx      327 b- defN 23-Apr-29 11:50 icpp/ic/wasi_sdk_traps/ic_trap.c
 -rw-rw-r--  2.0 unx       70 b- defN 23-Apr-29 11:50 icpp/ic/wasi_sdk_traps/ic_trap.h
 -rw-rw-r--  2.0 unx     4743 b- defN 23-May-19 20:47 icpp/ic/wasi_sdk_traps/posix.c
 -rw-r--r--  2.0 unx    10198 b- defN 23-May-19 20:47 icpp/ic/wasi_sdk_traps/unreachable.c
--rw-r--r--  2.0 unx      983 b- defN 23-May-19 21:00 icpp_free-2.3.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2274 b- defN 23-May-19 21:00 icpp_free-2.3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-19 21:00 icpp_free-2.3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-May-19 21:00 icpp_free-2.3.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-May-19 21:00 icpp_free-2.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    18573 b- defN 23-May-19 21:00 icpp_free-2.3.0.dist-info/RECORD
-203 files, 502452 bytes uncompressed, 174483 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx      983 b- defN 23-May-30 13:57 icpp_free-2.4.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2274 b- defN 23-May-30 13:57 icpp_free-2.4.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-30 13:57 icpp_free-2.4.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-May-30 13:57 icpp_free-2.4.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-May-30 13:57 icpp_free-2.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    18657 b- defN 23-May-30 13:57 icpp_free-2.4.0.dist-info/RECORD
+204 files, 508152 bytes uncompressed, 175278 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -54,14 +54,17 @@
 
 Filename: icpp/version_wasi_sdk.py
 Comment: 
 
 Filename: icpp/canisters/greet/README.md
 Comment: 
 
+Filename: icpp/canisters/greet/demo.sh
+Comment: 
+
 Filename: icpp/canisters/greet/dfx.json
 Comment: 
 
 Filename: icpp/canisters/greet/icpp.toml
 Comment: 
 
 Filename: icpp/canisters/greet/native/main.cpp
@@ -585,26 +588,26 @@
 
 Filename: icpp/ic/wasi_sdk_traps/posix.c
 Comment: 
 
 Filename: icpp/ic/wasi_sdk_traps/unreachable.c
 Comment: 
 
-Filename: icpp_free-2.3.0.dist-info/LICENSE
+Filename: icpp_free-2.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: icpp_free-2.3.0.dist-info/METADATA
+Filename: icpp_free-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: icpp_free-2.3.0.dist-info/WHEEL
+Filename: icpp_free-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: icpp_free-2.3.0.dist-info/entry_points.txt
+Filename: icpp_free-2.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: icpp_free-2.3.0.dist-info/top_level.txt
+Filename: icpp_free-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: icpp_free-2.3.0.dist-info/RECORD
+Filename: icpp_free-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## icpp/config_default.py

```diff
@@ -70,14 +70,75 @@
 )
 IC_CPP_FILES = (
     " ".join(
         [
             str(x)
             for x in list(ICPP_PATH.glob("ic/ic0/*.cpp"))
             + list(ICPP_PATH.glob("ic/candid/*.cpp"))
+            # FOR DEBUGGING
+            # + list(ICPP_PATH.glob("ic/candid/candid_assert.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_deserialize.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_opcode.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_serialize.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_base.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_bool.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_empty.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_float32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_float64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_int.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_int8.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_int16.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_int32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_int64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_nat.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_nat8.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_nat16.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_nat32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_nat64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_null.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_text.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_base.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_bool.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_float32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_float64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_int.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_int8.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_int16.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_int32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_int64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_nat.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_nat8.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_nat16.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_nat32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_nat64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_principal.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_opt_text.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_prim.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_record.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_reserved.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_table.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_variant.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_base.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_bool.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_float32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_float64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_int.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_int8.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_int16.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_int32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_int64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_nat.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_nat8.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_nat16.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_nat32.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_nat64.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_text.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/vec_bytes.cpp"))  # ok
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_vec_principal.cpp"))
+            # + list(ICPP_PATH.glob("ic/candid/candid_type_principal.cpp"))  # nok
             + list(ICPP_PATH.glob("ic/icapi/*.cpp"))
             + list(ICPP_PATH.glob("ic/pro/*.cpp"))
             + list(
                 ICPP_PATH.glob("ic/vendors/hash-library/crc32.cpp")
             )  # TODO: Amalgate into .hpp
             # + list(ICPP_PATH.glob("ic/vendors/*.cpp"))
         ]
```

## icpp/version.py

```diff
@@ -5,8 +5,8 @@
 (-) do not add anything but the version number here!
 
 We do it this way, so both __init__.py and setup.py can use it.
 
 see:
 https://packaging.python.org/guides/single-sourcing-package-version/
 """
-__version__ = "2.3.0"
+__version__ = "2.4.0"
```

## icpp/ic/candid/candid_type_principal.cpp

```diff
@@ -7,37 +7,38 @@
 #include <cassert>
 
 #include "cppcodec/base32_rfc4648.hpp"
 #include "hash-library/crc32.h"
 
 #include "ic_api.h"
 
+// DON'T DO THIS. IT BREAKS ALL UPDATE CALLS
 //                                                               data_bytes
-const std::string PRINCIPAL_ID_ANONYMOUS = "2vxsx-fae";          // 1 byte: x04
-const std::string PRINCIPAL_ID_MANAGEMENT_CANISTER = "aaaaa-aa"; // no bytes
+// const std::string PRINCIPAL_ID_ANONYMOUS = "2vxsx-fae";          // 1 byte: x04
+// const std::string PRINCIPAL_ID_MANAGEMENT_CANISTER = "aaaaa-aa"; // no bytes
 
-const uint32_t MAX_LENGTH_IN_BYTES = 29;
-const uint32_t CRC_LENGTH_IN_BYTES = 4;
+// const uint32_t MAX_LENGTH_IN_BYTES = 29;
+// const uint32_t CRC_LENGTH_IN_BYTES = 4;
 
-const std::string PRINCIPAL_OPAQUE_REFERENCE_NOT_SUPPORTED =
-    "Principal Error: Found a value different that 1 for the reference. Opaque reference not supported.";
-const std::string PRINCIPAL_ERROR_BYTES_TOO_LONG =
-    "Principal Error: Bytes is longer than 29 bytes.";
-const std::string PRINCIPAL_ERROR_INVALID_BASE32 =
-    "Principal Error: Text must be in valid Base32 encoding.";
-const std::string PRINCIPAL_ERROR_TEXT_TOO_SHORT =
-    "Principal Error: Text is too short.";
-const std::string PRINCIPAL_ERROR_TEXT_TOO_LONG =
-    "Principal Error: Text is too long.";
-const std::string PRINCIPAL_ERROR_CHECK_SEQUENCE_NOT_MATCH =
-    "Principal Error: CRC32 checksum doesn't match.";
-const std::string PRINCIPAL_ERROR_ABNORMAL_GROUPED =
-    "Principal Error: Text should be separated by - (dash) every 5 characters";
-const std::string PRINCIPAL_ERROR_INVALID_BASE32_ENCODING =
-    "Principal Error: Text must be in valid Base32 encoding. Decoding/Encoding roundtrip fails.";
+// const std::string PRINCIPAL_OPAQUE_REFERENCE_NOT_SUPPORTED =
+//     "Principal Error: Found a value different that 1 for the reference. Opaque reference not supported.";
+// const std::string PRINCIPAL_ERROR_BYTES_TOO_LONG =
+//     "Principal Error: Bytes is longer than 29 bytes.";
+// const std::string PRINCIPAL_ERROR_INVALID_BASE32 =
+//     "Principal Error: Text must be in valid Base32 encoding.";
+// const std::string PRINCIPAL_ERROR_TEXT_TOO_SHORT =
+//     "Principal Error: Text is too short.";
+// const std::string PRINCIPAL_ERROR_TEXT_TOO_LONG =
+//     "Principal Error: Text is too long.";
+// const std::string PRINCIPAL_ERROR_CHECK_SEQUENCE_NOT_MATCH =
+//     "Principal Error: CRC32 checksum doesn't match.";
+// const std::string PRINCIPAL_ERROR_ABNORMAL_GROUPED =
+//     "Principal Error: Text should be separated by - (dash) every 5 characters";
+// const std::string PRINCIPAL_ERROR_INVALID_BASE32_ENCODING =
+//     "Principal Error: Text must be in valid Base32 encoding. Decoding/Encoding roundtrip fails.";
 
 CandidTypePrincipal::CandidTypePrincipal() : CandidTypePrim() {
   initialize("");
 }
 
 // These constructors allows for setting the value during Deserialization
 CandidTypePrincipal::CandidTypePrincipal(std::string *p_v) : CandidTypePrim() {
@@ -64,15 +65,15 @@
 }
 
 CandidTypePrincipal::~CandidTypePrincipal() {}
 
 // Initialize things
 void CandidTypePrincipal::initialize(const std::string &v) {
   if (v == "") {
-    m_v = PRINCIPAL_ID_ANONYMOUS;
+    m_v = "2vxsx-fae";
     // Fill the user's data placeholder, if a pointer was provided
     if (m_pv) *m_pv = m_v;
   } else m_v = v;
   bytes_from_string();
   set_datatype();
   encode_I();
   encode_M();
@@ -122,15 +123,16 @@
   uint8_t ref_r;
   if (B.parse_int_fixed_width(offset, ref_r, parse_error)) {
     std::string to_be_parsed = "Unused opaque reference.";
     CandidDeserialize::trap_with_parse_error(offset_start, offset, to_be_parsed,
                                              parse_error);
   }
   if (ref_r != 1) {
-    IC_API::trap(PRINCIPAL_OPAQUE_REFERENCE_NOT_SUPPORTED);
+    IC_API::trap(
+        "Principal Error: Found a value different that 1 for the reference. Opaque reference not supported.");
   }
 
   // Get the length
   __uint128_t numbytes;
   parse_error = "";
   __uint128_t numBytes_principal;
   if (B.parse_uleb128(offset, numBytes_principal, numbytes, parse_error)) {
@@ -162,56 +164,55 @@
   // Do the reverse of: m_v = Encode(data) := Group(LowerCase(Base32(CRC32(data) || data)))
 
   std::string s = m_v;
   ungroup(s);
   make_ascii_uppercase(s);
   std::vector<uint8_t> bytes = base32_decode(s);
 
-  if (bytes.size() < CRC_LENGTH_IN_BYTES) {
-    IC_API::trap(PRINCIPAL_ERROR_TEXT_TOO_SHORT);
+  if (bytes.size() < 4) {
+    IC_API::trap("Principal Error: Text is too short.");
   }
 
   // First 4 bytes are a CRC32 checksum of the data that follows. The data bytes are the principal ID
-  std::vector<uint8_t> crc_bytes(bytes.begin(),
-                                 bytes.begin() + CRC_LENGTH_IN_BYTES);
-  std::vector<uint8_t> data_bytes(bytes.begin() + CRC_LENGTH_IN_BYTES,
-                                  bytes.end());
+  std::vector<uint8_t> crc_bytes(bytes.begin(), bytes.begin() + 4);
+  std::vector<uint8_t> data_bytes(bytes.begin() + 4, bytes.end());
 
-  if (data_bytes.size() > MAX_LENGTH_IN_BYTES) {
-    IC_API::trap(PRINCIPAL_ERROR_TEXT_TOO_LONG);
+  if (data_bytes.size() > 29) {
+    IC_API::trap("Principal Error: Text is too long.");
   }
 
   // Verify the CRC32 checksum of the data bytes
   std::array<uint8_t, 4> crc_data = crc32(data_bytes);
   if (!std::equal(crc_bytes.begin(), crc_bytes.end(), crc_data.begin())) {
-    IC_API::trap(PRINCIPAL_ERROR_CHECK_SEQUENCE_NOT_MATCH);
+    IC_API::trap("Principal Error: CRC32 checksum doesn't match.");
   }
 
   // from https://internetcomputer.org/docs/current/references/id-encoding-spec
   //   w3gef-eqbai -> 0102 -> w3gef-eqbai
   //   w3gef-eqbaj -> 0102 -> w3gef-eqbai ==> Error due to non-zero padding bits
   //
   // Verify that roundtrip back to string gives same result
   std::string s_roundtrip = string_from_bytes(data_bytes);
   if (s_roundtrip != m_v) {
-    IC_API::trap(PRINCIPAL_ERROR_INVALID_BASE32_ENCODING);
+    IC_API::trap(
+        "Principal Error: Text must be in valid Base32 encoding. Decoding/Encoding roundtrip fails.");
   }
 
   // All is OK, store the bytes of the Principal ID
   m_v_bytes.append_bytes(data_bytes.data(), data_bytes.size());
 }
 
 // convert bytes of principal into string representation
 std::string
 CandidTypePrincipal::string_from_bytes(const std::vector<uint8_t> &data_bytes) {
   // spec: https://internetcomputer.org/docs/current/references/id-encoding-spec
   // m_v = Encode(data) := Group(LowerCase(Base32(CRC32(data) || data)))
 
-  if (data_bytes.size() > MAX_LENGTH_IN_BYTES) {
-    IC_API::trap(PRINCIPAL_ERROR_TEXT_TOO_LONG);
+  if (data_bytes.size() > 29) {
+    IC_API::trap("Principal Error: Text is too long.");
   }
 
   // CRC32(data) - checksum of the data bytes
   std::array<uint8_t, 4> crc_bytes = crc32(data_bytes);
 
   // Base32(CRC32(data) || data)
   std::vector<uint8_t> bytes(crc_bytes.begin(), crc_bytes.end());
@@ -224,15 +225,16 @@
 
   return s;
 }
 
 void CandidTypePrincipal::ungroup(std::string &s) {
   for (size_t i = 5; i < s.size(); i += 6) {
     if (s[i] != '-') {
-      IC_API::trap(PRINCIPAL_ERROR_ABNORMAL_GROUPED);
+      IC_API::trap(
+          "Principal Error: Text should be separated by - (dash) every 5 characters");
     }
   }
   s.erase(std::remove(s.begin(), s.end(), '-'), s.end());
 }
 
 void CandidTypePrincipal::group(std::string &s) {
   if (s.size() > 0) {
```

## icpp/ic/icapi/ic_api.cpp

```diff
@@ -38,15 +38,23 @@
     debug_print("\n--");
     debug_print("IC_API caller's principal:" + m_caller.get_text());
     debug_print("IC_API received these bytes over the wire:");
     m_B_in.debug_print();
   }
 }
 
-IC_API::~IC_API() {}
+IC_API::~IC_API() {
+  // If the method did not yet call to_wire, do it automatic without content
+  if (!m_called_to_wire) {
+    to_wire();
+  }
+
+  // Send the out over the wire
+  msg_reply();
+}
 
 void IC_API::debug_print(const char *message) {
 
   // https:
   // //wiki.sei.cmu.edu/confluence/display/c/INT36-C.+Converting+a+pointer+to+integer+or+integer+to+pointer
   //
   // Use `(uintptr_t)(void *)message` instead of `(uintptr_t)(void *)message`:
@@ -187,24 +195,24 @@
   // Optionally, debug print the final result
   if (m_debug_print) {
     debug_print("\n--");
     debug_print("IC_API 'to_wire' is sending these bytes back:");
     m_B_out.debug_print();
   }
 
-  // Send it out over the wire
-  msg_reply();
+  // Do NOT yet send it out yet via msg_reply. We do this in the desctructor
 }
 
 // Appends the content of m_B_out, replies over the wire, re-sets the didl vectors
 void IC_API::msg_reply() {
 
   m_B_out.trap_if_vec_does_not_start_with_DIDL();
 
   ic0_msg_reply_data_append((uintptr_t)(void *)m_B_out.vec().data(),
                             (uint32_t)m_B_out.size());
-  ic0_msg_reply();
-
   // clear the didl vectors
   m_B_in.clear();
   m_B_out.clear();
+
+  // send it
+  ic0_msg_reply();
 }
```

## Comparing `icpp_free-2.3.0.dist-info/LICENSE` & `icpp_free-2.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `icpp_free-2.3.0.dist-info/METADATA` & `icpp_free-2.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-free
-Version: 2.3.0
+Version: 2.4.0
 Summary: A development platform for C++ smart contracts of the Internet Computer
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: Freemium
 Keywords: Internet Computer,C++,Smart Contracts,blockchain
 Classifier: Development Status :: 4 - Beta
```

## Comparing `icpp_free-2.3.0.dist-info/RECORD` & `icpp_free-2.4.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 icpp/__init__.py,sha256=5BfpNFB6SJywAquvhh7hDVg7sv90_DxJP_cWmvsk2Dc,747
 icpp/__main__.py,sha256=fK15a0FT8qE_XkPGLsFwoPXk7_2ExKzIw2Bhj1SQWwI,1086
 icpp/commands_build_native.py,sha256=bBn8QwjYmzpwNRkzIJF4kpFUr7DL1tAGW4p7kWyBfa8,1053
 icpp/commands_build_wasm.py,sha256=5q7vIhfvZK_b5StH3OG2kMHkTCalsVVekm2YqYgdaV8,5433
 icpp/commands_get.py,sha256=UpriQcUxFU_ahs2Niq7tDwo5d8ZArDo9NcuuYEg1xo0,1122
 icpp/commands_init.py,sha256=gL5AsNL3DqEpla9v2GVHimp7ILAWSKoZBzjbJC7G7rs,753
 icpp/commands_install_wasi_sdk.py,sha256=TRY3p9jzMhhp1G_CMqrUroh4kzQx1SF3tfselmHENg4,3584
-icpp/config_default.py,sha256=1R_F7pl7l1v9Xu1sUY0LyvTCjVu8RN3M3J7UJoHiqZI,5138
+icpp/config_default.py,sha256=Un3r74j1p_bTowUpUIpw_IUJy0lyVeVGuK_W9JFxef0,9612
 icpp/conftest_base.py,sha256=USIU4LOaTrO_G-GKUc4HNftbyuxNzmiltYqgZXHCNeI,2488
 icpp/decorators.py,sha256=L4ZLaoFNuXmiApFqkLTEazHcPx2bWgCTIciNDltN2Hg,2944
 icpp/icpp_toml.py,sha256=4azeRkGyKRx7p3bin7U99NcR2zoboCyt7Ftut3HHS6A,3776
 icpp/options_build.py,sha256=A8RlkYF19wYn1TyQ9TwuMEan2rZ8lJiVRdMsJw93ADs,670
 icpp/options_main.py,sha256=0pXSxX2WFgvelftoyU3vVY9ya98h5U7aiOobLopqkMM,925
 icpp/pro.py,sha256=So9VAIHXfogodjQdNA6mEqcoP2lebq45riqPu3RxYO8,879
 icpp/py.typed,sha256=ZYhofmNLSj2zLe3tuB6mCBQnkX7Hw-vARfbOds4MQJI,98
 icpp/run_shell_cmd.py,sha256=km76SFWq1RgEojH3llp1Na1hP0gSNCKIBsv82bcvphk,5280
 icpp/smoketest.py,sha256=sy6-FSONdgVYgPD2AVeI5cqwoSqFst2tx_1BC0yply8,1463
-icpp/version.py,sha256=S9m32rH2txd0-FRgLNqM_h-EG2jOxM3KlZapx2f2XzM,322
+icpp/version.py,sha256=--dYsnVevGHlF3Tt3flNIyjxoaKCR5MAZCRM7cA6gII,322
 icpp/version_wasi_sdk.py,sha256=XruElxEMxITxIbuH2HyHuSIrTLvQu-dNhIeZwliLv7s,272
 icpp/canisters/greet/README.md,sha256=4_7TnftpGy_nmsBWYxonMxPOp0ZlaAy-RSxG-Um-LTQ,92
+icpp/canisters/greet/demo.sh,sha256=sOVvwST_h8hXHTl4hZRyjFlF0IOgzPEQSIIlK0JvMEE,774
 icpp/canisters/greet/dfx.json,sha256=YJgIaBigJY2m6AHAFkmpNVpiGOAUfacBWMubaGa91is,269
 icpp/canisters/greet/icpp.toml,sha256=xwT4N36kEaCxE_rg2hUY5C4Q5g8dj49VrDv5Z9Rp8SA,474
 icpp/canisters/greet/native/main.cpp,sha256=Iat-ZRjyK9WaTy7lxZ52lrygWhAZhLOxbh8fET74wfc,2061
 icpp/canisters/greet/native/main.h,sha256=5xMtQn9aTHwcjRjCw1BQsrqXx1Uj1bw679lHJTkHD6U,137
 icpp/canisters/greet/src/greet.cpp,sha256=F5THJX203Wm8rf1qGJnfkoapyOpBlb7k0zGtXdRGaak,3022
 icpp/canisters/greet/src/greet.did,sha256=Ac6INjTZLV61gXyFqVcmyeD8FCa0FEbWn0eAH0ufEk4,469
 icpp/canisters/greet/src/greet.h,sha256=Iz4df8nFZImP-VzSSZIRRbMR5EEn5s78RwJsZGMZD6M,354
@@ -99,15 +100,15 @@
 icpp/ic/candid/candid_type_opt_nat8.h,sha256=47BAjR22h02t9kIxaJP4le1_37ihEMOdQAIVApDQ62w,825
 icpp/ic/candid/candid_type_opt_principal.cpp,sha256=QoYoSwnTtQYSdFh94_90a6KB9xMDguQg0oFoKno4-40,2926
 icpp/ic/candid/candid_type_opt_principal.h,sha256=6Q__TuFFrOSA-R_0sRYv3jygm_gkxV05c6QL4zHYl8w,880
 icpp/ic/candid/candid_type_opt_text.cpp,sha256=7dXJ0Rk3-PzHWaEWPNq7Vm-2dDCMtV2YYnZPukzjpcc,2925
 icpp/ic/candid/candid_type_opt_text.h,sha256=s5IzG7mMsvN-q0RGKYax540dF4fokDpI5EodWFKCxz0,853
 icpp/ic/candid/candid_type_prim.cpp,sha256=-DOK_w670MHSZBLq_b8L-kI-QqXl7-MjyHcHfPCrUV8,148
 icpp/ic/candid/candid_type_prim.h,sha256=70cVRF2qkzCNFFmBFy6dh4WnEU3Rx7YnNh2kD0PYTHU,484
-icpp/ic/candid/candid_type_principal.cpp,sha256=j1_bE37AdNSJ0ufyHbqQaPLisWNTF93HHDlXVRpHY28,9545
+icpp/ic/candid/candid_type_principal.cpp,sha256=XgJG87NUhq4Ew509hzxC9p6ZYSd3p3XyMilm4EVvHj8,9697
 icpp/ic/candid/candid_type_principal.h,sha256=Blm0rX5N8X4UVcP3C2YAin3iLRvJmlUKpwnPOLqsTO8,1819
 icpp/ic/candid/candid_type_record.cpp,sha256=veuqsjjX4RXn9DMwXgT7SKb1m4ak3cDWtcGbTPzt9zk,10646
 icpp/ic/candid/candid_type_record.h,sha256=MeqycC5tLaU0_ZKNYJnAXu0ORO5srSnVfBnZQOig40s,1206
 icpp/ic/candid/candid_type_reserved.cpp,sha256=9GSHw2AG2o2zPLi2YpVStRErXNvn_tPvjUYh6twMNM0,1045
 icpp/ic/candid/candid_type_reserved.h,sha256=h1-24Et_kz6H6po9q31XxwgRFxaqjRsYa_gXtuh-UeA,434
 icpp/ic/candid/candid_type_table.cpp,sha256=xY96PMiDwCPhhOsIQuLnyX_t1-2yDJgEQPbql1J8Z6k,2579
 icpp/ic/candid/candid_type_table.h,sha256=6ZGjPHe9B2I4kPrcg50Qy5GaR18zs3WEnEMJwfpCaHk,676
@@ -151,15 +152,15 @@
 icpp/ic/candid/vec_bytes.h,sha256=d3pQLIO32QHeZVzkJM3yQBP-hL4bzvhJgwT0F7Ywh0o,7774
 icpp/ic/ic0/ic0.h,sha256=Kp0YetTZj7yzQDXQtwSW1tKD2ZxIUvxXrSP51SUIZ2E,3407
 icpp/ic/ic0mock/global.h,sha256=iLBQbjovKsiEEHH8DlUR9yrKbpg6pVpG-lEkWhTLN5k,110
 icpp/ic/ic0mock/ic0.cpp,sha256=6T1XJp-NxR1DKh_y728G2Y7yyQuKA8Xq3hNYRek-e54,3288
 icpp/ic/ic0mock/ic0.h,sha256=LIwEeVZVfiXet4pxs9Ot3rPfhg1CtoYVIxPayVxNufY,2091
 icpp/ic/ic0mock/mock_ic.cpp,sha256=SW5_QJ1DaafDcACvw5Y9kMti47AlBv43gUhdObc1vx0,1372
 icpp/ic/ic0mock/mock_ic.h,sha256=-Vxlmw_xM_Zksve6K5Grpd---F5_SrbC_jNSqMdyu8c,1495
-icpp/ic/icapi/ic_api.cpp,sha256=ByAkZovV0-5TCODMFd2FA0Av_qjq68m8zo5dfKg5PB0,5969
+icpp/ic/icapi/ic_api.cpp,sha256=X3qUBqkD-cqOisU6gCqSCs1Yn8coRYCEtJ_JwI10_98,6185
 icpp/ic/icapi/ic_api.h,sha256=eKUmo9xBEHJp-ImsUkYlx2V-0dNid1lWXnfMTynRLtw,2106
 icpp/ic/icapi/wasm_symbol.h,sha256=4LMDxhayAWrroYbNVAcbrL_dWoh0fBVw0BjbxScgpEo,463
 icpp/ic/pro/pro.cpp,sha256=r7G6voSt78p9169JdFhFmS74oFomUEA65R4QRhqIm4k,754
 icpp/ic/pro/pro.h,sha256=EcDcDN4b524nAXDVsNgFJ6vxSEBzBQmkcv34rLUBrSk,393
 icpp/ic/vendors/cppcodec/LICENSE,sha256=wHaXDIE5_9WyjXiO9iQh0fAZWB4kvF4edUEDYx6fwZI,1155
 icpp/ic/vendors/cppcodec/base32_crockford.hpp,sha256=5FagwZyyT-p6LfsC5smTqaQh7K0vKGqBH69Uys6OI7Y,3933
 icpp/ic/vendors/cppcodec/base32_default_crockford.hpp,sha256=k2Z8btmOdcz56QdR2bso2Uf3Ndk81BBkFtoKIpTaLHc,1366
@@ -191,13 +192,13 @@
 icpp/ic/vendors/hash-library/crc32.h,sha256=lG9w03MUpmdeR-bru4e9yJwbvqXLWqYR48tERwL2tXM,1736
 icpp/ic/vendors/hash-library/readme.md,sha256=TISl0NHkS8RLxNyylJJQCDyNiH5-nWixii_pPRqk5Y8,1758
 icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c,sha256=wK61MY-YDkEBG8qIbV-NfUVCCaEQI3AR2GdEhE2z7h8,1370
 icpp/ic/wasi_sdk_traps/ic_trap.c,sha256=YMpQZaaYomfXWU5CqJnCLtYtVvrYNzTWbvwN1slGtbc,327
 icpp/ic/wasi_sdk_traps/ic_trap.h,sha256=XI8GZ_O5sOMpHd3PefoXR_69a1PoFM1Xsbrhl-b3Te4,70
 icpp/ic/wasi_sdk_traps/posix.c,sha256=E808LK-GO22gTm57e2XDeeVSHJ-w6JMubbSo-_u_ZiY,4743
 icpp/ic/wasi_sdk_traps/unreachable.c,sha256=On8IQmEUBJDLOCe1vKVRc55YQbPgm7H1iVzsl6QZldA,10198
-icpp_free-2.3.0.dist-info/LICENSE,sha256=951fAgXYy6YePgpTPC2RI47NRbB-93NVxlnEYaWPYUY,983
-icpp_free-2.3.0.dist-info/METADATA,sha256=H9qxiXSCWkw40v3pcsHEjWevDHXdRoImfpYRhsZMrIs,2274
-icpp_free-2.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-icpp_free-2.3.0.dist-info/entry_points.txt,sha256=TQp3Ak8BiWuu54ZQg6JgcoUle5WojECMzYYL9AXSW6E,44
-icpp_free-2.3.0.dist-info/top_level.txt,sha256=-18t6pp4U_1wjW3LmJN2N7O-rpg6U7Ly1X53MpUk9pA,5
-icpp_free-2.3.0.dist-info/RECORD,,
+icpp_free-2.4.0.dist-info/LICENSE,sha256=951fAgXYy6YePgpTPC2RI47NRbB-93NVxlnEYaWPYUY,983
+icpp_free-2.4.0.dist-info/METADATA,sha256=zsOhx1o1Ap2aEuu2sh7xfc_WDvqPZ8bzwa_kYsLYa9w,2274
+icpp_free-2.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+icpp_free-2.4.0.dist-info/entry_points.txt,sha256=TQp3Ak8BiWuu54ZQg6JgcoUle5WojECMzYYL9AXSW6E,44
+icpp_free-2.4.0.dist-info/top_level.txt,sha256=-18t6pp4U_1wjW3LmJN2N7O-rpg6U7Ly1X53MpUk9pA,5
+icpp_free-2.4.0.dist-info/RECORD,,
```

