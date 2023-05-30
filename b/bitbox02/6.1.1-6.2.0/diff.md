# Comparing `tmp/bitbox02-6.1.1.tar.gz` & `tmp/bitbox02-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbox02-6.1.1.tar", last modified: Tue Aug  9 14:09:53 2022, max compression
+gzip compressed data, was "bitbox02-6.2.0.tar", last modified: Tue May 30 21:24:19 2023, max compression
```

## Comparing `bitbox02-6.1.1.tar` & `bitbox02-6.2.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxrwxr-x   0 beerosagos  (1000) beerosagos  (1000)        0 2022-08-09 14:09:53.915446 bitbox02-6.1.1/
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)    11432 2022-05-19 08:42:05.000000 bitbox02-6.1.1/LICENSE
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)      923 2022-08-09 14:09:53.915446 bitbox02-6.1.1/PKG-INFO
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)      381 2022-05-19 08:42:05.000000 bitbox02-6.1.1/README.md
-drwxrwxr-x   0 beerosagos  (1000) beerosagos  (1000)        0 2022-08-09 14:09:53.911446 bitbox02-6.1.1/bitbox02/
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        0 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/__init__.py
-drwxrwxr-x   0 beerosagos  (1000) beerosagos  (1000)        0 2022-08-09 14:09:53.915446 bitbox02-6.1.1/bitbox02/bitbox02/
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1642 2022-08-09 13:37:09.000000 bitbox02-6.1.1/bitbox02/bitbox02/__init__.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)    43541 2022-06-30 12:59:57.000000 bitbox02-6.1.1/bitbox02/bitbox02/bitbox02.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     7373 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/bitbox02/bootloader.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        0 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/bitbox02/py.typed
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     2371 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/bitbox02/secp256k1.py
-drwxrwxr-x   0 beerosagos  (1000) beerosagos  (1000)        0 2022-08-09 14:09:53.915446 bitbox02-6.1.1/bitbox02/communication/
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1030 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/communication/__init__.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)    27923 2022-06-30 12:59:57.000000 bitbox02-6.1.1/bitbox02/communication/bitbox_api_protocol.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1669 2022-06-30 12:59:57.000000 bitbox02-6.1.1/bitbox02/communication/communication.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     4591 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/communication/devices.py
-drwxrwxr-x   0 beerosagos  (1000) beerosagos  (1000)        0 2022-08-09 14:09:53.915446 bitbox02-6.1.1/bitbox02/communication/generated/
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        0 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/__init__.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1401 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/antiklepto_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     2102 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/backup_commands_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     3851 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/backup_commands_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     2699 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/bitbox02_system_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     5248 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/bitbox02_system_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)    10220 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/btc_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)    32256 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/btc_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     6703 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/cardano_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1664 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/common_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     3152 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/common_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     6698 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/eth_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)    19336 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/eth_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     5757 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/hww_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)    13514 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/hww_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1205 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/keystore_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1308 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/keystore_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1386 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/mnemonic_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1541 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/mnemonic_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1444 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/perform_attestation_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1990 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/perform_attestation_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1186 2022-08-09 08:10:47.000000 bitbox02-6.1.1/bitbox02/communication/generated/system_pb2.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1394 2022-07-13 10:17:31.000000 bitbox02-6.1.1/bitbox02/communication/generated/system_pb2.pyi
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        0 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/communication/py.typed
-drwxrwxr-x   0 beerosagos  (1000) beerosagos  (1000)        0 2022-08-09 14:09:53.915446 bitbox02-6.1.1/bitbox02/communication/u2fhid/
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)      709 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/communication/u2fhid/__init__.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     5800 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/communication/u2fhid/u2fhid.py
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        0 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/py.typed
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     8023 2022-05-19 08:42:05.000000 bitbox02-6.1.1/bitbox02/util.py
-drwxrwxr-x   0 beerosagos  (1000) beerosagos  (1000)        0 2022-08-09 14:09:53.911446 bitbox02-6.1.1/bitbox02.egg-info/
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)      923 2022-08-09 14:09:53.000000 bitbox02-6.1.1/bitbox02.egg-info/PKG-INFO
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     1837 2022-08-09 14:09:53.000000 bitbox02-6.1.1/bitbox02.egg-info/SOURCES.txt
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        1 2022-08-09 14:09:53.000000 bitbox02-6.1.1/bitbox02.egg-info/dependency_links.txt
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        1 2022-06-16 13:04:00.000000 bitbox02-6.1.1/bitbox02.egg-info/not-zip-safe
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)      121 2022-08-09 14:09:53.000000 bitbox02-6.1.1/bitbox02.egg-info/requires.txt
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)        9 2022-08-09 14:09:53.000000 bitbox02-6.1.1/bitbox02.egg-info/top_level.txt
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)       38 2022-08-09 14:09:53.915446 bitbox02-6.1.1/setup.cfg
--rw-rw-r--   0 beerosagos  (1000) beerosagos  (1000)     2902 2022-08-09 09:20:47.000000 bitbox02-6.1.1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.502000 bitbox02-6.2.0/
+-rw-r--r--   0 user      (1000) user      (1000)     1085 2023-05-30 21:24:19.502000 bitbox02-6.2.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      381 2023-01-29 19:30:16.000000 bitbox02-6.2.0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02/bitbox02/
+-rw-r--r--   0 user      (1000) user      (1000)     1642 2023-03-07 13:33:28.000000 bitbox02-6.2.0/bitbox02/bitbox02/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    43686 2023-05-18 09:01:54.000000 bitbox02-6.2.0/bitbox02/bitbox02/bitbox02.py
+-rw-r--r--   0 user      (1000) user      (1000)     7373 2023-02-02 14:05:49.000000 bitbox02-6.2.0/bitbox02/bitbox02/bootloader.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/bitbox02/py.typed
+-rw-r--r--   0 user      (1000) user      (1000)     2371 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/bitbox02/secp256k1.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02/communication/
+-rw-r--r--   0 user      (1000) user      (1000)     1030 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    27923 2023-04-28 20:50:57.000000 bitbox02-6.2.0/bitbox02/communication/bitbox_api_protocol.py
+-rw-r--r--   0 user      (1000) user      (1000)     1669 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/communication.py
+-rw-r--r--   0 user      (1000) user      (1000)     4666 2023-05-29 02:11:48.000000 bitbox02-6.2.0/bitbox02/communication/devices.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.502000 bitbox02-6.2.0/bitbox02/communication/generated/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1401 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/antiklepto_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     2102 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     3851 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     2699 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     5248 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)    10516 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)    33375 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     6703 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/cardano_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1664 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     3152 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     6698 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)    19589 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     5757 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)    13514 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1205 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/keystore_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1308 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/keystore_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1386 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/mnemonic_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1541 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/mnemonic_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1444 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/perform_attestation_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1990 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/perform_attestation_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)     1186 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.py
+-rw-r--r--   0 user      (1000) user      (1000)     1394 2023-05-22 23:23:06.000000 bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.pyi
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/py.typed
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.502000 bitbox02-6.2.0/bitbox02/communication/u2fhid/
+-rw-r--r--   0 user      (1000) user      (1000)      709 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/u2fhid/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5800 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/communication/u2fhid/u2fhid.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/py.typed
+-rw-r--r--   0 user      (1000) user      (1000)     8023 2023-01-29 19:30:16.000000 bitbox02-6.2.0/bitbox02/util.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-30 21:24:19.501000 bitbox02-6.2.0/bitbox02.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1085 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1829 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-02-02 08:31:34.000000 bitbox02-6.2.0/bitbox02.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)      114 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        9 2023-05-30 21:24:19.000000 bitbox02-6.2.0/bitbox02.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-05-30 21:24:19.502000 bitbox02-6.2.0/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     2895 2023-05-30 21:17:12.000000 bitbox02-6.2.0/setup.py
```

### Comparing `bitbox02-6.1.1/bitbox02/bitbox02/__init__.py` & `bitbox02-6.2.0/bitbox02/bitbox02/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Library to interact with a BitBox02 device. """
 
 from __future__ import print_function
 import sys
 
-__version__ = "6.1.1"
+__version__ = "6.2.0"
 
 if sys.version_info.major != 3 or sys.version_info.minor < 6:
     print(
         "Python version is {}.{}, but 3.6+ is required by this script.".format(
             sys.version_info.major, sys.version_info.minor
         ),
         file=sys.stderr,
```

### Comparing `bitbox02-6.1.1/bitbox02/bitbox02/bitbox02.py` & `bitbox02-6.2.0/bitbox02/bitbox02/bitbox02.py`

 * *Files 1% similar despite different names*

```diff
@@ -384,14 +384,15 @@
         self,
         coin: "btc.BTCCoin.V",
         script_configs: Sequence[btc.BTCScriptConfigWithKeypath],
         inputs: Sequence[BTCInputType],
         outputs: Sequence[BTCOutputType],
         version: int = 1,
         locktime: int = 0,
+        format_unit: "btc.BTCSignInitRequest.FormatUnit.V" = btc.BTCSignInitRequest.FormatUnit.DEFAULT,
     ) -> Sequence[Tuple[int, bytes]]:
         """
         coin: the first element of all provided keypaths must match the coin:
         - BTC: 0 + HARDENED
         - Testnets: 1 + HARDENED
         - LTC: 2 + HARDENED
         script_configs: types of all inputs and change outputs. The first element of all provided
@@ -426,14 +427,15 @@
             btc.BTCSignInitRequest(
                 coin=coin,
                 script_configs=script_configs,
                 version=version,
                 num_inputs=len(inputs),
                 num_outputs=len(outputs),
                 locktime=locktime,
+                format_unit=format_unit,
             )
         )
         next_response = self._msg_query(request, expected_response="btc_sign_next").btc_sign_next
 
         is_inputs_pass2 = False
         while True:
             if next_response.type == btc.BTCSignNextResponse.INPUT:
```

### Comparing `bitbox02-6.1.1/bitbox02/bitbox02/bootloader.py` & `bitbox02-6.2.0/bitbox02/bitbox02/bootloader.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/bitbox02/secp256k1.py` & `bitbox02-6.2.0/bitbox02/bitbox02/secp256k1.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/__init__.py` & `bitbox02-6.2.0/bitbox02/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/bitbox_api_protocol.py` & `bitbox02-6.2.0/bitbox02/communication/bitbox_api_protocol.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/communication.py` & `bitbox02-6.2.0/bitbox02/communication/communication.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/devices.py` & `bitbox02-6.2.0/bitbox02/communication/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,10 +156,10 @@
         raise NoneFoundException
     return devices[0]
 
 
 def parse_device_version(serial_number: str) -> semver.VersionInfo:
     match = re.search(r"v([0-9]+\.[0-9]+\.[0-9]+.*)", serial_number)
     if match is None:
-        return None
+        raise Exception(f"Could not parse version string from serial_number: {serial_number}")
 
     return semver.VersionInfo.parse(match.group(1))
```

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/antiklepto_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/antiklepto_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/backup_commands_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/backup_commands_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/backup_commands_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/bitbox02_system_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/bitbox02_system_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/bitbox02_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/btc_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import common_pb2 as common__pb2
 from . import antiklepto_pb2 as antiklepto__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tbtc.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x10\x61ntiklepto.proto\"\xb9\x03\n\x0f\x42TCScriptConfig\x12G\n\x0bsimple_type\x18\x01 \x01(\x0e\x32\x30.shiftcrypto.bitbox02.BTCScriptConfig.SimpleTypeH\x00\x12\x42\n\x08multisig\x18\x02 \x01(\x0b\x32..shiftcrypto.bitbox02.BTCScriptConfig.MultisigH\x00\x1a\xd9\x01\n\x08Multisig\x12\x11\n\tthreshold\x18\x01 \x01(\r\x12)\n\x05xpubs\x18\x02 \x03(\x0b\x32\x1a.shiftcrypto.bitbox02.XPub\x12\x16\n\x0eour_xpub_index\x18\x03 \x01(\r\x12N\n\x0bscript_type\x18\x04 \x01(\x0e\x32\x39.shiftcrypto.bitbox02.BTCScriptConfig.Multisig.ScriptType\"\'\n\nScriptType\x12\t\n\x05P2WSH\x10\x00\x12\x0e\n\nP2WSH_P2SH\x10\x01\"3\n\nSimpleType\x12\x0f\n\x0bP2WPKH_P2SH\x10\x00\x12\n\n\x06P2WPKH\x10\x01\x12\x08\n\x04P2TR\x10\x02\x42\x08\n\x06\x63onfig\"\xfc\x02\n\rBTCPubRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\x41\n\txpub_type\x18\x03 \x01(\x0e\x32,.shiftcrypto.bitbox02.BTCPubRequest.XPubTypeH\x00\x12>\n\rscript_config\x18\x04 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfigH\x00\x12\x0f\n\x07\x64isplay\x18\x05 \x01(\x08\"\x8e\x01\n\x08XPubType\x12\x08\n\x04TPUB\x10\x00\x12\x08\n\x04XPUB\x10\x01\x12\x08\n\x04YPUB\x10\x02\x12\x08\n\x04ZPUB\x10\x03\x12\x08\n\x04VPUB\x10\x04\x12\x08\n\x04UPUB\x10\x05\x12\x10\n\x0c\x43\x41PITAL_VPUB\x10\x06\x12\x10\n\x0c\x43\x41PITAL_ZPUB\x10\x07\x12\x10\n\x0c\x43\x41PITAL_UPUB\x10\x08\x12\x10\n\x0c\x43\x41PITAL_YPUB\x10\tB\x08\n\x06output\"k\n\x1a\x42TCScriptConfigWithKeypath\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\xd7\x01\n\x12\x42TCSignInitRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12H\n\x0escript_configs\x18\x02 \x03(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x12\n\nnum_inputs\x18\x05 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x06 \x01(\r\x12\x10\n\x08locktime\x18\x07 \x01(\r\"\xe8\x02\n\x13\x42TCSignNextResponse\x12<\n\x04type\x18\x01 \x01(\x0e\x32..shiftcrypto.bitbox02.BTCSignNextResponse.Type\x12\r\n\x05index\x18\x02 \x01(\r\x12\x15\n\rhas_signature\x18\x03 \x01(\x08\x12\x11\n\tsignature\x18\x04 \x01(\x0c\x12\x12\n\nprev_index\x18\x05 \x01(\r\x12W\n\x1d\x61nti_klepto_signer_commitment\x18\x06 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitment\"m\n\x04Type\x12\t\n\x05INPUT\x10\x00\x12\n\n\x06OUTPUT\x10\x01\x12\x08\n\x04\x44ONE\x10\x02\x12\x0f\n\x0bPREVTX_INIT\x10\x03\x12\x10\n\x0cPREVTX_INPUT\x10\x04\x12\x11\n\rPREVTX_OUTPUT\x10\x05\x12\x0e\n\nHOST_NONCE\x10\x06\"\xea\x01\n\x13\x42TCSignInputRequest\x12\x13\n\x0bprevOutHash\x18\x01 \x01(\x0c\x12\x14\n\x0cprevOutIndex\x18\x02 \x01(\r\x12\x14\n\x0cprevOutValue\x18\x03 \x01(\x04\x12\x10\n\x08sequence\x18\x04 \x01(\r\x12\x0f\n\x07keypath\x18\x06 \x03(\r\x12\x1b\n\x13script_config_index\x18\x07 \x01(\r\x12R\n\x15host_nonce_commitment\x18\x08 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"\xa5\x01\n\x14\x42TCSignOutputRequest\x12\x0c\n\x04ours\x18\x01 \x01(\x08\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.shiftcrypto.bitbox02.BTCOutputType\x12\r\n\x05value\x18\x03 \x01(\x04\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\x12\x0f\n\x07keypath\x18\x05 \x03(\r\x12\x1b\n\x13script_config_index\x18\x06 \x01(\r\"\x99\x01\n\x1b\x42TCScriptConfigRegistration\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\x0c\n\nBTCSuccess\"m\n\"BTCIsScriptConfigRegisteredRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\"<\n#BTCIsScriptConfigRegisteredResponse\x12\x15\n\ris_registered\x18\x01 \x01(\x08\"\xfc\x01\n\x1e\x42TCRegisterScriptConfigRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\x12\x0c\n\x04name\x18\x02 \x01(\t\x12P\n\txpub_type\x18\x03 \x01(\x0e\x32=.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequest.XPubType\"1\n\x08XPubType\x12\x11\n\rAUTO_ELECTRUM\x10\x00\x12\x12\n\x0e\x41UTO_XPUB_TPUB\x10\x01\"b\n\x14\x42TCPrevTxInitRequest\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x12\n\nnum_inputs\x18\x02 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x03 \x01(\r\x12\x10\n\x08locktime\x18\x04 \x01(\r\"r\n\x15\x42TCPrevTxInputRequest\x12\x15\n\rprev_out_hash\x18\x01 \x01(\x0c\x12\x16\n\x0eprev_out_index\x18\x02 \x01(\r\x12\x18\n\x10signature_script\x18\x03 \x01(\x0c\x12\x10\n\x08sequence\x18\x04 \x01(\r\">\n\x16\x42TCPrevTxOutputRequest\x12\r\n\x05value\x18\x01 \x01(\x04\x12\x15\n\rpubkey_script\x18\x02 \x01(\x0c\"\xee\x01\n\x15\x42TCSignMessageRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12G\n\rscript_config\x18\x02 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0b\n\x03msg\x18\x03 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\x04 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"+\n\x16\x42TCSignMessageResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\"\xb6\x04\n\nBTCRequest\x12_\n\x1bis_script_config_registered\x18\x01 \x01(\x0b\x32\x38.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredRequestH\x00\x12V\n\x16register_script_config\x18\x02 \x01(\x0b\x32\x34.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequestH\x00\x12\x41\n\x0bprevtx_init\x18\x03 \x01(\x0b\x32*.shiftcrypto.bitbox02.BTCPrevTxInitRequestH\x00\x12\x43\n\x0cprevtx_input\x18\x04 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCPrevTxInputRequestH\x00\x12\x45\n\rprevtx_output\x18\x05 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCPrevTxOutputRequestH\x00\x12\x43\n\x0csign_message\x18\x06 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCSignMessageRequestH\x00\x12P\n\x14\x61ntiklepto_signature\x18\x07 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignatureRequestH\x00\x42\t\n\x07request\"\x90\x03\n\x0b\x42TCResponse\x12\x33\n\x07success\x18\x01 \x01(\x0b\x32 .shiftcrypto.bitbox02.BTCSuccessH\x00\x12`\n\x1bis_script_config_registered\x18\x02 \x01(\x0b\x32\x39.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredResponseH\x00\x12>\n\tsign_next\x18\x03 \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignNextResponseH\x00\x12\x44\n\x0csign_message\x18\x04 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCSignMessageResponseH\x00\x12X\n\x1c\x61ntiklepto_signer_commitment\x18\x05 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitmentH\x00\x42\n\n\x08response*/\n\x07\x42TCCoin\x12\x07\n\x03\x42TC\x10\x00\x12\x08\n\x04TBTC\x10\x01\x12\x07\n\x03LTC\x10\x02\x12\x08\n\x04TLTC\x10\x03*R\n\rBTCOutputType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05P2PKH\x10\x01\x12\x08\n\x04P2SH\x10\x02\x12\n\n\x06P2WPKH\x10\x03\x12\t\n\x05P2WSH\x10\x04\x12\x08\n\x04P2TR\x10\x05\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tbtc.proto\x12\x14shiftcrypto.bitbox02\x1a\x0c\x63ommon.proto\x1a\x10\x61ntiklepto.proto\"\xb9\x03\n\x0f\x42TCScriptConfig\x12G\n\x0bsimple_type\x18\x01 \x01(\x0e\x32\x30.shiftcrypto.bitbox02.BTCScriptConfig.SimpleTypeH\x00\x12\x42\n\x08multisig\x18\x02 \x01(\x0b\x32..shiftcrypto.bitbox02.BTCScriptConfig.MultisigH\x00\x1a\xd9\x01\n\x08Multisig\x12\x11\n\tthreshold\x18\x01 \x01(\r\x12)\n\x05xpubs\x18\x02 \x03(\x0b\x32\x1a.shiftcrypto.bitbox02.XPub\x12\x16\n\x0eour_xpub_index\x18\x03 \x01(\r\x12N\n\x0bscript_type\x18\x04 \x01(\x0e\x32\x39.shiftcrypto.bitbox02.BTCScriptConfig.Multisig.ScriptType\"\'\n\nScriptType\x12\t\n\x05P2WSH\x10\x00\x12\x0e\n\nP2WSH_P2SH\x10\x01\"3\n\nSimpleType\x12\x0f\n\x0bP2WPKH_P2SH\x10\x00\x12\n\n\x06P2WPKH\x10\x01\x12\x08\n\x04P2TR\x10\x02\x42\x08\n\x06\x63onfig\"\xfc\x02\n\rBTCPubRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12\x0f\n\x07keypath\x18\x02 \x03(\r\x12\x41\n\txpub_type\x18\x03 \x01(\x0e\x32,.shiftcrypto.bitbox02.BTCPubRequest.XPubTypeH\x00\x12>\n\rscript_config\x18\x04 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfigH\x00\x12\x0f\n\x07\x64isplay\x18\x05 \x01(\x08\"\x8e\x01\n\x08XPubType\x12\x08\n\x04TPUB\x10\x00\x12\x08\n\x04XPUB\x10\x01\x12\x08\n\x04YPUB\x10\x02\x12\x08\n\x04ZPUB\x10\x03\x12\x08\n\x04VPUB\x10\x04\x12\x08\n\x04UPUB\x10\x05\x12\x10\n\x0c\x43\x41PITAL_VPUB\x10\x06\x12\x10\n\x0c\x43\x41PITAL_ZPUB\x10\x07\x12\x10\n\x0c\x43\x41PITAL_UPUB\x10\x08\x12\x10\n\x0c\x43\x41PITAL_YPUB\x10\tB\x08\n\x06output\"k\n\x1a\x42TCScriptConfigWithKeypath\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\xc5\x02\n\x12\x42TCSignInitRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12H\n\x0escript_configs\x18\x02 \x03(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0f\n\x07version\x18\x04 \x01(\r\x12\x12\n\nnum_inputs\x18\x05 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x06 \x01(\r\x12\x10\n\x08locktime\x18\x07 \x01(\r\x12H\n\x0b\x66ormat_unit\x18\x08 \x01(\x0e\x32\x33.shiftcrypto.bitbox02.BTCSignInitRequest.FormatUnit\"\"\n\nFormatUnit\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x07\n\x03SAT\x10\x01\"\xe8\x02\n\x13\x42TCSignNextResponse\x12<\n\x04type\x18\x01 \x01(\x0e\x32..shiftcrypto.bitbox02.BTCSignNextResponse.Type\x12\r\n\x05index\x18\x02 \x01(\r\x12\x15\n\rhas_signature\x18\x03 \x01(\x08\x12\x11\n\tsignature\x18\x04 \x01(\x0c\x12\x12\n\nprev_index\x18\x05 \x01(\r\x12W\n\x1d\x61nti_klepto_signer_commitment\x18\x06 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitment\"m\n\x04Type\x12\t\n\x05INPUT\x10\x00\x12\n\n\x06OUTPUT\x10\x01\x12\x08\n\x04\x44ONE\x10\x02\x12\x0f\n\x0bPREVTX_INIT\x10\x03\x12\x10\n\x0cPREVTX_INPUT\x10\x04\x12\x11\n\rPREVTX_OUTPUT\x10\x05\x12\x0e\n\nHOST_NONCE\x10\x06\"\xea\x01\n\x13\x42TCSignInputRequest\x12\x13\n\x0bprevOutHash\x18\x01 \x01(\x0c\x12\x14\n\x0cprevOutIndex\x18\x02 \x01(\r\x12\x14\n\x0cprevOutValue\x18\x03 \x01(\x04\x12\x10\n\x08sequence\x18\x04 \x01(\r\x12\x0f\n\x07keypath\x18\x06 \x03(\r\x12\x1b\n\x13script_config_index\x18\x07 \x01(\r\x12R\n\x15host_nonce_commitment\x18\x08 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"\xa5\x01\n\x14\x42TCSignOutputRequest\x12\x0c\n\x04ours\x18\x01 \x01(\x08\x12\x31\n\x04type\x18\x02 \x01(\x0e\x32#.shiftcrypto.bitbox02.BTCOutputType\x12\r\n\x05value\x18\x03 \x01(\x04\x12\x0f\n\x07payload\x18\x04 \x01(\x0c\x12\x0f\n\x07keypath\x18\x05 \x03(\r\x12\x1b\n\x13script_config_index\x18\x06 \x01(\r\"\x99\x01\n\x1b\x42TCScriptConfigRegistration\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12<\n\rscript_config\x18\x02 \x01(\x0b\x32%.shiftcrypto.bitbox02.BTCScriptConfig\x12\x0f\n\x07keypath\x18\x03 \x03(\r\"\x0c\n\nBTCSuccess\"m\n\"BTCIsScriptConfigRegisteredRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\"<\n#BTCIsScriptConfigRegisteredResponse\x12\x15\n\ris_registered\x18\x01 \x01(\x08\"\xfc\x01\n\x1e\x42TCRegisterScriptConfigRequest\x12G\n\x0cregistration\x18\x01 \x01(\x0b\x32\x31.shiftcrypto.bitbox02.BTCScriptConfigRegistration\x12\x0c\n\x04name\x18\x02 \x01(\t\x12P\n\txpub_type\x18\x03 \x01(\x0e\x32=.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequest.XPubType\"1\n\x08XPubType\x12\x11\n\rAUTO_ELECTRUM\x10\x00\x12\x12\n\x0e\x41UTO_XPUB_TPUB\x10\x01\"b\n\x14\x42TCPrevTxInitRequest\x12\x0f\n\x07version\x18\x01 \x01(\r\x12\x12\n\nnum_inputs\x18\x02 \x01(\r\x12\x13\n\x0bnum_outputs\x18\x03 \x01(\r\x12\x10\n\x08locktime\x18\x04 \x01(\r\"r\n\x15\x42TCPrevTxInputRequest\x12\x15\n\rprev_out_hash\x18\x01 \x01(\x0c\x12\x16\n\x0eprev_out_index\x18\x02 \x01(\r\x12\x18\n\x10signature_script\x18\x03 \x01(\x0c\x12\x10\n\x08sequence\x18\x04 \x01(\r\">\n\x16\x42TCPrevTxOutputRequest\x12\r\n\x05value\x18\x01 \x01(\x04\x12\x15\n\rpubkey_script\x18\x02 \x01(\x0c\"\xee\x01\n\x15\x42TCSignMessageRequest\x12+\n\x04\x63oin\x18\x01 \x01(\x0e\x32\x1d.shiftcrypto.bitbox02.BTCCoin\x12G\n\rscript_config\x18\x02 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.BTCScriptConfigWithKeypath\x12\x0b\n\x03msg\x18\x03 \x01(\x0c\x12R\n\x15host_nonce_commitment\x18\x04 \x01(\x0b\x32\x33.shiftcrypto.bitbox02.AntiKleptoHostNonceCommitment\"+\n\x16\x42TCSignMessageResponse\x12\x11\n\tsignature\x18\x01 \x01(\x0c\"\xb6\x04\n\nBTCRequest\x12_\n\x1bis_script_config_registered\x18\x01 \x01(\x0b\x32\x38.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredRequestH\x00\x12V\n\x16register_script_config\x18\x02 \x01(\x0b\x32\x34.shiftcrypto.bitbox02.BTCRegisterScriptConfigRequestH\x00\x12\x41\n\x0bprevtx_init\x18\x03 \x01(\x0b\x32*.shiftcrypto.bitbox02.BTCPrevTxInitRequestH\x00\x12\x43\n\x0cprevtx_input\x18\x04 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCPrevTxInputRequestH\x00\x12\x45\n\rprevtx_output\x18\x05 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCPrevTxOutputRequestH\x00\x12\x43\n\x0csign_message\x18\x06 \x01(\x0b\x32+.shiftcrypto.bitbox02.BTCSignMessageRequestH\x00\x12P\n\x14\x61ntiklepto_signature\x18\x07 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignatureRequestH\x00\x42\t\n\x07request\"\x90\x03\n\x0b\x42TCResponse\x12\x33\n\x07success\x18\x01 \x01(\x0b\x32 .shiftcrypto.bitbox02.BTCSuccessH\x00\x12`\n\x1bis_script_config_registered\x18\x02 \x01(\x0b\x32\x39.shiftcrypto.bitbox02.BTCIsScriptConfigRegisteredResponseH\x00\x12>\n\tsign_next\x18\x03 \x01(\x0b\x32).shiftcrypto.bitbox02.BTCSignNextResponseH\x00\x12\x44\n\x0csign_message\x18\x04 \x01(\x0b\x32,.shiftcrypto.bitbox02.BTCSignMessageResponseH\x00\x12X\n\x1c\x61ntiklepto_signer_commitment\x18\x05 \x01(\x0b\x32\x30.shiftcrypto.bitbox02.AntiKleptoSignerCommitmentH\x00\x42\n\n\x08response*/\n\x07\x42TCCoin\x12\x07\n\x03\x42TC\x10\x00\x12\x08\n\x04TBTC\x10\x01\x12\x07\n\x03LTC\x10\x02\x12\x08\n\x04TLTC\x10\x03*R\n\rBTCOutputType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05P2PKH\x10\x01\x12\x08\n\x04P2SH\x10\x02\x12\n\n\x06P2WPKH\x10\x03\x12\t\n\x05P2WSH\x10\x04\x12\x08\n\x04P2TR\x10\x05\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'btc_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _BTCCOIN._serialized_start=4125
-  _BTCCOIN._serialized_end=4172
-  _BTCOUTPUTTYPE._serialized_start=4174
-  _BTCOUTPUTTYPE._serialized_end=4256
+  _BTCCOIN._serialized_start=4235
+  _BTCCOIN._serialized_end=4282
+  _BTCOUTPUTTYPE._serialized_start=4284
+  _BTCOUTPUTTYPE._serialized_end=4366
   _BTCSCRIPTCONFIG._serialized_start=68
   _BTCSCRIPTCONFIG._serialized_end=509
   _BTCSCRIPTCONFIG_MULTISIG._serialized_start=229
   _BTCSCRIPTCONFIG_MULTISIG._serialized_end=446
   _BTCSCRIPTCONFIG_MULTISIG_SCRIPTTYPE._serialized_start=407
   _BTCSCRIPTCONFIG_MULTISIG_SCRIPTTYPE._serialized_end=446
   _BTCSCRIPTCONFIG_SIMPLETYPE._serialized_start=448
@@ -37,43 +37,45 @@
   _BTCPUBREQUEST._serialized_start=512
   _BTCPUBREQUEST._serialized_end=892
   _BTCPUBREQUEST_XPUBTYPE._serialized_start=740
   _BTCPUBREQUEST_XPUBTYPE._serialized_end=882
   _BTCSCRIPTCONFIGWITHKEYPATH._serialized_start=894
   _BTCSCRIPTCONFIGWITHKEYPATH._serialized_end=1001
   _BTCSIGNINITREQUEST._serialized_start=1004
-  _BTCSIGNINITREQUEST._serialized_end=1219
-  _BTCSIGNNEXTRESPONSE._serialized_start=1222
-  _BTCSIGNNEXTRESPONSE._serialized_end=1582
-  _BTCSIGNNEXTRESPONSE_TYPE._serialized_start=1473
-  _BTCSIGNNEXTRESPONSE_TYPE._serialized_end=1582
-  _BTCSIGNINPUTREQUEST._serialized_start=1585
-  _BTCSIGNINPUTREQUEST._serialized_end=1819
-  _BTCSIGNOUTPUTREQUEST._serialized_start=1822
-  _BTCSIGNOUTPUTREQUEST._serialized_end=1987
-  _BTCSCRIPTCONFIGREGISTRATION._serialized_start=1990
-  _BTCSCRIPTCONFIGREGISTRATION._serialized_end=2143
-  _BTCSUCCESS._serialized_start=2145
-  _BTCSUCCESS._serialized_end=2157
-  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_start=2159
-  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_end=2268
-  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_start=2270
-  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_end=2330
-  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_start=2333
-  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_end=2585
-  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_start=2536
-  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_end=2585
-  _BTCPREVTXINITREQUEST._serialized_start=2587
-  _BTCPREVTXINITREQUEST._serialized_end=2685
-  _BTCPREVTXINPUTREQUEST._serialized_start=2687
-  _BTCPREVTXINPUTREQUEST._serialized_end=2801
-  _BTCPREVTXOUTPUTREQUEST._serialized_start=2803
-  _BTCPREVTXOUTPUTREQUEST._serialized_end=2865
-  _BTCSIGNMESSAGEREQUEST._serialized_start=2868
-  _BTCSIGNMESSAGEREQUEST._serialized_end=3106
-  _BTCSIGNMESSAGERESPONSE._serialized_start=3108
-  _BTCSIGNMESSAGERESPONSE._serialized_end=3151
-  _BTCREQUEST._serialized_start=3154
-  _BTCREQUEST._serialized_end=3720
-  _BTCRESPONSE._serialized_start=3723
-  _BTCRESPONSE._serialized_end=4123
+  _BTCSIGNINITREQUEST._serialized_end=1329
+  _BTCSIGNINITREQUEST_FORMATUNIT._serialized_start=1295
+  _BTCSIGNINITREQUEST_FORMATUNIT._serialized_end=1329
+  _BTCSIGNNEXTRESPONSE._serialized_start=1332
+  _BTCSIGNNEXTRESPONSE._serialized_end=1692
+  _BTCSIGNNEXTRESPONSE_TYPE._serialized_start=1583
+  _BTCSIGNNEXTRESPONSE_TYPE._serialized_end=1692
+  _BTCSIGNINPUTREQUEST._serialized_start=1695
+  _BTCSIGNINPUTREQUEST._serialized_end=1929
+  _BTCSIGNOUTPUTREQUEST._serialized_start=1932
+  _BTCSIGNOUTPUTREQUEST._serialized_end=2097
+  _BTCSCRIPTCONFIGREGISTRATION._serialized_start=2100
+  _BTCSCRIPTCONFIGREGISTRATION._serialized_end=2253
+  _BTCSUCCESS._serialized_start=2255
+  _BTCSUCCESS._serialized_end=2267
+  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_start=2269
+  _BTCISSCRIPTCONFIGREGISTEREDREQUEST._serialized_end=2378
+  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_start=2380
+  _BTCISSCRIPTCONFIGREGISTEREDRESPONSE._serialized_end=2440
+  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_start=2443
+  _BTCREGISTERSCRIPTCONFIGREQUEST._serialized_end=2695
+  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_start=2646
+  _BTCREGISTERSCRIPTCONFIGREQUEST_XPUBTYPE._serialized_end=2695
+  _BTCPREVTXINITREQUEST._serialized_start=2697
+  _BTCPREVTXINITREQUEST._serialized_end=2795
+  _BTCPREVTXINPUTREQUEST._serialized_start=2797
+  _BTCPREVTXINPUTREQUEST._serialized_end=2911
+  _BTCPREVTXOUTPUTREQUEST._serialized_start=2913
+  _BTCPREVTXOUTPUTREQUEST._serialized_end=2975
+  _BTCSIGNMESSAGEREQUEST._serialized_start=2978
+  _BTCSIGNMESSAGEREQUEST._serialized_end=3216
+  _BTCSIGNMESSAGERESPONSE._serialized_start=3218
+  _BTCSIGNMESSAGERESPONSE._serialized_end=3261
+  _BTCREQUEST._serialized_start=3264
+  _BTCREQUEST._serialized_end=3830
+  _BTCRESPONSE._serialized_start=3833
+  _BTCRESPONSE._serialized_end=4233
 # @@protoc_insertion_point(module_scope)
```

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/btc_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/btc_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -233,43 +233,67 @@
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["script_config",b"script_config"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["keypath",b"keypath","script_config",b"script_config"]) -> None: ...
 global___BTCScriptConfigWithKeypath = BTCScriptConfigWithKeypath
 
 class BTCSignInitRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    class _FormatUnit:
+        ValueType = typing.NewType('ValueType', builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+    class _FormatUnitEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[BTCSignInitRequest._FormatUnit.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        DEFAULT: BTCSignInitRequest._FormatUnit.ValueType  # 0
+        """According to `coin` (BTC, LTC, etc.)."""
+
+        SAT: BTCSignInitRequest._FormatUnit.ValueType  # 1
+        """Only valid for BTC/TBTC, formats as "sat"/"tsat"."""
+
+    class FormatUnit(_FormatUnit, metaclass=_FormatUnitEnumTypeWrapper):
+        pass
+
+    DEFAULT: BTCSignInitRequest.FormatUnit.ValueType  # 0
+    """According to `coin` (BTC, LTC, etc.)."""
+
+    SAT: BTCSignInitRequest.FormatUnit.ValueType  # 1
+    """Only valid for BTC/TBTC, formats as "sat"/"tsat"."""
+
+
     COIN_FIELD_NUMBER: builtins.int
     SCRIPT_CONFIGS_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     NUM_INPUTS_FIELD_NUMBER: builtins.int
     NUM_OUTPUTS_FIELD_NUMBER: builtins.int
     LOCKTIME_FIELD_NUMBER: builtins.int
+    FORMAT_UNIT_FIELD_NUMBER: builtins.int
     coin: global___BTCCoin.ValueType
     @property
     def script_configs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___BTCScriptConfigWithKeypath]:
         """used script configs in inputs and changes"""
         pass
     version: builtins.int
     """must be 1 or 2"""
 
     num_inputs: builtins.int
     num_outputs: builtins.int
     locktime: builtins.int
     """must be <500000000"""
 
+    format_unit: global___BTCSignInitRequest.FormatUnit.ValueType
     def __init__(self,
         *,
         coin: global___BTCCoin.ValueType = ...,
         script_configs: typing.Optional[typing.Iterable[global___BTCScriptConfigWithKeypath]] = ...,
         version: builtins.int = ...,
         num_inputs: builtins.int = ...,
         num_outputs: builtins.int = ...,
         locktime: builtins.int = ...,
+        format_unit: global___BTCSignInitRequest.FormatUnit.ValueType = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["coin",b"coin","locktime",b"locktime","num_inputs",b"num_inputs","num_outputs",b"num_outputs","script_configs",b"script_configs","version",b"version"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["coin",b"coin","format_unit",b"format_unit","locktime",b"locktime","num_inputs",b"num_inputs","num_outputs",b"num_outputs","script_configs",b"script_configs","version",b"version"]) -> None: ...
 global___BTCSignInitRequest = BTCSignInitRequest
 
 class BTCSignNextResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class _Type:
         ValueType = typing.NewType('ValueType', builtins.int)
         V: typing_extensions.TypeAlias = ValueType
```

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/cardano_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/cardano_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/common_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/common_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/eth_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/eth_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/eth_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,21 +17,30 @@
 class _ETHCoin:
     ValueType = typing.NewType('ValueType', builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 class _ETHCoinEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ETHCoin.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     ETH: _ETHCoin.ValueType  # 0
     RopstenETH: _ETHCoin.ValueType  # 1
+    """Removed in v9.14.0 - deprecated"""
+
     RinkebyETH: _ETHCoin.ValueType  # 2
+    """Removed in v9.14.0 - deprecated"""
+
 class ETHCoin(_ETHCoin, metaclass=_ETHCoinEnumTypeWrapper):
+    """Kept for backwards compatibility. Use chain_id instead, introduced in v9.10.0."""
     pass
 
 ETH: ETHCoin.ValueType  # 0
 RopstenETH: ETHCoin.ValueType  # 1
+"""Removed in v9.14.0 - deprecated"""
+
 RinkebyETH: ETHCoin.ValueType  # 2
+"""Removed in v9.14.0 - deprecated"""
+
 global___ETHCoin = ETHCoin
 
 
 class ETHPubRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     class _OutputType:
         ValueType = typing.NewType('ValueType', builtins.int)
```

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/hww_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/hww_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/hww_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/keystore_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/keystore_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/keystore_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/keystore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/mnemonic_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/mnemonic_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/mnemonic_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/mnemonic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/perform_attestation_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/perform_attestation_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/perform_attestation_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/perform_attestation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/system_pb2.py` & `bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/generated/system_pb2.pyi` & `bitbox02-6.2.0/bitbox02/communication/generated/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/u2fhid/__init__.py` & `bitbox02-6.2.0/bitbox02/communication/u2fhid/__init__.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/communication/u2fhid/u2fhid.py` & `bitbox02-6.2.0/bitbox02/communication/u2fhid/u2fhid.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02/util.py` & `bitbox02-6.2.0/bitbox02/util.py`

 * *Files identical despite different names*

### Comparing `bitbox02-6.1.1/bitbox02.egg-info/SOURCES.txt` & `bitbox02-6.2.0/bitbox02.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 bitbox02/__init__.py
 bitbox02/py.typed
 bitbox02/util.py
 bitbox02.egg-info/PKG-INFO
 bitbox02.egg-info/SOURCES.txt
```

### Comparing `bitbox02-6.1.1/setup.py` & `bitbox02-6.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             "mnemonic_pb2.pyi",
             "perform_attestation_pb2.pyi",
             "random_number_pb2.pyi",
             "system_pb2.pyi",
         ],
     },
     install_requires=[
-        "hidapi>=0.7.99.post21",
+        "hidapi>=0.14.0",
         "noiseprotocol>=0.3",
         "protobuf>=3.20",
         "ecdsa>=0.14",
         "semver>=2.8.1",
         # Needed as long as we support python < 3.7
         "typing_extensions>=3.7.4",
         "base58>=2.0.0",
```

