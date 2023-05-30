# Comparing `tmp/sshkey-tools-0.9.1.tar.gz` & `tmp/sshkey-tools-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshkey-tools-0.9.1.tar", last modified: Thu May 18 21:35:24 2023, max compression
+gzip compressed data, was "sshkey-tools-0.9.2.tar", last modified: Tue May 30 15:40:41 2023, max compression
```

## Comparing `sshkey-tools-0.9.1.tar` & `sshkey-tools-0.9.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15293 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.506806 sshkey-tools-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/src/sshkey_tools/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20238 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    29285 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-18 21:35:12.000000 sshkey-tools-0.9.1/src/sshkey_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:35:24.510807 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:35:24.000000 sshkey-tools-0.9.1/src/sshkey_tools.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.350950 sshkey-tools-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/src/sshkey_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49394 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-30 15:40:24.000000 sshkey-tools-0.9.2/src/sshkey_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:40:41.354951 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:40:41.000000 sshkey-tools-0.9.2/src/sshkey_tools.egg-info/zip-safe
```

### Comparing `sshkey-tools-0.9.1/LICENSE` & `sshkey-tools-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.1/PKG-INFO` & `sshkey-tools-0.9.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-Metadata-Version: 2.1
-Name: sshkey-tools
-Version: 0.9.1
-Summary: A Python module for generating, parsing and handling OpenSSH keys and certificates
-Home-page: https://github.com/scheiblingco/sshkey-tools
-Author: Lars Scheibling
-Author-email: lars@scheibling.se
-License: GnuPG 3.0
-Keywords: python openssh ssh keys sshkey ssh-keygen ssh-certificate certificate parser decoder
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sshkey-tools
 
 Python package for managing OpenSSH keypairs and certificates ([protocol.CERTKEYS](https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys)). Supported functionality includes:
 
-[TOC]
+# Notice
+The DSA algorithm is considered deprecated and will be removed in a future version. If possible, use RSA, [(ECDSA)](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a) or ED25519 as a first-hand choice.
+
+Notice from OpenSSH:
+```
+OpenSSH 7.0 and greater similarly disable the ssh-dss (DSA) public key algorithm. It too is weak and we recommend against its use. It can be re-enabled using the HostKeyAlgorithms configuration option: sshd_config(5) HostKeyAlgorithms
+```
+
+[ECDSA has some flaws](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a), especially when using short nonces or re-using nonces, it can still be used but exercise some caution in regards to nonces/re-signing identical data multiple times.
+
 
 # Features
 ### SSH Keys
-- Supports RSA, DSA, ECDSA and ED25519 keys
+- Supports RSA, DSA (Note: Deprecated), ECDSA and ED25519 keys
 - Import existing keys from file, string, byte data or [pyca/cryptography](https://github.com/pyca/cryptography) class
 - Generate new keys
 - Get public key from private keys
 - Sign bytestrings with private keys
 - Export to file, string or bytes
 - Generate fingerprint
 
@@ -36,19 +29,15 @@
 - Verify certificate signature against internal or separate public key
 - Create new certificates from CA private key and subject public key
 - Create new certificates using old certificate as template
 - Sign certificates
 - Export certificates to file, string or bytes
 
 # Roadmap
-- [x] Rewrite certificate field functionality for simpler usage
-- [ ] Re-add functionality for changing RSA hash method
-- [ ] Add CLI functionality
-- [ ] Convert to/from putty format (keys only)
-
+See issues for planned features and fixes
 
 # Installation
 
 ## With pip
 
 ```bash
 pip3 install sshkey-tools
@@ -63,14 +52,21 @@
 cd sshkey-tools
 pip3 install ./
 ```
 
 # Documentation
 You can find the full documentation at [scheiblingco.github.io/sshkey-tools/](https://scheiblingco.github.io/sshkey-tools/)
 
+## Building the documentation
+```bash
+pdoc3 src/sshkey_tools/ -o docs --html
+cp -rf docs/sshkey_tools/* docs/
+rm -rf docs/sshkey_tools
+```
+
 ## SSH Keypairs (generating, loading, exporting)
 ```python
 # Import the certificate classes
 from sshkey_tools.keys import (
     RsaPrivateKey,
     DsaPrivateKey,
     EcdsaPrivateKey,
@@ -138,23 +134,28 @@
 b"\0xc\0a\........"
 ```
 
 ## SSH Key Signatures
 The loaded private key objects can be used to sign bytestrings, and the public keys can be used to verify signatures on those
 ```python
 from sshkey_tools.keys import RsaPrivateKey, RsaPublicKey
+from sshkey_tools.fields import RsaAlgs
 
 signable_data = b'This is a message that will be signed'
 
 privkey = RsaPrivateKey.generate()
 pubkey = RsaPrivateKey.public_key
 
 # Sign the data
 signature = privkey.sign(signable_data)
 
+# When using an RSA key for the signature, you can specify the hashing algorithm
+# The default algorithm is SHA512
+signature = privkey.sign(signable_data, RsaAlgs.SHA512)
+
 # Verify the signature (Throws exception if invalid)
 pubkey.verify(signable_data, signature)
 ```
 
 ## OpenSSH Certificates
 ### Introduction
 Certificates are a way to handle access management/PAM for OpenSSH with the ability to dynamically grant access during a specific time, to specific servers and/or with specific attributes. There are a couple of upsides to using certificates instead of public/private keys, mainly: 
@@ -180,15 +181,15 @@
 |Attribute|Type(Length)|Key|Example Value|Description|
 |---|---|---|---|---|
 |Serial|Integer(64-bit)|serial|1234567890|An optional certificate serial number set by the CA to provide an abbreviated way to refer to certificates from that CA. If a CA does not wish to number its certificates, it must set this field to zero.|
 |Certificate type|Integer(1 or 2)|cert_type|1|The type of the certificate, 1 for user certificates, 2 for host certificates|
 |Key ID|string(variable)|key_id|someuser@somehost|Free-form text field that is filled in by the CA at the time of signing; the intention is that the contents of this field are used to identify the identity principal in log messages.|
 |Valid Principals|List(string(variable))|principals|['some-user', 'some-group', production-webservers']|These principals list the names for which this certificate is valid hostnames for SSH_CERT_TYPE_HOST certificates and usernames for  SH_CERT_TYPE_USER certificates. As a special case, a zero-length "valid principals" field means the certificate is valid for any principal of the specified type.|
 |Valid After|Timestamp|valid_after|datetime.now()|Timestamp for the start of the validity period for the certificate|
-|Valid Before|Timestamp|valid_before|datetime.now()+timedelta(hours=8) or 1658322031|Timestamp for the end of the validity period for the certificate. Needs to be larger than valid_after|
+|Valid Before|Timestamp|valid_before|datetime.now()+timedelta(hours=8) or 1658322031|Timestamp for the end of the validity period for the certificate. Needs to be larger than valid_after, can be a string (ex. 2d, 2w, 1h4m, 99d) or forever (MAX_INT64)|
 |Critical Options|Dict(string, string)|critical_options|[]|Zero or more of the available critical options (see below)|
 |Extensions|Dict(string, string)/List/Tuple/Set|extensions|[]|Zero or more of the available extensions (see below)|
 
 
 #### Critical Options
 |Name|Format|Description|
 |---|---|---|
@@ -322,14 +323,18 @@
 new_ca = PrivateKey.from_file('filename-ca')
 certificate.replace_ca(new_ca)
 certificate.sign()
 
 ```
 
 ## Changelog
+### 0.9.1
+- Updated documentation
+- Fix for bug where exception would occur when trying to export a key without a comment set
+
 ### 0.9
 - Adjustments to certificate field handling for easier usage/syntax autocompletion
 - Updated testing
 - Removed method for changing RSA hash method (now default SHA512)
 
 ### 0.8.2
 - Fixed bug where an RSA certificate would send the RSA alg to the sign() function of another key type
```

### Comparing `sshkey-tools-0.9.1/README.md` & `sshkey-tools-0.9.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,41 @@
+Metadata-Version: 2.1
+Name: sshkey-tools
+Version: 0.9.2
+Summary: A Python module for generating, parsing and handling OpenSSH keys and certificates
+Home-page: https://github.com/scheiblingco/sshkey-tools
+Author: Lars Scheibling
+Author-email: lars@scheibling.se
+License: GnuPG 3.0
+Keywords: python openssh ssh keys sshkey ssh-keygen ssh-certificate certificate parser decoder
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sshkey-tools
 
 Python package for managing OpenSSH keypairs and certificates ([protocol.CERTKEYS](https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys)). Supported functionality includes:
 
-[TOC]
+# Notice
+The DSA algorithm is considered deprecated and will be removed in a future version. If possible, use RSA, [(ECDSA)](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a) or ED25519 as a first-hand choice.
+
+Notice from OpenSSH:
+```
+OpenSSH 7.0 and greater similarly disable the ssh-dss (DSA) public key algorithm. It too is weak and we recommend against its use. It can be re-enabled using the HostKeyAlgorithms configuration option: sshd_config(5) HostKeyAlgorithms
+```
+
+[ECDSA has some flaws](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a), especially when using short nonces or re-using nonces, it can still be used but exercise some caution in regards to nonces/re-signing identical data multiple times.
+
 
 # Features
 ### SSH Keys
-- Supports RSA, DSA, ECDSA and ED25519 keys
+- Supports RSA, DSA (Note: Deprecated), ECDSA and ED25519 keys
 - Import existing keys from file, string, byte data or [pyca/cryptography](https://github.com/pyca/cryptography) class
 - Generate new keys
 - Get public key from private keys
 - Sign bytestrings with private keys
 - Export to file, string or bytes
 - Generate fingerprint
 
@@ -20,19 +45,15 @@
 - Verify certificate signature against internal or separate public key
 - Create new certificates from CA private key and subject public key
 - Create new certificates using old certificate as template
 - Sign certificates
 - Export certificates to file, string or bytes
 
 # Roadmap
-- [x] Rewrite certificate field functionality for simpler usage
-- [ ] Re-add functionality for changing RSA hash method
-- [ ] Add CLI functionality
-- [ ] Convert to/from putty format (keys only)
-
+See issues for planned features and fixes
 
 # Installation
 
 ## With pip
 
 ```bash
 pip3 install sshkey-tools
@@ -47,14 +68,21 @@
 cd sshkey-tools
 pip3 install ./
 ```
 
 # Documentation
 You can find the full documentation at [scheiblingco.github.io/sshkey-tools/](https://scheiblingco.github.io/sshkey-tools/)
 
+## Building the documentation
+```bash
+pdoc3 src/sshkey_tools/ -o docs --html
+cp -rf docs/sshkey_tools/* docs/
+rm -rf docs/sshkey_tools
+```
+
 ## SSH Keypairs (generating, loading, exporting)
 ```python
 # Import the certificate classes
 from sshkey_tools.keys import (
     RsaPrivateKey,
     DsaPrivateKey,
     EcdsaPrivateKey,
@@ -122,23 +150,28 @@
 b"\0xc\0a\........"
 ```
 
 ## SSH Key Signatures
 The loaded private key objects can be used to sign bytestrings, and the public keys can be used to verify signatures on those
 ```python
 from sshkey_tools.keys import RsaPrivateKey, RsaPublicKey
+from sshkey_tools.fields import RsaAlgs
 
 signable_data = b'This is a message that will be signed'
 
 privkey = RsaPrivateKey.generate()
 pubkey = RsaPrivateKey.public_key
 
 # Sign the data
 signature = privkey.sign(signable_data)
 
+# When using an RSA key for the signature, you can specify the hashing algorithm
+# The default algorithm is SHA512
+signature = privkey.sign(signable_data, RsaAlgs.SHA512)
+
 # Verify the signature (Throws exception if invalid)
 pubkey.verify(signable_data, signature)
 ```
 
 ## OpenSSH Certificates
 ### Introduction
 Certificates are a way to handle access management/PAM for OpenSSH with the ability to dynamically grant access during a specific time, to specific servers and/or with specific attributes. There are a couple of upsides to using certificates instead of public/private keys, mainly: 
@@ -164,15 +197,15 @@
 |Attribute|Type(Length)|Key|Example Value|Description|
 |---|---|---|---|---|
 |Serial|Integer(64-bit)|serial|1234567890|An optional certificate serial number set by the CA to provide an abbreviated way to refer to certificates from that CA. If a CA does not wish to number its certificates, it must set this field to zero.|
 |Certificate type|Integer(1 or 2)|cert_type|1|The type of the certificate, 1 for user certificates, 2 for host certificates|
 |Key ID|string(variable)|key_id|someuser@somehost|Free-form text field that is filled in by the CA at the time of signing; the intention is that the contents of this field are used to identify the identity principal in log messages.|
 |Valid Principals|List(string(variable))|principals|['some-user', 'some-group', production-webservers']|These principals list the names for which this certificate is valid hostnames for SSH_CERT_TYPE_HOST certificates and usernames for  SH_CERT_TYPE_USER certificates. As a special case, a zero-length "valid principals" field means the certificate is valid for any principal of the specified type.|
 |Valid After|Timestamp|valid_after|datetime.now()|Timestamp for the start of the validity period for the certificate|
-|Valid Before|Timestamp|valid_before|datetime.now()+timedelta(hours=8) or 1658322031|Timestamp for the end of the validity period for the certificate. Needs to be larger than valid_after|
+|Valid Before|Timestamp|valid_before|datetime.now()+timedelta(hours=8) or 1658322031|Timestamp for the end of the validity period for the certificate. Needs to be larger than valid_after, can be a string (ex. 2d, 2w, 1h4m, 99d) or forever (MAX_INT64)|
 |Critical Options|Dict(string, string)|critical_options|[]|Zero or more of the available critical options (see below)|
 |Extensions|Dict(string, string)/List/Tuple/Set|extensions|[]|Zero or more of the available extensions (see below)|
 
 
 #### Critical Options
 |Name|Format|Description|
 |---|---|---|
@@ -306,14 +339,18 @@
 new_ca = PrivateKey.from_file('filename-ca')
 certificate.replace_ca(new_ca)
 certificate.sign()
 
 ```
 
 ## Changelog
+### 0.9.1
+- Updated documentation
+- Fix for bug where exception would occur when trying to export a key without a comment set
+
 ### 0.9
 - Adjustments to certificate field handling for easier usage/syntax autocompletion
 - Updated testing
 - Removed method for changing RSA hash method (now default SHA512)
 
 ### 0.8.2
 - Fixed bug where an RSA certificate would send the RSA alg to the sign() function of another key type
```

### Comparing `sshkey-tools-0.9.1/setup.py` & `sshkey-tools-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools/__version__.py` & `sshkey-tools-0.9.2/src/sshkey_tools/__version__.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools/cert.py` & `sshkey-tools-0.9.2/src/sshkey_tools/cert.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,15 @@
     """
     General class for SSH Certificates, used for loading and parsing.
     To create new certificates, use the respective keytype classes
     or the from_public_key classmethod
     """
 
     DEFAULT_KEY_TYPE = "none@openssh.com"
+
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         subject_pubkey: PublicKey = None,
         ca_privkey: PrivateKey = None,
         fields: CertificateFields = CertificateFields,
         header: CertificateHeader = CertificateHeader,
@@ -490,25 +491,29 @@
         """
         Retrieves the signable data for the certificate in byte form
         """
         return concat_to_bytestring(
             bytes(self.header), bytes(self.fields), bytes(self.footer)
         )
 
-    def sign(self) -> bool:
+    def sign(self, **kwargs) -> bool:
         """Sign the certificate
 
+        Args:
+            **kwargs: Arguments to pass to the signature signing method
+                      ex. hash_alg for RSA signatures
+
         Raises:
             _EX.NotSignedException: The certificate could not be signed
 
         Returns:
             bool: Whether successful
         """
         if self.can_sign():
-            self.footer.signature.sign(data=self.get_signable())
+            self.footer.signature.sign(data=self.get_signable(), **kwargs)
 
             return True
         raise _EX.NotSignedException("There was an error while signing the certificate")
 
     def verify(
         self, public_key: PublicKey = None, raise_on_error: bool = False
     ) -> bool:
```

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools/exceptions.py` & `sshkey-tools-0.9.2/src/sshkey_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools/fields.py` & `sshkey-tools-0.9.2/src/sshkey_tools/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     concat_to_string,
     ensure_bytestring,
     ensure_string,
     generate_secure_nonce,
     long_to_bytes,
     random_keyid,
     random_serial,
+    str_to_time_delta,
 )
 
 NoneType = type(None)
 MAX_INT32 = 2**32
 MAX_INT64 = 2**64
 NEWLINE = "\n"
 
@@ -134,15 +135,15 @@
 
         return True
 
     def __validate_required__(self) -> Union[bool, Exception]:
         """
         Validates if the field is set when required
         """
-        if self.DEFAULT == self.value is None:
+        if self.DEFAULT and self.value is None:
             return _EX.InvalidFieldDataException(
                 f"{self.get_name()} is a required field"
             )
         return True
 
     def __validate_value__(self) -> Union[bool, Exception]:
         """
@@ -260,41 +261,46 @@
     Field representing a bytestring value
     """
 
     DATA_TYPE = (bytes, str)
     DEFAULT = b""
 
     @classmethod
-    def encode(cls, value: bytes) -> bytes:
+    def encode(cls, value: bytes, encoding: str = "utf-8") -> bytes:
         """
         Encodes a string or bytestring into a packed byte string
 
         Args:
             value (Union[str, bytes]): The string/bytestring to encode
-            encoding (str): The encoding to user for the string
+            encoding (str): The optional encoding, not used when passing
+                            a byte value.
 
         Returns:
             bytes: Packed byte string containing the source data
         """
         cls.__validate_type__(value, True)
-        return pack(">I", len(value)) + ensure_bytestring(value)
+        return pack(">I", len(value)) + ensure_bytestring(value, encoding)
 
     @staticmethod
-    def decode(data: bytes) -> Tuple[bytes, bytes]:
+    def decode(data: bytes, encoding: str = None) -> Tuple[bytes, bytes]:
         """
         Unpacks the next string from a packed byte string
 
         Args:
             data (bytes): The packed byte string to unpack
 
         Returns:
             tuple(bytes, bytes):  The next block of bytes from the packed byte
                                   string and remainder of the data
         """
         length = unpack(">I", data[:4])[0] + 4
+
+        if encoding is not None:
+            return ensure_string(data[4:length], encoding), data[length:]
+
         return ensure_bytestring(data[4:length]), data[length:]
 
 
 class StringField(BytestringField):
     """
     Field representing a string value
     """
@@ -310,32 +316,29 @@
         Args:
             value (Union[str, bytes]): The string/bytestring to encode
             encoding (str): The encoding to user for the string
 
         Returns:
             bytes: Packed byte string containing the source data
         """
-        cls.__validate_type__(value, True)
-        return BytestringField.encode(ensure_bytestring(value, encoding))
+        return super().encode(value, encoding)
 
     @staticmethod
     def decode(data: bytes, encoding: str = "utf-8") -> Tuple[str, bytes]:
         """
         Unpacks the next string from a packed byte string
 
         Args:
             data (bytes): The packed byte string to unpack
 
         Returns:
             tuple(bytes, bytes):  The next block of bytes from the packed byte
                                   string and remainder of the data
         """
-        value, data = BytestringField.decode(data)
-
-        return value.decode(encoding), data
+        return BytestringField.decode(data, encoding)
 
 
 class Integer32Field(CertificateField):
     """
     Certificate field representing a 32-bit integer
     """
 
@@ -436,29 +439,46 @@
 
 class DateTimeField(Integer64Field):
     """
     Certificate field representing a datetime value.
     The value is saved as a 64-bit integer (unix timestamp)
     """
 
-    DATA_TYPE = (datetime, int)
+    DATA_TYPE = (datetime, int, str)
     DEFAULT = datetime.now
 
     @classmethod
-    def encode(cls, value: Union[datetime, int]) -> bytes:
-        """Encodes a datetime object to a byte string
+    def encode(cls, value: Union[datetime, int, str]) -> bytes:
+        """Encodes a datetime object, integer or time string to a byte string
+           Time strings are parsed with pytimeparse2, for example:
+            32m
+            2h32m
+            3d2h32m
+            1w3d2h32m
+            1w 3d 2h 32m
+            1 w 3 d 2 h 32 m
+            4:13
+            4:13:02
+            4:13:02.266
+            forever (Returns as MAX_INT64)
 
         Args:
-            value (datetime): Datetime object
+            value (datetime, int, str): Datetime object
 
         Returns:
             bytes: Packed byte string containing datetime timestamp
         """
         cls.__validate_type__(value, True)
 
+        if isinstance(value, str):
+            if value == "forever":
+                return Integer64Field.encode(MAX_INT64 - 1)
+
+            value = int((datetime.now() + str_to_time_delta(value)).timestamp())
+
         if isinstance(value, datetime):
             value = int(value.timestamp())
 
         return Integer64Field.encode(value)
 
     @staticmethod
     def decode(data: bytes) -> datetime:
@@ -721,22 +741,22 @@
         if isinstance(self.__validate_type__(self.value), Exception):
             return _EX.InvalidFieldDataException(
                 f"{self.get_name()} Could not validate value, invalid type"
             )
 
         if ensure_string(self.value) not in self.ALLOWED_VALUES:
             return _EX.InvalidFieldDataException(
-                "Expected one of the following values: " +
-                NEWLINE.join(self.ALLOWED_VALUES)
+                "Expected one of the following values: "
+                + NEWLINE.join(self.ALLOWED_VALUES)
             )
 
         return True
 
 
-class NonceField(StringField):
+class NonceField(BytestringField):
     """
     Contains the nonce for the certificate, randomly generated
     this protects the integrity of the private key, especially
     for ecdsa.
     """
 
     DEFAULT = generate_secure_nonce
@@ -1270,17 +1290,20 @@
         self.value = signature
 
         if signature is not None and ensure_bytestring(signature) not in ("", " "):
             self.is_signed = True
 
     def __table__(self) -> tuple:
         msg = "No signature"
-        if self.is_signed:
+        if self.is_signed and self.private_key is not None:
             msg = f"Signed with private key {self.private_key.get_fingerprint()}"
 
+        if self.is_signed and self.private_key is None:
+            msg = "Signed with: See pubkey fingerprint above"
+
         return ("Signature", msg)
 
     @staticmethod
     def from_object(private_key: PrivateKey):
         """
         Load a private key from a PrivateKey object
 
@@ -1328,15 +1351,15 @@
     def can_sign(self):
         """
         Determines if a signature can be generated from
         this private key
         """
         return self.private_key is not None
 
-    def sign(self, data: bytes) -> None:
+    def sign(self, data: bytes, **kwargs) -> None:
         """
         Placeholder signing function
         """
         raise _EX.InvalidClassCallException("The base class has no sign function")
 
     def __bytes__(self) -> None:
         return self.encode(self.value)
```

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools/keys.py` & `sshkey-tools-0.9.2/src/sshkey_tools/keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from cryptography.hazmat.primitives.asymmetric import dsa as _DSA
 from cryptography.hazmat.primitives.asymmetric import ec as _ECDSA
 from cryptography.hazmat.primitives.asymmetric import ed25519 as _ED25519
 from cryptography.hazmat.primitives.asymmetric import padding as _PADDING
 from cryptography.hazmat.primitives.asymmetric import rsa as _RSA
 
 from . import exceptions as _EX
-from .utils import ensure_bytestring, ensure_string
+from .utils import ensure_bytestring, ensure_string, nullsafe_getattr
 from .utils import md5_fingerprint as _FP_MD5
 from .utils import sha256_fingerprint as _FP_SHA256
 from .utils import sha512_fingerprint as _FP_SHA512
 
 PUBKEY_MAP = {
     _RSAPublicKey: "RsaPublicKey",
     _DSAPublicKey: "DsaPublicKey",
@@ -126,19 +126,22 @@
         self.serialized = kwargs.get("serialized", None)
 
         self.export_opts = [
             _SERIALIZATION.Encoding.OpenSSH,
             _SERIALIZATION.PublicFormat.OpenSSH,
         ]
 
+        # Ensure comment is not None
+        self.comment = nullsafe_getattr(self, "comment", "")
+
     @classmethod
     def from_class(
         cls,
         key_class: PubkeyClasses,
-        comment: Union[str, bytes] = None,
+        comment: Union[str, bytes] = "",
         key_type: Union[str, bytes] = None,
     ) -> "PublicKey":
         """
         Creates a new SSH Public key from a cryptography class
 
         Args:
             key_class (PubkeyClasses): The cryptography class containing the public key
@@ -262,15 +265,15 @@
         Returns:
             str: The public key in OpenSSH format
             encoding(str, optional): The encoding of the file. Defaults to 'utf-8'.
         """
         return " ".join(
             [
                 ensure_string(self.serialize(), encoding),
-                ensure_string(getattr(self, "comment", ""), encoding),
+                ensure_string(nullsafe_getattr(self, "comment", ""), encoding),
             ]
         )
 
     def to_file(self, path: str, encoding: str = "utf-8") -> None:
         """
         Export the public key to a file
```

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools/utils.py` & `sshkey-tools-0.9.2/src/sshkey_tools/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 """
 Utilities for handling keys and certificates
 """
 import hashlib as hl
 import sys
+import datetime
+
 from base64 import b64encode
 from random import randint
 from secrets import randbits
 from typing import Dict, List, Union
 from uuid import uuid4
 
+from pytimeparse2 import parse as time_parse
+
+
 NoneType = type(None)
 
 
 def ensure_string(
     obj: Union[str, bytes, list, tuple, set, dict, NoneType],
     encoding: str = "utf-8",
     required: bool = False,
@@ -224,29 +229,98 @@
     """
     digest = hl.sha512(data).digest()
     return ("SHA512:" if prefix else "") + b64encode(digest).replace(b"=", b"").decode(
         "utf-8"
     )
 
 
+def nullsafe_getattr(obj, attr: str, default):
+    """
+    Null-safe getattr, ensuring the result is not None.
+    If the result is None, the default value is returned instead.
+
+    Args:
+        obj: The object
+        attr: The attribute to get
+        default: The default value
+    """
+    att = getattr(obj, attr, default)
+    if att is None:
+        att = default
+
+    return att
+
+
 def join_dicts(*dicts) -> dict:
     """
     Joins two or more dictionaries together.
     In case of duplicate keys, the latest one wins.
 
     Returns:
         dict: Joined dictionary
     """
     py_version = sys.version_info[0:2]
     return_dict = {}
 
     if py_version[0] == 3 and py_version[1] > 9:
-
         for add_dict in dicts:
             return_dict = return_dict | add_dict
 
         return return_dict
 
     for add_dict in dicts:
         return_dict = {**return_dict, **add_dict}
 
     return return_dict
+
+
+def str_to_time_delta(str_delta: str) -> datetime.timedelta:
+    """Uses the package pytimeparse2 by wroberts/onegreyonewhite
+        to convert a string into a timedelta object.
+        Examples:
+            - 32m
+            - 2h32m
+            - 3d2h32m
+            - 1w3d2h32m
+            - 1w 3d 2h 32m
+            - 1 w 3 d 2 h 32 m
+            - 4:13
+            - 4:13:02
+            - 4:13:02.266
+            - 2:04:13:02.266
+            - 2 days, 4:13:02 (uptime format)
+            - 2 days, 4:13:02.266
+            - 5hr34m56s
+            - 5 hours, 34 minutes, 56 seconds
+            - 5 hrs, 34 mins, 56 secs
+            - 2 days, 5 hours, 34 minutes, 56 seconds
+            - 1.2 m
+            - 1.2 min
+            - 1.2 mins
+            - 1.2 minute
+            - 1.2 minutes
+            - 172 hours
+            - 172 hr
+            - 172 h
+            - 172 hrs
+            - 172 hour
+            - 1.24 days
+            - 5 d
+            - 5 day
+            - 5 days
+            - 5.6 wk
+            - 5.6 week
+            - 5.6 weeks
+
+    Args:
+        str_delta (str): The time delta string to convert
+
+    Returns:
+        datetime.timedelta: The time delta object
+    """
+    try:
+        parsed = time_parse(str_delta, as_timedelta=True, raise_exception=True)
+        return parsed
+    except Exception as ex:
+        raise ValueError(
+            f"Could not parse time delta string {str_delta} : {ex}"
+        ) from ex
```

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools.egg-info/PKG-INFO` & `sshkey-tools-0.9.2/src/sshkey_tools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshkey-tools
-Version: 0.9.1
+Version: 0.9.2
 Summary: A Python module for generating, parsing and handling OpenSSH keys and certificates
 Home-page: https://github.com/scheiblingco/sshkey-tools
 Author: Lars Scheibling
 Author-email: lars@scheibling.se
 License: GnuPG 3.0
 Keywords: python openssh ssh keys sshkey ssh-keygen ssh-certificate certificate parser decoder
 Classifier: Programming Language :: Python :: 3
@@ -14,19 +14,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sshkey-tools
 
 Python package for managing OpenSSH keypairs and certificates ([protocol.CERTKEYS](https://github.com/openssh/openssh-portable/blob/master/PROTOCOL.certkeys)). Supported functionality includes:
 
-[TOC]
+# Notice
+The DSA algorithm is considered deprecated and will be removed in a future version. If possible, use RSA, [(ECDSA)](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a) or ED25519 as a first-hand choice.
+
+Notice from OpenSSH:
+```
+OpenSSH 7.0 and greater similarly disable the ssh-dss (DSA) public key algorithm. It too is weak and we recommend against its use. It can be re-enabled using the HostKeyAlgorithms configuration option: sshd_config(5) HostKeyAlgorithms
+```
+
+[ECDSA has some flaws](https://billatnapier.medium.com/ecdsa-weakness-where-nonces-are-reused-2be63856a01a), especially when using short nonces or re-using nonces, it can still be used but exercise some caution in regards to nonces/re-signing identical data multiple times.
+
 
 # Features
 ### SSH Keys
-- Supports RSA, DSA, ECDSA and ED25519 keys
+- Supports RSA, DSA (Note: Deprecated), ECDSA and ED25519 keys
 - Import existing keys from file, string, byte data or [pyca/cryptography](https://github.com/pyca/cryptography) class
 - Generate new keys
 - Get public key from private keys
 - Sign bytestrings with private keys
 - Export to file, string or bytes
 - Generate fingerprint
 
@@ -36,19 +45,15 @@
 - Verify certificate signature against internal or separate public key
 - Create new certificates from CA private key and subject public key
 - Create new certificates using old certificate as template
 - Sign certificates
 - Export certificates to file, string or bytes
 
 # Roadmap
-- [x] Rewrite certificate field functionality for simpler usage
-- [ ] Re-add functionality for changing RSA hash method
-- [ ] Add CLI functionality
-- [ ] Convert to/from putty format (keys only)
-
+See issues for planned features and fixes
 
 # Installation
 
 ## With pip
 
 ```bash
 pip3 install sshkey-tools
@@ -63,14 +68,21 @@
 cd sshkey-tools
 pip3 install ./
 ```
 
 # Documentation
 You can find the full documentation at [scheiblingco.github.io/sshkey-tools/](https://scheiblingco.github.io/sshkey-tools/)
 
+## Building the documentation
+```bash
+pdoc3 src/sshkey_tools/ -o docs --html
+cp -rf docs/sshkey_tools/* docs/
+rm -rf docs/sshkey_tools
+```
+
 ## SSH Keypairs (generating, loading, exporting)
 ```python
 # Import the certificate classes
 from sshkey_tools.keys import (
     RsaPrivateKey,
     DsaPrivateKey,
     EcdsaPrivateKey,
@@ -138,23 +150,28 @@
 b"\0xc\0a\........"
 ```
 
 ## SSH Key Signatures
 The loaded private key objects can be used to sign bytestrings, and the public keys can be used to verify signatures on those
 ```python
 from sshkey_tools.keys import RsaPrivateKey, RsaPublicKey
+from sshkey_tools.fields import RsaAlgs
 
 signable_data = b'This is a message that will be signed'
 
 privkey = RsaPrivateKey.generate()
 pubkey = RsaPrivateKey.public_key
 
 # Sign the data
 signature = privkey.sign(signable_data)
 
+# When using an RSA key for the signature, you can specify the hashing algorithm
+# The default algorithm is SHA512
+signature = privkey.sign(signable_data, RsaAlgs.SHA512)
+
 # Verify the signature (Throws exception if invalid)
 pubkey.verify(signable_data, signature)
 ```
 
 ## OpenSSH Certificates
 ### Introduction
 Certificates are a way to handle access management/PAM for OpenSSH with the ability to dynamically grant access during a specific time, to specific servers and/or with specific attributes. There are a couple of upsides to using certificates instead of public/private keys, mainly: 
@@ -180,15 +197,15 @@
 |Attribute|Type(Length)|Key|Example Value|Description|
 |---|---|---|---|---|
 |Serial|Integer(64-bit)|serial|1234567890|An optional certificate serial number set by the CA to provide an abbreviated way to refer to certificates from that CA. If a CA does not wish to number its certificates, it must set this field to zero.|
 |Certificate type|Integer(1 or 2)|cert_type|1|The type of the certificate, 1 for user certificates, 2 for host certificates|
 |Key ID|string(variable)|key_id|someuser@somehost|Free-form text field that is filled in by the CA at the time of signing; the intention is that the contents of this field are used to identify the identity principal in log messages.|
 |Valid Principals|List(string(variable))|principals|['some-user', 'some-group', production-webservers']|These principals list the names for which this certificate is valid hostnames for SSH_CERT_TYPE_HOST certificates and usernames for  SH_CERT_TYPE_USER certificates. As a special case, a zero-length "valid principals" field means the certificate is valid for any principal of the specified type.|
 |Valid After|Timestamp|valid_after|datetime.now()|Timestamp for the start of the validity period for the certificate|
-|Valid Before|Timestamp|valid_before|datetime.now()+timedelta(hours=8) or 1658322031|Timestamp for the end of the validity period for the certificate. Needs to be larger than valid_after|
+|Valid Before|Timestamp|valid_before|datetime.now()+timedelta(hours=8) or 1658322031|Timestamp for the end of the validity period for the certificate. Needs to be larger than valid_after, can be a string (ex. 2d, 2w, 1h4m, 99d) or forever (MAX_INT64)|
 |Critical Options|Dict(string, string)|critical_options|[]|Zero or more of the available critical options (see below)|
 |Extensions|Dict(string, string)/List/Tuple/Set|extensions|[]|Zero or more of the available extensions (see below)|
 
 
 #### Critical Options
 |Name|Format|Description|
 |---|---|---|
@@ -322,14 +339,18 @@
 new_ca = PrivateKey.from_file('filename-ca')
 certificate.replace_ca(new_ca)
 certificate.sign()
 
 ```
 
 ## Changelog
+### 0.9.1
+- Updated documentation
+- Fix for bug where exception would occur when trying to export a key without a comment set
+
 ### 0.9
 - Adjustments to certificate field handling for easier usage/syntax autocompletion
 - Updated testing
 - Removed method for changing RSA hash method (now default SHA512)
 
 ### 0.8.2
 - Fixed bug where an RSA certificate would send the RSA alg to the sign() function of another key type
```

### Comparing `sshkey-tools-0.9.1/src/sshkey_tools.egg-info/SOURCES.txt` & `sshkey-tools-0.9.2/src/sshkey_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

