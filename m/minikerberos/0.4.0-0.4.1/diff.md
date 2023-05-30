# Comparing `tmp/minikerberos-0.4.0.tar.gz` & `tmp/minikerberos-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minikerberos-0.4.0.tar", last modified: Wed Feb 15 14:17:01 2023, max compression
+gzip compressed data, was "minikerberos-0.4.1.tar", last modified: Tue May 30 13:57:04 2023, max compression
```

## Comparing `minikerberos-0.4.0.tar` & `minikerberos-0.4.1.tar`

### file list

```diff
@@ -1,98 +1,96 @@
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.313579 minikerberos-0.4.0/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1077 2023-02-15 14:10:35.000000 minikerberos-0.4.0/LICENSE
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       34 2022-11-13 21:11:55.000000 minikerberos-0.4.0/MANIFEST.in
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      403 2023-02-15 14:17:01.313579 minikerberos-0.4.0/PKG-INFO
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     4303 2023-02-15 14:10:35.000000 minikerberos-0.4.0/README.md
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.305579 minikerberos-0.4.0/minikerberos/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      271 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      135 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/_version.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    32274 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/aioclient.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    32290 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/client.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.309579 minikerberos-0.4.0/minikerberos/common/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/common/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    27473 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/ccache.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      461 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/constants.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    20017 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/creds.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     8599 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/factory.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     8717 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/keytab.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     4192 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/kirbi.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1869 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/spn.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      562 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/common/target.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     3356 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/common/utils.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.309579 minikerberos-0.4.0/minikerberos/common/windows/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/common/windows/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    12518 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/common/windows/crypt32.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    23499 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/common/windows/defines.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.309579 minikerberos-0.4.0/minikerberos/examples/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    10819 2022-11-17 23:46:41.000000 minikerberos-0.4.0/minikerberos/examples/CVE_2022_33647.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     8978 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/CVE_2022_33679.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/examples/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      952 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/__main__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      817 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/ccache2kirbi.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2484 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/ccache_editor.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      486 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/ccacheroast.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1233 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/getNT.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2862 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/getS4U2proxy.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2867 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/getS4U2self.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2582 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/getTGS.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1719 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/getTGT.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     3761 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/kerb23hashdecrypt.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1065 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/kirbi2ccache.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2912 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/examples/spnroast.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.309579 minikerberos-0.4.0/minikerberos/gssapi/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/gssapi/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2971 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/gssapi/channelbindings.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    12555 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/gssapi/gssapi.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.309579 minikerberos-0.4.0/minikerberos/network/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/network/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1845 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/network/aioclientsocket.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2779 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/network/clientsocket.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    15198 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/pkinit.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.313579 minikerberos-0.4.0/minikerberos/protocol/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    29728 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/protocol/asn1_structs.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     5365 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/protocol/constants.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      940 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/dirtydh.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    24206 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/protocol/encryption.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     9443 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/protocol/errors.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.313579 minikerberos-0.4.0/minikerberos/protocol/external/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    13476 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/dtypes.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    28211 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/enum.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    65750 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/ndr.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1821 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/nrpc.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     7075 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/pac.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1345 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/rpcrt.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    22940 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/external/structure.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1827 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/protocol/external/ticketutil.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2862 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/mskile.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     4367 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/rfc4556.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      938 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/rfc_iakerb.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2668 2022-11-13 21:11:55.000000 minikerberos-0.4.0/minikerberos/protocol/structures.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2742 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/protocol/ticketutils.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     4047 2023-02-15 14:10:35.000000 minikerberos-0.4.0/minikerberos/security.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.305579 minikerberos-0.4.0/minikerberos.egg-info/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      403 2023-02-15 14:17:01.000000 minikerberos-0.4.0/minikerberos.egg-info/PKG-INFO
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2653 2023-02-15 14:17:01.000000 minikerberos-0.4.0/minikerberos.egg-info/SOURCES.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-02-15 14:17:01.000000 minikerberos-0.4.0/minikerberos.egg-info/dependency_links.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      873 2023-02-15 14:17:01.000000 minikerberos-0.4.0/minikerberos.egg-info/entry_points.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       77 2023-02-15 14:17:01.000000 minikerberos-0.4.0/minikerberos.egg-info/requires.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       19 2023-02-15 14:17:01.000000 minikerberos-0.4.0/minikerberos.egg-info/top_level.txt
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-02-15 14:16:59.000000 minikerberos-0.4.0/minikerberos.egg-info/zip-safe
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       80 2023-02-15 14:10:35.000000 minikerberos-0.4.0/pyproject.toml
--rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2023-02-15 14:17:01.313579 minikerberos-0.4.0/setup.cfg
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2166 2023-02-15 14:10:35.000000 minikerberos-0.4.0/setup.py
-drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:17:01.313579 minikerberos-0.4.0/tests/
--rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/__init__.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     3360 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/config.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     6588 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_ccache.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    12286 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_conn.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    10634 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_conn_blocking.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)    10102 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_credential.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     6248 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_encryption.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     7544 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_examples.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1666 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_keytab.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     1300 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_kirbi.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     2185 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_security.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)     4869 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_url.py
--rw-rw-r--   0 webdev    (1000) webdev    (1000)      182 2023-02-15 14:10:35.000000 minikerberos-0.4.0/tests/test_version.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.376586 minikerberos-0.4.1/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1077 2023-03-05 19:48:27.000000 minikerberos-0.4.1/LICENSE
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       34 2023-03-05 19:48:27.000000 minikerberos-0.4.1/MANIFEST.in
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      403 2023-05-30 13:57:04.376586 minikerberos-0.4.1/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4303 2023-03-05 19:48:27.000000 minikerberos-0.4.1/README.md
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.364586 minikerberos-0.4.1/minikerberos/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      271 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      135 2023-05-30 13:25:02.000000 minikerberos-0.4.1/minikerberos/_version.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    32274 2023-04-13 15:02:40.000000 minikerberos-0.4.1/minikerberos/aioclient.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    32290 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/client.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.368586 minikerberos-0.4.1/minikerberos/common/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    27473 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/ccache.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      461 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/constants.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    20017 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/creds.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8599 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/factory.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8717 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/keytab.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4192 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/kirbi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1869 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/spn.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      562 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/target.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3356 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/utils.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.368586 minikerberos-0.4.1/minikerberos/common/windows/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/windows/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    12518 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/windows/crypt32.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    23499 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/common/windows/defines.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.372586 minikerberos-0.4.1/minikerberos/examples/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10819 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/CVE_2022_33647.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8978 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/CVE_2022_33679.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      952 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/__main__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      817 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/ccache2kirbi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2484 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/ccache_editor.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      486 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/ccacheroast.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1233 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/getNT.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2862 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/getS4U2proxy.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2867 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/getS4U2self.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2582 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/getTGS.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1719 2023-04-13 14:38:22.000000 minikerberos-0.4.1/minikerberos/examples/getTGT.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3761 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/kerb23hashdecrypt.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1065 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/kirbi2ccache.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2912 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/examples/spnroast.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.372586 minikerberos-0.4.1/minikerberos/gssapi/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/gssapi/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2971 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/gssapi/channelbindings.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    12555 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/gssapi/gssapi.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.372586 minikerberos-0.4.1/minikerberos/network/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/network/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1845 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/network/aioclientsocket.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2779 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/network/clientsocket.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15198 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/pkinit.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.372586 minikerberos-0.4.1/minikerberos/protocol/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    29728 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/asn1_structs.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5365 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/constants.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      940 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/dirtydh.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    24206 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/encryption.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9443 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/errors.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.376586 minikerberos-0.4.1/minikerberos/protocol/external/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13476 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/dtypes.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    28211 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/enum.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    65750 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/ndr.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1821 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/nrpc.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7075 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/pac.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1345 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/rpcrt.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    22940 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/structure.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1827 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/external/ticketutil.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2862 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/mskile.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4367 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/rfc4556.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      938 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/rfc_iakerb.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2668 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/structures.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2742 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/protocol/ticketutils.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4047 2023-03-05 19:48:27.000000 minikerberos-0.4.1/minikerberos/security.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.368586 minikerberos-0.4.1/minikerberos.egg-info/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      403 2023-05-30 13:57:04.000000 minikerberos-0.4.1/minikerberos.egg-info/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2619 2023-05-30 13:57:04.000000 minikerberos-0.4.1/minikerberos.egg-info/SOURCES.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 13:57:04.000000 minikerberos-0.4.1/minikerberos.egg-info/dependency_links.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      873 2023-05-30 13:57:04.000000 minikerberos-0.4.1/minikerberos.egg-info/entry_points.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       77 2023-05-30 13:57:04.000000 minikerberos-0.4.1/minikerberos.egg-info/requires.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       13 2023-05-30 13:57:04.000000 minikerberos-0.4.1/minikerberos.egg-info/top_level.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 13:57:02.000000 minikerberos-0.4.1/minikerberos.egg-info/zip-safe
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       88 2023-03-05 19:48:27.000000 minikerberos-0.4.1/pyproject.toml
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2023-05-30 13:57:04.376586 minikerberos-0.4.1/setup.cfg
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2184 2023-05-30 13:52:29.000000 minikerberos-0.4.1/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:57:04.376586 minikerberos-0.4.1/tests/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6588 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_ccache.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    12286 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_conn.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10634 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_conn_blocking.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10102 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_credential.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6248 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_encryption.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7544 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_examples.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1666 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_keytab.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1300 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_kirbi.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2185 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_security.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4869 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_url.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      182 2023-03-05 19:48:27.000000 minikerberos-0.4.1/tests/test_version.py
```

### Comparing `minikerberos-0.4.0/LICENSE` & `minikerberos-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/README.md` & `minikerberos-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/aioclient.py` & `minikerberos-0.4.1/minikerberos/aioclient.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/client.py` & `minikerberos-0.4.1/minikerberos/client.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/ccache.py` & `minikerberos-0.4.1/minikerberos/common/ccache.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/creds.py` & `minikerberos-0.4.1/minikerberos/common/creds.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/factory.py` & `minikerberos-0.4.1/minikerberos/common/factory.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/keytab.py` & `minikerberos-0.4.1/minikerberos/common/keytab.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/kirbi.py` & `minikerberos-0.4.1/minikerberos/common/kirbi.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/spn.py` & `minikerberos-0.4.1/minikerberos/common/spn.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/target.py` & `minikerberos-0.4.1/minikerberos/common/target.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/utils.py` & `minikerberos-0.4.1/minikerberos/common/utils.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/windows/crypt32.py` & `minikerberos-0.4.1/minikerberos/common/windows/crypt32.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/common/windows/defines.py` & `minikerberos-0.4.1/minikerberos/common/windows/defines.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/CVE_2022_33647.py` & `minikerberos-0.4.1/minikerberos/examples/CVE_2022_33647.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/CVE_2022_33679.py` & `minikerberos-0.4.1/minikerberos/examples/CVE_2022_33679.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/__main__.py` & `minikerberos-0.4.1/minikerberos/examples/__main__.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/ccache2kirbi.py` & `minikerberos-0.4.1/minikerberos/examples/ccache2kirbi.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/ccache_editor.py` & `minikerberos-0.4.1/minikerberos/examples/ccache_editor.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/getNT.py` & `minikerberos-0.4.1/minikerberos/examples/getNT.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/getS4U2proxy.py` & `minikerberos-0.4.1/minikerberos/examples/getS4U2proxy.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/getS4U2self.py` & `minikerberos-0.4.1/minikerberos/examples/getS4U2self.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/getTGS.py` & `minikerberos-0.4.1/minikerberos/examples/getTGS.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/getTGT.py` & `minikerberos-0.4.1/minikerberos/examples/getTGT.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/kerb23hashdecrypt.py` & `minikerberos-0.4.1/minikerberos/examples/kerb23hashdecrypt.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/kirbi2ccache.py` & `minikerberos-0.4.1/minikerberos/examples/kirbi2ccache.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/examples/spnroast.py` & `minikerberos-0.4.1/minikerberos/examples/spnroast.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/gssapi/channelbindings.py` & `minikerberos-0.4.1/minikerberos/gssapi/channelbindings.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/gssapi/gssapi.py` & `minikerberos-0.4.1/minikerberos/gssapi/gssapi.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/network/aioclientsocket.py` & `minikerberos-0.4.1/minikerberos/network/aioclientsocket.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/network/clientsocket.py` & `minikerberos-0.4.1/minikerberos/network/clientsocket.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/pkinit.py` & `minikerberos-0.4.1/minikerberos/pkinit.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/asn1_structs.py` & `minikerberos-0.4.1/minikerberos/protocol/asn1_structs.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/constants.py` & `minikerberos-0.4.1/minikerberos/protocol/constants.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/dirtydh.py` & `minikerberos-0.4.1/minikerberos/protocol/dirtydh.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/encryption.py` & `minikerberos-0.4.1/minikerberos/protocol/encryption.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/errors.py` & `minikerberos-0.4.1/minikerberos/protocol/errors.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/dtypes.py` & `minikerberos-0.4.1/minikerberos/protocol/external/dtypes.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/enum.py` & `minikerberos-0.4.1/minikerberos/protocol/external/enum.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/ndr.py` & `minikerberos-0.4.1/minikerberos/protocol/external/ndr.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/nrpc.py` & `minikerberos-0.4.1/minikerberos/protocol/external/nrpc.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/pac.py` & `minikerberos-0.4.1/minikerberos/protocol/external/pac.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/rpcrt.py` & `minikerberos-0.4.1/minikerberos/protocol/external/rpcrt.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/structure.py` & `minikerberos-0.4.1/minikerberos/protocol/external/structure.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/external/ticketutil.py` & `minikerberos-0.4.1/minikerberos/protocol/external/ticketutil.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/mskile.py` & `minikerberos-0.4.1/minikerberos/protocol/mskile.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/rfc4556.py` & `minikerberos-0.4.1/minikerberos/protocol/rfc4556.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/rfc_iakerb.py` & `minikerberos-0.4.1/minikerberos/protocol/rfc_iakerb.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/structures.py` & `minikerberos-0.4.1/minikerberos/protocol/structures.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/protocol/ticketutils.py` & `minikerberos-0.4.1/minikerberos/protocol/ticketutils.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos/security.py` & `minikerberos-0.4.1/minikerberos/security.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/minikerberos.egg-info/SOURCES.txt` & `minikerberos-0.4.1/minikerberos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,14 @@
 minikerberos/protocol/external/enum.py
 minikerberos/protocol/external/ndr.py
 minikerberos/protocol/external/nrpc.py
 minikerberos/protocol/external/pac.py
 minikerberos/protocol/external/rpcrt.py
 minikerberos/protocol/external/structure.py
 minikerberos/protocol/external/ticketutil.py
-tests/__init__.py
-tests/config.py
 tests/test_ccache.py
 tests/test_conn.py
 tests/test_conn_blocking.py
 tests/test_credential.py
 tests/test_encryption.py
 tests/test_examples.py
 tests/test_keytab.py
```

### Comparing `minikerberos-0.4.0/minikerberos.egg-info/entry_points.txt` & `minikerberos-0.4.1/minikerberos.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/setup.py` & `minikerberos-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	version=verstr,
 
 	# Application author details:
 	author="Tamas Jos",
 	author_email="info@skelsec.com",
 
 	# Packages
-	packages=find_packages(),
+	packages=find_packages(exclude=["tests*"]),
 
 	# Include additional files into the package
 	include_package_data=True,
 
 
 	# Details
 	url="https://github.com/skelsec/minikerberos",
@@ -42,16 +42,16 @@
 		"Programming Language :: Python :: 3.6",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	install_requires=[
 		'asn1crypto>=1.3.0',
 		'oscrypto>=1.2.1',
-		'asysocks>=0.2.2',
-		'unicrypto>=0.0.10',
+		'asysocks==0.2.7',
+		'unicrypto==0.0.10',
 		'tqdm',
         'six',
 	],
 
 	entry_points={
 		'console_scripts': [
 			'minikerberos-ccacheedit   = minikerberos.examples.ccache_editor:main',
```

### Comparing `minikerberos-0.4.0/tests/test_ccache.py` & `minikerberos-0.4.1/tests/test_ccache.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_conn.py` & `minikerberos-0.4.1/tests/test_conn.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_conn_blocking.py` & `minikerberos-0.4.1/tests/test_conn_blocking.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_credential.py` & `minikerberos-0.4.1/tests/test_credential.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_encryption.py` & `minikerberos-0.4.1/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_examples.py` & `minikerberos-0.4.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_keytab.py` & `minikerberos-0.4.1/tests/test_keytab.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_kirbi.py` & `minikerberos-0.4.1/tests/test_kirbi.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_security.py` & `minikerberos-0.4.1/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `minikerberos-0.4.0/tests/test_url.py` & `minikerberos-0.4.1/tests/test_url.py`

 * *Files identical despite different names*

