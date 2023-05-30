# Comparing `tmp/eulith-trezor-0.0.1.tar.gz` & `tmp/eulith-trezor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulith-trezor-0.0.1.tar", last modified: Tue May 30 19:38:45 2023, max compression
+gzip compressed data, was "eulith-trezor-0.0.2.tar", last modified: Tue May 30 19:42:26 2023, max compression
```

## Comparing `eulith-trezor-0.0.1.tar` & `eulith-trezor-0.0.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.934851 eulith-trezor-0.0.1/
--rw-r--r--   0 kristian   (501) staff       (20)      845 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/AUTHORS
--rw-r--r--   0 kristian   (501) staff       (20)    34509 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/CHANGELOG.md
--rw-r--r--   0 kristian   (501) staff       (20)     7651 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/COPYING
--rw-r--r--   0 kristian   (501) staff       (20)      216 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/MANIFEST.in
--rw-r--r--   0 kristian   (501) staff       (20)    39981 2023-05-30 19:38:45.934991 eulith-trezor-0.0.1/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)     4640 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/README.md
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.911768 eulith-trezor-0.0.1/bash_completion.d/
--rw-r--r--   0 kristian   (501) staff       (20)      509 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/bash_completion.d/trezorctl.sh
--rw-r--r--   0 kristian   (501) staff       (20)      103 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/requirements-optional.txt
--rw-r--r--   0 kristian   (501) staff       (20)      215 2023-05-30 19:05:08.000000 eulith-trezor-0.0.1/requirements.txt
--rw-r--r--   0 kristian   (501) staff       (20)      778 2023-05-30 19:38:45.935309 eulith-trezor-0.0.1/setup.cfg
--rwxr-xr-x   0 kristian   (501) staff       (20)     2627 2023-05-30 19:33:50.000000 eulith-trezor-0.0.1/setup.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.909437 eulith-trezor-0.0.1/src/
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.912907 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/
--rw-r--r--   0 kristian   (501) staff       (20)    39981 2023-05-30 19:38:45.000000 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/PKG-INFO
--rw-r--r--   0 kristian   (501) staff       (20)     2848 2023-05-30 19:38:45.000000 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/SOURCES.txt
--rw-r--r--   0 kristian   (501) staff       (20)        1 2023-05-30 19:38:45.000000 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/dependency_links.txt
--rw-r--r--   0 kristian   (501) staff       (20)       58 2023-05-30 19:38:45.000000 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/entry_points.txt
--rw-r--r--   0 kristian   (501) staff       (20)        1 2023-05-30 19:37:34.000000 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/not-zip-safe
--rw-r--r--   0 kristian   (501) staff       (20)      517 2023-05-30 19:38:45.000000 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/requires.txt
--rw-r--r--   0 kristian   (501) staff       (20)       10 2023-05-30 19:38:45.000000 eulith-trezor-0.0.1/src/eulith_trezor.egg-info/top_level.txt
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.921491 eulith-trezor-0.0.1/src/trezorlib/
--rw-r--r--   0 kristian   (501) staff       (20)      703 2023-05-30 19:38:25.000000 eulith-trezor-0.0.1/src/trezorlib/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     7594 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/_ed25519.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.922418 eulith-trezor-0.0.1/src/trezorlib/_internal/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/_internal/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     9090 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/_internal/emulator.py
--rw-r--r--   0 kristian   (501) staff       (20)    16788 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/_internal/firmware_headers.py
--rw-r--r--   0 kristian   (501) staff       (20)     2660 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/binance.py
--rw-r--r--   0 kristian   (501) staff       (20)    15097 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/btc.py
--rw-r--r--   0 kristian   (501) staff       (20)    33111 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cardano.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.926332 eulith-trezor-0.0.1/src/trezorlib/cli/
--rw-r--r--   0 kristian   (501) staff       (20)     6980 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     2322 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/binance.py
--rw-r--r--   0 kristian   (501) staff       (20)    14540 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/btc.py
--rw-r--r--   0 kristian   (501) staff       (20)    10522 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/cardano.py
--rw-r--r--   0 kristian   (501) staff       (20)     2552 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/cosi.py
--rw-r--r--   0 kristian   (501) staff       (20)     3537 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/crypto.py
--rw-r--r--   0 kristian   (501) staff       (20)     3433 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/debug.py
--rw-r--r--   0 kristian   (501) staff       (20)    10002 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/device.py
--rw-r--r--   0 kristian   (501) staff       (20)     1990 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/eos.py
--rw-r--r--   0 kristian   (501) staff       (20)    19318 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/ethereum.py
--rw-r--r--   0 kristian   (501) staff       (20)     4411 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/fido.py
--rw-r--r--   0 kristian   (501) staff       (20)    21462 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/firmware.py
--rw-r--r--   0 kristian   (501) staff       (20)     2363 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/monero.py
--rw-r--r--   0 kristian   (501) staff       (20)     2352 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/nem.py
--rw-r--r--   0 kristian   (501) staff       (20)     2025 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/ripple.py
--rw-r--r--   0 kristian   (501) staff       (20)    11156 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/settings.py
--rw-r--r--   0 kristian   (501) staff       (20)     3298 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/stellar.py
--rw-r--r--   0 kristian   (501) staff       (20)     2274 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/tezos.py
--rwxr-xr-x   0 kristian   (501) staff       (20)    12805 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cli/trezorctl.py
--rw-r--r--   0 kristian   (501) staff       (20)    18867 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/client.py
--rw-r--r--   0 kristian   (501) staff       (20)     6056 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/cosi.py
--rw-r--r--   0 kristian   (501) staff       (20)    42139 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/debuglink.py
--rw-r--r--   0 kristian   (501) staff       (20)     4375 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/definitions.py
--rw-r--r--   0 kristian   (501) staff       (20)     8184 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/device.py
--rw-r--r--   0 kristian   (501) staff       (20)    11278 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/eos.py
--rw-r--r--   0 kristian   (501) staff       (20)    13564 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/ethereum.py
--rw-r--r--   0 kristian   (501) staff       (20)     1601 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/exceptions.py
--rw-r--r--   0 kristian   (501) staff       (20)     1969 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/fido.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.927920 eulith-trezor-0.0.1/src/trezorlib/firmware/
--rw-r--r--   0 kristian   (501) staff       (20)     3612 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/firmware/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     1217 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/firmware/consts.py
--rw-r--r--   0 kristian   (501) staff       (20)     6339 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/firmware/core.py
--rw-r--r--   0 kristian   (501) staff       (20)     6526 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/firmware/legacy.py
--rw-r--r--   0 kristian   (501) staff       (20)     5976 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/firmware/models.py
--rw-r--r--   0 kristian   (501) staff       (20)     1252 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/firmware/util.py
--rw-r--r--   0 kristian   (501) staff       (20)     4760 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/firmware/vendor.py
--rw-r--r--   0 kristian   (501) staff       (20)     2260 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/log.py
--rw-r--r--   0 kristian   (501) staff       (20)     3499 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/mapping.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     6356 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/merkle_tree.py
--rw-r--r--   0 kristian   (501) staff       (20)   261786 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/messages.py
--rw-r--r--   0 kristian   (501) staff       (20)     3224 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/misc.py
--rw-r--r--   0 kristian   (501) staff       (20)     1871 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/models.py
--rw-r--r--   0 kristian   (501) staff       (20)     1676 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/monero.py
--rw-r--r--   0 kristian   (501) staff       (20)     7467 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/nem.py
--rw-r--r--   0 kristian   (501) staff       (20)    20836 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/protobuf.py
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/py.typed
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.928225 eulith-trezor-0.0.1/src/trezorlib/qt/
--rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/qt/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     5543 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/qt/pinmatrix.py
--rw-r--r--   0 kristian   (501) staff       (20)     2140 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/ripple.py
--rw-r--r--   0 kristian   (501) staff       (20)    13873 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/stellar.py
--rw-r--r--   0 kristian   (501) staff       (20)     1702 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/tezos.py
--rw-r--r--   0 kristian   (501) staff       (20)     7918 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/toif.py
--rw-r--r--   0 kristian   (501) staff       (20)    11186 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/tools.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.929696 eulith-trezor-0.0.1/src/trezorlib/transport/
--rw-r--r--   0 kristian   (501) staff       (20)     5167 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/transport/__init__.py
--rw-r--r--   0 kristian   (501) staff       (20)     5986 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/transport/bridge.py
--rw-r--r--   0 kristian   (501) staff       (20)     5556 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/transport/hid.py
--rw-r--r--   0 kristian   (501) staff       (20)     5372 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/transport/protocol.py
--rw-r--r--   0 kristian   (501) staff       (20)     4961 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/transport/udp.py
--rw-r--r--   0 kristian   (501) staff       (20)     5753 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/transport/webusb.py
--rw-r--r--   0 kristian   (501) staff       (20)     9029 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/src/trezorlib/ui.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.931574 eulith-trezor-0.0.1/tests/
--rw-r--r--   0 kristian   (501) staff       (20)    10705 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_btc.py
--rw-r--r--   0 kristian   (501) staff       (20)     6933 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_cosi.py
--rw-r--r--   0 kristian   (501) staff       (20)     4231 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_firmware.py
--rw-r--r--   0 kristian   (501) staff       (20)     3209 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_merkle_tree.py
--rw-r--r--   0 kristian   (501) staff       (20)     1571 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_nem.py
--rw-r--r--   0 kristian   (501) staff       (20)     9635 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_protobuf_encoding.py
--rw-r--r--   0 kristian   (501) staff       (20)     7343 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_protobuf_misc.py
--rw-r--r--   0 kristian   (501) staff       (20)    34184 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_stellar.py
--rw-r--r--   0 kristian   (501) staff       (20)     1845 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_tools.py
--rw-r--r--   0 kristian   (501) staff       (20)     1838 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tests/test_transport.py
-drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:38:45.934655 eulith-trezor-0.0.1/tools/
--rwxr-xr-x   0 kristian   (501) staff       (20)     6692 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/build_tx.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     3000 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/deserialize_tx.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     4593 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/encfs_aes_getpass.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     1328 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/firmware-fingerprint.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     1225 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/helloworld.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     2049 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/mem_flashblock.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     1923 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/mem_read.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     1360 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/mem_write.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     2949 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/mnemonic_check.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     5798 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/pwd_reader.py
--rw-r--r--   0 kristian   (501) staff       (20)     9847 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/pybridge.py
--rwxr-xr-x   0 kristian   (501) staff       (20)      959 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/rng_entropy_collector.py
--rwxr-xr-x   0 kristian   (501) staff       (20)     3621 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/trezor-otp.py
--rw-r--r--   0 kristian   (501) staff       (20)     3842 2023-05-30 19:02:38.000000 eulith-trezor-0.0.1/tools/trezorctl_script_client.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.579352 eulith-trezor-0.0.2/
+-rw-r--r--   0 kristian   (501) staff       (20)      845 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/AUTHORS
+-rw-r--r--   0 kristian   (501) staff       (20)    34509 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/CHANGELOG.md
+-rw-r--r--   0 kristian   (501) staff       (20)     7651 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/COPYING
+-rw-r--r--   0 kristian   (501) staff       (20)      216 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/MANIFEST.in
+-rw-r--r--   0 kristian   (501) staff       (20)    36938 2023-05-30 19:42:26.579465 eulith-trezor-0.0.2/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)     1597 2023-05-30 19:42:07.000000 eulith-trezor-0.0.2/README.md
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.556527 eulith-trezor-0.0.2/bash_completion.d/
+-rw-r--r--   0 kristian   (501) staff       (20)      509 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/bash_completion.d/trezorctl.sh
+-rw-r--r--   0 kristian   (501) staff       (20)      103 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/requirements-optional.txt
+-rw-r--r--   0 kristian   (501) staff       (20)      215 2023-05-30 19:05:08.000000 eulith-trezor-0.0.2/requirements.txt
+-rw-r--r--   0 kristian   (501) staff       (20)      778 2023-05-30 19:42:26.579779 eulith-trezor-0.0.2/setup.cfg
+-rwxr-xr-x   0 kristian   (501) staff       (20)     2627 2023-05-30 19:33:50.000000 eulith-trezor-0.0.2/setup.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.553141 eulith-trezor-0.0.2/src/
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.557598 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/
+-rw-r--r--   0 kristian   (501) staff       (20)    36938 2023-05-30 19:42:26.000000 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/PKG-INFO
+-rw-r--r--   0 kristian   (501) staff       (20)     2848 2023-05-30 19:42:26.000000 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/SOURCES.txt
+-rw-r--r--   0 kristian   (501) staff       (20)        1 2023-05-30 19:42:26.000000 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/dependency_links.txt
+-rw-r--r--   0 kristian   (501) staff       (20)       58 2023-05-30 19:42:26.000000 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/entry_points.txt
+-rw-r--r--   0 kristian   (501) staff       (20)        1 2023-05-30 19:37:34.000000 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/not-zip-safe
+-rw-r--r--   0 kristian   (501) staff       (20)      517 2023-05-30 19:42:26.000000 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/requires.txt
+-rw-r--r--   0 kristian   (501) staff       (20)       10 2023-05-30 19:42:26.000000 eulith-trezor-0.0.2/src/eulith_trezor.egg-info/top_level.txt
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.566573 eulith-trezor-0.0.2/src/trezorlib/
+-rw-r--r--   0 kristian   (501) staff       (20)      703 2023-05-30 19:42:20.000000 eulith-trezor-0.0.2/src/trezorlib/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7594 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/_ed25519.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.567335 eulith-trezor-0.0.2/src/trezorlib/_internal/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/_internal/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9090 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/_internal/emulator.py
+-rw-r--r--   0 kristian   (501) staff       (20)    16788 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/_internal/firmware_headers.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2660 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/binance.py
+-rw-r--r--   0 kristian   (501) staff       (20)    15097 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/btc.py
+-rw-r--r--   0 kristian   (501) staff       (20)    33111 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cardano.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.571543 eulith-trezor-0.0.2/src/trezorlib/cli/
+-rw-r--r--   0 kristian   (501) staff       (20)     6980 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2322 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/binance.py
+-rw-r--r--   0 kristian   (501) staff       (20)    14540 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/btc.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10522 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/cardano.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2552 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/cosi.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3537 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/crypto.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3433 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/debug.py
+-rw-r--r--   0 kristian   (501) staff       (20)    10002 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/device.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1990 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/eos.py
+-rw-r--r--   0 kristian   (501) staff       (20)    19318 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/ethereum.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4411 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/fido.py
+-rw-r--r--   0 kristian   (501) staff       (20)    21462 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/firmware.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2363 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/monero.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2352 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/nem.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2025 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/ripple.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11156 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/settings.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3298 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/stellar.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2274 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/tezos.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)    12805 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cli/trezorctl.py
+-rw-r--r--   0 kristian   (501) staff       (20)    18867 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/client.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6056 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/cosi.py
+-rw-r--r--   0 kristian   (501) staff       (20)    42139 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/debuglink.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4375 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/definitions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     8184 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/device.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11278 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/eos.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13564 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/ethereum.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1601 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/exceptions.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1969 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/fido.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.573060 eulith-trezor-0.0.2/src/trezorlib/firmware/
+-rw-r--r--   0 kristian   (501) staff       (20)     3612 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/firmware/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1217 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/firmware/consts.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6339 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/firmware/core.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6526 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/firmware/legacy.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5976 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/firmware/models.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1252 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/firmware/util.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4760 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/firmware/vendor.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2260 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/log.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3499 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/mapping.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     6356 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/merkle_tree.py
+-rw-r--r--   0 kristian   (501) staff       (20)   261786 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/messages.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3224 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/misc.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1871 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/models.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1676 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/monero.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7467 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/nem.py
+-rw-r--r--   0 kristian   (501) staff       (20)    20836 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/protobuf.py
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/py.typed
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.573382 eulith-trezor-0.0.2/src/trezorlib/qt/
+-rw-r--r--   0 kristian   (501) staff       (20)        0 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/qt/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5543 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/qt/pinmatrix.py
+-rw-r--r--   0 kristian   (501) staff       (20)     2140 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/ripple.py
+-rw-r--r--   0 kristian   (501) staff       (20)    13873 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/stellar.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1702 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/tezos.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7918 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/toif.py
+-rw-r--r--   0 kristian   (501) staff       (20)    11186 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/tools.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.574947 eulith-trezor-0.0.2/src/trezorlib/transport/
+-rw-r--r--   0 kristian   (501) staff       (20)     5167 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/transport/__init__.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5986 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/transport/bridge.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5556 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/transport/hid.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5372 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/transport/protocol.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4961 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/transport/udp.py
+-rw-r--r--   0 kristian   (501) staff       (20)     5753 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/transport/webusb.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9029 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/src/trezorlib/ui.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.576974 eulith-trezor-0.0.2/tests/
+-rw-r--r--   0 kristian   (501) staff       (20)    10705 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_btc.py
+-rw-r--r--   0 kristian   (501) staff       (20)     6933 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_cosi.py
+-rw-r--r--   0 kristian   (501) staff       (20)     4231 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_firmware.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3209 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_merkle_tree.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1571 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_nem.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9635 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_protobuf_encoding.py
+-rw-r--r--   0 kristian   (501) staff       (20)     7343 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_protobuf_misc.py
+-rw-r--r--   0 kristian   (501) staff       (20)    34184 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_stellar.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1845 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_tools.py
+-rw-r--r--   0 kristian   (501) staff       (20)     1838 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tests/test_transport.py
+drwxr-xr-x   0 kristian   (501) staff       (20)        0 2023-05-30 19:42:26.579205 eulith-trezor-0.0.2/tools/
+-rwxr-xr-x   0 kristian   (501) staff       (20)     6692 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/build_tx.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     3000 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/deserialize_tx.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     4593 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/encfs_aes_getpass.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     1328 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/firmware-fingerprint.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     1225 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/helloworld.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     2049 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/mem_flashblock.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     1923 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/mem_read.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     1360 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/mem_write.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     2949 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/mnemonic_check.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     5798 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/pwd_reader.py
+-rw-r--r--   0 kristian   (501) staff       (20)     9847 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/pybridge.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)      959 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/rng_entropy_collector.py
+-rwxr-xr-x   0 kristian   (501) staff       (20)     3621 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/trezor-otp.py
+-rw-r--r--   0 kristian   (501) staff       (20)     3842 2023-05-30 19:02:38.000000 eulith-trezor-0.0.2/tools/trezorctl_script_client.py
```

### Comparing `eulith-trezor-0.0.1/AUTHORS` & `eulith-trezor-0.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/CHANGELOG.md` & `eulith-trezor-0.0.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/COPYING` & `eulith-trezor-0.0.2/COPYING`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/PKG-INFO` & `eulith-trezor-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulith-trezor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for communicating with Trezor Hardware Wallet (with modifications from Eulith)
 Home-page: https://github.com/kristian1108/trezor-firmware
 Author: Trezor & Eulith
 Author-email: admin@eulith.com
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -18,34 +18,38 @@
 Provides-Extra: qt-widgets
 Provides-Extra: extra
 Provides-Extra: stellar
 Provides-Extra: full
 License-File: COPYING
 License-File: AUTHORS
 
-# trezorlib
-
-[![repology](https://repology.org/badge/tiny-repos/python:trezor.svg)](https://repology.org/metapackage/python:trezor) [![image](https://badges.gitter.im/trezor/community.svg)](https://gitter.im/trezor/community)
+# eulith-trezorlib
 
 Python library and command-line client for communicating with Trezor
-Hardware Wallet.
+Hardware Wallet, modified to work more closely with Eulith clients & applications.
+
+See <https://trezor.io> and <https://eulith.com> for more information.
+
+## !! This is a derivative package of Trezor !!
+For the original package, please see https://github.com/trezor/trezor-firmware
 
-See <https://trezor.io> for more information.
+This package has been modified primarily to sort out dependency issues that come up when
+trying to use the original trezor package with Ethereum tooling like `web3py`.
 
 ## Install
 
 Python Trezor tools require Python 3.6 or higher, and libusb 1.0. The easiest
 way to install it is with `pip`. The rest of this guide assumes you have
 a working `pip`; if not, you can refer to [this
 guide](https://packaging.python.org/tutorials/installing-packages/).
 
 On a typical system, you already have all you need. Install `trezor` with:
 
 ```sh
-pip3 install trezor
+pip3 install eulith-trezor
 ```
 
 On Windows, you also need to either install [Trezor Bridge](https://suite.trezor.io/web/bridge/), or
 [libusb](https://github.com/libusb/libusb/wiki/Windows) and the appropriate
 [drivers](https://zadig.akeo.ie/).
 
 ### Firmware version requirements
@@ -56,133 +60,14 @@
 For firmware versions below 1.8.0 and 2.1.0 respectively, the only supported operation
 is "upgrade firmware".
 
 Trezor One with firmware _older than 1.7.0_ and bootloader _older than 1.6.0_
 (including pre-2021 fresh-out-of-the-box units) will not be recognized, unless
 you install HIDAPI support (see below).
 
-### Installation options
-
-* **Ethereum**: To support Ethereum signing from command line, additional packages are
-  needed. Install with:
-
-  ```sh
-  pip3 install trezor[ethereum]
-  ```
-
-* **Stellar**: To support Stellar signing from command line, additional packages are
-  needed. Install with:
-
-  ```sh
-  pip3 install trezor[stellar]
-  ```
-
-* **Firmware-less Trezor One**: If you are setting up a brand new Trezor One
-  manufactured before 2021 (with pre-installed bootloader older than 1.6.0), you will
-  need HIDAPI support. On Linux, you will need the following packages (or their
-  equivalents) as prerequisites: `python3-dev`, `cython3`, `libusb-1.0-0-dev`,
-  `libudev-dev`.
-
-  Install with:
-
-  ```sh
-  pip3 install trezor[hidapi]
-  ```
-
-To install all three, use `pip3 install trezor[hidapi,ethereum,stellar]`.
-
-### Distro packages
-
-Check out [Repology](https://repology.org/metapackage/python:trezor) to see if your
-operating system has an up-to-date python-trezor package.
-
-### Installing latest version from GitHub
-
-```sh
-pip3 install "git+https://github.com/trezor/trezor-firmware#egg=trezor&subdirectory=python"
-```
-
-### Running from source
-
-Install the [Poetry](https://python-poetry.org/) tool, checkout
-`trezor-firmware` from git, and enter the poetry shell:
-
-```sh
-pip3 install poetry
-git clone https://github.com/trezor/trezor-firmware
-cd trezor-firmware
-poetry install
-poetry shell
-```
-
-In this environment, trezorlib and the `trezorctl` tool is running from the live
-sources, so your changes are immediately effective.
-
-## Command line client (trezorctl)
-
-The included `trezorctl` python script can perform various tasks such as
-changing setting in the Trezor, signing transactions, retrieving account
-info and addresses. See the
-[python/docs/](https://github.com/trezor/trezor-firmware/tree/master/python/docs)
-sub folder for detailed examples and options.
-
-NOTE: An older version of the `trezorctl` command is [available for
-Debian Stretch](https://packages.debian.org/en/stretch/python-trezor)
-(and comes pre-installed on [Tails OS](https://tails.boum.org/)).
-
-## Python Library
-
-You can use this python library to interact with a Trezor and use its capabilities in
-your application. See examples here in the
-[tools/](https://github.com/trezor/trezor-firmware/tree/master/python/docs/tools)
-sub folder.
-
-## PIN Entering
-
-When you are asked for PIN, you have to enter scrambled PIN. Follow the
-numbers shown on Trezor display and enter the their positions using the
-numeric keyboard mapping:
-
-|   |   |   |
-|---|---|---|
-| 7 | 8 | 9 |
-| 4 | 5 | 6 |
-| 1 | 2 | 3 |
-
-Example: your PIN is **1234** and Trezor is displaying the following:
-
-|   |   |   |
-|---|---|---|
-| 2 | 8 | 3 |
-| 5 | 4 | 6 |
-| 7 | 9 | 1 |
-
-You have to enter: **3795**
-
-## Contributing
-
-If you want to change protobuf or coin definitions, you will need to regenerate
-definitions in the `python/` subdirectory.
-
-First, make sure your submodules are up-to-date with:
-
-```sh
-git submodule update --init --recursive
-```
-
-Then, rebuild the protobuf messages by running, from the `trezor-firmware` top-level
-directory:
-
-```sh
-make gen
-```
-
-To get support for BTC-like coins, these steps are enough and no further
-changes to the library are necessary.
-
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
```

### Comparing `eulith-trezor-0.0.1/setup.cfg` & `eulith-trezor-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/setup.py` & `eulith-trezor-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/eulith_trezor.egg-info/PKG-INFO` & `eulith-trezor-0.0.2/src/eulith_trezor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulith-trezor
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library for communicating with Trezor Hardware Wallet (with modifications from Eulith)
 Home-page: https://github.com/kristian1108/trezor-firmware
 Author: Trezor & Eulith
 Author-email: admin@eulith.com
 License: LGPLv3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
@@ -18,34 +18,38 @@
 Provides-Extra: qt-widgets
 Provides-Extra: extra
 Provides-Extra: stellar
 Provides-Extra: full
 License-File: COPYING
 License-File: AUTHORS
 
-# trezorlib
-
-[![repology](https://repology.org/badge/tiny-repos/python:trezor.svg)](https://repology.org/metapackage/python:trezor) [![image](https://badges.gitter.im/trezor/community.svg)](https://gitter.im/trezor/community)
+# eulith-trezorlib
 
 Python library and command-line client for communicating with Trezor
-Hardware Wallet.
+Hardware Wallet, modified to work more closely with Eulith clients & applications.
+
+See <https://trezor.io> and <https://eulith.com> for more information.
+
+## !! This is a derivative package of Trezor !!
+For the original package, please see https://github.com/trezor/trezor-firmware
 
-See <https://trezor.io> for more information.
+This package has been modified primarily to sort out dependency issues that come up when
+trying to use the original trezor package with Ethereum tooling like `web3py`.
 
 ## Install
 
 Python Trezor tools require Python 3.6 or higher, and libusb 1.0. The easiest
 way to install it is with `pip`. The rest of this guide assumes you have
 a working `pip`; if not, you can refer to [this
 guide](https://packaging.python.org/tutorials/installing-packages/).
 
 On a typical system, you already have all you need. Install `trezor` with:
 
 ```sh
-pip3 install trezor
+pip3 install eulith-trezor
 ```
 
 On Windows, you also need to either install [Trezor Bridge](https://suite.trezor.io/web/bridge/), or
 [libusb](https://github.com/libusb/libusb/wiki/Windows) and the appropriate
 [drivers](https://zadig.akeo.ie/).
 
 ### Firmware version requirements
@@ -56,133 +60,14 @@
 For firmware versions below 1.8.0 and 2.1.0 respectively, the only supported operation
 is "upgrade firmware".
 
 Trezor One with firmware _older than 1.7.0_ and bootloader _older than 1.6.0_
 (including pre-2021 fresh-out-of-the-box units) will not be recognized, unless
 you install HIDAPI support (see below).
 
-### Installation options
-
-* **Ethereum**: To support Ethereum signing from command line, additional packages are
-  needed. Install with:
-
-  ```sh
-  pip3 install trezor[ethereum]
-  ```
-
-* **Stellar**: To support Stellar signing from command line, additional packages are
-  needed. Install with:
-
-  ```sh
-  pip3 install trezor[stellar]
-  ```
-
-* **Firmware-less Trezor One**: If you are setting up a brand new Trezor One
-  manufactured before 2021 (with pre-installed bootloader older than 1.6.0), you will
-  need HIDAPI support. On Linux, you will need the following packages (or their
-  equivalents) as prerequisites: `python3-dev`, `cython3`, `libusb-1.0-0-dev`,
-  `libudev-dev`.
-
-  Install with:
-
-  ```sh
-  pip3 install trezor[hidapi]
-  ```
-
-To install all three, use `pip3 install trezor[hidapi,ethereum,stellar]`.
-
-### Distro packages
-
-Check out [Repology](https://repology.org/metapackage/python:trezor) to see if your
-operating system has an up-to-date python-trezor package.
-
-### Installing latest version from GitHub
-
-```sh
-pip3 install "git+https://github.com/trezor/trezor-firmware#egg=trezor&subdirectory=python"
-```
-
-### Running from source
-
-Install the [Poetry](https://python-poetry.org/) tool, checkout
-`trezor-firmware` from git, and enter the poetry shell:
-
-```sh
-pip3 install poetry
-git clone https://github.com/trezor/trezor-firmware
-cd trezor-firmware
-poetry install
-poetry shell
-```
-
-In this environment, trezorlib and the `trezorctl` tool is running from the live
-sources, so your changes are immediately effective.
-
-## Command line client (trezorctl)
-
-The included `trezorctl` python script can perform various tasks such as
-changing setting in the Trezor, signing transactions, retrieving account
-info and addresses. See the
-[python/docs/](https://github.com/trezor/trezor-firmware/tree/master/python/docs)
-sub folder for detailed examples and options.
-
-NOTE: An older version of the `trezorctl` command is [available for
-Debian Stretch](https://packages.debian.org/en/stretch/python-trezor)
-(and comes pre-installed on [Tails OS](https://tails.boum.org/)).
-
-## Python Library
-
-You can use this python library to interact with a Trezor and use its capabilities in
-your application. See examples here in the
-[tools/](https://github.com/trezor/trezor-firmware/tree/master/python/docs/tools)
-sub folder.
-
-## PIN Entering
-
-When you are asked for PIN, you have to enter scrambled PIN. Follow the
-numbers shown on Trezor display and enter the their positions using the
-numeric keyboard mapping:
-
-|   |   |   |
-|---|---|---|
-| 7 | 8 | 9 |
-| 4 | 5 | 6 |
-| 1 | 2 | 3 |
-
-Example: your PIN is **1234** and Trezor is displaying the following:
-
-|   |   |   |
-|---|---|---|
-| 2 | 8 | 3 |
-| 5 | 4 | 6 |
-| 7 | 9 | 1 |
-
-You have to enter: **3795**
-
-## Contributing
-
-If you want to change protobuf or coin definitions, you will need to regenerate
-definitions in the `python/` subdirectory.
-
-First, make sure your submodules are up-to-date with:
-
-```sh
-git submodule update --init --recursive
-```
-
-Then, rebuild the protobuf messages by running, from the `trezor-firmware` top-level
-directory:
-
-```sh
-make gen
-```
-
-To get support for BTC-like coins, these steps are enough and no further
-changes to the library are necessary.
-
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
```

### Comparing `eulith-trezor-0.0.1/src/eulith_trezor.egg-info/SOURCES.txt` & `eulith-trezor-0.0.2/src/eulith_trezor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/eulith_trezor.egg-info/requires.txt` & `eulith-trezor-0.0.2/src/eulith_trezor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/__init__.py` & `eulith-trezor-0.0.2/src/trezorlib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Lesser General Public License for more details.
 #
 # You should have received a copy of the License along with this library.
 # If not, see <https://www.gnu.org/licenses/lgpl-3.0.html>.
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

### Comparing `eulith-trezor-0.0.1/src/trezorlib/_ed25519.py` & `eulith-trezor-0.0.2/src/trezorlib/_ed25519.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/_internal/emulator.py` & `eulith-trezor-0.0.2/src/trezorlib/_internal/emulator.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/_internal/firmware_headers.py` & `eulith-trezor-0.0.2/src/trezorlib/_internal/firmware_headers.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/binance.py` & `eulith-trezor-0.0.2/src/trezorlib/binance.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/btc.py` & `eulith-trezor-0.0.2/src/trezorlib/btc.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cardano.py` & `eulith-trezor-0.0.2/src/trezorlib/cardano.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/__init__.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/binance.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/binance.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/btc.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/btc.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/cardano.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/cardano.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/cosi.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/cosi.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/crypto.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/crypto.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/debug.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/debug.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/device.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/device.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/eos.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/eos.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/ethereum.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/ethereum.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/fido.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/fido.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/firmware.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/firmware.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/monero.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/monero.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/nem.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/nem.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/ripple.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/ripple.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/settings.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/settings.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/stellar.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/stellar.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/tezos.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/tezos.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cli/trezorctl.py` & `eulith-trezor-0.0.2/src/trezorlib/cli/trezorctl.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/client.py` & `eulith-trezor-0.0.2/src/trezorlib/client.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/cosi.py` & `eulith-trezor-0.0.2/src/trezorlib/cosi.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/debuglink.py` & `eulith-trezor-0.0.2/src/trezorlib/debuglink.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/definitions.py` & `eulith-trezor-0.0.2/src/trezorlib/definitions.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/device.py` & `eulith-trezor-0.0.2/src/trezorlib/device.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/eos.py` & `eulith-trezor-0.0.2/src/trezorlib/eos.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/ethereum.py` & `eulith-trezor-0.0.2/src/trezorlib/ethereum.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/exceptions.py` & `eulith-trezor-0.0.2/src/trezorlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/fido.py` & `eulith-trezor-0.0.2/src/trezorlib/fido.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/firmware/__init__.py` & `eulith-trezor-0.0.2/src/trezorlib/firmware/__init__.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/firmware/consts.py` & `eulith-trezor-0.0.2/src/trezorlib/firmware/consts.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/firmware/core.py` & `eulith-trezor-0.0.2/src/trezorlib/firmware/core.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/firmware/legacy.py` & `eulith-trezor-0.0.2/src/trezorlib/firmware/legacy.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/firmware/models.py` & `eulith-trezor-0.0.2/src/trezorlib/firmware/models.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/firmware/util.py` & `eulith-trezor-0.0.2/src/trezorlib/firmware/util.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/firmware/vendor.py` & `eulith-trezor-0.0.2/src/trezorlib/firmware/vendor.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/log.py` & `eulith-trezor-0.0.2/src/trezorlib/log.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/mapping.py` & `eulith-trezor-0.0.2/src/trezorlib/mapping.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/merkle_tree.py` & `eulith-trezor-0.0.2/src/trezorlib/merkle_tree.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/messages.py` & `eulith-trezor-0.0.2/src/trezorlib/messages.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/misc.py` & `eulith-trezor-0.0.2/src/trezorlib/misc.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/models.py` & `eulith-trezor-0.0.2/src/trezorlib/models.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/monero.py` & `eulith-trezor-0.0.2/src/trezorlib/monero.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/nem.py` & `eulith-trezor-0.0.2/src/trezorlib/nem.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/protobuf.py` & `eulith-trezor-0.0.2/src/trezorlib/protobuf.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/qt/pinmatrix.py` & `eulith-trezor-0.0.2/src/trezorlib/qt/pinmatrix.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/ripple.py` & `eulith-trezor-0.0.2/src/trezorlib/ripple.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/stellar.py` & `eulith-trezor-0.0.2/src/trezorlib/stellar.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/tezos.py` & `eulith-trezor-0.0.2/src/trezorlib/tezos.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/toif.py` & `eulith-trezor-0.0.2/src/trezorlib/toif.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/tools.py` & `eulith-trezor-0.0.2/src/trezorlib/tools.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/transport/__init__.py` & `eulith-trezor-0.0.2/src/trezorlib/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/transport/bridge.py` & `eulith-trezor-0.0.2/src/trezorlib/transport/bridge.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/transport/hid.py` & `eulith-trezor-0.0.2/src/trezorlib/transport/hid.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/transport/protocol.py` & `eulith-trezor-0.0.2/src/trezorlib/transport/protocol.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/transport/udp.py` & `eulith-trezor-0.0.2/src/trezorlib/transport/udp.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/transport/webusb.py` & `eulith-trezor-0.0.2/src/trezorlib/transport/webusb.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/src/trezorlib/ui.py` & `eulith-trezor-0.0.2/src/trezorlib/ui.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_btc.py` & `eulith-trezor-0.0.2/tests/test_btc.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_cosi.py` & `eulith-trezor-0.0.2/tests/test_cosi.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_firmware.py` & `eulith-trezor-0.0.2/tests/test_firmware.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_merkle_tree.py` & `eulith-trezor-0.0.2/tests/test_merkle_tree.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_nem.py` & `eulith-trezor-0.0.2/tests/test_nem.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_protobuf_encoding.py` & `eulith-trezor-0.0.2/tests/test_protobuf_encoding.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_protobuf_misc.py` & `eulith-trezor-0.0.2/tests/test_protobuf_misc.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_stellar.py` & `eulith-trezor-0.0.2/tests/test_stellar.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_tools.py` & `eulith-trezor-0.0.2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tests/test_transport.py` & `eulith-trezor-0.0.2/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/build_tx.py` & `eulith-trezor-0.0.2/tools/build_tx.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/deserialize_tx.py` & `eulith-trezor-0.0.2/tools/deserialize_tx.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/encfs_aes_getpass.py` & `eulith-trezor-0.0.2/tools/encfs_aes_getpass.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/firmware-fingerprint.py` & `eulith-trezor-0.0.2/tools/firmware-fingerprint.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/helloworld.py` & `eulith-trezor-0.0.2/tools/helloworld.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/mem_flashblock.py` & `eulith-trezor-0.0.2/tools/mem_flashblock.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/mem_read.py` & `eulith-trezor-0.0.2/tools/mem_read.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/mem_write.py` & `eulith-trezor-0.0.2/tools/mem_write.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/mnemonic_check.py` & `eulith-trezor-0.0.2/tools/mnemonic_check.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/pwd_reader.py` & `eulith-trezor-0.0.2/tools/pwd_reader.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/pybridge.py` & `eulith-trezor-0.0.2/tools/pybridge.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/rng_entropy_collector.py` & `eulith-trezor-0.0.2/tools/rng_entropy_collector.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/trezor-otp.py` & `eulith-trezor-0.0.2/tools/trezor-otp.py`

 * *Files identical despite different names*

### Comparing `eulith-trezor-0.0.1/tools/trezorctl_script_client.py` & `eulith-trezor-0.0.2/tools/trezorctl_script_client.py`

 * *Files identical despite different names*

