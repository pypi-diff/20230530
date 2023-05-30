# Comparing `tmp/cryptography-40.0.2.tar.gz` & `tmp/cryptography-41.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptography-40.0.2.tar", last modified: Fri Apr 14 12:24:20 2023, max compression
+gzip compressed data, was "cryptography-41.0.0.tar", last modified: Tue May 30 21:37:39 2023, max compression
```

## Comparing `cryptography-40.0.2.tar` & `cryptography-41.0.0.tar`

### file list

```diff
@@ -1,397 +1,431 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.976802 cryptography-40.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    90017 2023-04-14 12:24:12.000000 cryptography-40.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-14 12:24:12.000000 cryptography-40.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-14 12:24:12.000000 cryptography-40.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-14 12:24:12.000000 cryptography-40.0.2/LICENSE.APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-14 12:24:12.000000 cryptography-40.0.2/LICENSE.BSD
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-14 12:24:12.000000 cryptography-40.0.2/LICENSE.PSF
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-14 12:24:12.000000 cryptography-40.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-14 12:24:20.976802 cryptography-40.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-14 12:24:12.000000 cryptography-40.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.940802 cryptography-40.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.940802 cryptography-40.0.2/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/_ext/cryptography-docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/_ext/linkcode_res.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.940802 cryptography-40.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/api-stability.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/community.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.940802 cryptography-40.0.2/docs/development/
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/c-bindings.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/arc4/
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/arc4/generate_arc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/arc4/verify_arc4.go
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/arc4.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/cast5/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/cast5/generate_cast5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/cast5/verify_cast5.go
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/cast5.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/hkdf/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/hkdf/generate_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/hkdf/verify_hkdf.go
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/hkdf.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/idea/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/idea/generate_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/idea/verify_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/idea.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/rsa-oaep-sha2/
--rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/rsa-oaep-sha2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/secp256k1/
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/secp256k1/generate_secp256k1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/secp256k1/verify_secp256k1.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/secp256k1.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/development/custom-vectors/seed/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/seed/generate_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/seed/verify_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/custom-vectors/seed.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/reviewing-patches.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/submitting-patches.rst
--rw-r--r--   0 runner    (1001) docker     (123)    57409 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/development/test-vectors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/doing-a-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/fernet.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.936802 cryptography-40.0.2/docs/hazmat/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/aead.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.944802 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/
--rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/dh.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/dsa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29032 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/ec.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/ed25519.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/ed448.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/rsa.rst
--rw-r--r--   0 runner    (1001) docker     (123)    56412 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/serialization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/x25519.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/asymmetric/x448.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/constant-time.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/cryptographic-hashes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    44144 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/key-derivation-functions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/keywrap.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.948802 cryptography-40.0.2/docs/hazmat/primitives/mac/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/mac/cmac.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/mac/hmac.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/mac/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/mac/poly1305.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/padding.rst
--rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/symmetric-encryption.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/hazmat/primitives/twofactor.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/openssl.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/random-numbers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/security.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/spelling_wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.948802 cryptography-40.0.2/docs/x509/
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/x509/certificate-transparency.rst
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/x509/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    29768 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/x509/ocsp.rst
--rw-r--r--   0 runner    (1001) docker     (123)   122551 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/x509/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-04-14 12:24:12.000000 cryptography-40.0.2/docs/x509/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-14 12:24:12.000000 cryptography-40.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-14 12:24:20.976802 cryptography-40.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-14 12:24:12.000000 cryptography-40.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.936802 cryptography-40.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.948802 cryptography-40.0.2/src/_cffi_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/build_openssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/_cffi_src/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/bignum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/bio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/dh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/err.py
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/evp.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/fips.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/nid.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/opensslv.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/osrandom_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/rsa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/_cffi_src/openssl/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/src/osrandom_engine.c
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/src/osrandom_engine.h
--rw-r--r--   0 runner    (1001) docker     (123)    25825 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/x509.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/x509_vfy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/x509name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/openssl/x509v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/_cffi_src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/fernet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/cryptography/hazmat/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14155 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/_oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/cryptography/hazmat/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/aead.py
--rw-r--r--   0 runner    (1001) docker     (123)    91919 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10346 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/ciphers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/decode_asn1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/dh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/ed25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/ed448.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/poly1305.py
--rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/x448.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/cryptography/hazmat/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.956802 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/_openssl.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/asn1.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/ocsp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.956802 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/x509.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.956802 cryptography-40.0.2/src/cryptography/hazmat/bindings/openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/openssl/_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/bindings/openssl/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.956802 cryptography-40.0.2/src/cryptography/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/_asymmetric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/_cipheralgorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.956802 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/dh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/ec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/ed25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/ed448.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/x448.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/aead.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/modes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/constant_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/hmac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/concatkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/kbkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/scrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/x963kdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/keywrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/poly1305.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)    48438 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/cryptography/hazmat/primitives/twofactor/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/twofactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/twofactor/hotp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/hazmat/primitives/twofactor/totp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/cryptography/x509/
--rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34966 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/certificate_transparency.py
--rw-r--r--   0 runner    (1001) docker     (123)    65516 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/general_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/ocsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/cryptography/x509/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.952803 cryptography-40.0.2/src/cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-14 12:24:20.000000 cryptography-40.0.2/src/cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12737 2023-04-14 12:24:20.000000 cryptography-40.0.2/src/cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:24:20.000000 cryptography-40.0.2/src/cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:24:20.000000 cryptography-40.0.2/src/cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 12:24:20.000000 cryptography-40.0.2/src/cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 12:24:20.000000 cryptography-40.0.2/src/cryptography.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/rust/
--rw-r--r--   0 runner    (1001) docker     (123)    19541 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/rust/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/asn1.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.960802 cryptography-40.0.2/src/rust/src/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/backend/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/backend/x25519.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/buf.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/intern.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/oid.rs
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/pkcs7.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/pool.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.964802 cryptography-40.0.2/src/rust/src/x509/
--rw-r--r--   0 runner    (1001) docker     (123)    39187 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/certificate.rs
--rw-r--r--   0 runner    (1001) docker     (123)    26188 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/common.rs
--rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/crl.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/csr.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20409 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/extensions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/ocsp.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/ocsp_req.rs
--rw-r--r--   0 runner    (1001) docker     (123)    31118 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/ocsp_resp.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/oid.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/sct.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20162 2023-04-14 12:24:12.000000 cryptography-40.0.2/src/rust/src/x509/sign.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.964802 cryptography-40.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.964802 cryptography-40.0.2/tests/bench/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/bench/test_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/bench/test_ec_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/bench/test_x509.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/deprecated_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/doubles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.964802 cryptography-40.0.2/tests/hazmat/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.964802 cryptography-40.0.2/tests/hazmat/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21624 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/backends/test_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/backends/test_openssl_memleak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.964802 cryptography-40.0.2/tests/hazmat/bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/bindings/test_openssl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.972802 cryptography-40.0.2/tests/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/fixtures_dh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/fixtures_dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/fixtures_ec.py
--rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/fixtures_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_3des.py
--rw-r--r--   0 runner    (1001) docker     (123)    26688 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_aead.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_aes_gcm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_arc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_asym_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_cast5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_ciphers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_concatkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_constant_time.py
--rw-r--r--   0 runner    (1001) docker     (123)    35872 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_dh.py
--rw-r--r--   0 runner    (1001) docker     (123)    37527 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    45778 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_ed25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_ed448.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_hash_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_hkdf_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_hmac_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_idea.py
--rw-r--r--   0 runner    (1001) docker     (123)    26335 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_kbkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_kbkdf_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_keywrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_pbkdf2hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (123)    28929 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_poly1305.py
--rw-r--r--   0 runner    (1001) docker     (123)    99477 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_scrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    54757 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_sm4.py
--rw-r--r--   0 runner    (1001) docker     (123)    67773 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_x448.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_x963_vectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/test_x963kdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.972802 cryptography-40.0.2/tests/hazmat/primitives/twofactor/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/twofactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/twofactor/test_hotp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/twofactor/test_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)    17245 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/hazmat/test_oid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/test_cryptography_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/test_fernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/test_rust_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   188472 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    29977 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.972802 cryptography-40.0.2/tests/wycheproof/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_chacha20poly1305.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_cmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_dsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_ecdh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_keywrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_x25519.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/test_x448.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/wycheproof/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:20.976802 cryptography-40.0.2/tests/x509/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/x509/test_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    53477 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/x509/test_ocsp.py
--rw-r--r--   0 runner    (1001) docker     (123)   230252 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/x509/test_x509.py
--rw-r--r--   0 runner    (1001) docker     (123)    31009 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/x509/test_x509_crlbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)   213694 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/x509/test_x509_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-04-14 12:24:12.000000 cryptography-40.0.2/tests/x509/test_x509_revokedcertbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-14 12:24:12.000000 cryptography-40.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.161162 cryptography-41.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    91024 2023-05-30 21:37:26.000000 cryptography-41.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 21:37:26.000000 cryptography-41.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-30 21:37:26.000000 cryptography-41.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-30 21:37:26.000000 cryptography-41.0.0/LICENSE.APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-30 21:37:26.000000 cryptography-41.0.0/LICENSE.BSD
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-30 21:37:26.000000 cryptography-41.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-30 21:37:39.161162 cryptography-41.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-30 21:37:26.000000 cryptography-41.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/_ext/cryptography-docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/_ext/linkcode_res.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/api-stability.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/community.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.101161 cryptography-41.0.0/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/c-bindings.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/arc4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/arc4/generate_arc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/arc4/verify_arc4.go
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/arc4.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/cast5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/cast5/generate_cast5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/cast5/verify_cast5.go
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/cast5.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/hkdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/hkdf/generate_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/hkdf/verify_hkdf.go
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/hkdf.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/idea/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/idea/generate_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/idea/verify_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/idea.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/
+-rw-r--r--   0 runner    (1001) docker     (123)    14456 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/secp256k1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/secp256k1/generate_secp256k1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/secp256k1/verify_secp256k1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/secp256k1.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/development/custom-vectors/seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/seed/generate_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/seed/verify_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/custom-vectors/seed.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/reviewing-patches.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/submitting-patches.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    58752 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/development/test-vectors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/doing-a-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/fernet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.093161 cryptography-41.0.0/docs/hazmat/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.105161 cryptography-41.0.0/docs/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/aead.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dsa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28533 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ec.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7857 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed25519.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed448.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26600 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/rsa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    56191 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x25519.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x448.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/constant-time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/cryptographic-hashes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    44313 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/key-derivation-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/keywrap.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/docs/hazmat/primitives/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/cmac.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/hmac.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/mac/poly1305.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/padding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/symmetric-encryption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/hazmat/primitives/twofactor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/openssl.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/random-numbers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/security.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/docs/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/certificate-transparency.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    29766 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/ocsp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   127728 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-05-30 21:37:26.000000 cryptography-41.0.0/docs/x509/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-30 21:37:26.000000 cryptography-41.0.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-30 21:37:26.000000 cryptography-41.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:37:39.161162 cryptography-41.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-30 21:37:26.000000 cryptography-41.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.093161 cryptography-41.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.109161 cryptography-41.0.0/src/_cffi_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/build_openssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/_cffi_src/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/bignum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/bio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/err.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/evp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/evp_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/fips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/nid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/opensslv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25732 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509_vfy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/openssl/x509v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/_cffi_src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/fernet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography/hazmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/_oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography/hazmat/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.121162 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73231 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ciphers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/decode_asn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11474 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21825 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.121162 cryptography-41.0.0/src/cryptography/hazmat/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.121162 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/_openssl.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/asn1.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/ocsp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.125162 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/x509.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.125162 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.125162 cryptography-41.0.0/src/cryptography/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/_asymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/_cipheralgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ed448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x448.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/constant_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/hmac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/concatkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/kbkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/x963kdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/poly1305.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50088 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.129162 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/hotp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/cryptography/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35677 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/certificate_transparency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68365 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/cryptography/x509/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.117161 cryptography-41.0.0/src/cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:37:38.000000 cryptography-41.0.0/src/cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 21:37:39.000000 cryptography-41.0.0/src/cryptography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)    12879 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-cffi/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-cffi/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-cffi/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-cffi/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-cffi/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-openssl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/src/fips.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/src/hmac.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-openssl/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.133162 cryptography-41.0.0/src/rust/cryptography-x509/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.137162 cryptography-41.0.0/src/rust/cryptography-x509/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/common.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/crl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/csr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7673 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/extensions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/ocsp_req.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/ocsp_resp.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/oid.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/cryptography-x509/src/pkcs7.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.137162 cryptography-41.0.0/src/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/asn1.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.141162 cryptography-41.0.0/src/rust/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/dh.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/dsa.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/ed25519.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/ed448.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/hashes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/hmac.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/kdf.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/poly1305.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/x25519.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/backend/x448.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/buf.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/exceptions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/oid.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/pkcs7.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/pool.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.141162 cryptography-41.0.0/src/rust/src/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20407 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/common.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    23375 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/crl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13920 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/csr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20187 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/extensions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/ocsp.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/ocsp_req.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    30555 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/ocsp_resp.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/sct.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    29557 2023-05-30 21:37:26.000000 cryptography-41.0.0/src/rust/src/x509/sign.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_ec_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/bench/test_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/deprecated_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/doubles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/hazmat/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/hazmat/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/backends/test_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/backends/test_openssl_memleak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.145162 cryptography-41.0.0/tests/hazmat/bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/bindings/test_openssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.157162 cryptography-41.0.0/tests/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29306 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/fixtures_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_3des.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26688 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_aead.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_aes_gcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_arc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_asym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_cast5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ciphers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_concatkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_constant_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36819 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_dh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38287 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46372 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ed448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hash_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hkdf_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_hmac_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_idea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26335 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_kbkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_kbkdf_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28916 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_poly1305.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99908 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55019 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_sm4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69339 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x448.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x963_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/test_x963kdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.157162 cryptography-41.0.0/tests/hazmat/primitives/twofactor/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/twofactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_hotp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/hazmat/test_oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_cryptography_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_fernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_rust_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188472 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29807 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.161162 cryptography-41.0.0/tests/wycheproof/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_chacha20poly1305.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_cmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_ecdh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/test_x448.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/wycheproof/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:39.161162 cryptography-41.0.0/tests/x509/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53924 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   244850 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31158 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509_crlbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)   218778 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-05-30 21:37:26.000000 cryptography-41.0.0/tests/x509/test_x509_revokedcertbuilder.py
```

### Comparing `cryptography-40.0.2/CHANGELOG.rst` & `cryptography-41.0.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,60 @@
 Changelog
 =========
 
+.. _v41-0-0:
+
+41.0.0 - 2023-05-30
+~~~~~~~~~~~~~~~~~~~
+
+* **BACKWARDS INCOMPATIBLE:** Support for OpenSSL less than 1.1.1d has been
+  removed.  Users on older version of OpenSSL will need to upgrade.
+* **BACKWARDS INCOMPATIBLE:** Support for Python 3.6 has been removed.
+* **BACKWARDS INCOMPATIBLE:** Dropped support for LibreSSL < 3.6.
+* Updated the minimum supported Rust version (MSRV) to 1.56.0, from 1.48.0.
+* Updated Windows, macOS, and Linux wheels to be compiled with OpenSSL 3.1.1.
+* Added support for the :class:`~cryptography.x509.OCSPAcceptableResponses`
+  OCSP extension.
+* Added support for the :class:`~cryptography.x509.MSCertificateTemplate`
+  proprietary Microsoft certificate extension.
+* Implemented support for equality checks on all asymmetric public key types.
+* Added support for ``aes256-gcm@openssh.com`` encrypted keys in
+  :func:`~cryptography.hazmat.primitives.serialization.load_ssh_private_key`.
+* Added support for obtaining X.509 certificate signature algorithm parameters
+  (including PSS) via
+  :meth:`~cryptography.x509.Certificate.signature_algorithm_parameters`.
+* Support signing :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`
+  X.509 certificates via the new keyword-only argument ``rsa_padding`` on
+  :meth:`~cryptography.x509.CertificateBuilder.sign`.
+* Added support for
+  :class:`~cryptography.hazmat.primitives.ciphers.aead.ChaCha20Poly1305`
+  on BoringSSL.
+
 .. _v40-0-2:
 
 40.0.2 - 2023-04-14
 ~~~~~~~~~~~~~~~~~~~
 
 * Fixed compilation when using LibreSSL 3.7.2.
+* Added some functions to support an upcoming ``pyOpenSSL`` release.
 
 .. _v40-0-1:
 
 40.0.1 - 2023-03-24
 ~~~~~~~~~~~~~~~~~~~
 
 * Fixed a bug where certain operations would fail if an object happened to be
   in the top-half of the memory-space. This only impacted 32-bit systems.
 
 .. _v40-0-0:
 
 40.0.0 - 2023-03-24
 ~~~~~~~~~~~~~~~~~~~
 
+
 * **BACKWARDS INCOMPATIBLE:** As announced in the 39.0.0 changelog, the way
   ``cryptography`` links OpenSSL has changed. This only impacts users who
   build ``cryptography`` from source (i.e., not from a ``wheel``), and
   specify their own version of OpenSSL. For those users, the ``CFLAGS``,
   ``LDFLAGS``, ``INCLUDE``, ``LIB``, and ``CRYPTOGRAPHY_SUPPRESS_LINK_FLAGS``
   environment variables are no longer valid. Instead, users need to configure
   their builds `as documented here`_.
@@ -1768,24 +1798,24 @@
 * Add support for the
   :class:`~cryptography.hazmat.primitives.asymmetric.ec.SECP256K1` elliptic
   curve.
 * Fixed compilation when using an OpenSSL which was compiled with the
   ``no-comp`` (``OPENSSL_NO_COMP``) option.
 * Support :attr:`~cryptography.hazmat.primitives.serialization.Encoding.DER`
   serialization of public keys using the ``public_bytes`` method of
-  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKeyWithSerialization`,
-  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKeyWithSerialization`,
+  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKey`,
+  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKey`,
   and
-  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKeyWithSerialization`.
+  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKey`.
 * Support :attr:`~cryptography.hazmat.primitives.serialization.Encoding.DER`
   serialization of private keys using the ``private_bytes`` method of
-  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKeyWithSerialization`,
-  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKeyWithSerialization`,
+  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey`,
+  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKey`,
   and
-  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKeyWithSerialization`.
+  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey`.
 * Add support for parsing X.509 certificate signing requests (CSRs) with
   :func:`~cryptography.x509.load_pem_x509_csr` and
   :func:`~cryptography.x509.load_der_x509_csr`.
 * Moved ``cryptography.exceptions.InvalidToken`` to
   :class:`cryptography.hazmat.primitives.twofactor.InvalidToken` and deprecated
   the old location. This was moved to minimize confusion between this exception
   and :class:`cryptography.fernet.InvalidToken`.
@@ -1850,50 +1880,40 @@
 * Fixed building against LibreSSL, a compile-time substitute for OpenSSL.
 * FreeBSD 9.2 was removed from the continuous integration system.
 * Updated Windows wheels to be compiled against OpenSSL 1.0.2.
 * :func:`~cryptography.hazmat.primitives.serialization.load_pem_public_key`
   and :func:`~cryptography.hazmat.primitives.serialization.load_der_public_key`
   now support PKCS1 RSA public keys (in addition to the previous support for
   SubjectPublicKeyInfo format for RSA, EC, and DSA).
-* Added
-  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKeyWithSerialization`
-  and deprecated ``EllipticCurvePrivateKeyWithNumbers``.
+* Added ``EllipticCurvePrivateKeyWithSerialization`` and deprecated
+  ``EllipticCurvePrivateKeyWithNumbers``.
 * Added
   :meth:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey.private_bytes`
   to
   :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey`.
-* Added
-  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKeyWithSerialization`
-  and deprecated ``RSAPrivateKeyWithNumbers``.
+* Added ``RSAPrivateKeyWithSerialization`` and deprecated ``RSAPrivateKeyWithNumbers``.
 * Added
   :meth:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey.private_bytes`
   to
   :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey`.
-* Added
-  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKeyWithSerialization`
-  and deprecated ``DSAPrivateKeyWithNumbers``.
+* Added ``DSAPrivateKeyWithSerialization`` and deprecated ``DSAPrivateKeyWithNumbers``.
 * Added
   :meth:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKey.private_bytes`
   to
   :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKey`.
-* Added
-  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKeyWithSerialization`
-  and deprecated ``RSAPublicKeyWithNumbers``.
+* Added ``RSAPublicKeyWithSerialization`` and deprecated ``RSAPublicKeyWithNumbers``.
 * Added ``public_bytes`` to
-  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKeyWithSerialization`.
-* Added
-  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKeyWithSerialization`
-  and deprecated ``EllipticCurvePublicKeyWithNumbers``.
+  :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKey`.
+* Added ``EllipticCurvePublicKeyWithSerialization`` and deprecated
+  ``EllipticCurvePublicKeyWithNumbers``.
 * Added ``public_bytes`` to
-  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKeyWithSerialization`.
-* Added
-  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKeyWithSerialization`
-  and deprecated ``DSAPublicKeyWithNumbers``.
+  :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKey`.
+* Added ``DSAPublicKeyWithSerialization`` and deprecated ``DSAPublicKeyWithNumbers``.
 * Added ``public_bytes`` to
-  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKeyWithSerialization`.
+  :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKey`.
 * :class:`~cryptography.hazmat.primitives.hashes.HashAlgorithm` and
   :class:`~cryptography.hazmat.primitives.hashes.HashContext` were moved from
   ``cryptography.hazmat.primitives.interfaces`` to
   :mod:`~cryptography.hazmat.primitives.hashes`.
 * :class:`~cryptography.hazmat.primitives.ciphers.CipherContext`,
   :class:`~cryptography.hazmat.primitives.ciphers.AEADCipherContext`,
   :class:`~cryptography.hazmat.primitives.ciphers.AEADEncryptionContext`,
```

### Comparing `cryptography-40.0.2/CONTRIBUTING.rst` & `cryptography-41.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/LICENSE.APACHE` & `cryptography-41.0.0/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/LICENSE.BSD` & `cryptography-41.0.0/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/PKG-INFO` & `cryptography-41.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 Metadata-Version: 2.1
 Name: cryptography
-Version: 40.0.2
+Version: 41.0.0
 Summary: cryptography is a package which provides cryptographic recipes and primitives to Python developers.
-Home-page: https://github.com/pyca/cryptography
-Author: The Python Cryptographic Authority and individual contributors
-Author-email: cryptography-dev@python.org
-License: (Apache-2.0 OR BSD-3-Clause) AND PSF-2.0
-Project-URL: Documentation, https://cryptography.io/
-Project-URL: Source, https://github.com/pyca/cryptography/
-Project-URL: Issues, https://github.com/pyca/cryptography/issues
-Project-URL: Changelog, https://cryptography.io/en/latest/changelog/
+Author-email: The Python Cryptographic Authority and individual contributors <cryptography-dev@python.org>
+License: Apache-2.0 OR BSD-3-Clause
+Project-URL: homepage, https://github.com/pyca/cryptography
+Project-URL: documentation, https://cryptography.io/
+Project-URL: source, https://github.com/pyca/cryptography/
+Project-URL: issues, https://github.com/pyca/cryptography/issues
+Project-URL: changelog, https://cryptography.io/en/latest/changelog/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: tox
+Provides-Extra: ssh
+Provides-Extra: nox
 Provides-Extra: test
 Provides-Extra: test-randomorder
 Provides-Extra: docs
 Provides-Extra: docstest
 Provides-Extra: sdist
 Provides-Extra: pep8test
-Provides-Extra: ssh
 License-File: LICENSE
 License-File: LICENSE.APACHE
 License-File: LICENSE.BSD
-License-File: LICENSE.PSF
 
 pyca/cryptography
 =================
 
 .. image:: https://img.shields.io/pypi/v/cryptography.svg
     :target: https://pypi.org/project/cryptography/
     :alt: Latest Version
@@ -60,15 +57,15 @@
 
 .. image:: https://github.com/pyca/cryptography/workflows/CI/badge.svg?branch=main
     :target: https://github.com/pyca/cryptography/actions?query=workflow%3ACI+branch%3Amain
 
 
 ``cryptography`` is a package which provides cryptographic recipes and
 primitives to Python developers. Our goal is for it to be your "cryptographic
-standard library". It supports Python 3.6+ and PyPy3 7.3.10+.
+standard library". It supports Python 3.7+ and PyPy3 7.3.10+.
 
 ``cryptography`` includes both high level recipes and low level interfaces to
 common cryptographic algorithms such as symmetric ciphers, message digests, and
 key derivation functions. For example, to encrypt something with
 ``cryptography``'s high level symmetric encryption recipe:
 
 .. code-block:: pycon
```

### Comparing `cryptography-40.0.2/README.rst` & `cryptography-41.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 .. image:: https://github.com/pyca/cryptography/workflows/CI/badge.svg?branch=main
     :target: https://github.com/pyca/cryptography/actions?query=workflow%3ACI+branch%3Amain
 
 
 ``cryptography`` is a package which provides cryptographic recipes and
 primitives to Python developers. Our goal is for it to be your "cryptographic
-standard library". It supports Python 3.6+ and PyPy3 7.3.10+.
+standard library". It supports Python 3.7+ and PyPy3 7.3.10+.
 
 ``cryptography`` includes both high level recipes and low level interfaces to
 common cryptographic algorithms such as symmetric ciphers, message digests, and
 key derivation functions. For example, to encrypt something with
 ``cryptography``'s high level symmetric encryption recipe:
 
 .. code-block:: pycon
```

### Comparing `cryptography-40.0.2/docs/Makefile` & `cryptography-41.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/_ext/cryptography-docs.py` & `cryptography-41.0.0/docs/_ext/cryptography-docs.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/_ext/linkcode_res.py` & `cryptography-41.0.0/docs/_ext/linkcode_res.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/api-stability.rst` & `cryptography-41.0.0/docs/api-stability.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/community.rst` & `cryptography-41.0.0/docs/community.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/conf.py` & `cryptography-41.0.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Cryptography"
-copyright = "2013-2022, Individual Contributors"
+copyright = "2013-2023, Individual Contributors"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 
 base_dir = os.path.join(os.path.dirname(__file__), os.pardir)
@@ -179,32 +179,29 @@
         "Individual Contributors",
         "Cryptography",
         "One line description of project.",
         "Miscellaneous",
     ),
 ]
 
-# Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"https://docs.python.org/3": None}
+intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 
 epub_theme = "epub"
 
 # Retry requests in the linkcheck builder so that we're resillient against
 # transient network errors.
 linkcheck_retries = 10
 
 linkcheck_timeout = 5
 
 linkcheck_ignore = [
     # Insecure renegotiation settings
     r"https://info.isl.ntt.co.jp/crypt/eng/camellia/",
     # Inconsistent small DH params they seem incapable of fixing
     r"https://www.secg.org/sec1-v2.pdf",
-    # Cert is issued from an untrusted root
-    r"https://e-trust.gosuslugi.ru",
     # Incomplete cert chain
     r"https://www.oscca.gov.cn",
     # Cloudflare returns 403s for all non-browser requests
     r"https://speakerdeck.com",
 ]
 
 autosectionlabel_prefix_document = True
```

### Comparing `cryptography-40.0.2/docs/development/c-bindings.rst` & `cryptography-41.0.0/docs/development/c-bindings.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/arc4/generate_arc4.py` & `cryptography-41.0.0/docs/development/custom-vectors/arc4/generate_arc4.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/arc4/verify_arc4.go` & `cryptography-41.0.0/docs/development/custom-vectors/arc4/verify_arc4.go`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/arc4.rst` & `cryptography-41.0.0/docs/development/custom-vectors/arc4.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/cast5/generate_cast5.py` & `cryptography-41.0.0/docs/development/custom-vectors/cast5/generate_cast5.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/cast5/verify_cast5.go` & `cryptography-41.0.0/docs/development/custom-vectors/cast5/verify_cast5.go`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/cast5.rst` & `cryptography-41.0.0/docs/development/custom-vectors/cast5.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/hkdf/generate_hkdf.py` & `cryptography-41.0.0/docs/development/custom-vectors/hkdf/generate_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/hkdf/verify_hkdf.go` & `cryptography-41.0.0/docs/development/custom-vectors/hkdf/verify_hkdf.go`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/hkdf.rst` & `cryptography-41.0.0/docs/development/custom-vectors/hkdf.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/idea/generate_idea.py` & `cryptography-41.0.0/docs/development/custom-vectors/idea/generate_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/idea/verify_idea.py` & `cryptography-41.0.0/docs/development/custom-vectors/idea/verify_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/idea.rst` & `cryptography-41.0.0/docs/development/custom-vectors/idea.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java` & `cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py` & `cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/rsa-oaep-sha2.rst` & `cryptography-41.0.0/docs/development/custom-vectors/rsa-oaep-sha2.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/secp256k1/generate_secp256k1.py` & `cryptography-41.0.0/docs/development/custom-vectors/secp256k1/generate_secp256k1.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/secp256k1/verify_secp256k1.py` & `cryptography-41.0.0/docs/development/custom-vectors/secp256k1/verify_secp256k1.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/secp256k1.rst` & `cryptography-41.0.0/docs/development/custom-vectors/secp256k1.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/seed/generate_seed.py` & `cryptography-41.0.0/docs/development/custom-vectors/seed/generate_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/seed/verify_seed.py` & `cryptography-41.0.0/docs/development/custom-vectors/seed/verify_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/custom-vectors/seed.rst` & `cryptography-41.0.0/docs/development/custom-vectors/seed.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/index.rst` & `cryptography-41.0.0/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/reviewing-patches.rst` & `cryptography-41.0.0/docs/development/reviewing-patches.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/development/submitting-patches.rst` & `cryptography-41.0.0/docs/development/submitting-patches.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 Code
 ----
 
 When in doubt, refer to :pep:`8` for Python code. You can check if your code
 meets our automated requirements by formatting it with ``black`` and running
 ``ruff`` against it. If you've installed the development requirements this
-will automatically use our configuration. You can also run the ``tox`` job with
-``tox -e flake``.
+will automatically use our configuration. You can also run the ``nox`` job with
+``nox -e flake``.
 
 `Write comments as complete sentences.`_
 
 Class names which contains acronyms or initialisms should always be
 capitalized. A class should be named ``HTTPClient``, not ``HttpClient``.
 
 Every code file must start with the boilerplate licensing notice:
@@ -91,15 +91,15 @@
 provide a set of test vectors. See :doc:`/development/test-vectors` for more
 details.
 
 Documentation
 -------------
 
 All features should be documented with prose in the ``docs`` section. To ensure
-it builds you can run ``tox -e docs``.
+it builds you can run ``nox -e docs``.
 
 Because of the inherent challenges in implementing correct cryptographic
 systems, we want to make our documentation point people in the right directions
 as much as possible. To that end:
 
 * When documenting a generic interface, use a strong algorithm in examples.
   (e.g. when showing a hashing example, don't use
```

### Comparing `cryptography-40.0.2/docs/development/test-vectors.rst` & `cryptography-41.0.0/docs/development/test-vectors.rst`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,18 @@
   (`server-ed448-cert.pem`_)
 * ``accvraiz1.pem`` - An RSA root certificate that contains an
   ``explicitText`` entry with a ``BMPString`` type.
 * ``scottishpower-bitstring-dn.pem`` - An ECDSA certificate that contains
   a subject DN with a bit string type.
 * ``cryptography-scts-tbs-precert.der`` - The "to-be-signed" pre-certificate
   bytes from ``cryptography-scts.pem``, with the SCT list extension removed.
+* ``belgian-eid-invalid-visiblestring.pem`` - A certificate with UTF-8
+  bytes in a ``VisibleString`` type.
+* ``ee-pss-sha1-cert.pem`` - An RSA PSS certificate using a SHA1 signature and
+  SHA1 for MGF1 from the OpenSSL test suite.
 
 Custom X.509 Vectors
 ~~~~~~~~~~~~~~~~~~~~
 
 * ``invalid_version.pem`` - Contains an RSA 2048 bit certificate with the
   X.509 version field set to ``0x7``.
 * ``post2000utctime.pem`` - Contains an RSA 2048 bit certificate with the
@@ -474,19 +478,31 @@
 * ``invalid-sct-length.der`` - A certificate with an SCT with an internal
   length greater than the amount of data.
 * ``bad_country.pem`` - A certificate with country name and jurisdiction
   country name values in its subject and issuer distinguished names which
   are longer than 2 characters.
 * ``rsa_pss_cert.pem`` - A self-signed certificate with an RSA PSS signature
   with ``asymmetric/PKCS8/rsa_pss_2048.pem`` as its key.
+* ``rsa_pss_cert_invalid_mgf.der`` - A self-signed certificate with an invalid
+  RSA PSS signature that has a non-MGF1 OID for its mask generation function in the
+  signature algorithm.
+* ``rsa_pss_cert_no_sig_params.der`` - A self-signed certificate with an invalid
+  RSA PSS signature algorithm that is missing signature parameters for PSS.
+* ``rsa_pss_cert_unsupported_mgf_hash.der`` - A self-signed certificate with an
+  unsupported MGF1 hash algorithm in the signature algorithm.
 * ``long-form-name-attribute.pem`` - A certificate with ``subject`` and ``issuer``
   names containing attributes whose value's tag is encoded in long-form.
 * ``mismatch_inner_outer_sig_algorithm.der`` - A leaf certificate derived from
   ``x509/cryptography.io.pem`` but modifying the ``tbs_cert.signature_algorithm``
   OID to not match the outer signature algorithm OID.
+* ``ms-certificate-template.pem`` - A certificate with a ``msCertificateTemplate``
+  extension.
+* ``rsa_pss_sha256_no_null.pem`` - A certificate with an RSA PSS signature
+  with no encoded ``NULL`` for the PSS hash algorithm parameters. This certificate
+  was generated by LibreSSL.
 
 Custom X.509 Request Vectors
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 * ``dsa_sha1.pem`` and ``dsa_sha1.der`` - Contain a certificate request using
   1024-bit DSA parameters and SHA1 generated using OpenSSL.
 * ``rsa_md4.pem`` and ``rsa_md4.der`` - Contain a certificate request using
@@ -654,16 +670,18 @@
   extension.
 * ``x509/ocsp/req-ext-unknown-oid.der`` - An OCSP request containing an
   extension with an unknown OID.
 * ``x509/ocsp/req-duplicate-ext.der`` - An OCSP request with duplicate
   extensions.
 * ``x509/ocsp/resp-unknown-extension.der`` - An OCSP response containing an
   extension with an unknown OID.
-* ``x509/ocsp/resp-unknown-hash-alg.der`` - AN OCSP response containing an
+* ``x509/ocsp/resp-unknown-hash-alg.der`` - An OCSP response containing an
   invalid hash algorithm OID.
+* ``x509/ocsp/req-acceptable-responses.der`` - An OCSP request containing an
+  acceptable responses extension.
 
 Custom PKCS12 Test Vectors
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 * ``pkcs12/cert-key-aes256cbc.p12`` - A PKCS12 file containing a cert
   (``x509/custom/ca/ca.pem``) and key (``x509/custom/ca/ca_key.pem``)
   both encrypted with AES 256 CBC with the password ``cryptography``.
 * ``pkcs12/cert-none-key-none.p12`` - A PKCS12 file containing a cert
@@ -795,14 +813,18 @@
 * ``pkcs7/amazon-roots.der`` - A DER encoded PCKS7 file containing Amazon Root
   CA 2 and 3 generated by OpenSSL.
 * ``pkcs7/enveloped.pem`` - A PEM encoded PKCS7 file with enveloped data.
 
 Custom OpenSSH Test Vectors
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+* ``ed25519-aesgcm-psw.key`` and ``ed25519-aesgcm-psw.key.pub`` generated by
+  exporting an Ed25519 key from ``1password 8`` with the password "password".
+  This key is encrypted using the ``aes256-gcm@openssh.com`` algorithm.
+
 Generated by
 ``asymmetric/OpenSSH/gen.sh``
 using command-line tools from OpenSSH_7.6p1 package.
 
 * ``dsa-nopsw.key``, ``dsa-nopsw.key.pub``, ``dsa-nopsw.key-cert.pub`` -
   DSA-1024 private key; and corresponding public key in plain format
   and with self-signed certificate.
@@ -993,21 +1015,21 @@
 .. _`BoringSSL ChaCha20Poly1305 tests`: https://boringssl.googlesource.com/boringssl/+/2e2a226ac9201ac411a84b5e79ac3a7333d8e1c9/crypto/cipher_extra/test/chacha20_poly1305_tests.txt
 .. _`BoringSSL evp tests`: https://boringssl.googlesource.com/boringssl/+/ce3773f9fe25c3b54390bc51d72572f251c7d7e6/crypto/evp/evp_tests.txt
 .. _`RIPEMD website`: https://homes.esat.kuleuven.be/~bosselae/ripemd160.html
 .. _`draft RFC`: https://tools.ietf.org/html/draft-josefsson-scrypt-kdf-01
 .. _`Specification repository`: https://github.com/fernet/spec
 .. _`errata`: https://www.rfc-editor.org/errata_search.php?rfc=6238
 .. _`OpenSSL example key`: https://github.com/openssl/openssl/blob/d02b48c63a58ea4367a0e905979f140b7d090f86/test/testrsa.pem
-.. _`GnuTLS key parsing tests`: https://gitlab.com/gnutls/gnutls/commit/f16ef39ef0303b02d7fa590a37820440c466ce8d
+.. _`GnuTLS key parsing tests`: https://gitlab.com/gnutls/gnutls/-/commit/f16ef39ef0303b02d7fa590a37820440c466ce8d
 .. _`enc-rsa-pkcs8.pem`: https://gitlab.com/gnutls/gnutls/blob/f8d943b38bf74eaaa11d396112daf43cb8aa82ae/tests/pkcs8-decode/encpkcs8.pem
 .. _`enc2-rsa-pkcs8.pem`: https://gitlab.com/gnutls/gnutls/blob/f8d943b38bf74eaaa11d396112daf43cb8aa82ae/tests/pkcs8-decode/enc2pkcs8.pem
 .. _`unenc-rsa-pkcs8.pem`: https://gitlab.com/gnutls/gnutls/blob/f8d943b38bf74eaaa11d396112daf43cb8aa82ae/tests/pkcs8-decode/unencpkcs8.pem
 .. _`pkcs12_s2k_pem.c`: https://gitlab.com/gnutls/gnutls/blob/f8d943b38bf74eaaa11d396112daf43cb8aa82ae/tests/pkcs12_s2k_pem.c
 .. _`Botan's ECC private keys`: https://github.com/randombit/botan/tree/4917f26a2b154e841cd27c1bcecdd41d2bdeb6ce/src/tests/data/ecc
-.. _`GnuTLS example keys`: https://gitlab.com/gnutls/gnutls/commit/ad2061deafdd7db78fd405f9d143b0a7c579da7b
+.. _`GnuTLS example keys`: https://gitlab.com/gnutls/gnutls/-/commit/ad2061deafdd7db78fd405f9d143b0a7c579da7b
 .. _`NESSIE IDEA vectors`: https://www.cosic.esat.kuleuven.be/nessie/testvectors/bc/idea/Idea-128-64.verified.test-vectors
 .. _`NESSIE`: https://en.wikipedia.org/wiki/NESSIE
 .. _`Ed25519 website`: https://ed25519.cr.yp.to/software.html
 .. _`NIST SP-800-38B`: https://csrc.nist.gov/publications/detail/sp/800-38b/archive/2005-05-01
 .. _`NIST PKI Testing`: https://csrc.nist.gov/Projects/PKI-Testing
 .. _`testx509.pem`: https://github.com/openssl/openssl/blob/master/test/testx509.pem
 .. _`DigiCert Global Root G3`: http://cacerts.digicert.com/DigiCertGlobalRootG3.crt
```

### Comparing `cryptography-40.0.2/docs/doing-a-release.rst` & `cryptography-41.0.0/docs/doing-a-release.rst`

 * *Files 7% similar despite different names*

```diff
@@ -36,29 +36,28 @@
 
 Bumping the version number
 --------------------------
 
 The next step in doing a release is bumping the version number in the
 software.
 
-* Update the version number in ``src/cryptography/__about__.py``.
-* Update the version number in ``vectors/cryptography_vectors/__about__.py``.
+* Run ``python release.py bump-version {new_version}``
 * Set the release date in the :doc:`/changelog`.
 * Do a commit indicating this.
 * Send a pull request with this.
 * Wait for it to be merged.
 
 Performing the release
 ----------------------
 
 The commit that merged the version number bump is now the official release
 commit for this release. You will need to have ``gpg`` installed and a ``gpg``
 key in order to do a release. Once this has happened:
 
-* Run ``python release.py {version}``.
+* Run ``python release.py release {version}``.
 
 The release should now be available on PyPI and a tag should be available in
 the repository.
 
 Verifying the release
 ---------------------
 
@@ -83,17 +82,16 @@
 ------------------
 
 * Send an email to the `mailing list`_ and `python-announce`_ announcing the
   release.
 * Close the `milestone`_ for the previous release on GitHub.
 * For major version releases, send a pull request to pyOpenSSL increasing the
   maximum ``cryptography`` version pin and perform a pyOpenSSL release.
-* Update the version number to the next major (e.g. ``0.5.dev1``) in
-  ``src/cryptography/__about__.py`` and
-  ``vectors/cryptography_vectors/__about__.py``.
+* Update the version number to the next major (e.g. ``0.5.dev1``) with
+  ``python release.py bump-version {new_version}``.
 * Add new :doc:`/changelog` entry with next version and note that it is under
   active development
 * Send a pull request with these items
 * Check for any outstanding code undergoing a deprecation cycle by looking in
   ``cryptography.utils`` for ``DeprecatedIn**`` definitions. If any exist open
   a ticket to increment them for the next release.
```

### Comparing `cryptography-40.0.2/docs/exceptions.rst` & `cryptography-41.0.0/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/faq.rst` & `cryptography-41.0.0/docs/faq.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 Frequently asked questions
 ==========================
 
+What issues can you help with in your issue tracker?
+----------------------------------------------------
+
+The primary purpose of our issue tracker is to enable us to identify and
+resolve bugs and feature requests in ``cryptography``, so any time a user
+files a bug, we start by asking: Is this a ``cryptography`` bug, or is it a
+bug somewhere else?
+
+That said, we do our best to help users to debug issues that are in their code
+or environments. Please note, however, that there's a limit to our ability to
+assist users in resolving problems that are specific to their environments,
+particularly when we have no way to reproduce the issue.
+
+Lastly, we're not able to provide support for general Python or Python
+packaging issues.
+
 .. _faq-howto-handle-deprecation-warning:
 
 I cannot suppress the deprecation warning that ``cryptography`` emits on import
 -------------------------------------------------------------------------------
 
 .. hint::
 
@@ -98,23 +114,14 @@
 Frequently ``InternalError`` is raised when there are errors on the OpenSSL
 error stack that were placed there by other libraries that are also using
 OpenSSL. Try removing the other libraries and see if the problem persists.
 If you have no other libraries using OpenSSL in your process, or they do not
 appear to be at fault, it's possible that this is a bug in ``cryptography``.
 Please file an `issue`_ with instructions on how to reproduce it.
 
-error: ``-Werror=sign-conversion``: No option ``-Wsign-conversion`` during installation
----------------------------------------------------------------------------------------
-
-The compiler you are using is too old and not supported by ``cryptography``.
-Please upgrade to a more recent version. If you are running OpenBSD 6.1 or
-earlier the default compiler is extremely old. Use ``pkg_add`` to install a
-newer ``gcc`` and then install ``cryptography`` using
-``CC=/path/to/newer/gcc pip install cryptography``.
-
 Installing cryptography with OpenSSL 0.9.8, 1.0.0, 1.0.1, 1.0.2, 1.1.0 fails
 ----------------------------------------------------------------------------
 
 The OpenSSL project has dropped support for the 0.9.8, 1.0.0, 1.0.1, 1.0.2,
 and 1.1.0 release series. Since they are no longer receiving security patches
 from upstream, ``cryptography`` is also dropping support for them. To fix this
 issue you should upgrade to a newer version of OpenSSL (1.1.1 or later). This
@@ -150,15 +157,15 @@
 greater than or equal to the version it specifies. Recent versions of ``pip``
 will automatically install ``abi3`` wheels.
 
 Why can't I import my PEM file?
 -------------------------------
 
 PEM is a format (defined by several RFCs, but originally :rfc:`1421`) for
-encoding keys, certificates and others cryptographic data into a regular form.
+encoding keys, certificates, and others cryptographic data into a regular form.
 The data is encoded as base64 and wrapped with a header and footer.
 
 If you are having trouble importing PEM files, make sure your file fits
 the following rules:
 
 * has a one-line header like this: ``-----BEGIN [FILE TYPE]-----``
   (where ``[FILE TYPE]`` is ``CERTIFICATE``, ``PUBLIC KEY``, ``PRIVATE KEY``,
```

### Comparing `cryptography-40.0.2/docs/fernet.rst` & `cryptography-41.0.0/docs/fernet.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/glossary.rst` & `cryptography-41.0.0/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/aead.rst` & `cryptography-41.0.0/docs/hazmat/primitives/aead.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/dh.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dh.rst`

 * *Files 4% similar despite different names*

```diff
@@ -170,21 +170,14 @@
 
         :param format: A value from the
             :class:`~cryptography.hazmat.primitives.serialization.ParameterFormat`
             enum. At the moment only ``PKCS3`` is supported.
 
         :return bytes: Serialized parameters.
 
-.. class:: DHParametersWithSerialization
-
-    .. versionadded:: 1.7
-
-    Alias for :class:`DHParameters`.
-
-
 Key interfaces
 ~~~~~~~~~~~~~~
 
 .. class:: DHPrivateKey
 
     .. versionadded:: 1.7
 
@@ -243,21 +236,14 @@
         :param encryption_algorithm: An instance of an object conforming to the
             :class:`~cryptography.hazmat.primitives.serialization.KeySerializationEncryption`
             interface.
 
         :return bytes: Serialized key.
 
 
-.. class:: DHPrivateKeyWithSerialization
-
-    .. versionadded:: 1.7
-
-    Alias for :class:`DHPrivateKey`.
-
-
 .. class:: DHPublicKey
 
     .. versionadded:: 1.7
 
     .. attribute:: key_size
 
         The bit length of the prime modulus.
@@ -289,21 +275,14 @@
             :class:`~cryptography.hazmat.primitives.serialization.Encoding` enum.
 
         :param format: A value from the
             :class:`~cryptography.hazmat.primitives.serialization.PublicFormat` enum.
 
         :return bytes: Serialized key.
 
-.. class:: DHPublicKeyWithSerialization
-
-    .. versionadded:: 1.7
-
-    Alias for :class:`DHPublicKey`.
-
-
 Numbers
 ~~~~~~~
 
 .. class:: DHParameterNumbers(p, g, q=None)
 
     .. versionadded:: 0.8
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/dsa.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/dsa.rst`

 * *Files 2% similar despite different names*

```diff
@@ -332,21 +332,14 @@
         :param encryption_algorithm: An instance of an object conforming to the
             :class:`~cryptography.hazmat.primitives.serialization.KeySerializationEncryption`
             interface.
 
         :return bytes: Serialized key.
 
 
-.. class:: DSAPrivateKeyWithSerialization
-
-    .. versionadded:: 0.8
-
-    Alias for :class:`DSAPrivateKey`.
-
-
 .. class:: DSAPublicKey
 
     .. versionadded:: 0.3
 
     A `DSA`_ public key.
 
     .. attribute:: key_size
@@ -408,19 +401,12 @@
             if the ``data`` you want to sign has already been hashed.
 
         :returns: None
         :raises cryptography.exceptions.InvalidSignature: If the signature does
             not validate.
 
 
-.. class:: DSAPublicKeyWithSerialization
-
-    .. versionadded:: 0.8
-
-    Alias for :class:`DSAPublicKey`.
-
-
 .. _`DSA`: https://en.wikipedia.org/wiki/Digital_Signature_Algorithm
 .. _`public-key`: https://en.wikipedia.org/wiki/Public-key_cryptography
 .. _`FIPS 186-4`: https://csrc.nist.gov/publications/detail/fips/186/4/final
 .. _`at least 2048`: https://www.cosic.esat.kuleuven.be/ecrypt/ecrypt2/documents/D.SPA.20.pdf
 .. _`ongoing protestations`: https://buttondown.email/cryptography-dispatches/archive/cryptography-dispatches-dsa-is-past-its-prime/
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/ec.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ec.rst`

 * *Files 2% similar despite different names*

```diff
@@ -530,19 +530,15 @@
         The digest algorithm to be used with the signature scheme.
 
 
 .. class:: EllipticCurvePrivateKey
 
     .. versionadded:: 0.5
 
-    An elliptic curve private key for use with an algorithm such as `ECDSA`_ or
-    `EdDSA`_. An elliptic curve private key that is not an
-    :term:`opaque key` also implements
-    :class:`EllipticCurvePrivateKeyWithSerialization` to provide serialization
-    methods.
+    An elliptic curve private key for use with an algorithm such as `ECDSA`_.
 
     .. method:: exchange(algorithm, peer_public_key)
 
         .. versionadded:: 1.1
 
         Performs a key exchange operation using the provided algorithm with
         the peer's public key.
@@ -628,21 +624,14 @@
         :param encryption_algorithm: An instance of an object conforming to the
             :class:`~cryptography.hazmat.primitives.serialization.KeySerializationEncryption`
             interface.
 
         :return bytes: Serialized key.
 
 
-.. class:: EllipticCurvePrivateKeyWithSerialization
-
-    .. versionadded:: 0.8
-
-    Alias for :class:`EllipticCurvePrivateKey`.
-
-
 .. class:: EllipticCurvePublicKey
 
     .. versionadded:: 0.5
 
     An elliptic curve public key.
 
      .. attribute:: curve
@@ -730,21 +719,14 @@
 
         :raises ValueError: Raised when an invalid point is supplied.
 
         :raises TypeError: Raised when curve is not an
             :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurve`.
 
 
-.. class:: EllipticCurvePublicKeyWithSerialization
-
-    .. versionadded:: 0.6
-
-    Alias for :class:`EllipticCurvePublicKey`.
-
-
 
 Serialization
 ~~~~~~~~~~~~~
 
 This sample demonstrates how to generate a private key and serialize it.
 
 
@@ -933,11 +915,10 @@
 .. _`800-56Ar2`: https://csrc.nist.gov/publications/detail/sp/800-56a/rev-2/final
 .. _`some concern`: https://crypto.stackexchange.com/questions/10263/should-we-trust-the-nist-recommended-ecc-parameters
 .. _`less than 224 bits`: https://www.cosic.esat.kuleuven.be/ecrypt/ecrypt2/documents/D.SPA.20.pdf
 .. _`elliptic curve diffie-hellman is faster than diffie-hellman`: https://digitalcommons.unl.edu/cgi/viewcontent.cgi?article=1100&context=cseconfwork
 .. _`minimize the number of security concerns for elliptic-curve cryptography`: https://cr.yp.to/ecdh/curve25519-20060209.pdf
 .. _`SafeCurves`: https://safecurves.cr.yp.to/
 .. _`ECDSA`: https://en.wikipedia.org/wiki/ECDSA
-.. _`EdDSA`: https://en.wikipedia.org/wiki/EdDSA
 .. _`forward secrecy`: https://en.wikipedia.org/wiki/Forward_secrecy
 .. _`SEC 1 v2.0`: https://www.secg.org/sec1-v2.pdf
 .. _`bad cryptographic practice`: https://crypto.stackexchange.com/a/3313
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/ed25519.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed25519.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/ed448.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/ed448.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/index.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/rsa.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/rsa.rst`

 * *Files 1% similar despite different names*

```diff
@@ -638,21 +638,14 @@
         :param encryption_algorithm: An instance of an object conforming to the
             :class:`~cryptography.hazmat.primitives.serialization.KeySerializationEncryption`
             interface.
 
         :return bytes: Serialized key.
 
 
-.. class:: RSAPrivateKeyWithSerialization
-
-    .. versionadded:: 0.8
-
-    Alias for :class:`RSAPrivateKey`.
-
-
 .. class:: RSAPublicKey
 
     .. versionadded:: 0.2
 
     An `RSA`_ public key.
 
     .. method:: encrypt(plaintext, padding)
@@ -779,21 +772,14 @@
 
         :raises cryptography.exceptions.InvalidSignature: If the signature is
             invalid.
 
         :raises cryptography.exceptions.UnsupportedAlgorithm: If signature
             data recovery is not supported with the provided ``padding`` type.
 
-.. class:: RSAPublicKeyWithSerialization
-
-    .. versionadded:: 0.8
-
-    Alias for :class:`RSAPublicKey`.
-
-
 .. _`RSA`: https://en.wikipedia.org/wiki/RSA_(cryptosystem)
 .. _`public-key`: https://en.wikipedia.org/wiki/Public-key_cryptography
 .. _`specific mathematical properties`: https://en.wikipedia.org/wiki/RSA_(cryptosystem)#Key_generation
 .. _`use 65537`: https://www.daemonology.net/blog/2009-06-11-cryptographic-right-answers.html
 .. _`at least 2048`: https://www.cosic.esat.kuleuven.be/ecrypt/ecrypt2/documents/D.SPA.20.pdf
 .. _`OpenPGP`: https://en.wikipedia.org/wiki/Pretty_Good_Privacy
 .. _`Chinese Remainder Theorem`: https://en.wikipedia.org/wiki/RSA_%28cryptosystem%29#Using_the_Chinese_remainder_algorithm
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/serialization.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/serialization.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1215,20 +1215,20 @@
 .. class:: PrivateFormat
     :canonical: cryptography.hazmat.primitives._serialization.PrivateFormat
 
     .. versionadded:: 0.8
 
     An enumeration for private key formats. Used with the ``private_bytes``
     method available on
-    :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKeyWithSerialization`
+    :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey`
     ,
-    :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKeyWithSerialization`
-    , :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKeyWithSerialization`
+    :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey`
+    , :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey`
     and
-    :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKeyWithSerialization`.
+    :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKey`.
 
     .. attribute:: TraditionalOpenSSL
 
         Frequently known as PKCS#1 format. Still a widely used format, but
         generally considered legacy.
 
         A PEM encoded RSA key will look like::
@@ -1322,20 +1322,20 @@
 
 .. class:: PublicFormat
 
     .. versionadded:: 0.8
 
     An enumeration for public key formats. Used with the ``public_bytes``
     method available on
-    :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKeyWithSerialization`
+    :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKey`
     ,
-    :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKeyWithSerialization`
-    , :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHPublicKeyWithSerialization`
+    :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKey`
+    , :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHPublicKey`
     , and
-    :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKeyWithSerialization`.
+    :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPublicKey`.
 
     .. attribute:: SubjectPublicKeyInfo
 
         This is the typical public key format. It consists of an algorithm
         identifier and the public key as a bit string. Choose this unless
         you have specific needs.
 
@@ -1386,33 +1386,33 @@
 
 .. class:: ParameterFormat
 
     .. versionadded:: 2.0
 
     An enumeration for parameters formats. Used with the ``parameter_bytes``
     method available on
-    :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHParametersWithSerialization`.
+    :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHParameters`.
 
     .. attribute:: PKCS3
 
         ASN1 DH parameters sequence as defined in `PKCS3`_.
 
 Serialization Encodings
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 .. class:: Encoding
     :canonical: cryptography.hazmat.primitives._serialization.Encoding
 
     An enumeration for encoding types. Used with the ``private_bytes`` method
     available on
-    :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKeyWithSerialization`
+    :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey`
     ,
-    :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKeyWithSerialization`
-    , :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKeyWithSerialization`,
-    :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKeyWithSerialization`,
+    :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey`
+    , :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHPrivateKey`,
+    :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKey`,
     and
     :class:`~cryptography.hazmat.primitives.asymmetric.x448.X448PrivateKey`
     as well as ``public_bytes`` on
     :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPublicKey`,
     :class:`~cryptography.hazmat.primitives.asymmetric.dh.DHPublicKey`,
     :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePublicKey`,
     and
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/utils.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/utils.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/x25519.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x25519.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/asymmetric/x448.rst` & `cryptography-41.0.0/docs/hazmat/primitives/asymmetric/x448.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/constant-time.rst` & `cryptography-41.0.0/docs/hazmat/primitives/constant-time.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/cryptographic-hashes.rst` & `cryptography-41.0.0/docs/hazmat/primitives/cryptographic-hashes.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/key-derivation-functions.rst` & `cryptography-41.0.0/docs/hazmat/primitives/key-derivation-functions.rst`

 * *Files 1% similar despite different names*

```diff
@@ -456,15 +456,16 @@
         highly recommended. Ideally as many bits of entropy as the security
         level of the hash: often that means cryptographically random and as
         long as the hash output. Worse (shorter, less entropy) salt values can
         still meaningfully contribute to security. May be reused. Does not have
         to be secret, but may cause stronger security guarantees if secret; see
         :rfc:`5869` and the `HKDF paper`_ for more details. If ``None`` is
         explicitly passed a default salt of ``algorithm.digest_size // 8`` null
-        bytes will be used.
+        bytes will be used. See `understanding HKDF`_ for additional detail about
+        the salt and info parameters.
 
     :param bytes info: Application specific context information.  If ``None``
         is explicitly passed an empty byte string will be used.
 
     :raises TypeError: This exception is raised if ``salt`` or ``info`` is not
                        ``bytes``.
 
@@ -1033,7 +1034,8 @@
 .. _`PBKDF2`: https://en.wikipedia.org/wiki/PBKDF2
 .. _`key stretching`: https://en.wikipedia.org/wiki/Key_stretching
 .. _`HKDF`: https://en.wikipedia.org/wiki/HKDF
 .. _`HKDF paper`: https://eprint.iacr.org/2010/264
 .. _`here`: https://stackoverflow.com/a/30308723/1170681
 .. _`recommends`: https://tools.ietf.org/html/rfc7914#section-2
 .. _`The scrypt paper`: https://www.tarsnap.com/scrypt/scrypt.pdf
+.. _`understanding HKDF`: https://soatok.blog/2021/11/17/understanding-hkdf/
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/keywrap.rst` & `cryptography-41.0.0/docs/hazmat/primitives/keywrap.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/mac/cmac.rst` & `cryptography-41.0.0/docs/hazmat/primitives/mac/cmac.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/mac/hmac.rst` & `cryptography-41.0.0/docs/hazmat/primitives/mac/hmac.rst`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         >>> h.verify(signature)
         >>>
         >>> h_copy.verify(b"an incorrect signature")
         Traceback (most recent call last):
         ...
         cryptography.exceptions.InvalidSignature: Signature did not match digest.
 
-    :param key: Secret key as ``bytes``.
+    :param key: The secret key.
     :type key: :term:`bytes-like`
     :param algorithm: An
         :class:`~cryptography.hazmat.primitives.hashes.HashAlgorithm`
         instance such as those described in
         :ref:`Cryptographic Hashes <cryptographic-hash-algorithms>`.
 
     :raises cryptography.exceptions.UnsupportedAlgorithm: This is raised if the
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/mac/poly1305.rst` & `cryptography-41.0.0/docs/hazmat/primitives/mac/poly1305.rst`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         >>> p = poly1305.Poly1305(key)
         >>> p.update(b"message to authenticate")
         >>> p.verify(b"an incorrect tag")
         Traceback (most recent call last):
         ...
         cryptography.exceptions.InvalidSignature: Value did not match computed tag.
 
-    :param key: Secret key as ``bytes``.
+    :param key: The secret key.
     :type key: :term:`bytes-like`
     :raises cryptography.exceptions.UnsupportedAlgorithm: This is raised if
         the version of OpenSSL ``cryptography`` is compiled against does not
         support this algorithm.
 
     .. method:: update(data)
```

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/padding.rst` & `cryptography-41.0.0/docs/hazmat/primitives/padding.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/symmetric-encryption.rst` & `cryptography-41.0.0/docs/hazmat/primitives/symmetric-encryption.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/hazmat/primitives/twofactor.rst` & `cryptography-41.0.0/docs/hazmat/primitives/twofactor.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/index.rst` & `cryptography-41.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/installation.rst` & `cryptography-41.0.0/docs/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 If this does not work please **upgrade your pip** first, as that is the
 single most common cause of installation problems.
 
 Supported platforms
 -------------------
 
-Currently we test ``cryptography`` on Python 3.6+ and PyPy3 7.3.10+ on these
+Currently we test ``cryptography`` on Python 3.7+ and PyPy3 7.3.10+ on these
 operating systems.
 
 * x86-64 RHEL 8.x
 * x86-64 CentOS 9 Stream
 * x86-64 Fedora (latest)
 * x86-64 macOS 12 Monterey
 * ARM64 macOS 13 Ventura
-* x86-64 Ubuntu 18.04, 20.04, 22.04, rolling
+* x86-64 Ubuntu 20.04, 22.04, rolling
 * ARM64 Ubuntu 22.04
 * x86-64 Debian Buster (10.x), Bullseye (11.x), Bookworm (12.x)
   and Sid (unstable)
 * x86-64 Alpine (latest)
 * ARM64 Alpine (latest)
 * 32-bit and 64-bit Python on 64-bit Windows Server 2022
 
@@ -52,15 +52,15 @@
 .. code-block:: console
 
     $ pip install cryptography
 
 If you prefer to compile it yourself you'll need to have OpenSSL installed.
 You can compile OpenSSL yourself as well or use `a binary distribution`_.
 Be sure to download the proper version for your architecture and Python
-(VC2015 is required for 3.6 and above). Wherever you place your copy of OpenSSL
+(VC2015 is required for 3.7 and above). Wherever you place your copy of OpenSSL
 you'll need to set the ``OPENSSL_DIR`` environment variable to include the
 proper location. For example:
 
 .. code-block:: console
 
     C:\> \path\to\vcvarsall.bat x86_amd64
     C:\> set OPENSSL_DIR=C:\OpenSSL-win64
@@ -75,19 +75,18 @@
 .. _build-on-linux:
 
 Building cryptography on Linux
 ------------------------------
 
 .. note::
 
-    If you are on RHEL/CentOS/Fedora/Debian/Ubuntu or another distribution
-    derived from the preceding list, then you should **upgrade pip** and
-    attempt to install ``cryptography`` again before following the instructions
-    to compile it below. These platforms will receive a binary wheel and
-    require no compiler if you have an updated ``pip``!
+    You should **upgrade pip** and attempt to install ``cryptography`` again
+    before following the instructions to compile it below. Most Linux
+    platforms will receive a binary wheel and require no compiler if you have
+    an updated ``pip``!
 
 ``cryptography`` ships ``manylinux`` wheels (as of 2.0) so all dependencies
 are included. For users on **pip 19.3** or above running on a ``manylinux2014``
 (or greater) compatible distribution (or **pip 21.2.4** for ``musllinux``) all
 you should need to do is:
 
 .. code-block:: console
@@ -102,46 +101,46 @@
 available<installation:Rust>`.
 
 Alpine
 ~~~~~~
 
 .. warning::
 
-    The Rust available by default in Alpine < 3.14 is older than the minimum
+    The Rust available by default in Alpine < 3.15 is older than the minimum
     supported version. See the :ref:`Rust installation instructions
     <installation:Rust>` for information about installing a newer Rust.
 
 .. code-block:: console
 
     $ sudo apk add gcc musl-dev python3-dev libffi-dev openssl-dev cargo pkgconfig
 
 If you get an error with ``openssl-dev`` you may have to use ``libressl-dev``.
 
 Debian/Ubuntu
 ~~~~~~~~~~~~~
 
 .. warning::
 
-    The Rust available in some Debian versions is older than the minimum
-    supported version. Debian Bullseye is sufficiently new, but otherwise
+    The Rust available in most Debian versions is older than the minimum
+    supported version. Debian Bookworm is sufficiently new, but otherwise
     please see the :ref:`Rust installation instructions <installation:Rust>`
     for information about installing a newer Rust.
 
 .. code-block:: console
 
     $ sudo apt-get install build-essential libssl-dev libffi-dev \
         python3-dev cargo pkg-config
 
 Fedora/RHEL/CentOS
 ~~~~~~~~~~~~~~~~~~
 
 .. warning::
 
-    For RHEL and CentOS you must be on version 8.3 or newer for the command
-    below to install a sufficiently new Rust. If your Rust is less than 1.48.0
+    For RHEL and CentOS you must be on version 8.6 or newer for the command
+    below to install a sufficiently new Rust. If your Rust is less than 1.56.0
     please see the :ref:`Rust installation instructions <installation:Rust>`
     for information about installing a newer Rust.
 
 .. code-block:: console
 
     $ sudo dnf install redhat-rpm-config gcc libffi-devel python3-devel \
         openssl-devel cargo pkg-config
@@ -311,15 +310,15 @@
     If you are using Linux, then you should **upgrade pip** (in
     a virtual environment!) and attempt to install ``cryptography`` again before
     trying to install the Rust toolchain. On most Linux distributions, the latest
     version of ``pip`` will be able to install a binary wheel, so you won't need
     a Rust toolchain.
 
 Building ``cryptography`` requires having a working Rust toolchain. The current
-minimum supported Rust version is 1.48.0. **This is newer than the Rust some
+minimum supported Rust version is 1.56.0. **This is newer than the Rust some
 package managers ship**, so users may need to install with the
 instructions below.
 
 Instructions for installing Rust can be found on `the Rust Project's website`_.
 We recommend installing Rust with ``rustup`` (as documented by the Rust
 Project) in order to ensure you have a recent version.
```

### Comparing `cryptography-40.0.2/docs/limitations.rst` & `cryptography-41.0.0/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/make.bat` & `cryptography-41.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/random-numbers.rst` & `cryptography-41.0.0/docs/random-numbers.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/security.rst` & `cryptography-41.0.0/docs/security.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/spelling_wordlist.txt` & `cryptography-41.0.0/docs/spelling_wordlist.txt`

 * *Files 8% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 iterable
 Kerberos
 Keychain
 Koblitz
 Lange
 logins
 metadata
+MGF
 Monterey
 Mozilla
 multi
 namespace
 namespaces
 macOS
 naïve
@@ -125,14 +126,15 @@
 toolchain
 tunable
 Ubuntu
 unencrypted
 unicode
 unpadded
 unpadding
+Ventura
 verifier
 Verifier
 Verisign
 versioning
 wildcard
 WoSign
 Wycheproof
```

### Comparing `cryptography-40.0.2/docs/x509/certificate-transparency.rst` & `cryptography-41.0.0/docs/x509/certificate-transparency.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/docs/x509/ocsp.rst` & `cryptography-41.0.0/docs/x509/ocsp.rst`

 * *Files 1% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 
         :param private_key: The
             :class:`~cryptography.hazmat.primitives.asymmetric.rsa.RSAPrivateKey`,
             :class:`~cryptography.hazmat.primitives.asymmetric.dsa.DSAPrivateKey`,
             :class:`~cryptography.hazmat.primitives.asymmetric.ec.EllipticCurvePrivateKey`,
             :class:`~cryptography.hazmat.primitives.asymmetric.ed25519.Ed25519PrivateKey` or
             :class:`~cryptography.hazmat.primitives.asymmetric.ed448.Ed448PrivateKey`
-            that will be used to sign the certificate.
+            that will be used to sign the response.
 
         :param algorithm: The
             :class:`~cryptography.hazmat.primitives.hashes.HashAlgorithm` that
             will be used to generate the signature.  This must be ``None`` if
             the ``private_key`` is an
             :class:`~cryptography.hazmat.primitives.asymmetric.ed25519.Ed25519PrivateKey`
             or an
@@ -800,8 +800,8 @@
         The algorithm used to generate the ``issuer_key_hash`` and
         ``issuer_name_hash``.
 
     .. attribute:: serial_number
 
         :type: int
 
-        The serial number of the certificate that was checked.
+        The serial number of the certificate that was checked.
```

### Comparing `cryptography-40.0.2/docs/x509/reference.rst` & `cryptography-41.0.0/docs/x509/reference.rst`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,38 @@
     a/9GeOKPiq90UMrCI+CAsIbzuPOaAp3g69JonuDwcs4cu8ui1udxs9q7ox3qSWGZ
     G1U/hmwvZH9kfIv5BKIzNLy4oxXPDJ7MZIBsxVxaNv8KUQ/JLtpVJa3oYqEx18+V
     JNr8Pr3y61X8pLmJnaCu+ixshiy2gjxXxDFBVEEt1G9JHrSs3R+yvcHxCrM3+ian
     Nh4=
     -----END CERTIFICATE-----
     """.strip()
 
+    rsa_pss_pem_cert = b"""
+    -----BEGIN CERTIFICATE-----
+    MIIDfTCCAjCgAwIBAgIUP4D/5rcT93vdYGPhsKf+hbes/JgwQgYJKoZIhvcNAQEK
+    MDWgDzANBglghkgBZQMEAgEFAKEcMBoGCSqGSIb3DQEBCDANBglghkgBZQMEAgEF
+    AKIEAgIA3jAaMRgwFgYDVQQDDA9jcnlwdG9ncmFwaHkuaW8wHhcNMjIwNDMwMjAz
+    MTE4WhcNMzMwNDEyMjAzMTE4WjAaMRgwFgYDVQQDDA9jcnlwdG9ncmFwaHkuaW8w
+    ggEgMAsGCSqGSIb3DQEBCgOCAQ8AMIIBCgKCAQEAt1jpboUoNppBVamc+nA+zEjl
+    jn/gPbRFCvyveRd8Yr0p8y1mlmjKXcQlXcHPVM4TopgFXqDykIHXxJxLV56ysb4K
+    UGe0nxpmhEso5ZGUgkDIIoH0NAQAsS8rS2ZzNJcLrLGrMY6DRgFsa+G6h2DvMwgl
+    nsX++a8FIm7Vu+OZnfWpDEuhJU4TRtHVviJSYkFMckyYBB48k1MU+0b4pezHconZ
+    mMEisBFFbwarNvowf2i/tRESe3myKXfiJsZZ2UzdE3FqycSgw1tx8qV/Z8myozUW
+    uihIdw8TGbbsJhEeVFxQEP/DVzC6HHDI3EVpr2jPYeIE60hhZwM7jUmQscLerQID
+    AQABo1MwUTAdBgNVHQ4EFgQUb1QD8QEIQn5DALIAujTDATssNcQwHwYDVR0jBBgw
+    FoAUb1QD8QEIQn5DALIAujTDATssNcQwDwYDVR0TAQH/BAUwAwEB/zBCBgkqhkiG
+    9w0BAQowNaAPMA0GCWCGSAFlAwQCAQUAoRwwGgYJKoZIhvcNAQEIMA0GCWCGSAFl
+    AwQCAQUAogQCAgDeA4IBAQAvKBXlx07tdmtfhNTPn16dupBIS5344ZE4tfGSE5Ir
+    iA1X0bukKQ6V+6xJXGreaIw0wvwtIeI/R0JwcR114HBDqjt40vklyNSpGCJzgkfD
+    Q/d8JXN/MLyQrk+5F9JMy+HuZAgefAQAjugC6389Klpqx2Z1CgwmALhjIs48GnMp
+    Iz9vU2O6RDkMBlBRdmfkJVjhhPvJYpDDW1ic5O3pxtMoiC1tAHHMm4gzM1WCFeOh
+    cDNxABlvVNPTnqkOhKBmmwRaBwdvvksgeu2RyBNR0KEy44gWzYB9/Ter2t4Z8ASq
+    qCv8TuYr2QGaCnI2FVS5S9n6l4JNkFHqPMtuhrkr3gEz
+    -----END CERTIFICATE-----
+    """.strip()
+
 Loading Certificates
 ~~~~~~~~~~~~~~~~~~~~
 
 .. function:: load_pem_x509_certificate(data)
     :canonical: cryptography.x509.base.load_pem_x509_certificate
 
     .. versionadded:: 0.7
@@ -409,14 +433,42 @@
 
 
         .. doctest::
 
             >>> cert.signature_algorithm_oid
             <ObjectIdentifier(oid=1.2.840.113549.1.1.11, name=sha256WithRSAEncryption)>
 
+    .. attribute:: signature_algorithm_parameters
+
+        .. versionadded:: 41.0.0
+
+        Returns the parameters of the signature algorithm used to sign the
+        certificate. For RSA signatures it will return either a
+        :class:`~cryptography.hazmat.primitives.asymmetric.padding.PKCS1v15` or
+        :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS` object.
+
+        For ECDSA signatures it will
+        return an :class:`~cryptography.hazmat.primitives.asymmetric.ec.ECDSA`.
+
+        For EdDSA and DSA signatures it will return ``None``.
+
+        These objects can be used to verify signatures on the certificate.
+
+        :returns: None,
+            :class:`~cryptography.hazmat.primitives.asymmetric.padding.PKCS1v15`,
+            :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`, or
+            :class:`~cryptography.hazmat.primitives.asymmetric.ec.ECDSA`
+
+        .. doctest::
+
+            >>> from cryptography.hazmat.primitives.asymmetric import padding
+            >>> pss_cert = x509.load_pem_x509_certificate(rsa_pss_pem_cert)
+            >>> isinstance(pss_cert.signature_algorithm_parameters, padding.PSS)
+            True
+
     .. attribute:: extensions
 
         :type: :class:`Extensions`
 
         The extensions encoded in the certificate.
 
         :raises cryptography.x509.DuplicateExtension: If more than one
@@ -816,15 +868,15 @@
 
         :param extval: An extension conforming to the
             :class:`~cryptography.x509.ExtensionType` interface.
 
         :param critical: Set to ``True`` if the extension must be understood and
              handled by whoever reads the certificate.
 
-    .. method:: sign(private_key, algorithm)
+    .. method:: sign(private_key, algorithm, *, rsa_padding=None)
 
         Sign the certificate using the CA's private key.
 
         :param private_key: The key that will be used to sign the certificate,
             one of
             :data:`~cryptography.hazmat.primitives.asymmetric.types.CertificateIssuerPrivateKeyTypes`.
 
@@ -835,14 +887,30 @@
             :class:`~cryptography.hazmat.primitives.asymmetric.ed25519.Ed25519PrivateKey`
             or an
             :class:`~cryptography.hazmat.primitives.asymmetric.ed448.Ed448PrivateKey`
             and an instance of a
             :class:`~cryptography.hazmat.primitives.hashes.HashAlgorithm`
             otherwise.
 
+        :param rsa_padding:
+
+            .. versionadded:: 41.0.0
+
+            This is a keyword-only argument. If ``private_key`` is an
+            ``RSAPrivateKey`` then this can be set to either
+            :class:`~cryptography.hazmat.primitives.asymmetric.padding.PKCS1v15` or
+            :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS` to sign
+            with those respective paddings. If this is ``None`` then RSA
+            keys will default to ``PKCS1v15`` padding. All other key types **must**
+            not pass a value other than ``None``.
+
+        :type rsa_padding: ``None``,
+            :class:`~cryptography.hazmat.primitives.asymmetric.padding.PKCS1v15`,
+            or :class:`~cryptography.hazmat.primitives.asymmetric.padding.PSS`
+
         :returns: :class:`~cryptography.x509.Certificate`
 
 
 X.509 CSR (Certificate Signing Request) Object
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. class:: CertificateSigningRequest
@@ -2659,14 +2727,42 @@
 
     .. attribute:: value
 
         :type: bytes
 
         Returns the DER encoded bytes payload of the extension.
 
+.. class:: MSCertificateTemplate(template_id, major_version, minor_version)
+    :canonical: cryptography.x509.extensions.MSCertificateTemplate
+
+    .. versionadded:: 41.0.0
+
+    The Microsoft certificate template extension is a proprietary Microsoft
+    PKI extension that is used to provide information about the template
+    associated with the certificate.
+
+    .. attribute:: oid
+
+        :type: :class:`ObjectIdentifier`
+
+        Returns
+        :attr:`~cryptography.x509.oid.ExtensionOID.MS_CERTIFICATE_TEMPLATE`.
+
+    .. attribute:: template_id
+
+        :type: :class:`ObjectIdentifier`
+
+    .. attribute:: major_version
+
+        :type: int or None
+
+    .. attribute:: minor_version
+
+        :type: int or None
+
 .. class:: CertificatePolicies(policies)
     :canonical: cryptography.x509.extensions.CertificatePolicies
 
     .. versionadded:: 0.9
 
     The certificate policies extension is an iterable, containing one or more
     :class:`PolicyInformation` instances.
@@ -2870,14 +2966,37 @@
         Returns
         :attr:`~cryptography.x509.oid.OCSPExtensionOID.NONCE`.
 
     .. attribute:: nonce
 
         :type: bytes
 
+.. class:: OCSPAcceptableResponses(response)
+    :canonical: cryptography.x509.extensions.OCSPAcceptableResponses
+
+    .. versionadded:: 41.0.0
+
+    OCSP acceptable responses is an extension that is only valid inside
+    :class:`~cryptography.x509.ocsp.OCSPRequest` objects. This allows an OCSP
+    client to tell the server what types of responses it supports. In practice
+    this is rarely used, because there is only one kind of OCSP response in
+    wide use.
+
+    .. attribute:: oid
+
+        :type: :class:`ObjectIdentifier`
+
+        Returns
+        :attr:`~cryptography.x509.oid.OCSPExtensionOID.ACCEPTABLE_RESPONSES`.
+
+    .. attribute:: nonce
+
+        :type: bytes
+
+
 X.509 Request Attributes
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 .. class:: Attributes
     :canonical: cryptography.x509.base.Attributes
 
     .. versionadded:: 36.0.0
@@ -2979,14 +3098,20 @@
 
         Corresponds to the dotted string ``"2.5.4.42"``.
 
     .. attribute:: TITLE
 
         Corresponds to the dotted string ``"2.5.4.12"``.
 
+    .. attribute:: INITIALS
+
+        .. versionadded:: 41.0.0
+
+        Corresponds to the dotted string ``"2.5.4.43"``.
+
     .. attribute:: GENERATION_QUALIFIER
 
         Corresponds to the dotted string ``"2.5.4.44"``.
 
     .. attribute:: X500_UNIQUE_IDENTIFIER
 
         .. versionadded:: 1.6
@@ -3477,14 +3602,20 @@
 
         Corresponds to the dotted string ``"2.5.29.33"``.
 
     .. attribute:: SUBJECT_DIRECTORY_ATTRIBUTES
 
         Corresponds to the dotted string ``"2.5.29.9"``.
 
+    .. attribute:: MS_CERTIFICATE_TEMPLATE
+
+        .. versionadded:: 41.0.0
+
+        Corresponds to the dotted string ``"1.3.6.1.4.1.311.21.7"``.
+
 
 .. class:: CRLEntryExtensionOID
     :canonical: cryptography.hazmat._oid.CRLEntryExtensionOID
 
     .. versionadded:: 1.2
 
     .. attribute:: CERTIFICATE_ISSUER
@@ -3505,14 +3636,20 @@
 
     .. versionadded:: 2.4
 
     .. attribute:: NONCE
 
         Corresponds to the dotted string ``"1.3.6.1.5.5.7.48.1.2"``.
 
+    .. attribute:: ACCEPTABLE_RESPONSES
+
+        .. versionadded:: 41.0.0
+
+        Corresponds to the dotted string ``"1.3.6.1.5.5.7.48.1.4"``.
+
 
 .. class:: AttributeOID
     :canonical: cryptography.hazmat._oid.AttributeOID
 
     .. versionadded:: 3.0
 
     .. attribute:: CHALLENGE_PASSWORD
```

### Comparing `cryptography-40.0.2/docs/x509/tutorial.rst` & `cryptography-41.0.0/docs/x509/tutorial.rst`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/setup.py` & `cryptography-41.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,29 +39,26 @@
 base_dir = os.path.dirname(__file__)
 src_dir = os.path.join(base_dir, "src")
 
 # When executing the setup.py, we need to be able to import ourselves, this
 # means that we need to add the src/ directory to the sys.path.
 sys.path.insert(0, src_dir)
 
+if hasattr(sys, "pypy_version_info") and sys.pypy_version_info < (7, 3, 10):
+    raise RuntimeError("cryptography is not compatible with PyPy3 < 7.3.10")
+
 try:
-    # See setup.cfg for most of the config metadata.
+    # See pyproject.toml for most of the config metadata.
     setup(
         rust_extensions=[
             RustExtension(
                 "cryptography.hazmat.bindings._rust",
                 "src/rust/Cargo.toml",
                 py_limited_api=True,
-                # Enable abi3 mode if we're not using PyPy.
-                features=(
-                    []
-                    if platform.python_implementation() == "PyPy"
-                    else ["pyo3/abi3-py36"]
-                ),
-                rust_version=">=1.48.0",
+                rust_version=">=1.56.0",
             )
         ],
     )
 except:  # noqa: E722
     # Note: This is a bare exception that re-raises so that we don't interfere
     # with anything the installation machinery might want to do. Because we
     # print this for any exception this msg can appear (e.g. in verbose logs)
@@ -97,16 +94,15 @@
         print(f"    {dist}: {version}")
     version = "n/a"
     if shutil.which("rustc") is not None:
         try:
             # If for any reason `rustc --version` fails, silently ignore it
             rustc_output = subprocess.run(
                 ["rustc", "--version"],
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
+                capture_output=True,
                 timeout=0.5,
                 encoding="utf8",
                 check=True,
             ).stdout
             version = re.sub("^rustc ", "", rustc_output.strip())
         except subprocess.SubprocessError:
             pass
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/asn1.py` & `cryptography-41.0.0/src/_cffi_src/openssl/asn1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/asn1.h>
 """
 
 TYPES = """
 typedef int... time_t;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/bignum.py` & `cryptography-41.0.0/src/_cffi_src/openssl/bignum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/bn.h>
 """
 
 TYPES = """
 static const long Cryptography_HAS_BN_FLAGS;
@@ -34,16 +35,14 @@
 BIGNUM *BN_CTX_get(BN_CTX *);
 void BN_CTX_end(BN_CTX *);
 
 BN_MONT_CTX *BN_MONT_CTX_new(void);
 int BN_MONT_CTX_set(BN_MONT_CTX *, const BIGNUM *, BN_CTX *);
 void BN_MONT_CTX_free(BN_MONT_CTX *);
 
-BIGNUM *BN_dup(const BIGNUM *);
-
 int BN_set_word(BIGNUM *, BN_ULONG);
 
 char *BN_bn2hex(const BIGNUM *);
 int BN_hex2bn(BIGNUM **, const char *);
 
 int BN_bn2bin(const BIGNUM *, unsigned char *);
 BIGNUM *BN_bin2bn(const unsigned char *, int, BIGNUM *);
@@ -56,16 +55,14 @@
                     BN_CTX *, BN_MONT_CTX *);
 int BN_mod_exp_mont_consttime(BIGNUM *, const BIGNUM *, const BIGNUM *,
                               const BIGNUM *, BN_CTX *, BN_MONT_CTX *);
 BIGNUM *BN_mod_inverse(BIGNUM *, const BIGNUM *, const BIGNUM *, BN_CTX *);
 
 int BN_num_bytes(const BIGNUM *);
 
-int BN_mod(BIGNUM *, const BIGNUM *, const BIGNUM *, BN_CTX *);
-
 /* The following 3 prime methods are exposed for Tribler. */
 int BN_generate_prime_ex(BIGNUM *, int, int, const BIGNUM *,
                          const BIGNUM *, BN_GENCB *);
 int BN_is_prime_ex(const BIGNUM *, int, BN_CTX *, BN_GENCB *);
 const int BN_prime_checks_for_size(int);
 """
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/bio.py` & `cryptography-41.0.0/src/_cffi_src/openssl/bio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/bio.h>
 """
 
 TYPES = """
 typedef ... BIO;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/callbacks.py` & `cryptography-41.0.0/src/_cffi_src/openssl/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <string.h>
 """
 
 TYPES = """
 typedef struct {
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/cmac.py` & `cryptography-41.0.0/src/_cffi_src/openssl/cmac.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #if !defined(OPENSSL_NO_CMAC)
 #include <openssl/cmac.h>
 #endif
 """
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/crypto.py` & `cryptography-41.0.0/src/_cffi_src/openssl/crypto.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/crypto.h>
 """
 
 TYPES = """
 static const long Cryptography_HAS_MEM_FUNCTIONS;
-static const long Cryptography_HAS_OPENSSL_CLEANUP;
 
 static const int OPENSSL_VERSION;
 static const int OPENSSL_CFLAGS;
 static const int OPENSSL_BUILT_ON;
 static const int OPENSSL_PLATFORM;
 static const int OPENSSL_DIR;
 """
@@ -37,21 +37,14 @@
 
 void *Cryptography_malloc_wrapper(size_t, const char *, int);
 void *Cryptography_realloc_wrapper(void *, size_t, const char *, int);
 void Cryptography_free_wrapper(void *, const char *, int);
 """
 
 CUSTOMIZATIONS = """
-#if CRYPTOGRAPHY_LIBRESSL_LESS_THAN_360
-static const long Cryptography_HAS_OPENSSL_CLEANUP = 0;
-void (*OPENSSL_cleanup)(void) = NULL;
-#else
-static const long Cryptography_HAS_OPENSSL_CLEANUP = 1;
-#endif
-
 #if CRYPTOGRAPHY_IS_LIBRESSL || CRYPTOGRAPHY_IS_BORINGSSL
 static const long Cryptography_HAS_MEM_FUNCTIONS = 0;
 int (*Cryptography_CRYPTO_set_mem_functions)(
     void *(*)(size_t, const char *, int),
     void *(*)(void *, size_t, const char *, int),
     void (*)(void *, const char *, int)) = NULL;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/cryptography.py` & `cryptography-41.0.0/src/_cffi_src/openssl/cryptography.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 /* define our OpenSSL API compatibility level to 1.1.0. Any symbols older than
    that will raise an error during compilation. */
 #define OPENSSL_API_COMPAT 0x10100000L
 
 #if defined(_WIN32)
@@ -38,58 +39,40 @@
 #if defined(OPENSSL_IS_BORINGSSL)
 #define CRYPTOGRAPHY_IS_BORINGSSL 1
 #else
 #define CRYPTOGRAPHY_IS_BORINGSSL 0
 #endif
 
 #if CRYPTOGRAPHY_IS_LIBRESSL
-#define CRYPTOGRAPHY_LIBRESSL_LESS_THAN_360 \
-    (LIBRESSL_VERSION_NUMBER < 0x3060000f)
 #define CRYPTOGRAPHY_LIBRESSL_LESS_THAN_370 \
     (LIBRESSL_VERSION_NUMBER < 0x3070000f)
 
 #else
-#define CRYPTOGRAPHY_LIBRESSL_LESS_THAN_360 (0)
 #define CRYPTOGRAPHY_LIBRESSL_LESS_THAN_370 (0)
 #endif
 
-#if OPENSSL_VERSION_NUMBER < 0x10101000
-    #error "pyca/cryptography MUST be linked with Openssl 1.1.1 or later"
+#if OPENSSL_VERSION_NUMBER < 0x10101040
+    #error "pyca/cryptography MUST be linked with Openssl 1.1.1d or later"
 #endif
 
-#define CRYPTOGRAPHY_OPENSSL_111D_OR_GREATER \
-    (OPENSSL_VERSION_NUMBER >= 0x10101040 && !CRYPTOGRAPHY_IS_LIBRESSL)
 #define CRYPTOGRAPHY_OPENSSL_300_OR_GREATER \
     (OPENSSL_VERSION_NUMBER >= 0x30000000 && !CRYPTOGRAPHY_IS_LIBRESSL)
 
-#define CRYPTOGRAPHY_OPENSSL_LESS_THAN_111B \
-    (OPENSSL_VERSION_NUMBER < 0x10101020 || CRYPTOGRAPHY_IS_LIBRESSL)
-#define CRYPTOGRAPHY_OPENSSL_LESS_THAN_111D \
-    (OPENSSL_VERSION_NUMBER < 0x10101040 || CRYPTOGRAPHY_IS_LIBRESSL)
 #define CRYPTOGRAPHY_OPENSSL_LESS_THAN_111E \
     (OPENSSL_VERSION_NUMBER < 0x10101050 || CRYPTOGRAPHY_IS_LIBRESSL)
-#if (CRYPTOGRAPHY_OPENSSL_LESS_THAN_111D && !CRYPTOGRAPHY_IS_LIBRESSL && \
-    !defined(OPENSSL_NO_ENGINE)) || defined(USE_OSRANDOM_RNG_FOR_TESTING)
-#define CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE 1
-#else
-#define CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE 0
-#endif
-/* Ed25519 support is available from OpenSSL 1.1.1b and LibreSSL 3.7.0. */
+/* Ed25519 support is in all supported OpenSSLs as well as LibreSSL 3.7.0. */
 #define CRYPTOGRAPHY_HAS_WORKING_ED25519 \
-    (!CRYPTOGRAPHY_OPENSSL_LESS_THAN_111B || \
+    (!CRYPTOGRAPHY_IS_LIBRESSL || \
     (CRYPTOGRAPHY_IS_LIBRESSL && !CRYPTOGRAPHY_LIBRESSL_LESS_THAN_370))
 """
 
 TYPES = """
-static const int CRYPTOGRAPHY_OPENSSL_111D_OR_GREATER;
 static const int CRYPTOGRAPHY_OPENSSL_300_OR_GREATER;
 
-static const int CRYPTOGRAPHY_OPENSSL_LESS_THAN_111B;
 static const int CRYPTOGRAPHY_OPENSSL_LESS_THAN_111E;
-static const int CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE;
 static const int CRYPTOGRAPHY_HAS_WORKING_ED25519;
 
 static const int CRYPTOGRAPHY_LIBRESSL_LESS_THAN_370;
 
 static const int CRYPTOGRAPHY_IS_LIBRESSL;
 static const int CRYPTOGRAPHY_IS_BORINGSSL;
 """
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/dsa.py` & `cryptography-41.0.0/src/_cffi_src/openssl/dsa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/dsa.h>
 """
 
 TYPES = """
 typedef ... DSA;
@@ -18,18 +19,15 @@
 DSA *DSAparams_dup(DSA *);
 int DSA_size(const DSA *);
 int DSA_sign(int, const unsigned char *, int, unsigned char *, unsigned int *,
              DSA *);
 int DSA_verify(int, const unsigned char *, int, const unsigned char *, int,
                DSA *);
 
-void DSA_get0_pqg(const DSA *, const BIGNUM **, const BIGNUM **,
-                  const BIGNUM **);
 int DSA_set0_pqg(DSA *, BIGNUM *, BIGNUM *, BIGNUM *);
-void DSA_get0_key(const DSA *, const BIGNUM **, const BIGNUM **);
 int DSA_set0_key(DSA *, BIGNUM *, BIGNUM *);
 int DSA_generate_parameters_ex(DSA *, int, unsigned char *, int,
                                int *, unsigned long *, BN_GENCB *);
 """
 
 CUSTOMIZATIONS = """
 """
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/ec.py` & `cryptography-41.0.0/src/_cffi_src/openssl/ec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/ec.h>
 #include <openssl/obj_mac.h>
 """
 
 TYPES = """
@@ -30,15 +31,14 @@
 
 EC_GROUP *EC_GROUP_new_by_curve_name(int);
 
 int EC_GROUP_get_curve_name(const EC_GROUP *);
 
 size_t EC_get_builtin_curves(EC_builtin_curve *, size_t);
 
-EC_KEY *EC_KEY_new(void);
 void EC_KEY_free(EC_KEY *);
 
 EC_KEY *EC_KEY_new_by_curve_name(int);
 const EC_GROUP *EC_KEY_get0_group(const EC_KEY *);
 const BIGNUM *EC_KEY_get0_private_key(const EC_KEY *);
 int EC_KEY_set_private_key(EC_KEY *, const BIGNUM *);
 const EC_POINT *EC_KEY_get0_public_key(const EC_KEY *);
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/ecdsa.py` & `cryptography-41.0.0/src/_cffi_src/openssl/ecdsa.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/ecdsa.h>
 """
 
 TYPES = """
 """
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/engine.py` & `cryptography-41.0.0/src/_cffi_src/openssl/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/engine.h>
 """
 
 TYPES = """
 typedef ... ENGINE;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/err.py` & `cryptography-41.0.0/src/_cffi_src/openssl/err.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/err.h>
 """
 
 TYPES = """
 static const int CIPHER_R_DATA_NOT_MULTIPLE_OF_BLOCK_LENGTH;
@@ -45,15 +46,15 @@
 CUSTOMIZATIONS = """
 /* This define is tied to provider support and is conditionally
    removed if Cryptography_HAS_PROVIDERS is false */
 #ifndef ERR_LIB_PROV
 #define ERR_LIB_PROV 0
 #endif
 
-#if !CRYPTOGRAPHY_OPENSSL_111D_OR_GREATER || CRYPTOGRAPHY_IS_BORINGSSL
+#ifndef EVP_R_XTS_DUPLICATED_KEYS
 static const int EVP_R_XTS_DUPLICATED_KEYS = 0;
 #endif
 
 #if CRYPTOGRAPHY_IS_BORINGSSL
 static const int ERR_LIB_PKCS12 = 0;
 static const int EVP_F_EVP_ENCRYPTFINAL_EX = 0;
 static const int EVP_R_BAD_DECRYPT = 0;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/evp.py` & `cryptography-41.0.0/src/_cffi_src/openssl/evp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/evp.h>
 """
 
 TYPES = """
 typedef ... EVP_CIPHER;
@@ -53,28 +54,22 @@
                      const unsigned char *, int);
 int EVP_CipherFinal_ex(EVP_CIPHER_CTX *, unsigned char *, int *);
 int EVP_CIPHER_CTX_reset(EVP_CIPHER_CTX *);
 EVP_CIPHER_CTX *EVP_CIPHER_CTX_new(void);
 void EVP_CIPHER_CTX_free(EVP_CIPHER_CTX *);
 int EVP_CIPHER_CTX_set_key_length(EVP_CIPHER_CTX *, int);
 
-int EVP_MD_CTX_copy_ex(EVP_MD_CTX *, const EVP_MD_CTX *);
-int EVP_DigestInit_ex(EVP_MD_CTX *, const EVP_MD *, ENGINE *);
-int EVP_DigestUpdate(EVP_MD_CTX *, const void *, size_t);
-int EVP_DigestFinal_ex(EVP_MD_CTX *, unsigned char *, unsigned int *);
 int EVP_DigestFinalXOF(EVP_MD_CTX *, unsigned char *, size_t);
 const EVP_MD *EVP_get_digestbyname(const char *);
 
 EVP_PKEY *EVP_PKEY_new(void);
 void EVP_PKEY_free(EVP_PKEY *);
 int EVP_PKEY_type(int);
 int EVP_PKEY_size(EVP_PKEY *);
 RSA *EVP_PKEY_get1_RSA(EVP_PKEY *);
-DSA *EVP_PKEY_get1_DSA(EVP_PKEY *);
-DH *EVP_PKEY_get1_DH(EVP_PKEY *);
 
 int EVP_PKEY_encrypt(EVP_PKEY_CTX *, unsigned char *, size_t *,
                      const unsigned char *, size_t);
 int EVP_PKEY_decrypt(EVP_PKEY_CTX *, unsigned char *, size_t *,
                      const unsigned char *, size_t);
 
 int EVP_SignInit(EVP_MD_CTX *, const EVP_MD *);
@@ -82,25 +77,16 @@
 int EVP_SignFinal(EVP_MD_CTX *, unsigned char *, unsigned int *, EVP_PKEY *);
 
 int EVP_VerifyInit(EVP_MD_CTX *, const EVP_MD *);
 int EVP_VerifyUpdate(EVP_MD_CTX *, const void *, size_t);
 int EVP_VerifyFinal(EVP_MD_CTX *, const unsigned char *, unsigned int,
                     EVP_PKEY *);
 
-int EVP_DigestSignInit(EVP_MD_CTX *, EVP_PKEY_CTX **, const EVP_MD *,
-                       ENGINE *, EVP_PKEY *);
-int EVP_DigestSignUpdate(EVP_MD_CTX *, const void *, size_t);
-int EVP_DigestSignFinal(EVP_MD_CTX *, unsigned char *, size_t *);
-int EVP_DigestVerifyInit(EVP_MD_CTX *, EVP_PKEY_CTX **, const EVP_MD *,
-                         ENGINE *, EVP_PKEY *);
-
-
 
 EVP_PKEY_CTX *EVP_PKEY_CTX_new(EVP_PKEY *, ENGINE *);
-EVP_PKEY_CTX *EVP_PKEY_CTX_new_id(int, ENGINE *);
 void EVP_PKEY_CTX_free(EVP_PKEY_CTX *);
 int EVP_PKEY_sign_init(EVP_PKEY_CTX *);
 int EVP_PKEY_sign(EVP_PKEY_CTX *, unsigned char *, size_t *,
                   const unsigned char *, size_t);
 int EVP_PKEY_verify_init(EVP_PKEY_CTX *);
 int EVP_PKEY_verify(EVP_PKEY_CTX *, const unsigned char *, size_t,
                     const unsigned char *, size_t);
@@ -112,49 +98,35 @@
 
 int EVP_PKEY_set1_RSA(EVP_PKEY *, RSA *);
 int EVP_PKEY_set1_DSA(EVP_PKEY *, DSA *);
 int EVP_PKEY_set1_DH(EVP_PKEY *, DH *);
 
 int EVP_PKEY_cmp(const EVP_PKEY *, const EVP_PKEY *);
 
-int EVP_PKEY_keygen_init(EVP_PKEY_CTX *);
-int EVP_PKEY_keygen(EVP_PKEY_CTX *, EVP_PKEY **);
 int EVP_PKEY_derive_init(EVP_PKEY_CTX *);
 int EVP_PKEY_derive_set_peer(EVP_PKEY_CTX *, EVP_PKEY *);
 int EVP_PKEY_derive_set_peer_ex(EVP_PKEY_CTX *, EVP_PKEY *, int);
 int EVP_PKEY_derive(EVP_PKEY_CTX *, unsigned char *, size_t *);
 
 int EVP_PKEY_id(const EVP_PKEY *);
 
 EVP_MD_CTX *EVP_MD_CTX_new(void);
 void EVP_MD_CTX_free(EVP_MD_CTX *);
 
-int EVP_DigestSign(EVP_MD_CTX *, unsigned char *, size_t *,
-                   const unsigned char *, size_t);
-int EVP_DigestVerify(EVP_MD_CTX *, const unsigned char *, size_t,
-                     const unsigned char *, size_t);
-
 int EVP_PKEY_bits(const EVP_PKEY *);
 
 int EVP_PKEY_assign_RSA(EVP_PKEY *, RSA *);
 
 EC_KEY *EVP_PKEY_get1_EC_KEY(EVP_PKEY *);
 int EVP_PKEY_set1_EC_KEY(EVP_PKEY *, EC_KEY *);
 
 int EVP_CIPHER_CTX_ctrl(EVP_CIPHER_CTX *, int, int, void *);
 
-int PKCS5_PBKDF2_HMAC(const char *, int, const unsigned char *, int, int,
-                      const EVP_MD *, int, unsigned char *);
-
 int EVP_PKEY_CTX_set_signature_md(EVP_PKEY_CTX *, const EVP_MD *);
 
-int EVP_PBE_scrypt(const char *, size_t, const unsigned char *, size_t,
-                   uint64_t, uint64_t, uint64_t, uint64_t, unsigned char *,
-                   size_t);
-
 EVP_PKEY *EVP_PKEY_new_raw_private_key(int, ENGINE *, const unsigned char *,
                                        size_t);
 EVP_PKEY *EVP_PKEY_new_raw_public_key(int, ENGINE *, const unsigned char *,
                                       size_t);
 int EVP_PKEY_get_raw_private_key(const EVP_PKEY *, unsigned char *, size_t *);
 int EVP_PKEY_get_raw_public_key(const EVP_PKEY *, unsigned char *, size_t *);
 
@@ -168,17 +140,14 @@
 #else
 const long Cryptography_HAS_EVP_PKEY_DHX = 0;
 const long EVP_PKEY_DHX = -1;
 #endif
 
 #if CRYPTOGRAPHY_IS_LIBRESSL || defined(OPENSSL_NO_SCRYPT)
 static const long Cryptography_HAS_SCRYPT = 0;
-int (*EVP_PBE_scrypt)(const char *, size_t, const unsigned char *, size_t,
-                      uint64_t, uint64_t, uint64_t, uint64_t, unsigned char *,
-                      size_t) = NULL;
 #else
 static const long Cryptography_HAS_SCRYPT = 1;
 #endif
 
 #if CRYPTOGRAPHY_IS_LIBRESSL
 static const long Cryptography_HAS_EVP_DIGESTFINAL_XOF = 0;
 int (*EVP_DigestFinalXOF)(EVP_MD_CTX *, unsigned char *, size_t) = NULL;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/fips.py` & `cryptography-41.0.0/src/_cffi_src/openssl/fips.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/crypto.h>
 """
 
 TYPES = """
 static const long Cryptography_HAS_FIPS;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/nid.py` & `cryptography-41.0.0/src/_cffi_src/openssl/nid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/obj_mac.h>
 """
 
 TYPES = """
 static const int Cryptography_HAS_ED448;
 static const int Cryptography_HAS_ED25519;
 static const int Cryptography_HAS_POLY1305;
 
 static const int NID_undef;
 static const int NID_aes_256_cbc;
 static const int NID_pbe_WithSHA1And3_Key_TripleDES_CBC;
-static const int NID_X448;
 static const int NID_ED25519;
 static const int NID_ED448;
 static const int NID_poly1305;
 
 static const int NID_subject_alt_name;
 static const int NID_crl_reason;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/pem.py` & `cryptography-41.0.0/src/_cffi_src/openssl/pem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/pem.h>
 """
 
 TYPES = """
 typedef int pem_password_cb(char *buf, int size, int rwflag, void *userdata);
@@ -37,15 +38,14 @@
 X509_REQ *PEM_read_bio_X509_REQ(BIO *, X509_REQ **, pem_password_cb *, void *);
 
 X509_CRL *PEM_read_bio_X509_CRL(BIO *, X509_CRL **, pem_password_cb *, void *);
 
 int PEM_write_bio_X509_CRL(BIO *, X509_CRL *);
 
 PKCS7 *PEM_read_bio_PKCS7(BIO *, PKCS7 **, pem_password_cb *, void *);
-int PEM_write_bio_PKCS7(BIO *, PKCS7 *);
 
 DH *PEM_read_bio_DHparams(BIO *, DH **, pem_password_cb *, void *);
 
 int PEM_write_bio_DSAPrivateKey(BIO *, DSA *, const EVP_CIPHER *,
                                 unsigned char *, int,
                                 pem_password_cb *, void *);
 
@@ -58,16 +58,11 @@
 int PEM_write_bio_RSAPublicKey(BIO *, const RSA *);
 
 EVP_PKEY *PEM_read_bio_PUBKEY(BIO *, EVP_PKEY **, pem_password_cb *, void *);
 int PEM_write_bio_PUBKEY(BIO *, EVP_PKEY *);
 int PEM_write_bio_ECPrivateKey(BIO *, EC_KEY *, const EVP_CIPHER *,
                                unsigned char *, int, pem_password_cb *,
                                void *);
-int PEM_write_bio_DHparams(BIO *, DH *);
-int PEM_write_bio_DHxparams(BIO *, DH *);
 """
 
 CUSTOMIZATIONS = """
-#if !defined(EVP_PKEY_DHX) || EVP_PKEY_DHX == -1
-int (*PEM_write_bio_DHxparams)(BIO *, DH *) = NULL;
-#endif
 """
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/pkcs12.py` & `cryptography-41.0.0/src/_cffi_src/openssl/pkcs12.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/pkcs12.h>
 """
 
 TYPES = """
 static const long Cryptography_HAS_PKCS12_SET_MAC;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/pkcs7.py` & `cryptography-41.0.0/src/_cffi_src/openssl/pkcs7.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/pkcs7.h>
 """
 
 TYPES = """
 static const long Cryptography_HAS_PKCS7_FUNCS;
@@ -43,16 +44,14 @@
 } PKCS7;
 
 static const int PKCS7_TEXT;
 """
 
 FUNCTIONS = """
 void PKCS7_free(PKCS7 *);
-PKCS7 *PKCS7_sign(X509 *, EVP_PKEY *, Cryptography_STACK_OF_X509 *,
-                   BIO *, int);
 int SMIME_write_PKCS7(BIO *, PKCS7 *, BIO *, int);
 int PEM_write_bio_PKCS7_stream(BIO *, PKCS7 *, BIO *, int);
 PKCS7_SIGNER_INFO *PKCS7_sign_add_signer(PKCS7 *, X509 *, EVP_PKEY *,
                                          const EVP_MD *, int);
 int PKCS7_final(PKCS7 *, BIO *, int);
 /* Included verify due to external consumer, see
    https://github.com/pyca/cryptography/issues/5433 */
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/provider.py` & `cryptography-41.0.0/src/_cffi_src/openssl/provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #if CRYPTOGRAPHY_OPENSSL_300_OR_GREATER
 #include <openssl/provider.h>
 #include <openssl/proverr.h>
 #endif
 """
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/rsa.py` & `cryptography-41.0.0/src/_cffi_src/openssl/rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/rsa.h>
 """
 
 TYPES = """
 typedef ... RSA;
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/ssl.py` & `cryptography-41.0.0/src/_cffi_src/openssl/ssl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/ssl.h>
 """
 
 TYPES = """
 static const long Cryptography_HAS_SSL_ST;
 static const long Cryptography_HAS_TLS_ST;
 static const long Cryptography_HAS_TLSv1_3_FUNCTIONS;
-static const long Cryptography_HAS_DTLS;
 static const long Cryptography_HAS_SIGALGS;
 static const long Cryptography_HAS_PSK;
 static const long Cryptography_HAS_PSK_TLSv1_3;
 static const long Cryptography_HAS_VERIFIED_CHAIN;
 static const long Cryptography_HAS_KEYLOG;
 static const long Cryptography_HAS_SSL_COOKIE;
 
@@ -331,16 +331,14 @@
 SSL_CTX *SSL_CTX_new(SSL_METHOD *);
 long SSL_CTX_get_timeout(const SSL_CTX *);
 
 const SSL_CIPHER *SSL_get_current_cipher(const SSL *);
 const char *SSL_get_version(const SSL *);
 int SSL_version(const SSL *);
 
-void *SSL_get_ex_data(const SSL *, int);
-
 void SSL_set_tlsext_host_name(SSL *, char *);
 void SSL_CTX_set_tlsext_servername_callback(
     SSL_CTX *,
     int (*)(SSL *, int *, void *));
 
 long SSL_set_tlsext_status_ocsp_resp(SSL *, unsigned char *, int);
 long SSL_get_tlsext_status_ocsp_resp(SSL *, const unsigned char **);
@@ -493,15 +491,14 @@
 #if CRYPTOGRAPHY_IS_LIBRESSL || CRYPTOGRAPHY_IS_BORINGSSL
 static const long Cryptography_HAS_DTLS_GET_DATA_MTU = 0;
 size_t (*DTLS_get_data_mtu)(SSL *) = NULL;
 #else
 static const long Cryptography_HAS_DTLS_GET_DATA_MTU = 1;
 #endif
 
-static const long Cryptography_HAS_DTLS = 1;
 /* Wrap DTLSv1_get_timeout to avoid cffi to handle a 'struct timeval'. */
 long Cryptography_DTLSv1_get_timeout(SSL *ssl, time_t *ptv_sec,
                                      long *ptv_usec) {
     struct timeval tv = { 0 };
     long r = DTLSv1_get_timeout(ssl, &tv);
 
     if (r == 1) {
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/x509.py` & `cryptography-41.0.0/src/_cffi_src/openssl/x509.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/ssl.h>
 
 /*
  * This is part of a work-around for the difficulty cffi has in dealing with
  * `STACK_OF(foo)` as the name of a type.  We invent a new, simpler name that
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/x509_vfy.py` & `cryptography-41.0.0/src/_cffi_src/openssl/x509_vfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/x509_vfy.h>
 
 /*
  * This is part of a work-around for the difficulty cffi has in dealing with
  * `STACK_OF(foo)` as the name of a type.  We invent a new, simpler name that
@@ -138,14 +139,15 @@
 int X509_STORE_load_locations(X509_STORE *, const char *, const char *);
 int X509_STORE_set1_param(X509_STORE *, X509_VERIFY_PARAM *);
 int X509_STORE_set_default_paths(X509_STORE *);
 int X509_STORE_set_flags(X509_STORE *, unsigned long);
 /* Included due to external consumer, see
    https://github.com/pyca/pyopenssl/issues/1031 */
 int X509_STORE_set_purpose(X509_STORE *, int);
+int X509_STORE_up_ref(X509_STORE *);
 void X509_STORE_free(X509_STORE *);
 
 /* X509_STORE_CTX */
 X509_STORE_CTX *X509_STORE_CTX_new(void);
 void X509_STORE_CTX_cleanup(X509_STORE_CTX *);
 void X509_STORE_CTX_free(X509_STORE_CTX *);
 int X509_STORE_CTX_init(X509_STORE_CTX *, X509_STORE *, X509 *,
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/x509name.py` & `cryptography-41.0.0/src/_cffi_src/openssl/x509name.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/x509.h>
 
 /*
  * See the comment above Cryptography_STACK_OF_X509 in x509.py
  */
@@ -34,15 +35,14 @@
 X509_NAME *X509_NAME_dup(X509_NAME *);
 int X509_NAME_entry_count(const X509_NAME *);
 X509_NAME_ENTRY *X509_NAME_get_entry(const X509_NAME *, int);
 char *X509_NAME_oneline(const X509_NAME *, char *, int);
 
 ASN1_OBJECT *X509_NAME_ENTRY_get_object(const X509_NAME_ENTRY *);
 ASN1_STRING *X509_NAME_ENTRY_get_data(const X509_NAME_ENTRY *);
-int X509_NAME_add_entry(X509_NAME *, X509_NAME_ENTRY *, int, int);
 
 int X509_NAME_add_entry_by_NID(X509_NAME *, int, int, const unsigned char *,
                                int, int, int);
 
 Cryptography_STACK_OF_X509_NAME *sk_X509_NAME_new_null(void);
 int sk_X509_NAME_num(Cryptography_STACK_OF_X509_NAME *);
 int sk_X509_NAME_push(Cryptography_STACK_OF_X509_NAME *, X509_NAME *);
```

### Comparing `cryptography-40.0.2/src/_cffi_src/openssl/x509v3.py` & `cryptography-41.0.0/src/_cffi_src/openssl/x509v3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 INCLUDES = """
 #include <openssl/x509v3.h>
 
 /*
  * This is part of a work-around for the difficulty cffi has in dealing with
  * `STACK_OF(foo)` as the name of a type.  We invent a new, simpler name that
```

### Comparing `cryptography-40.0.2/src/_cffi_src/utils.py` & `cryptography-41.0.0/src/_cffi_src/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import os
 import platform
 import sys
-from distutils.ccompiler import new_compiler
-from distutils.dist import Distribution
+import typing
 
 from cffi import FFI
 
 # Load the cryptography __about__ to get the current package version
 base_src = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 about = {}
 with open(os.path.join(base_src, "cryptography", "__about__.py")) as f:
     exec(f.read(), about)
 
 
 def build_ffi_for_binding(
-    module_name,
-    module_prefix,
-    modules,
-    libraries,
-    extra_compile_args,
+    module_name: str,
+    module_prefix: str,
+    modules: typing.List[str],
 ):
     """
     Modules listed in ``modules`` should have the following attributes:
 
     * ``INCLUDES``: A string containing C includes.
     * ``TYPES``: A string containing C declarations for types.
     * ``FUNCTIONS``: A string containing C declarations for functions & macros.
@@ -49,25 +47,21 @@
         customizations.append(module.CUSTOMIZATIONS)
 
     verify_source = "\n".join(includes + customizations)
     return build_ffi(
         module_name,
         cdef_source="\n".join(types + functions),
         verify_source=verify_source,
-        libraries=libraries,
-        extra_compile_args=extra_compile_args,
     )
 
 
 def build_ffi(
-    module_name,
-    cdef_source,
-    verify_source,
-    libraries,
-    extra_compile_args,
+    module_name: str,
+    cdef_source: str,
+    verify_source: str,
 ):
     ffi = FFI()
     # Always add the CRYPTOGRAPHY_PACKAGE_VERSION to the shared object
     cdef_source += "\nstatic const char *const CRYPTOGRAPHY_PACKAGE_VERSION;"
     verify_source += '\n#define CRYPTOGRAPHY_PACKAGE_VERSION "{}"'.format(
         about["__version__"]
     )
@@ -83,24 +77,9 @@
     return result;
 }
 """
     ffi.cdef(cdef_source)
     ffi.set_source(
         module_name,
         verify_source,
-        libraries=libraries,
-        extra_compile_args=extra_compile_args,
     )
     return ffi
-
-
-def compiler_type():
-    """
-    Gets the compiler type from distutils. On Windows with MSVC it will be
-    "msvc". On macOS and linux it is "unix".
-    """
-    dist = Distribution()
-    dist.parse_config_files()
-    cmd = dist.get_command_obj("build")
-    cmd.ensure_finalized()
-    compiler = new_compiler(compiler=cmd.compiler)
-    return compiler.compiler_type
```

### Comparing `cryptography-40.0.2/src/cryptography/exceptions.py` & `cryptography-41.0.0/src/cryptography/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
-from cryptography import utils
+from cryptography.hazmat.bindings._rust import exceptions as rust_exceptions
 
 if typing.TYPE_CHECKING:
     from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 
-
-class _Reasons(utils.Enum):
-    BACKEND_MISSING_INTERFACE = 0
-    UNSUPPORTED_HASH = 1
-    UNSUPPORTED_CIPHER = 2
-    UNSUPPORTED_PADDING = 3
-    UNSUPPORTED_MGF = 4
-    UNSUPPORTED_PUBLIC_KEY_ALGORITHM = 5
-    UNSUPPORTED_ELLIPTIC_CURVE = 6
-    UNSUPPORTED_SERIALIZATION = 7
-    UNSUPPORTED_X509 = 8
-    UNSUPPORTED_EXCHANGE_ALGORITHM = 9
-    UNSUPPORTED_DIFFIE_HELLMAN = 10
-    UNSUPPORTED_MAC = 11
+_Reasons = rust_exceptions._Reasons
 
 
 class UnsupportedAlgorithm(Exception):
     def __init__(
         self, message: str, reason: typing.Optional[_Reasons] = None
     ) -> None:
         super().__init__(message)
@@ -52,15 +40,15 @@
 
 class InvalidSignature(Exception):
     pass
 
 
 class InternalError(Exception):
     def __init__(
-        self, msg: str, err_code: typing.List["rust_openssl.OpenSSLError"]
+        self, msg: str, err_code: typing.List[rust_openssl.OpenSSLError]
     ) -> None:
         super().__init__(msg)
         self.err_code = err_code
 
 
 class InvalidKey(Exception):
     pass
```

### Comparing `cryptography-40.0.2/src/cryptography/fernet.py` & `cryptography-41.0.0/src/cryptography/fernet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import base64
 import binascii
 import os
 import time
 import typing
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/_oid.py` & `cryptography-41.0.0/src/cryptography/hazmat/_oid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography.hazmat.bindings._rust import (
     ObjectIdentifier as ObjectIdentifier,
 )
 from cryptography.hazmat.primitives import hashes
 
@@ -34,18 +36,20 @@
     CRL_NUMBER = ObjectIdentifier("2.5.29.20")
     DELTA_CRL_INDICATOR = ObjectIdentifier("2.5.29.27")
     PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS = ObjectIdentifier(
         "1.3.6.1.4.1.11129.2.4.2"
     )
     PRECERT_POISON = ObjectIdentifier("1.3.6.1.4.1.11129.2.4.3")
     SIGNED_CERTIFICATE_TIMESTAMPS = ObjectIdentifier("1.3.6.1.4.1.11129.2.4.5")
+    MS_CERTIFICATE_TEMPLATE = ObjectIdentifier("1.3.6.1.4.1.311.21.7")
 
 
 class OCSPExtensionOID:
     NONCE = ObjectIdentifier("1.3.6.1.5.5.7.48.1.2")
+    ACCEPTABLE_RESPONSES = ObjectIdentifier("1.3.6.1.5.5.7.48.1.4")
 
 
 class CRLEntryExtensionOID:
     CERTIFICATE_ISSUER = ObjectIdentifier("2.5.29.29")
     CRL_REASON = ObjectIdentifier("2.5.29.21")
     INVALIDITY_DATE = ObjectIdentifier("2.5.29.24")
 
@@ -58,14 +62,15 @@
     STREET_ADDRESS = ObjectIdentifier("2.5.4.9")
     ORGANIZATION_NAME = ObjectIdentifier("2.5.4.10")
     ORGANIZATIONAL_UNIT_NAME = ObjectIdentifier("2.5.4.11")
     SERIAL_NUMBER = ObjectIdentifier("2.5.4.5")
     SURNAME = ObjectIdentifier("2.5.4.4")
     GIVEN_NAME = ObjectIdentifier("2.5.4.42")
     TITLE = ObjectIdentifier("2.5.4.12")
+    INITIALS = ObjectIdentifier("2.5.4.43")
     GENERATION_QUALIFIER = ObjectIdentifier("2.5.4.44")
     X500_UNIQUE_IDENTIFIER = ObjectIdentifier("2.5.4.45")
     DN_QUALIFIER = ObjectIdentifier("2.5.4.46")
     PSEUDONYM = ObjectIdentifier("2.5.4.65")
     USER_ID = ObjectIdentifier("0.9.2342.19200300.100.1.1")
     DOMAIN_COMPONENT = ObjectIdentifier("0.9.2342.19200300.100.1.25")
     EMAIL_ADDRESS = ObjectIdentifier("1.2.840.113549.1.9.1")
@@ -260,14 +265,15 @@
     ExtensionOID.PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS: (
         "signedCertificateTimestampList"
     ),
     ExtensionOID.SIGNED_CERTIFICATE_TIMESTAMPS: (
         "signedCertificateTimestampList"
     ),
     ExtensionOID.PRECERT_POISON: "ctPoison",
+    ExtensionOID.MS_CERTIFICATE_TEMPLATE: "msCertificateTemplate",
     CRLEntryExtensionOID.CRL_REASON: "cRLReason",
     CRLEntryExtensionOID.INVALIDITY_DATE: "invalidityDate",
     CRLEntryExtensionOID.CERTIFICATE_ISSUER: "certificateIssuer",
     ExtensionOID.NAME_CONSTRAINTS: "nameConstraints",
     ExtensionOID.CRL_DISTRIBUTION_POINTS: "cRLDistributionPoints",
     ExtensionOID.CERTIFICATE_POLICIES: "certificatePolicies",
     ExtensionOID.POLICY_MAPPINGS: "policyMappings",
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/aead.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/aead.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography.exceptions import InvalidTag
 
 if typing.TYPE_CHECKING:
     from cryptography.hazmat.backends.openssl.backend import Backend
     from cryptography.hazmat.primitives.ciphers.aead import (
@@ -16,19 +18,219 @@
         ChaCha20Poly1305,
     )
 
     _AEADTypes = typing.Union[
         AESCCM, AESGCM, AESOCB3, AESSIV, ChaCha20Poly1305
     ]
 
+
+def _is_evp_aead_supported_cipher(
+    backend: Backend, cipher: _AEADTypes
+) -> bool:
+    """
+    Checks whether the given cipher is supported through
+    EVP_AEAD rather than the normal OpenSSL EVP_CIPHER API.
+    """
+    from cryptography.hazmat.primitives.ciphers.aead import ChaCha20Poly1305
+
+    return backend._lib.Cryptography_HAS_EVP_AEAD and isinstance(
+        cipher, ChaCha20Poly1305
+    )
+
+
+def _aead_cipher_supported(backend: Backend, cipher: _AEADTypes) -> bool:
+    if _is_evp_aead_supported_cipher(backend, cipher):
+        return True
+    else:
+        cipher_name = _evp_cipher_cipher_name(cipher)
+        if backend._fips_enabled and cipher_name not in backend._fips_aead:
+            return False
+        # SIV isn't loaded through get_cipherbyname but instead a new fetch API
+        # only available in 3.0+. But if we know we're on 3.0+ then we know
+        # it's supported.
+        if cipher_name.endswith(b"-siv"):
+            return backend._lib.CRYPTOGRAPHY_OPENSSL_300_OR_GREATER == 1
+        else:
+            return (
+                backend._lib.EVP_get_cipherbyname(cipher_name)
+                != backend._ffi.NULL
+            )
+
+
+def _aead_create_ctx(
+    backend: Backend,
+    cipher: _AEADTypes,
+    key: bytes,
+):
+    if _is_evp_aead_supported_cipher(backend, cipher):
+        return _evp_aead_create_ctx(backend, cipher, key)
+    else:
+        return _evp_cipher_create_ctx(backend, cipher, key)
+
+
+def _encrypt(
+    backend: Backend,
+    cipher: _AEADTypes,
+    nonce: bytes,
+    data: bytes,
+    associated_data: typing.List[bytes],
+    tag_length: int,
+    ctx: typing.Any = None,
+) -> bytes:
+    if _is_evp_aead_supported_cipher(backend, cipher):
+        return _evp_aead_encrypt(
+            backend, cipher, nonce, data, associated_data, tag_length, ctx
+        )
+    else:
+        return _evp_cipher_encrypt(
+            backend, cipher, nonce, data, associated_data, tag_length, ctx
+        )
+
+
+def _decrypt(
+    backend: Backend,
+    cipher: _AEADTypes,
+    nonce: bytes,
+    data: bytes,
+    associated_data: typing.List[bytes],
+    tag_length: int,
+    ctx: typing.Any = None,
+) -> bytes:
+    if _is_evp_aead_supported_cipher(backend, cipher):
+        return _evp_aead_decrypt(
+            backend, cipher, nonce, data, associated_data, tag_length, ctx
+        )
+    else:
+        return _evp_cipher_decrypt(
+            backend, cipher, nonce, data, associated_data, tag_length, ctx
+        )
+
+
+def _evp_aead_create_ctx(
+    backend: Backend,
+    cipher: _AEADTypes,
+    key: bytes,
+    tag_len: typing.Optional[int] = None,
+):
+    aead_cipher = _evp_aead_get_cipher(backend, cipher)
+    assert aead_cipher is not None
+    key_ptr = backend._ffi.from_buffer(key)
+    tag_len = (
+        backend._lib.EVP_AEAD_DEFAULT_TAG_LENGTH
+        if tag_len is None
+        else tag_len
+    )
+    ctx = backend._lib.Cryptography_EVP_AEAD_CTX_new(
+        aead_cipher, key_ptr, len(key), tag_len
+    )
+    backend.openssl_assert(ctx != backend._ffi.NULL)
+    ctx = backend._ffi.gc(ctx, backend._lib.EVP_AEAD_CTX_free)
+    return ctx
+
+
+def _evp_aead_get_cipher(backend: Backend, cipher: _AEADTypes):
+    from cryptography.hazmat.primitives.ciphers.aead import (
+        ChaCha20Poly1305,
+    )
+
+    # Currently only ChaCha20-Poly1305 is supported using this API
+    assert isinstance(cipher, ChaCha20Poly1305)
+    return backend._lib.EVP_aead_chacha20_poly1305()
+
+
+def _evp_aead_encrypt(
+    backend: Backend,
+    cipher: _AEADTypes,
+    nonce: bytes,
+    data: bytes,
+    associated_data: typing.List[bytes],
+    tag_length: int,
+    ctx: typing.Any,
+) -> bytes:
+    assert ctx is not None
+
+    aead_cipher = _evp_aead_get_cipher(backend, cipher)
+    assert aead_cipher is not None
+
+    out_len = backend._ffi.new("size_t *")
+    # max_out_len should be in_len plus the result of
+    # EVP_AEAD_max_overhead.
+    max_out_len = len(data) + backend._lib.EVP_AEAD_max_overhead(aead_cipher)
+    out_buf = backend._ffi.new("uint8_t[]", max_out_len)
+    data_ptr = backend._ffi.from_buffer(data)
+    nonce_ptr = backend._ffi.from_buffer(nonce)
+    aad = b"".join(associated_data)
+    aad_ptr = backend._ffi.from_buffer(aad)
+
+    res = backend._lib.EVP_AEAD_CTX_seal(
+        ctx,
+        out_buf,
+        out_len,
+        max_out_len,
+        nonce_ptr,
+        len(nonce),
+        data_ptr,
+        len(data),
+        aad_ptr,
+        len(aad),
+    )
+    backend.openssl_assert(res == 1)
+    encrypted_data = backend._ffi.buffer(out_buf, out_len[0])[:]
+    return encrypted_data
+
+
+def _evp_aead_decrypt(
+    backend: Backend,
+    cipher: _AEADTypes,
+    nonce: bytes,
+    data: bytes,
+    associated_data: typing.List[bytes],
+    tag_length: int,
+    ctx: typing.Any,
+) -> bytes:
+    if len(data) < tag_length:
+        raise InvalidTag
+
+    assert ctx is not None
+
+    out_len = backend._ffi.new("size_t *")
+    #  max_out_len should at least in_len
+    max_out_len = len(data)
+    out_buf = backend._ffi.new("uint8_t[]", max_out_len)
+    data_ptr = backend._ffi.from_buffer(data)
+    nonce_ptr = backend._ffi.from_buffer(nonce)
+    aad = b"".join(associated_data)
+    aad_ptr = backend._ffi.from_buffer(aad)
+
+    res = backend._lib.EVP_AEAD_CTX_open(
+        ctx,
+        out_buf,
+        out_len,
+        max_out_len,
+        nonce_ptr,
+        len(nonce),
+        data_ptr,
+        len(data),
+        aad_ptr,
+        len(aad),
+    )
+
+    if res == 0:
+        backend._consume_errors()
+        raise InvalidTag
+
+    decrypted_data = backend._ffi.buffer(out_buf, out_len[0])[:]
+    return decrypted_data
+
+
 _ENCRYPT = 1
 _DECRYPT = 0
 
 
-def _aead_cipher_name(cipher: "_AEADTypes") -> bytes:
+def _evp_cipher_cipher_name(cipher: _AEADTypes) -> bytes:
     from cryptography.hazmat.primitives.ciphers.aead import (
         AESCCM,
         AESGCM,
         AESOCB3,
         AESSIV,
         ChaCha20Poly1305,
     )
@@ -42,15 +244,15 @@
     elif isinstance(cipher, AESSIV):
         return f"aes-{len(cipher._key) * 8 // 2}-siv".encode("ascii")
     else:
         assert isinstance(cipher, AESGCM)
         return f"aes-{len(cipher._key) * 8}-gcm".encode("ascii")
 
 
-def _evp_cipher(cipher_name: bytes, backend: "Backend"):
+def _evp_cipher(cipher_name: bytes, backend: Backend):
     if cipher_name.endswith(b"-siv"):
         evp_cipher = backend._lib.EVP_CIPHER_fetch(
             backend._ffi.NULL,
             cipher_name,
             backend._ffi.NULL,
         )
         backend.openssl_assert(evp_cipher != backend._ffi.NULL)
@@ -58,39 +260,39 @@
     else:
         evp_cipher = backend._lib.EVP_get_cipherbyname(cipher_name)
         backend.openssl_assert(evp_cipher != backend._ffi.NULL)
 
     return evp_cipher
 
 
-def _aead_create_ctx(
-    backend: "Backend",
-    cipher: "_AEADTypes",
+def _evp_cipher_create_ctx(
+    backend: Backend,
+    cipher: _AEADTypes,
     key: bytes,
 ):
     ctx = backend._lib.EVP_CIPHER_CTX_new()
     backend.openssl_assert(ctx != backend._ffi.NULL)
     ctx = backend._ffi.gc(ctx, backend._lib.EVP_CIPHER_CTX_free)
-    cipher_name = _aead_cipher_name(cipher)
+    cipher_name = _evp_cipher_cipher_name(cipher)
     evp_cipher = _evp_cipher(cipher_name, backend)
     key_ptr = backend._ffi.from_buffer(key)
     res = backend._lib.EVP_CipherInit_ex(
         ctx,
         evp_cipher,
         backend._ffi.NULL,
         key_ptr,
         backend._ffi.NULL,
         0,
     )
     backend.openssl_assert(res != 0)
     return ctx
 
 
-def _aead_setup(
-    backend: "Backend",
+def _evp_cipher_aead_setup(
+    backend: Backend,
     cipher_name: bytes,
     key: bytes,
     nonce: bytes,
     tag: typing.Optional[bytes],
     tag_len: int,
     operation: int,
 ):
@@ -112,18 +314,21 @@
         backend._lib.EVP_CTRL_AEAD_SET_IVLEN,
         len(nonce),
         backend._ffi.NULL,
     )
     backend.openssl_assert(res != 0)
     if operation == _DECRYPT:
         assert tag is not None
-        _set_tag(backend, ctx, tag)
+        _evp_cipher_set_tag(backend, ctx, tag)
     elif cipher_name.endswith(b"-ccm"):
         res = backend._lib.EVP_CIPHER_CTX_ctrl(
-            ctx, backend._lib.EVP_CTRL_AEAD_SET_TAG, tag_len, backend._ffi.NULL
+            ctx,
+            backend._lib.EVP_CTRL_AEAD_SET_TAG,
+            tag_len,
+            backend._ffi.NULL,
         )
         backend.openssl_assert(res != 0)
 
     nonce_ptr = backend._ffi.from_buffer(nonce)
     key_ptr = backend._ffi.from_buffer(key)
     res = backend._lib.EVP_CipherInit_ex(
         ctx,
@@ -133,97 +338,102 @@
         nonce_ptr,
         int(operation == _ENCRYPT),
     )
     backend.openssl_assert(res != 0)
     return ctx
 
 
-def _set_tag(backend, ctx, tag: bytes) -> None:
+def _evp_cipher_set_tag(backend, ctx, tag: bytes) -> None:
     tag_ptr = backend._ffi.from_buffer(tag)
     res = backend._lib.EVP_CIPHER_CTX_ctrl(
         ctx, backend._lib.EVP_CTRL_AEAD_SET_TAG, len(tag), tag_ptr
     )
     backend.openssl_assert(res != 0)
 
 
-def _set_nonce_operation(backend, ctx, nonce: bytes, operation: int) -> None:
+def _evp_cipher_set_nonce_operation(
+    backend, ctx, nonce: bytes, operation: int
+) -> None:
     nonce_ptr = backend._ffi.from_buffer(nonce)
     res = backend._lib.EVP_CipherInit_ex(
         ctx,
         backend._ffi.NULL,
         backend._ffi.NULL,
         backend._ffi.NULL,
         nonce_ptr,
         int(operation == _ENCRYPT),
     )
     backend.openssl_assert(res != 0)
 
 
-def _set_length(backend: "Backend", ctx, data_len: int) -> None:
+def _evp_cipher_set_length(backend: Backend, ctx, data_len: int) -> None:
     intptr = backend._ffi.new("int *")
     res = backend._lib.EVP_CipherUpdate(
         ctx, backend._ffi.NULL, intptr, backend._ffi.NULL, data_len
     )
     backend.openssl_assert(res != 0)
 
 
-def _process_aad(backend: "Backend", ctx, associated_data: bytes) -> None:
+def _evp_cipher_process_aad(
+    backend: Backend, ctx, associated_data: bytes
+) -> None:
     outlen = backend._ffi.new("int *")
     a_data_ptr = backend._ffi.from_buffer(associated_data)
     res = backend._lib.EVP_CipherUpdate(
         ctx, backend._ffi.NULL, outlen, a_data_ptr, len(associated_data)
     )
     backend.openssl_assert(res != 0)
 
 
-def _process_data(backend: "Backend", ctx, data: bytes) -> bytes:
+def _evp_cipher_process_data(backend: Backend, ctx, data: bytes) -> bytes:
     outlen = backend._ffi.new("int *")
     buf = backend._ffi.new("unsigned char[]", len(data))
     data_ptr = backend._ffi.from_buffer(data)
     res = backend._lib.EVP_CipherUpdate(ctx, buf, outlen, data_ptr, len(data))
     if res == 0:
         # AES SIV can error here if the data is invalid on decrypt
         backend._consume_errors()
         raise InvalidTag
     return backend._ffi.buffer(buf, outlen[0])[:]
 
 
-def _encrypt(
-    backend: "Backend",
-    cipher: "_AEADTypes",
+def _evp_cipher_encrypt(
+    backend: Backend,
+    cipher: _AEADTypes,
     nonce: bytes,
     data: bytes,
     associated_data: typing.List[bytes],
     tag_length: int,
     ctx: typing.Any = None,
 ) -> bytes:
     from cryptography.hazmat.primitives.ciphers.aead import AESCCM, AESSIV
 
     if ctx is None:
-        cipher_name = _aead_cipher_name(cipher)
-        ctx = _aead_setup(
+        cipher_name = _evp_cipher_cipher_name(cipher)
+        ctx = _evp_cipher_aead_setup(
             backend,
             cipher_name,
             cipher._key,
             nonce,
             None,
             tag_length,
             _ENCRYPT,
         )
     else:
-        _set_nonce_operation(backend, ctx, nonce, _ENCRYPT)
+        _evp_cipher_set_nonce_operation(backend, ctx, nonce, _ENCRYPT)
 
-    # CCM requires us to pass the length of the data before processing anything
+    # CCM requires us to pass the length of the data before processing
+    # anything.
     # However calling this with any other AEAD results in an error
     if isinstance(cipher, AESCCM):
-        _set_length(backend, ctx, len(data))
+        _evp_cipher_set_length(backend, ctx, len(data))
 
     for ad in associated_data:
-        _process_aad(backend, ctx, ad)
-    processed_data = _process_data(backend, ctx, data)
+        _evp_cipher_process_aad(backend, ctx, ad)
+    processed_data = _evp_cipher_process_data(backend, ctx, data)
     outlen = backend._ffi.new("int *")
     # All AEADs we support besides OCB are streaming so they return nothing
     # in finalization. OCB can return up to (16 byte block - 1) bytes so
     # we need a buffer here too.
     buf = backend._ffi.new("unsigned char[]", 16)
     res = backend._lib.EVP_CipherFinal_ex(ctx, buf, outlen)
     backend.openssl_assert(res != 0)
@@ -232,76 +442,83 @@
     res = backend._lib.EVP_CIPHER_CTX_ctrl(
         ctx, backend._lib.EVP_CTRL_AEAD_GET_TAG, tag_length, tag_buf
     )
     backend.openssl_assert(res != 0)
     tag = backend._ffi.buffer(tag_buf)[:]
 
     if isinstance(cipher, AESSIV):
-        # RFC 5297 defines the output as IV || C, where the tag we generate is
-        # the "IV" and C is the ciphertext. This is the opposite of our
+        # RFC 5297 defines the output as IV || C, where the tag we generate
+        # is the "IV" and C is the ciphertext. This is the opposite of our
         # other AEADs, which are Ciphertext || Tag
         backend.openssl_assert(len(tag) == 16)
         return tag + processed_data
     else:
         return processed_data + tag
 
 
-def _decrypt(
-    backend: "Backend",
-    cipher: "_AEADTypes",
+def _evp_cipher_decrypt(
+    backend: Backend,
+    cipher: _AEADTypes,
     nonce: bytes,
     data: bytes,
     associated_data: typing.List[bytes],
     tag_length: int,
     ctx: typing.Any = None,
 ) -> bytes:
     from cryptography.hazmat.primitives.ciphers.aead import AESCCM, AESSIV
 
     if len(data) < tag_length:
         raise InvalidTag
 
     if isinstance(cipher, AESSIV):
-        # RFC 5297 defines the output as IV || C, where the tag we generate is
-        # the "IV" and C is the ciphertext. This is the opposite of our
+        # RFC 5297 defines the output as IV || C, where the tag we generate
+        # is the "IV" and C is the ciphertext. This is the opposite of our
         # other AEADs, which are Ciphertext || Tag
         tag = data[:tag_length]
         data = data[tag_length:]
     else:
         tag = data[-tag_length:]
         data = data[:-tag_length]
     if ctx is None:
-        cipher_name = _aead_cipher_name(cipher)
-        ctx = _aead_setup(
-            backend, cipher_name, cipher._key, nonce, tag, tag_length, _DECRYPT
+        cipher_name = _evp_cipher_cipher_name(cipher)
+        ctx = _evp_cipher_aead_setup(
+            backend,
+            cipher_name,
+            cipher._key,
+            nonce,
+            tag,
+            tag_length,
+            _DECRYPT,
         )
     else:
-        _set_nonce_operation(backend, ctx, nonce, _DECRYPT)
-        _set_tag(backend, ctx, tag)
+        _evp_cipher_set_nonce_operation(backend, ctx, nonce, _DECRYPT)
+        _evp_cipher_set_tag(backend, ctx, tag)
 
-    # CCM requires us to pass the length of the data before processing anything
+    # CCM requires us to pass the length of the data before processing
+    # anything.
     # However calling this with any other AEAD results in an error
     if isinstance(cipher, AESCCM):
-        _set_length(backend, ctx, len(data))
+        _evp_cipher_set_length(backend, ctx, len(data))
 
     for ad in associated_data:
-        _process_aad(backend, ctx, ad)
+        _evp_cipher_process_aad(backend, ctx, ad)
     # CCM has a different error path if the tag doesn't match. Errors are
     # raised in Update and Final is irrelevant.
     if isinstance(cipher, AESCCM):
         outlen = backend._ffi.new("int *")
         buf = backend._ffi.new("unsigned char[]", len(data))
         d_ptr = backend._ffi.from_buffer(data)
         res = backend._lib.EVP_CipherUpdate(ctx, buf, outlen, d_ptr, len(data))
         if res != 1:
             backend._consume_errors()
             raise InvalidTag
 
         processed_data = backend._ffi.buffer(buf, outlen[0])[:]
     else:
-        processed_data = _process_data(backend, ctx, data)
+        processed_data = _evp_cipher_process_data(backend, ctx, data)
         outlen = backend._ffi.new("int *")
         # OCB can return up to 15 bytes (16 byte block - 1) in finalization
         buf = backend._ffi.new("unsigned char[]", 16)
         res = backend._lib.EVP_CipherFinal_ex(ctx, buf, outlen)
         processed_data += backend._ffi.buffer(buf, outlen[0])[:]
         if res == 0:
             backend._consume_errors()
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/backend.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,32 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import collections
 import contextlib
 import itertools
 import typing
-import warnings
 from contextlib import contextmanager
 
 from cryptography import utils, x509
 from cryptography.exceptions import UnsupportedAlgorithm, _Reasons
 from cryptography.hazmat.backends.openssl import aead
 from cryptography.hazmat.backends.openssl.ciphers import _CipherContext
 from cryptography.hazmat.backends.openssl.cmac import _CMACContext
-from cryptography.hazmat.backends.openssl.dh import (
-    _dh_params_dup,
-    _DHParameters,
-    _DHPrivateKey,
-    _DHPublicKey,
-)
-from cryptography.hazmat.backends.openssl.dsa import (
-    _DSAParameters,
-    _DSAPrivateKey,
-    _DSAPublicKey,
-)
 from cryptography.hazmat.backends.openssl.ec import (
     _EllipticCurvePrivateKey,
     _EllipticCurvePublicKey,
 )
-from cryptography.hazmat.backends.openssl.ed448 import (
-    _ED448_KEY_SIZE,
-    _Ed448PrivateKey,
-    _Ed448PublicKey,
-)
-from cryptography.hazmat.backends.openssl.ed25519 import (
-    _Ed25519PrivateKey,
-    _Ed25519PublicKey,
-)
-from cryptography.hazmat.backends.openssl.hashes import _HashContext
-from cryptography.hazmat.backends.openssl.hmac import _HMACContext
-from cryptography.hazmat.backends.openssl.poly1305 import (
-    _POLY1305_KEY_SIZE,
-    _Poly1305Context,
-)
 from cryptography.hazmat.backends.openssl.rsa import (
     _RSAPrivateKey,
     _RSAPublicKey,
 )
-from cryptography.hazmat.backends.openssl.x448 import (
-    _X448PrivateKey,
-    _X448PublicKey,
-)
 from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 from cryptography.hazmat.bindings.openssl import binding
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives._asymmetric import AsymmetricPadding
 from cryptography.hazmat.primitives.asymmetric import (
     dh,
     dsa,
@@ -102,15 +72,14 @@
     CTR,
     ECB,
     GCM,
     OFB,
     XTS,
     Mode,
 )
-from cryptography.hazmat.primitives.kdf import scrypt
 from cryptography.hazmat.primitives.serialization import ssh
 from cryptography.hazmat.primitives.serialization.pkcs12 import (
     PBES,
     PKCS12Certificate,
     PKCS12KeyAndCertificates,
     PKCS12PrivateKeyTypes,
     _PKCS12CATypes,
@@ -174,28 +143,21 @@
     _fips_dh_min_key_size = 2048
     _fips_dh_min_modulus = 1 << _fips_dh_min_key_size
 
     def __init__(self) -> None:
         self._binding = binding.Binding()
         self._ffi = self._binding.ffi
         self._lib = self._binding.lib
-        self._fips_enabled = self._is_fips_enabled()
+        self._fips_enabled = rust_openssl.is_fips_enabled()
 
         self._cipher_registry: typing.Dict[
             typing.Tuple[typing.Type[CipherAlgorithm], typing.Type[Mode]],
             typing.Callable,
         ] = {}
         self._register_default_ciphers()
-        if self._fips_enabled and self._lib.CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE:
-            warnings.warn(
-                "OpenSSL FIPS mode is enabled. Can't enable DRBG fork safety.",
-                UserWarning,
-            )
-        else:
-            self.activate_osrandom_engine()
         self._dh_types = [self._lib.EVP_PKEY_DH]
         if self._lib.Cryptography_HAS_EVP_PKEY_DHX:
             self._dh_types.append(self._lib.EVP_PKEY_DHX)
 
     def __repr__(self) -> str:
         return "<OpenSSLBackend(version: {}, FIPS: {}, Legacy: {})>".format(
             self.openssl_version_text(),
@@ -206,87 +168,20 @@
     def openssl_assert(
         self,
         ok: bool,
         errors: typing.Optional[typing.List[rust_openssl.OpenSSLError]] = None,
     ) -> None:
         return binding._openssl_assert(self._lib, ok, errors=errors)
 
-    def _is_fips_enabled(self) -> bool:
-        if self._lib.Cryptography_HAS_300_FIPS:
-            mode = self._lib.EVP_default_properties_is_fips_enabled(
-                self._ffi.NULL
-            )
-        else:
-            mode = self._lib.FIPS_mode()
-
-        if mode == 0:
-            # OpenSSL without FIPS pushes an error on the error stack
-            self._lib.ERR_clear_error()
-        return bool(mode)
-
     def _enable_fips(self) -> None:
         # This function enables FIPS mode for OpenSSL 3.0.0 on installs that
         # have the FIPS provider installed properly.
         self._binding._enable_fips()
-        assert self._is_fips_enabled()
-        self._fips_enabled = self._is_fips_enabled()
-
-    def activate_builtin_random(self) -> None:
-        if self._lib.CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE:
-            # Obtain a new structural reference.
-            e = self._lib.ENGINE_get_default_RAND()
-            if e != self._ffi.NULL:
-                self._lib.ENGINE_unregister_RAND(e)
-                # Reset the RNG to use the built-in.
-                res = self._lib.RAND_set_rand_method(self._ffi.NULL)
-                self.openssl_assert(res == 1)
-                # decrement the structural reference from get_default_RAND
-                res = self._lib.ENGINE_finish(e)
-                self.openssl_assert(res == 1)
-
-    @contextlib.contextmanager
-    def _get_osurandom_engine(self):
-        # Fetches an engine by id and returns it. This creates a structural
-        # reference.
-        e = self._lib.ENGINE_by_id(self._lib.Cryptography_osrandom_engine_id)
-        self.openssl_assert(e != self._ffi.NULL)
-        # Initialize the engine for use. This adds a functional reference.
-        res = self._lib.ENGINE_init(e)
-        self.openssl_assert(res == 1)
-
-        try:
-            yield e
-        finally:
-            # Decrement the structural ref incremented by ENGINE_by_id.
-            res = self._lib.ENGINE_free(e)
-            self.openssl_assert(res == 1)
-            # Decrement the functional ref incremented by ENGINE_init.
-            res = self._lib.ENGINE_finish(e)
-            self.openssl_assert(res == 1)
-
-    def activate_osrandom_engine(self) -> None:
-        if self._lib.CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE:
-            # Unregister and free the current engine.
-            self.activate_builtin_random()
-            with self._get_osurandom_engine() as e:
-                # Set the engine as the default RAND provider.
-                res = self._lib.ENGINE_set_default_RAND(e)
-                self.openssl_assert(res == 1)
-            # Reset the RNG to use the engine
-            res = self._lib.RAND_set_rand_method(self._ffi.NULL)
-            self.openssl_assert(res == 1)
-
-    def osrandom_engine_implementation(self) -> str:
-        buf = self._ffi.new("char[]", 64)
-        with self._get_osurandom_engine() as e:
-            res = self._lib.ENGINE_ctrl_cmd(
-                e, b"get_implementation", len(buf), buf, self._ffi.NULL, 0
-            )
-            self.openssl_assert(res > 0)
-        return self._ffi.string(buf).decode("ascii")
+        assert rust_openssl.is_fips_enabled()
+        self._fips_enabled = rust_openssl.is_fips_enabled()
 
     def openssl_version_text(self) -> str:
         """
         Friendly string name of the loaded OpenSSL library. This is not
         necessarily the same version as it was compiled against.
 
         Example: OpenSSL 1.1.1d  10 Sep 2019
@@ -294,19 +189,14 @@
         return self._ffi.string(
             self._lib.OpenSSL_version(self._lib.OPENSSL_VERSION)
         ).decode("ascii")
 
     def openssl_version_number(self) -> int:
         return self._lib.OpenSSL_version_num()
 
-    def create_hmac_ctx(
-        self, key: bytes, algorithm: hashes.HashAlgorithm
-    ) -> _HMACContext:
-        return _HMACContext(self, key, algorithm)
-
     def _evp_md_from_algorithm(self, algorithm: hashes.HashAlgorithm):
         if algorithm.name == "blake2b" or algorithm.name == "blake2s":
             alg = "{}{}".format(
                 algorithm.name, algorithm.digest_size * 8
             ).encode("ascii")
         else:
             alg = algorithm.name.encode("ascii")
@@ -344,19 +234,14 @@
     def hmac_supported(self, algorithm: hashes.HashAlgorithm) -> bool:
         # FIPS mode still allows SHA1 for HMAC
         if self._fips_enabled and isinstance(algorithm, hashes.SHA1):
             return True
 
         return self.hash_supported(algorithm)
 
-    def create_hash_ctx(
-        self, algorithm: hashes.HashAlgorithm
-    ) -> hashes.HashContext:
-        return _HashContext(self, algorithm)
-
     def cipher_supported(self, cipher: CipherAlgorithm, mode: Mode) -> bool:
         if self._fips_enabled:
             # FIPS mode requires AES. TripleDES is disallowed/deprecated in
             # FIPS 140-3.
             if not isinstance(cipher, self._fips_ciphers):
                 return False
 
@@ -453,38 +338,14 @@
         self, cipher: CipherAlgorithm, mode: Mode
     ) -> _CipherContext:
         return _CipherContext(self, cipher, mode, _CipherContext._DECRYPT)
 
     def pbkdf2_hmac_supported(self, algorithm: hashes.HashAlgorithm) -> bool:
         return self.hmac_supported(algorithm)
 
-    def derive_pbkdf2_hmac(
-        self,
-        algorithm: hashes.HashAlgorithm,
-        length: int,
-        salt: bytes,
-        iterations: int,
-        key_material: bytes,
-    ) -> bytes:
-        buf = self._ffi.new("unsigned char[]", length)
-        evp_md = self._evp_md_non_null_from_algorithm(algorithm)
-        key_material_ptr = self._ffi.from_buffer(key_material)
-        res = self._lib.PKCS5_PBKDF2_HMAC(
-            key_material_ptr,
-            len(key_material),
-            salt,
-            len(salt),
-            iterations,
-            evp_md,
-            length,
-            buf,
-        )
-        self.openssl_assert(res == 1)
-        return self._ffi.buffer(buf)[:]
-
     def _consume_errors(self) -> typing.List[rust_openssl.OpenSSLError]:
         return rust_openssl.capture_error_stack()
 
     def _bn_to_int(self, bn) -> int:
         assert bn != self._ffi.NULL
         self.openssl_assert(not self._lib.BN_is_negative(bn))
 
@@ -492,28 +353,23 @@
         bin_ptr = self._ffi.new("unsigned char[]", bn_num_bytes)
         bin_len = self._lib.BN_bn2bin(bn, bin_ptr)
         # A zero length means the BN has value 0
         self.openssl_assert(bin_len >= 0)
         val = int.from_bytes(self._ffi.buffer(bin_ptr)[:bin_len], "big")
         return val
 
-    def _int_to_bn(self, num: int, bn=None):
+    def _int_to_bn(self, num: int):
         """
         Converts a python integer to a BIGNUM. The returned BIGNUM will not
         be garbage collected (to support adding them to structs that take
         ownership of the object). Be sure to register it for GC if it will
         be discarded after use.
         """
-        assert bn is None or bn != self._ffi.NULL
-
-        if bn is None:
-            bn = self._ffi.NULL
-
         binary = num.to_bytes(int(num.bit_length() / 8.0 + 1), "big")
-        bn_ptr = self._lib.BN_bin2bn(binary, len(binary), bn)
+        bn_ptr = self._lib.BN_bin2bn(binary, len(binary), self._ffi.NULL)
         self.openssl_assert(bn_ptr != self._ffi.NULL)
         return bn_ptr
 
     def generate_rsa_private_key(
         self, public_exponent: int, key_size: int
     ) -> rsa.RSAPrivateKey:
         rsa._verify_rsa_parameters(public_exponent, key_size)
@@ -686,41 +542,45 @@
             self.openssl_assert(res == 1)
             return self.load_der_private_key(
                 self._read_mem_bio(bio),
                 password=None,
                 unsafe_skip_rsa_key_validation=unsafe_skip_rsa_key_validation,
             )
         elif key_type == self._lib.EVP_PKEY_DSA:
-            dsa_cdata = self._lib.EVP_PKEY_get1_DSA(evp_pkey)
-            self.openssl_assert(dsa_cdata != self._ffi.NULL)
-            dsa_cdata = self._ffi.gc(dsa_cdata, self._lib.DSA_free)
-            return _DSAPrivateKey(self, dsa_cdata, evp_pkey)
+            return rust_openssl.dsa.private_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == self._lib.EVP_PKEY_EC:
             ec_cdata = self._lib.EVP_PKEY_get1_EC_KEY(evp_pkey)
             self.openssl_assert(ec_cdata != self._ffi.NULL)
             ec_cdata = self._ffi.gc(ec_cdata, self._lib.EC_KEY_free)
             return _EllipticCurvePrivateKey(self, ec_cdata, evp_pkey)
         elif key_type in self._dh_types:
-            dh_cdata = self._lib.EVP_PKEY_get1_DH(evp_pkey)
-            self.openssl_assert(dh_cdata != self._ffi.NULL)
-            dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-            return _DHPrivateKey(self, dh_cdata, evp_pkey)
+            return rust_openssl.dh.private_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == getattr(self._lib, "EVP_PKEY_ED25519", None):
             # EVP_PKEY_ED25519 is not present in CRYPTOGRAPHY_IS_LIBRESSL
-            return _Ed25519PrivateKey(self, evp_pkey)
+            return rust_openssl.ed25519.private_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == getattr(self._lib, "EVP_PKEY_X448", None):
             # EVP_PKEY_X448 is not present in CRYPTOGRAPHY_IS_LIBRESSL
-            return _X448PrivateKey(self, evp_pkey)
+            return rust_openssl.x448.private_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == self._lib.EVP_PKEY_X25519:
             return rust_openssl.x25519.private_key_from_ptr(
                 int(self._ffi.cast("uintptr_t", evp_pkey))
             )
         elif key_type == getattr(self._lib, "EVP_PKEY_ED448", None):
             # EVP_PKEY_ED448 is not present in CRYPTOGRAPHY_IS_LIBRESSL
-            return _Ed448PrivateKey(self, evp_pkey)
+            return rust_openssl.ed448.private_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         else:
             raise UnsupportedAlgorithm("Unsupported key type.")
 
     def _evp_pkey_to_public_key(self, evp_pkey) -> PublicKeyTypes:
         """
         Return the appropriate type of PublicKey given an evp_pkey cdata
         pointer.
@@ -743,43 +603,47 @@
             self.openssl_assert(rsa_cdata != self._ffi.NULL)
             rsa_cdata = self._ffi.gc(rsa_cdata, self._lib.RSA_free)
             bio = self._create_mem_bio_gc()
             res = self._lib.i2d_RSAPublicKey_bio(bio, rsa_cdata)
             self.openssl_assert(res == 1)
             return self.load_der_public_key(self._read_mem_bio(bio))
         elif key_type == self._lib.EVP_PKEY_DSA:
-            dsa_cdata = self._lib.EVP_PKEY_get1_DSA(evp_pkey)
-            self.openssl_assert(dsa_cdata != self._ffi.NULL)
-            dsa_cdata = self._ffi.gc(dsa_cdata, self._lib.DSA_free)
-            return _DSAPublicKey(self, dsa_cdata, evp_pkey)
+            return rust_openssl.dsa.public_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == self._lib.EVP_PKEY_EC:
             ec_cdata = self._lib.EVP_PKEY_get1_EC_KEY(evp_pkey)
             if ec_cdata == self._ffi.NULL:
                 errors = self._consume_errors()
                 raise ValueError("Unable to load EC key", errors)
             ec_cdata = self._ffi.gc(ec_cdata, self._lib.EC_KEY_free)
             return _EllipticCurvePublicKey(self, ec_cdata, evp_pkey)
         elif key_type in self._dh_types:
-            dh_cdata = self._lib.EVP_PKEY_get1_DH(evp_pkey)
-            self.openssl_assert(dh_cdata != self._ffi.NULL)
-            dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-            return _DHPublicKey(self, dh_cdata, evp_pkey)
+            return rust_openssl.dh.public_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == getattr(self._lib, "EVP_PKEY_ED25519", None):
             # EVP_PKEY_ED25519 is not present in CRYPTOGRAPHY_IS_LIBRESSL
-            return _Ed25519PublicKey(self, evp_pkey)
+            return rust_openssl.ed25519.public_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == getattr(self._lib, "EVP_PKEY_X448", None):
             # EVP_PKEY_X448 is not present in CRYPTOGRAPHY_IS_LIBRESSL
-            return _X448PublicKey(self, evp_pkey)
+            return rust_openssl.x448.public_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         elif key_type == self._lib.EVP_PKEY_X25519:
             return rust_openssl.x25519.public_key_from_ptr(
                 int(self._ffi.cast("uintptr_t", evp_pkey))
             )
         elif key_type == getattr(self._lib, "EVP_PKEY_ED448", None):
             # EVP_PKEY_ED448 is not present in CRYPTOGRAPHY_IS_LIBRESSL
-            return _Ed448PublicKey(self, evp_pkey)
+            return rust_openssl.ed448.public_key_from_ptr(
+                int(self._ffi.cast("uintptr_t", evp_pkey))
+            )
         else:
             raise UnsupportedAlgorithm("Unsupported key type.")
 
     def _oaep_hash_supported(self, algorithm: hashes.HashAlgorithm) -> bool:
         if self._fips_enabled and isinstance(algorithm, hashes.SHA1):
             return False
 
@@ -821,123 +685,49 @@
 
     def generate_dsa_parameters(self, key_size: int) -> dsa.DSAParameters:
         if key_size not in (1024, 2048, 3072, 4096):
             raise ValueError(
                 "Key size must be 1024, 2048, 3072, or 4096 bits."
             )
 
-        ctx = self._lib.DSA_new()
-        self.openssl_assert(ctx != self._ffi.NULL)
-        ctx = self._ffi.gc(ctx, self._lib.DSA_free)
-
-        res = self._lib.DSA_generate_parameters_ex(
-            ctx,
-            key_size,
-            self._ffi.NULL,
-            0,
-            self._ffi.NULL,
-            self._ffi.NULL,
-            self._ffi.NULL,
-        )
-
-        self.openssl_assert(res == 1)
-
-        return _DSAParameters(self, ctx)
+        return rust_openssl.dsa.generate_parameters(key_size)
 
     def generate_dsa_private_key(
         self, parameters: dsa.DSAParameters
     ) -> dsa.DSAPrivateKey:
-        ctx = self._lib.DSAparams_dup(
-            parameters._dsa_cdata  # type: ignore[attr-defined]
-        )
-        self.openssl_assert(ctx != self._ffi.NULL)
-        ctx = self._ffi.gc(ctx, self._lib.DSA_free)
-        self._lib.DSA_generate_key(ctx)
-        evp_pkey = self._dsa_cdata_to_evp_pkey(ctx)
-
-        return _DSAPrivateKey(self, ctx, evp_pkey)
+        return parameters.generate_private_key()
 
     def generate_dsa_private_key_and_parameters(
         self, key_size: int
     ) -> dsa.DSAPrivateKey:
         parameters = self.generate_dsa_parameters(key_size)
         return self.generate_dsa_private_key(parameters)
 
-    def _dsa_cdata_set_values(
-        self, dsa_cdata, p, q, g, pub_key, priv_key
-    ) -> None:
-        res = self._lib.DSA_set0_pqg(dsa_cdata, p, q, g)
-        self.openssl_assert(res == 1)
-        res = self._lib.DSA_set0_key(dsa_cdata, pub_key, priv_key)
-        self.openssl_assert(res == 1)
-
     def load_dsa_private_numbers(
         self, numbers: dsa.DSAPrivateNumbers
     ) -> dsa.DSAPrivateKey:
         dsa._check_dsa_private_numbers(numbers)
-        parameter_numbers = numbers.public_numbers.parameter_numbers
-
-        dsa_cdata = self._lib.DSA_new()
-        self.openssl_assert(dsa_cdata != self._ffi.NULL)
-        dsa_cdata = self._ffi.gc(dsa_cdata, self._lib.DSA_free)
-
-        p = self._int_to_bn(parameter_numbers.p)
-        q = self._int_to_bn(parameter_numbers.q)
-        g = self._int_to_bn(parameter_numbers.g)
-        pub_key = self._int_to_bn(numbers.public_numbers.y)
-        priv_key = self._int_to_bn(numbers.x)
-        self._dsa_cdata_set_values(dsa_cdata, p, q, g, pub_key, priv_key)
-
-        evp_pkey = self._dsa_cdata_to_evp_pkey(dsa_cdata)
-
-        return _DSAPrivateKey(self, dsa_cdata, evp_pkey)
+        return rust_openssl.dsa.from_private_numbers(numbers)
 
     def load_dsa_public_numbers(
         self, numbers: dsa.DSAPublicNumbers
     ) -> dsa.DSAPublicKey:
         dsa._check_dsa_parameters(numbers.parameter_numbers)
-        dsa_cdata = self._lib.DSA_new()
-        self.openssl_assert(dsa_cdata != self._ffi.NULL)
-        dsa_cdata = self._ffi.gc(dsa_cdata, self._lib.DSA_free)
-
-        p = self._int_to_bn(numbers.parameter_numbers.p)
-        q = self._int_to_bn(numbers.parameter_numbers.q)
-        g = self._int_to_bn(numbers.parameter_numbers.g)
-        pub_key = self._int_to_bn(numbers.y)
-        priv_key = self._ffi.NULL
-        self._dsa_cdata_set_values(dsa_cdata, p, q, g, pub_key, priv_key)
-
-        evp_pkey = self._dsa_cdata_to_evp_pkey(dsa_cdata)
-
-        return _DSAPublicKey(self, dsa_cdata, evp_pkey)
+        return rust_openssl.dsa.from_public_numbers(numbers)
 
     def load_dsa_parameter_numbers(
         self, numbers: dsa.DSAParameterNumbers
     ) -> dsa.DSAParameters:
         dsa._check_dsa_parameters(numbers)
-        dsa_cdata = self._lib.DSA_new()
-        self.openssl_assert(dsa_cdata != self._ffi.NULL)
-        dsa_cdata = self._ffi.gc(dsa_cdata, self._lib.DSA_free)
-
-        p = self._int_to_bn(numbers.p)
-        q = self._int_to_bn(numbers.q)
-        g = self._int_to_bn(numbers.g)
-        res = self._lib.DSA_set0_pqg(dsa_cdata, p, q, g)
-        self.openssl_assert(res == 1)
-
-        return _DSAParameters(self, dsa_cdata)
-
-    def _dsa_cdata_to_evp_pkey(self, dsa_cdata):
-        evp_pkey = self._create_evp_pkey_gc()
-        res = self._lib.EVP_PKEY_set1_DSA(evp_pkey, dsa_cdata)
-        self.openssl_assert(res == 1)
-        return evp_pkey
+        return rust_openssl.dsa.from_parameter_numbers(numbers)
 
     def dsa_supported(self) -> bool:
-        return not self._fips_enabled
+        return (
+            not self._lib.CRYPTOGRAPHY_IS_BORINGSSL and not self._fips_enabled
+        )
 
     def dsa_hash_supported(self, algorithm: hashes.HashAlgorithm) -> bool:
         if not self.dsa_supported():
             return False
         return self.signature_hash_supported(algorithm)
 
     def cmac_algorithm_supported(self, algorithm) -> bool:
@@ -1000,24 +790,15 @@
                 rsa_cdata = self._ffi.gc(rsa_cdata, self._lib.RSA_free)
                 evp_pkey = self._rsa_cdata_to_evp_pkey(rsa_cdata)
                 return _RSAPublicKey(self, rsa_cdata, evp_pkey)
             else:
                 self._handle_key_loading_error()
 
     def load_pem_parameters(self, data: bytes) -> dh.DHParameters:
-        mem_bio = self._bytes_to_bio(data)
-        # only DH is supported currently
-        dh_cdata = self._lib.PEM_read_bio_DHparams(
-            mem_bio.bio, self._ffi.NULL, self._ffi.NULL, self._ffi.NULL
-        )
-        if dh_cdata != self._ffi.NULL:
-            dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-            return _DHParameters(self, dh_cdata)
-        else:
-            self._handle_key_loading_error()
+        return rust_openssl.dh.from_pem_parameters(data)
 
     def load_der_private_key(
         self,
         data: bytes,
         password: typing.Optional[bytes],
         unsafe_skip_rsa_key_validation: bool,
     ) -> PrivateKeyTypes:
@@ -1075,30 +856,15 @@
                 rsa_cdata = self._ffi.gc(rsa_cdata, self._lib.RSA_free)
                 evp_pkey = self._rsa_cdata_to_evp_pkey(rsa_cdata)
                 return _RSAPublicKey(self, rsa_cdata, evp_pkey)
             else:
                 self._handle_key_loading_error()
 
     def load_der_parameters(self, data: bytes) -> dh.DHParameters:
-        mem_bio = self._bytes_to_bio(data)
-        dh_cdata = self._lib.d2i_DHparams_bio(mem_bio.bio, self._ffi.NULL)
-        if dh_cdata != self._ffi.NULL:
-            dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-            return _DHParameters(self, dh_cdata)
-        elif self._lib.Cryptography_HAS_EVP_PKEY_DHX:
-            # We check to see if the is dhx.
-            self._consume_errors()
-            res = self._lib.BIO_reset(mem_bio.bio)
-            self.openssl_assert(res == 1)
-            dh_cdata = self._lib.d2i_DHxparams_bio(mem_bio.bio, self._ffi.NULL)
-            if dh_cdata != self._ffi.NULL:
-                dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-                return _DHParameters(self, dh_cdata)
-
-        self._handle_key_loading_error()
+        return rust_openssl.dh.from_der_parameters(data)
 
     def _cert2ossl(self, cert: x509.Certificate) -> typing.Any:
         data = cert.public_bytes(serialization.Encoding.DER)
         mem_bio = self._bytes_to_bio(data)
         x509 = self._lib.d2i_X509_bio(mem_bio.bio, self._ffi.NULL)
         self.openssl_assert(x509 != self._ffi.NULL)
         x509 = self._ffi.gc(x509, self._lib.X509_free)
@@ -1106,17 +872,28 @@
 
     def _ossl2cert(self, x509_ptr: typing.Any) -> x509.Certificate:
         bio = self._create_mem_bio_gc()
         res = self._lib.i2d_X509_bio(bio, x509_ptr)
         self.openssl_assert(res == 1)
         return x509.load_der_x509_certificate(self._read_mem_bio(bio))
 
-    def _check_keys_correspond(self, key1, key2) -> None:
-        if self._lib.EVP_PKEY_cmp(key1._evp_pkey, key2._evp_pkey) != 1:
-            raise ValueError("Keys do not correspond")
+    def _key2ossl(self, key: PKCS12PrivateKeyTypes) -> typing.Any:
+        data = key.private_bytes(
+            serialization.Encoding.DER,
+            serialization.PrivateFormat.PKCS8,
+            serialization.NoEncryption(),
+        )
+        mem_bio = self._bytes_to_bio(data)
+
+        evp_pkey = self._lib.d2i_PrivateKey_bio(
+            mem_bio.bio,
+            self._ffi.NULL,
+        )
+        self.openssl_assert(evp_pkey != self._ffi.NULL)
+        return self._ffi.gc(evp_pkey, self._lib.EVP_PKEY_free)
 
     def _load_key(
         self, openssl_read_func, data, password, unsafe_skip_rsa_key_validation
     ) -> PrivateKeyTypes:
         mem_bio = self._bytes_to_bio(data)
 
         userdata = self._ffi.new("CRYPTOGRAPHY_PASSWORD_DATA *")
@@ -1547,42 +1324,32 @@
                     "supported in FIPS mode."
                 )
             key_type = self._lib.EVP_PKEY_id(evp_pkey)
 
             if encoding is serialization.Encoding.PEM:
                 if key_type == self._lib.EVP_PKEY_RSA:
                     write_bio = self._lib.PEM_write_bio_RSAPrivateKey
-                elif key_type == self._lib.EVP_PKEY_DSA:
-                    write_bio = self._lib.PEM_write_bio_DSAPrivateKey
-                elif key_type == self._lib.EVP_PKEY_EC:
-                    write_bio = self._lib.PEM_write_bio_ECPrivateKey
                 else:
-                    raise ValueError(
-                        "Unsupported key type for TraditionalOpenSSL"
-                    )
+                    assert key_type == self._lib.EVP_PKEY_EC
+                    write_bio = self._lib.PEM_write_bio_ECPrivateKey
                 return self._private_key_bytes_via_bio(
                     write_bio, cdata, password
                 )
 
             if encoding is serialization.Encoding.DER:
                 if password:
                     raise ValueError(
                         "Encryption is not supported for DER encoded "
                         "traditional OpenSSL keys"
                     )
                 if key_type == self._lib.EVP_PKEY_RSA:
                     write_bio = self._lib.i2d_RSAPrivateKey_bio
-                elif key_type == self._lib.EVP_PKEY_EC:
-                    write_bio = self._lib.i2d_ECPrivateKey_bio
-                elif key_type == self._lib.EVP_PKEY_DSA:
-                    write_bio = self._lib.i2d_DSAPrivateKey_bio
                 else:
-                    raise ValueError(
-                        "Unsupported key type for TraditionalOpenSSL"
-                    )
+                    assert key_type == self._lib.EVP_PKEY_EC
+                    write_bio = self._lib.i2d_ECPrivateKey_bio
                 return self._bio_func_output(write_bio, cdata)
 
             raise ValueError("Unsupported encoding for TraditionalOpenSSL")
 
         # OpenSSH + PEM
         if format is serialization.PrivateFormat.OpenSSH:
             if encoding is serialization.Encoding.PEM:
@@ -1681,243 +1448,82 @@
 
     def dh_supported(self) -> bool:
         return not self._lib.CRYPTOGRAPHY_IS_BORINGSSL
 
     def generate_dh_parameters(
         self, generator: int, key_size: int
     ) -> dh.DHParameters:
-        if key_size < dh._MIN_MODULUS_SIZE:
-            raise ValueError(
-                "DH key_size must be at least {} bits".format(
-                    dh._MIN_MODULUS_SIZE
-                )
-            )
-
-        if generator not in (2, 5):
-            raise ValueError("DH generator must be 2 or 5")
-
-        dh_param_cdata = self._lib.DH_new()
-        self.openssl_assert(dh_param_cdata != self._ffi.NULL)
-        dh_param_cdata = self._ffi.gc(dh_param_cdata, self._lib.DH_free)
-
-        res = self._lib.DH_generate_parameters_ex(
-            dh_param_cdata, key_size, generator, self._ffi.NULL
-        )
-        if res != 1:
-            errors = self._consume_errors()
-            raise ValueError("Unable to generate DH parameters", errors)
-
-        return _DHParameters(self, dh_param_cdata)
-
-    def _dh_cdata_to_evp_pkey(self, dh_cdata):
-        evp_pkey = self._create_evp_pkey_gc()
-        res = self._lib.EVP_PKEY_set1_DH(evp_pkey, dh_cdata)
-        self.openssl_assert(res == 1)
-        return evp_pkey
+        return rust_openssl.dh.generate_parameters(generator, key_size)
 
     def generate_dh_private_key(
         self, parameters: dh.DHParameters
     ) -> dh.DHPrivateKey:
-        dh_key_cdata = _dh_params_dup(
-            parameters._dh_cdata, self  # type: ignore[attr-defined]
-        )
-
-        res = self._lib.DH_generate_key(dh_key_cdata)
-        self.openssl_assert(res == 1)
-
-        evp_pkey = self._dh_cdata_to_evp_pkey(dh_key_cdata)
-
-        return _DHPrivateKey(self, dh_key_cdata, evp_pkey)
+        return parameters.generate_private_key()
 
     def generate_dh_private_key_and_parameters(
         self, generator: int, key_size: int
     ) -> dh.DHPrivateKey:
         return self.generate_dh_private_key(
             self.generate_dh_parameters(generator, key_size)
         )
 
     def load_dh_private_numbers(
         self, numbers: dh.DHPrivateNumbers
     ) -> dh.DHPrivateKey:
-        parameter_numbers = numbers.public_numbers.parameter_numbers
-
-        dh_cdata = self._lib.DH_new()
-        self.openssl_assert(dh_cdata != self._ffi.NULL)
-        dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-
-        p = self._int_to_bn(parameter_numbers.p)
-        g = self._int_to_bn(parameter_numbers.g)
-
-        if parameter_numbers.q is not None:
-            q = self._int_to_bn(parameter_numbers.q)
-        else:
-            q = self._ffi.NULL
-
-        pub_key = self._int_to_bn(numbers.public_numbers.y)
-        priv_key = self._int_to_bn(numbers.x)
-
-        res = self._lib.DH_set0_pqg(dh_cdata, p, q, g)
-        self.openssl_assert(res == 1)
-
-        res = self._lib.DH_set0_key(dh_cdata, pub_key, priv_key)
-        self.openssl_assert(res == 1)
-
-        codes = self._ffi.new("int[]", 1)
-        res = self._lib.DH_check(dh_cdata, codes)
-        self.openssl_assert(res == 1)
-
-        # DH_check will return DH_NOT_SUITABLE_GENERATOR if p % 24 does not
-        # equal 11 when the generator is 2 (a quadratic nonresidue).
-        # We want to ignore that error because p % 24 == 23 is also fine.
-        # Specifically, g is then a quadratic residue. Within the context of
-        # Diffie-Hellman this means it can only generate half the possible
-        # values. That sounds bad, but quadratic nonresidues leak a bit of
-        # the key to the attacker in exchange for having the full key space
-        # available. See: https://crypto.stackexchange.com/questions/12961
-        if codes[0] != 0 and not (
-            parameter_numbers.g == 2
-            and codes[0] ^ self._lib.DH_NOT_SUITABLE_GENERATOR == 0
-        ):
-            raise ValueError("DH private numbers did not pass safety checks.")
-
-        evp_pkey = self._dh_cdata_to_evp_pkey(dh_cdata)
-
-        return _DHPrivateKey(self, dh_cdata, evp_pkey)
+        return rust_openssl.dh.from_private_numbers(numbers)
 
     def load_dh_public_numbers(
         self, numbers: dh.DHPublicNumbers
     ) -> dh.DHPublicKey:
-        dh_cdata = self._lib.DH_new()
-        self.openssl_assert(dh_cdata != self._ffi.NULL)
-        dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-
-        parameter_numbers = numbers.parameter_numbers
-
-        p = self._int_to_bn(parameter_numbers.p)
-        g = self._int_to_bn(parameter_numbers.g)
-
-        if parameter_numbers.q is not None:
-            q = self._int_to_bn(parameter_numbers.q)
-        else:
-            q = self._ffi.NULL
-
-        pub_key = self._int_to_bn(numbers.y)
-
-        res = self._lib.DH_set0_pqg(dh_cdata, p, q, g)
-        self.openssl_assert(res == 1)
-
-        res = self._lib.DH_set0_key(dh_cdata, pub_key, self._ffi.NULL)
-        self.openssl_assert(res == 1)
-
-        evp_pkey = self._dh_cdata_to_evp_pkey(dh_cdata)
-
-        return _DHPublicKey(self, dh_cdata, evp_pkey)
+        return rust_openssl.dh.from_public_numbers(numbers)
 
     def load_dh_parameter_numbers(
         self, numbers: dh.DHParameterNumbers
     ) -> dh.DHParameters:
-        dh_cdata = self._lib.DH_new()
-        self.openssl_assert(dh_cdata != self._ffi.NULL)
-        dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-
-        p = self._int_to_bn(numbers.p)
-        g = self._int_to_bn(numbers.g)
-
-        if numbers.q is not None:
-            q = self._int_to_bn(numbers.q)
-        else:
-            q = self._ffi.NULL
-
-        res = self._lib.DH_set0_pqg(dh_cdata, p, q, g)
-        self.openssl_assert(res == 1)
-
-        return _DHParameters(self, dh_cdata)
+        return rust_openssl.dh.from_parameter_numbers(numbers)
 
     def dh_parameters_supported(
         self, p: int, g: int, q: typing.Optional[int] = None
     ) -> bool:
-        dh_cdata = self._lib.DH_new()
-        self.openssl_assert(dh_cdata != self._ffi.NULL)
-        dh_cdata = self._ffi.gc(dh_cdata, self._lib.DH_free)
-
-        p = self._int_to_bn(p)
-        g = self._int_to_bn(g)
-
-        if q is not None:
-            q = self._int_to_bn(q)
+        try:
+            rust_openssl.dh.from_parameter_numbers(
+                dh.DHParameterNumbers(p=p, g=g, q=q)
+            )
+        except ValueError:
+            return False
         else:
-            q = self._ffi.NULL
-
-        res = self._lib.DH_set0_pqg(dh_cdata, p, q, g)
-        self.openssl_assert(res == 1)
-
-        codes = self._ffi.new("int[]", 1)
-        res = self._lib.DH_check(dh_cdata, codes)
-        self.openssl_assert(res == 1)
-
-        return codes[0] == 0
+            return True
 
     def dh_x942_serialization_supported(self) -> bool:
         return self._lib.Cryptography_HAS_EVP_PKEY_DHX == 1
 
     def x25519_load_public_bytes(self, data: bytes) -> x25519.X25519PublicKey:
         return rust_openssl.x25519.from_public_bytes(data)
 
     def x25519_load_private_bytes(
         self, data: bytes
     ) -> x25519.X25519PrivateKey:
         return rust_openssl.x25519.from_private_bytes(data)
 
-    def _evp_pkey_keygen_gc(self, nid):
-        evp_pkey_ctx = self._lib.EVP_PKEY_CTX_new_id(nid, self._ffi.NULL)
-        self.openssl_assert(evp_pkey_ctx != self._ffi.NULL)
-        evp_pkey_ctx = self._ffi.gc(evp_pkey_ctx, self._lib.EVP_PKEY_CTX_free)
-        res = self._lib.EVP_PKEY_keygen_init(evp_pkey_ctx)
-        self.openssl_assert(res == 1)
-        evp_ppkey = self._ffi.new("EVP_PKEY **")
-        res = self._lib.EVP_PKEY_keygen(evp_pkey_ctx, evp_ppkey)
-        self.openssl_assert(res == 1)
-        self.openssl_assert(evp_ppkey[0] != self._ffi.NULL)
-        evp_pkey = self._ffi.gc(evp_ppkey[0], self._lib.EVP_PKEY_free)
-        return evp_pkey
-
     def x25519_generate_key(self) -> x25519.X25519PrivateKey:
         return rust_openssl.x25519.generate_key()
 
     def x25519_supported(self) -> bool:
         if self._fips_enabled:
             return False
         return not self._lib.CRYPTOGRAPHY_LIBRESSL_LESS_THAN_370
 
     def x448_load_public_bytes(self, data: bytes) -> x448.X448PublicKey:
-        if len(data) != 56:
-            raise ValueError("An X448 public key is 56 bytes long")
-
-        evp_pkey = self._lib.EVP_PKEY_new_raw_public_key(
-            self._lib.NID_X448, self._ffi.NULL, data, len(data)
-        )
-        self.openssl_assert(evp_pkey != self._ffi.NULL)
-        evp_pkey = self._ffi.gc(evp_pkey, self._lib.EVP_PKEY_free)
-        return _X448PublicKey(self, evp_pkey)
+        return rust_openssl.x448.from_public_bytes(data)
 
     def x448_load_private_bytes(self, data: bytes) -> x448.X448PrivateKey:
-        if len(data) != 56:
-            raise ValueError("An X448 private key is 56 bytes long")
-
-        data_ptr = self._ffi.from_buffer(data)
-        evp_pkey = self._lib.EVP_PKEY_new_raw_private_key(
-            self._lib.NID_X448, self._ffi.NULL, data_ptr, len(data)
-        )
-        self.openssl_assert(evp_pkey != self._ffi.NULL)
-        evp_pkey = self._ffi.gc(evp_pkey, self._lib.EVP_PKEY_free)
-        return _X448PrivateKey(self, evp_pkey)
+        return rust_openssl.x448.from_private_bytes(data)
 
     def x448_generate_key(self) -> x448.X448PrivateKey:
-        evp_pkey = self._evp_pkey_keygen_gc(self._lib.NID_X448)
-        return _X448PrivateKey(self, evp_pkey)
+        return rust_openssl.x448.generate_key()
 
     def x448_supported(self) -> bool:
         if self._fips_enabled:
             return False
         return (
             not self._lib.CRYPTOGRAPHY_IS_LIBRESSL
             and not self._lib.CRYPTOGRAPHY_IS_BORINGSSL
@@ -1927,134 +1533,43 @@
         if self._fips_enabled:
             return False
         return self._lib.CRYPTOGRAPHY_HAS_WORKING_ED25519
 
     def ed25519_load_public_bytes(
         self, data: bytes
     ) -> ed25519.Ed25519PublicKey:
-        utils._check_bytes("data", data)
-
-        if len(data) != ed25519._ED25519_KEY_SIZE:
-            raise ValueError("An Ed25519 public key is 32 bytes long")
-
-        evp_pkey = self._lib.EVP_PKEY_new_raw_public_key(
-            self._lib.NID_ED25519, self._ffi.NULL, data, len(data)
-        )
-        self.openssl_assert(evp_pkey != self._ffi.NULL)
-        evp_pkey = self._ffi.gc(evp_pkey, self._lib.EVP_PKEY_free)
-
-        return _Ed25519PublicKey(self, evp_pkey)
+        return rust_openssl.ed25519.from_public_bytes(data)
 
     def ed25519_load_private_bytes(
         self, data: bytes
     ) -> ed25519.Ed25519PrivateKey:
-        if len(data) != ed25519._ED25519_KEY_SIZE:
-            raise ValueError("An Ed25519 private key is 32 bytes long")
-
-        utils._check_byteslike("data", data)
-        data_ptr = self._ffi.from_buffer(data)
-        evp_pkey = self._lib.EVP_PKEY_new_raw_private_key(
-            self._lib.NID_ED25519, self._ffi.NULL, data_ptr, len(data)
-        )
-        self.openssl_assert(evp_pkey != self._ffi.NULL)
-        evp_pkey = self._ffi.gc(evp_pkey, self._lib.EVP_PKEY_free)
-
-        return _Ed25519PrivateKey(self, evp_pkey)
+        return rust_openssl.ed25519.from_private_bytes(data)
 
     def ed25519_generate_key(self) -> ed25519.Ed25519PrivateKey:
-        evp_pkey = self._evp_pkey_keygen_gc(self._lib.NID_ED25519)
-        return _Ed25519PrivateKey(self, evp_pkey)
+        return rust_openssl.ed25519.generate_key()
 
     def ed448_supported(self) -> bool:
         if self._fips_enabled:
             return False
         return (
-            not self._lib.CRYPTOGRAPHY_OPENSSL_LESS_THAN_111B
+            not self._lib.CRYPTOGRAPHY_IS_LIBRESSL
             and not self._lib.CRYPTOGRAPHY_IS_BORINGSSL
         )
 
     def ed448_load_public_bytes(self, data: bytes) -> ed448.Ed448PublicKey:
-        utils._check_bytes("data", data)
-        if len(data) != _ED448_KEY_SIZE:
-            raise ValueError("An Ed448 public key is 57 bytes long")
-
-        evp_pkey = self._lib.EVP_PKEY_new_raw_public_key(
-            self._lib.NID_ED448, self._ffi.NULL, data, len(data)
-        )
-        self.openssl_assert(evp_pkey != self._ffi.NULL)
-        evp_pkey = self._ffi.gc(evp_pkey, self._lib.EVP_PKEY_free)
-
-        return _Ed448PublicKey(self, evp_pkey)
+        return rust_openssl.ed448.from_public_bytes(data)
 
     def ed448_load_private_bytes(self, data: bytes) -> ed448.Ed448PrivateKey:
-        utils._check_byteslike("data", data)
-        if len(data) != _ED448_KEY_SIZE:
-            raise ValueError("An Ed448 private key is 57 bytes long")
-
-        data_ptr = self._ffi.from_buffer(data)
-        evp_pkey = self._lib.EVP_PKEY_new_raw_private_key(
-            self._lib.NID_ED448, self._ffi.NULL, data_ptr, len(data)
-        )
-        self.openssl_assert(evp_pkey != self._ffi.NULL)
-        evp_pkey = self._ffi.gc(evp_pkey, self._lib.EVP_PKEY_free)
-
-        return _Ed448PrivateKey(self, evp_pkey)
+        return rust_openssl.ed448.from_private_bytes(data)
 
     def ed448_generate_key(self) -> ed448.Ed448PrivateKey:
-        evp_pkey = self._evp_pkey_keygen_gc(self._lib.NID_ED448)
-        return _Ed448PrivateKey(self, evp_pkey)
-
-    def derive_scrypt(
-        self,
-        key_material: bytes,
-        salt: bytes,
-        length: int,
-        n: int,
-        r: int,
-        p: int,
-    ) -> bytes:
-        buf = self._ffi.new("unsigned char[]", length)
-        key_material_ptr = self._ffi.from_buffer(key_material)
-        res = self._lib.EVP_PBE_scrypt(
-            key_material_ptr,
-            len(key_material),
-            salt,
-            len(salt),
-            n,
-            r,
-            p,
-            scrypt._MEM_LIMIT,
-            buf,
-            length,
-        )
-        if res != 1:
-            errors = self._consume_errors()
-            # memory required formula explained here:
-            # https://blog.filippo.io/the-scrypt-parameters/
-            min_memory = 128 * n * r // (1024**2)
-            raise MemoryError(
-                "Not enough memory to derive key. These parameters require"
-                " {} MB of memory.".format(min_memory),
-                errors,
-            )
-        return self._ffi.buffer(buf)[:]
+        return rust_openssl.ed448.generate_key()
 
     def aead_cipher_supported(self, cipher) -> bool:
-        cipher_name = aead._aead_cipher_name(cipher)
-        if self._fips_enabled and cipher_name not in self._fips_aead:
-            return False
-        # SIV isn't loaded through get_cipherbyname but instead a new fetch API
-        # only available in 3.0+. But if we know we're on 3.0+ then we know
-        # it's supported.
-        if cipher_name.endswith(b"-siv"):
-            return self._lib.CRYPTOGRAPHY_OPENSSL_300_OR_GREATER == 1
-        else:
-            return (
-                self._lib.EVP_get_cipherbyname(cipher_name) != self._ffi.NULL
-            )
+        return aead._aead_cipher_supported(self, cipher)
 
     def _zero_data(self, data, length: int) -> None:
         # We clear things this way because at the moment we're not
         # sure of a better way that can guarantee it overwrites the
         # memory of a bytearray and doesn't just replace the underlying char *.
         for i in range(length):
             data[i] = 0
@@ -2286,23 +1801,22 @@
                 ossl_cas.append(ossl_ca)
                 res = self._lib.sk_X509_push(sk_x509, ossl_ca)
                 backend.openssl_assert(res >= 1)
 
         with self._zeroed_null_terminated_buf(password) as password_buf:
             with self._zeroed_null_terminated_buf(name) as name_buf:
                 ossl_cert = self._cert2ossl(cert) if cert else self._ffi.NULL
-                if key is not None:
-                    evp_pkey = key._evp_pkey  # type: ignore[union-attr]
-                else:
-                    evp_pkey = self._ffi.NULL
+                ossl_pkey = (
+                    self._key2ossl(key) if key is not None else self._ffi.NULL
+                )
 
                 p12 = self._lib.PKCS12_create(
                     password_buf,
                     name_buf,
-                    evp_pkey,
+                    ossl_pkey,
                     ossl_cert,
                     sk_x509,
                     nid_key,
                     nid_cert,
                     pkcs12_iter,
                     mac_iter,
                     0,
@@ -2331,21 +1845,14 @@
         return self._read_mem_bio(bio)
 
     def poly1305_supported(self) -> bool:
         if self._fips_enabled:
             return False
         return self._lib.Cryptography_HAS_POLY1305 == 1
 
-    def create_poly1305_ctx(self, key: bytes) -> _Poly1305Context:
-        utils._check_byteslike("key", key)
-        if len(key) != _POLY1305_KEY_SIZE:
-            raise ValueError("A poly1305 key is 32 bytes long")
-
-        return _Poly1305Context(self, key)
-
     def pkcs7_supported(self) -> bool:
         return not self._lib.CRYPTOGRAPHY_IS_BORINGSSL
 
     def load_pem_pkcs7_certificates(
         self, data: bytes
     ) -> typing.List[x509.Certificate]:
         utils._check_bytes("data", data)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/ciphers.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ciphers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography.exceptions import InvalidTag, UnsupportedAlgorithm, _Reasons
 from cryptography.hazmat.primitives import ciphers
 from cryptography.hazmat.primitives.ciphers import algorithms, modes
 
 if typing.TYPE_CHECKING:
@@ -13,17 +15,15 @@
 
 
 class _CipherContext:
     _ENCRYPT = 1
     _DECRYPT = 0
     _MAX_CHUNK_SIZE = 2**30 - 1
 
-    def __init__(
-        self, backend: "Backend", cipher, mode, operation: int
-    ) -> None:
+    def __init__(self, backend: Backend, cipher, mode, operation: int) -> None:
         self._backend = backend
         self._cipher = cipher
         self._mode = mode
         self._operation = operation
         self._tag: typing.Optional[bytes] = None
 
         if isinstance(self._cipher, ciphers.BlockCipherAlgorithm):
@@ -115,15 +115,15 @@
         )
 
         # Check for XTS mode duplicate keys error
         errors = self._backend._consume_errors()
         lib = self._backend._lib
         if res == 0 and (
             (
-                lib.CRYPTOGRAPHY_OPENSSL_111D_OR_GREATER
+                not lib.CRYPTOGRAPHY_IS_LIBRESSL
                 and errors[0]._lib_reason_match(
                     lib.ERR_LIB_EVP, lib.EVP_R_XTS_DUPLICATED_KEYS
                 )
             )
             or (
                 lib.Cryptography_HAS_PROVIDERS
                 and errors[0]._lib_reason_match(
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/cmac.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/cmac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography.exceptions import (
     InvalidSignature,
     UnsupportedAlgorithm,
     _Reasons,
 )
@@ -16,16 +18,16 @@
     from cryptography.hazmat.backends.openssl.backend import Backend
     from cryptography.hazmat.primitives import ciphers
 
 
 class _CMACContext:
     def __init__(
         self,
-        backend: "Backend",
-        algorithm: "ciphers.BlockCipherAlgorithm",
+        backend: Backend,
+        algorithm: ciphers.BlockCipherAlgorithm,
         ctx=None,
     ) -> None:
         if not backend.cmac_algorithm_supported(algorithm):
             raise UnsupportedAlgorithm(
                 "This backend does not support CMAC.",
                 _Reasons.UNSUPPORTED_CIPHER,
             )
@@ -68,15 +70,15 @@
         res = self._backend._lib.CMAC_Final(self._ctx, buf, length)
         self._backend.openssl_assert(res == 1)
 
         self._ctx = None
 
         return self._backend._ffi.buffer(buf)[:]
 
-    def copy(self) -> "_CMACContext":
+    def copy(self) -> _CMACContext:
         copied_ctx = self._backend._lib.CMAC_CTX_new()
         copied_ctx = self._backend._ffi.gc(
             copied_ctx, self._backend._lib.CMAC_CTX_free
         )
         res = self._backend._lib.CMAC_CTX_copy(copied_ctx, self._ctx)
         self._backend.openssl_assert(res == 1)
         return _CMACContext(self._backend, self._algorithm, ctx=copied_ctx)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/decode_asn1.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/decode_asn1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 from cryptography import x509
 
 #    CRLReason ::= ENUMERATED {
 #        unspecified             (0),
 #        keyCompromise           (1),
 #        cACompromise            (2),
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/ec.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/ec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography.exceptions import (
     InvalidSignature,
     UnsupportedAlgorithm,
     _Reasons,
 )
@@ -26,15 +28,15 @@
     if not isinstance(signature_algorithm, ec.ECDSA):
         raise UnsupportedAlgorithm(
             "Unsupported elliptic curve signature algorithm.",
             _Reasons.UNSUPPORTED_PUBLIC_KEY_ALGORITHM,
         )
 
 
-def _ec_key_curve_sn(backend: "Backend", ec_key) -> str:
+def _ec_key_curve_sn(backend: Backend, ec_key) -> str:
     group = backend._lib.EC_KEY_get0_group(ec_key)
     backend.openssl_assert(group != backend._ffi.NULL)
 
     nid = backend._lib.EC_GROUP_get_curve_name(group)
     # The following check is to find EC keys with unnamed curves and raise
     # an error for now.
     if nid == backend._lib.NID_undef:
@@ -56,78 +58,78 @@
     curve_name = backend._lib.OBJ_nid2sn(nid)
     backend.openssl_assert(curve_name != backend._ffi.NULL)
 
     sn = backend._ffi.string(curve_name).decode("ascii")
     return sn
 
 
-def _mark_asn1_named_ec_curve(backend: "Backend", ec_cdata):
+def _mark_asn1_named_ec_curve(backend: Backend, ec_cdata):
     """
     Set the named curve flag on the EC_KEY. This causes OpenSSL to
     serialize EC keys along with their curve OID which makes
     deserialization easier.
     """
 
     backend._lib.EC_KEY_set_asn1_flag(
         ec_cdata, backend._lib.OPENSSL_EC_NAMED_CURVE
     )
 
 
-def _check_key_infinity(backend: "Backend", ec_cdata) -> None:
+def _check_key_infinity(backend: Backend, ec_cdata) -> None:
     point = backend._lib.EC_KEY_get0_public_key(ec_cdata)
     backend.openssl_assert(point != backend._ffi.NULL)
     group = backend._lib.EC_KEY_get0_group(ec_cdata)
     backend.openssl_assert(group != backend._ffi.NULL)
     if backend._lib.EC_POINT_is_at_infinity(group, point):
         raise ValueError(
             "Cannot load an EC public key where the point is at infinity"
         )
 
 
-def _sn_to_elliptic_curve(backend: "Backend", sn: str) -> ec.EllipticCurve:
+def _sn_to_elliptic_curve(backend: Backend, sn: str) -> ec.EllipticCurve:
     try:
         return ec._CURVE_TYPES[sn]()
     except KeyError:
         raise UnsupportedAlgorithm(
             f"{sn} is not a supported elliptic curve",
             _Reasons.UNSUPPORTED_ELLIPTIC_CURVE,
         )
 
 
 def _ecdsa_sig_sign(
-    backend: "Backend", private_key: "_EllipticCurvePrivateKey", data: bytes
+    backend: Backend, private_key: _EllipticCurvePrivateKey, data: bytes
 ) -> bytes:
     max_size = backend._lib.ECDSA_size(private_key._ec_key)
     backend.openssl_assert(max_size > 0)
 
     sigbuf = backend._ffi.new("unsigned char[]", max_size)
     siglen_ptr = backend._ffi.new("unsigned int[]", 1)
     res = backend._lib.ECDSA_sign(
         0, data, len(data), sigbuf, siglen_ptr, private_key._ec_key
     )
     backend.openssl_assert(res == 1)
     return backend._ffi.buffer(sigbuf)[: siglen_ptr[0]]
 
 
 def _ecdsa_sig_verify(
-    backend: "Backend",
-    public_key: "_EllipticCurvePublicKey",
+    backend: Backend,
+    public_key: _EllipticCurvePublicKey,
     signature: bytes,
     data: bytes,
 ) -> None:
     res = backend._lib.ECDSA_verify(
         0, data, len(data), signature, len(signature), public_key._ec_key
     )
     if res != 1:
         backend._consume_errors()
         raise InvalidSignature
 
 
 class _EllipticCurvePrivateKey(ec.EllipticCurvePrivateKey):
-    def __init__(self, backend: "Backend", ec_key_cdata, evp_pkey):
+    def __init__(self, backend: Backend, ec_key_cdata, evp_pkey):
         self._backend = backend
         self._ec_key = ec_key_cdata
         self._evp_pkey = evp_pkey
 
         sn = _ec_key_curve_sn(backend, ec_key_cdata)
         self._curve = _sn_to_elliptic_curve(backend, sn)
         _mark_asn1_named_ec_curve(backend, ec_key_cdata)
@@ -211,15 +213,15 @@
             data,
             signature_algorithm.algorithm,
         )
         return _ecdsa_sig_sign(self._backend, self, data)
 
 
 class _EllipticCurvePublicKey(ec.EllipticCurvePublicKey):
-    def __init__(self, backend: "Backend", ec_key_cdata, evp_pkey):
+    def __init__(self, backend: Backend, ec_key_cdata, evp_pkey):
         self._backend = backend
         self._ec_key = ec_key_cdata
         self._evp_pkey = evp_pkey
 
         sn = _ec_key_curve_sn(backend, ec_key_cdata)
         self._curve = _sn_to_elliptic_curve(backend, sn)
         _mark_asn1_named_ec_curve(backend, ec_key_cdata)
@@ -229,14 +231,23 @@
     def curve(self) -> ec.EllipticCurve:
         return self._curve
 
     @property
     def key_size(self) -> int:
         return self.curve.key_size
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, _EllipticCurvePublicKey):
+            return NotImplemented
+
+        return (
+            self._backend._lib.EVP_PKEY_cmp(self._evp_pkey, other._evp_pkey)
+            == 1
+        )
+
     def public_numbers(self) -> ec.EllipticCurvePublicNumbers:
         group = self._backend._lib.EC_KEY_get0_group(self._ec_key)
         self._backend.openssl_assert(group != self._backend._ffi.NULL)
 
         point = self._backend._lib.EC_KEY_get0_public_key(self._ec_key)
         self._backend.openssl_assert(point != self._backend._ffi.NULL)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/rsa.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/rsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import threading
 import typing
 
 from cryptography.exceptions import (
     InvalidSignature,
     UnsupportedAlgorithm,
     _Reasons,
@@ -34,15 +36,15 @@
 )
 
 if typing.TYPE_CHECKING:
     from cryptography.hazmat.backends.openssl.backend import Backend
 
 
 def _get_rsa_pss_salt_length(
-    backend: "Backend",
+    backend: Backend,
     pss: PSS,
     key: typing.Union[RSAPrivateKey, RSAPublicKey],
     hash_algorithm: hashes.HashAlgorithm,
 ) -> int:
     salt = pss._salt_length
 
     if isinstance(salt, _MaxLength):
@@ -56,16 +58,16 @@
             )
         return backend._lib.RSA_PSS_SALTLEN_AUTO
     else:
         return salt
 
 
 def _enc_dec_rsa(
-    backend: "Backend",
-    key: typing.Union["_RSAPrivateKey", "_RSAPublicKey"],
+    backend: Backend,
+    key: typing.Union[_RSAPrivateKey, _RSAPublicKey],
     data: bytes,
     padding: AsymmetricPadding,
 ) -> bytes:
     if not isinstance(padding, AsymmetricPadding):
         raise TypeError("Padding must be an instance of AsymmetricPadding.")
 
     if isinstance(padding, PKCS1v15):
@@ -92,16 +94,16 @@
             _Reasons.UNSUPPORTED_PADDING,
         )
 
     return _enc_dec_rsa_pkey_ctx(backend, key, data, padding_enum, padding)
 
 
 def _enc_dec_rsa_pkey_ctx(
-    backend: "Backend",
-    key: typing.Union["_RSAPrivateKey", "_RSAPublicKey"],
+    backend: Backend,
+    key: typing.Union[_RSAPrivateKey, _RSAPublicKey],
     data: bytes,
     padding_enum: int,
     padding: AsymmetricPadding,
 ) -> bytes:
     init: typing.Callable[[typing.Any], int]
     crypt: typing.Callable[[typing.Any, typing.Any, int, bytes, int], int]
     if isinstance(key, _RSAPublicKey):
@@ -159,16 +161,16 @@
     backend._lib.ERR_clear_error()
     if res <= 0:
         raise ValueError("Encryption/decryption failed.")
     return resbuf
 
 
 def _rsa_sig_determine_padding(
-    backend: "Backend",
-    key: typing.Union["_RSAPrivateKey", "_RSAPublicKey"],
+    backend: Backend,
+    key: typing.Union[_RSAPrivateKey, _RSAPublicKey],
     padding: AsymmetricPadding,
     algorithm: typing.Optional[hashes.HashAlgorithm],
 ) -> int:
     if not isinstance(padding, AsymmetricPadding):
         raise TypeError("Expected provider of AsymmetricPadding.")
 
     pkey_size = backend._lib.EVP_PKEY_size(key._evp_pkey)
@@ -207,18 +209,18 @@
 
 
 # Hash algorithm can be absent (None) to initialize the context without setting
 # any message digest algorithm. This is currently only valid for the PKCS1v15
 # padding type, where it means that the signature data is encoded/decoded
 # as provided, without being wrapped in a DigestInfo structure.
 def _rsa_sig_setup(
-    backend: "Backend",
+    backend: Backend,
     padding: AsymmetricPadding,
     algorithm: typing.Optional[hashes.HashAlgorithm],
-    key: typing.Union["_RSAPublicKey", "_RSAPrivateKey"],
+    key: typing.Union[_RSAPublicKey, _RSAPrivateKey],
     init_func: typing.Callable[[typing.Any], int],
 ):
     padding_enum = _rsa_sig_determine_padding(backend, key, padding, algorithm)
     pkey_ctx = backend._lib.EVP_PKEY_CTX_new(key._evp_pkey, backend._ffi.NULL)
     backend.openssl_assert(pkey_ctx != backend._ffi.NULL)
     pkey_ctx = backend._ffi.gc(pkey_ctx, backend._lib.EVP_PKEY_CTX_free)
     res = init_func(pkey_ctx)
@@ -260,18 +262,18 @@
         res = backend._lib.EVP_PKEY_CTX_set_rsa_mgf1_md(pkey_ctx, mgf1_md)
         backend.openssl_assert(res > 0)
 
     return pkey_ctx
 
 
 def _rsa_sig_sign(
-    backend: "Backend",
+    backend: Backend,
     padding: AsymmetricPadding,
     algorithm: hashes.HashAlgorithm,
-    private_key: "_RSAPrivateKey",
+    private_key: _RSAPrivateKey,
     data: bytes,
 ) -> bytes:
     pkey_ctx = _rsa_sig_setup(
         backend,
         padding,
         algorithm,
         private_key,
@@ -292,18 +294,18 @@
             errors,
         )
 
     return backend._ffi.buffer(buf)[:]
 
 
 def _rsa_sig_verify(
-    backend: "Backend",
+    backend: Backend,
     padding: AsymmetricPadding,
     algorithm: hashes.HashAlgorithm,
-    public_key: "_RSAPublicKey",
+    public_key: _RSAPublicKey,
     signature: bytes,
     data: bytes,
 ) -> None:
     pkey_ctx = _rsa_sig_setup(
         backend,
         padding,
         algorithm,
@@ -319,18 +321,18 @@
     backend.openssl_assert(res >= 0)
     if res == 0:
         backend._consume_errors()
         raise InvalidSignature
 
 
 def _rsa_sig_recover(
-    backend: "Backend",
+    backend: Backend,
     padding: AsymmetricPadding,
     algorithm: typing.Optional[hashes.HashAlgorithm],
-    public_key: "_RSAPublicKey",
+    public_key: _RSAPublicKey,
     signature: bytes,
 ) -> bytes:
     pkey_ctx = _rsa_sig_setup(
         backend,
         padding,
         algorithm,
         public_key,
@@ -361,15 +363,15 @@
 class _RSAPrivateKey(RSAPrivateKey):
     _evp_pkey: object
     _rsa_cdata: object
     _key_size: int
 
     def __init__(
         self,
-        backend: "Backend",
+        backend: Backend,
         rsa_cdata,
         evp_pkey,
         *,
         unsafe_skip_rsa_key_validation: bool,
     ):
         res: int
         # RSA_check_key is slower in OpenSSL 3.0.0 due to improved
@@ -512,15 +514,15 @@
 
 
 class _RSAPublicKey(RSAPublicKey):
     _evp_pkey: object
     _rsa_cdata: object
     _key_size: int
 
-    def __init__(self, backend: "Backend", rsa_cdata, evp_pkey):
+    def __init__(self, backend: Backend, rsa_cdata, evp_pkey):
         self._backend = backend
         self._rsa_cdata = rsa_cdata
         self._evp_pkey = evp_pkey
 
         n = self._backend._ffi.new("BIGNUM **")
         self._backend._lib.RSA_get0_key(
             self._rsa_cdata,
@@ -531,14 +533,23 @@
         self._backend.openssl_assert(n[0] != self._backend._ffi.NULL)
         self._key_size = self._backend._lib.BN_num_bits(n[0])
 
     @property
     def key_size(self) -> int:
         return self._key_size
 
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, _RSAPublicKey):
+            return NotImplemented
+
+        return (
+            self._backend._lib.EVP_PKEY_cmp(self._evp_pkey, other._evp_pkey)
+            == 1
+        )
+
     def encrypt(self, plaintext: bytes, padding: AsymmetricPadding) -> bytes:
         return _enc_dec_rsa(self._backend, self, plaintext, padding)
 
     def public_numbers(self) -> RSAPublicNumbers:
         n = self._backend._ffi.new("BIGNUM **")
         e = self._backend._ffi.new("BIGNUM **")
         self._backend._lib.RSA_get0_key(
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/backends/openssl/utils.py` & `cryptography-41.0.0/src/cryptography/hazmat/backends/openssl/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
 
 if typing.TYPE_CHECKING:
     from cryptography.hazmat.backends.openssl.backend import Backend
 
 
-def _evp_pkey_derive(backend: "Backend", evp_pkey, peer_public_key) -> bytes:
+def _evp_pkey_derive(backend: Backend, evp_pkey, peer_public_key) -> bytes:
     ctx = backend._lib.EVP_PKEY_CTX_new(evp_pkey, backend._ffi.NULL)
     backend.openssl_assert(ctx != backend._ffi.NULL)
     ctx = backend._ffi.gc(ctx, backend._lib.EVP_PKEY_CTX_free)
     res = backend._lib.EVP_PKEY_derive_init(ctx)
     backend.openssl_assert(res == 1)
 
     if backend._lib.Cryptography_HAS_EVP_PKEY_SET_PEER_EX:
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/__init__.pyi` & `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/asn1.pyi` & `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/asn1.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/ocsp.pyi` & `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi` & `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/bindings/_rust/x509.pyi` & `cryptography-41.0.0/src/cryptography/hazmat/bindings/_rust/x509.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 import typing
 
 from cryptography import x509
 from cryptography.hazmat.primitives import hashes
+from cryptography.hazmat.primitives.asymmetric.padding import PSS, PKCS1v15
 from cryptography.hazmat.primitives.asymmetric.types import PrivateKeyTypes
 
 def load_pem_x509_certificate(data: bytes) -> x509.Certificate: ...
 def load_pem_x509_certificates(
     data: bytes,
 ) -> typing.List[x509.Certificate]: ...
 def load_der_x509_certificate(data: bytes) -> x509.Certificate: ...
@@ -19,14 +20,15 @@
 def load_der_x509_csr(data: bytes) -> x509.CertificateSigningRequest: ...
 def encode_name_bytes(name: x509.Name) -> bytes: ...
 def encode_extension_value(extension: x509.ExtensionType) -> bytes: ...
 def create_x509_certificate(
     builder: x509.CertificateBuilder,
     private_key: PrivateKeyTypes,
     hash_algorithm: typing.Optional[hashes.HashAlgorithm],
+    padding: typing.Optional[typing.Union[PKCS1v15, PSS]],
 ) -> x509.Certificate: ...
 def create_x509_csr(
     builder: x509.CertificateSigningRequestBuilder,
     private_key: PrivateKeyTypes,
     hash_algorithm: typing.Optional[hashes.HashAlgorithm],
 ) -> x509.CertificateSigningRequest: ...
 def create_x509_crl(
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/bindings/openssl/_conditional.py` & `cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/_conditional.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 
 def cryptography_has_set_cert_cb() -> typing.List[str]:
     return [
         "SSL_CTX_set_cert_cb",
         "SSL_set_cert_cb",
@@ -24,25 +26,17 @@
 def cryptography_has_tls_st() -> typing.List[str]:
     return [
         "TLS_ST_BEFORE",
         "TLS_ST_OK",
     ]
 
 
-def cryptography_has_scrypt() -> typing.List[str]:
-    return [
-        "EVP_PBE_scrypt",
-    ]
-
-
 def cryptography_has_evp_pkey_dhx() -> typing.List[str]:
     return [
         "EVP_PKEY_DHX",
-        "d2i_DHxparams_bio",
-        "i2d_DHxparams_bio",
     ]
 
 
 def cryptography_has_mem_functions() -> typing.List[str]:
     return [
         "Cryptography_CRYPTO_set_mem_functions",
     ]
@@ -118,20 +112,14 @@
     return [
         "SSL_CTX_add_client_custom_ext",
         "SSL_CTX_add_server_custom_ext",
         "SSL_extension_supported",
     ]
 
 
-def cryptography_has_openssl_cleanup() -> typing.List[str]:
-    return [
-        "OPENSSL_cleanup",
-    ]
-
-
 def cryptography_has_tlsv13_functions() -> typing.List[str]:
     return [
         "SSL_VERIFY_POST_HANDSHAKE",
         "SSL_CTX_set_ciphersuites",
         "SSL_verify_client_post_handshake",
         "SSL_CTX_set_post_handshake_auth",
         "SSL_set_post_handshake_auth",
@@ -158,15 +146,14 @@
         "ENGINE_finish",
         "ENGINE_get_default_RAND",
         "ENGINE_set_default_RAND",
         "ENGINE_unregister_RAND",
         "ENGINE_ctrl_cmd",
         "ENGINE_free",
         "ENGINE_get_name",
-        "Cryptography_add_osrandom_engine",
         "ENGINE_ctrl_cmd_string",
         "ENGINE_load_builtin_engines",
         "ENGINE_load_private_key",
         "ENGINE_load_public_key",
         "SSL_CTX_set_client_cert_engine",
     ]
 
@@ -271,38 +258,47 @@
     return ["SSL_get_extms_support"]
 
 
 def cryptography_has_evp_pkey_set_peer_ex() -> typing.List[str]:
     return ["EVP_PKEY_derive_set_peer_ex"]
 
 
+def cryptography_has_evp_aead() -> typing.List[str]:
+    return [
+        "EVP_aead_chacha20_poly1305",
+        "EVP_AEAD_CTX_free",
+        "EVP_AEAD_CTX_seal",
+        "EVP_AEAD_CTX_open",
+        "EVP_AEAD_max_overhead",
+        "Cryptography_EVP_AEAD_CTX_new",
+    ]
+
+
 # This is a mapping of
 # {condition: function-returning-names-dependent-on-that-condition} so we can
 # loop over them and delete unsupported names at runtime. It will be removed
 # when cffi supports #if in cdef. We use functions instead of just a dict of
 # lists so we can use coverage to measure which are used.
 CONDITIONAL_NAMES = {
     "Cryptography_HAS_SET_CERT_CB": cryptography_has_set_cert_cb,
     "Cryptography_HAS_SSL_ST": cryptography_has_ssl_st,
     "Cryptography_HAS_TLS_ST": cryptography_has_tls_st,
-    "Cryptography_HAS_SCRYPT": cryptography_has_scrypt,
     "Cryptography_HAS_EVP_PKEY_DHX": cryptography_has_evp_pkey_dhx,
     "Cryptography_HAS_MEM_FUNCTIONS": cryptography_has_mem_functions,
     "Cryptography_HAS_X509_STORE_CTX_GET_ISSUER": (
         cryptography_has_x509_store_ctx_get_issuer
     ),
     "Cryptography_HAS_ED448": cryptography_has_ed448,
     "Cryptography_HAS_ED25519": cryptography_has_ed25519,
     "Cryptography_HAS_POLY1305": cryptography_has_poly1305,
     "Cryptography_HAS_FIPS": cryptography_has_fips,
     "Cryptography_HAS_SIGALGS": cryptography_has_ssl_sigalgs,
     "Cryptography_HAS_PSK": cryptography_has_psk,
     "Cryptography_HAS_PSK_TLSv1_3": cryptography_has_psk_tlsv13,
     "Cryptography_HAS_CUSTOM_EXT": cryptography_has_custom_ext,
-    "Cryptography_HAS_OPENSSL_CLEANUP": cryptography_has_openssl_cleanup,
     "Cryptography_HAS_TLSv1_3_FUNCTIONS": cryptography_has_tlsv13_functions,
     "Cryptography_HAS_RAW_KEY": cryptography_has_raw_key,
     "Cryptography_HAS_EVP_DIGESTFINAL_XOF": (
         cryptography_has_evp_digestfinal_xof
     ),
     "Cryptography_HAS_ENGINE": cryptography_has_engine,
     "Cryptography_HAS_VERIFIED_CHAIN": cryptography_has_verified_chain,
@@ -325,8 +321,9 @@
     "Cryptography_HAS_SSL_OP_IGNORE_UNEXPECTED_EOF": (
         cryptography_has_ssl_op_ignore_unexpected_eof
     ),
     "Cryptography_HAS_GET_EXTMS_SUPPORT": cryptography_has_get_extms_support,
     "Cryptography_HAS_EVP_PKEY_SET_PEER_EX": (
         cryptography_has_evp_pkey_set_peer_ex
     ),
+    "Cryptography_HAS_EVP_AEAD": (cryptography_has_evp_aead),
 }
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/bindings/openssl/binding.py` & `cryptography-41.0.0/src/cryptography/hazmat/bindings/openssl/binding.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import os
 import sys
 import threading
 import types
 import typing
 import warnings
 
 import cryptography
-from cryptography import utils
 from cryptography.exceptions import InternalError
 from cryptography.hazmat.bindings._rust import _openssl, openssl
 from cryptography.hazmat.bindings.openssl._conditional import CONDITIONAL_NAMES
 
 
 def _openssl_assert(
     lib,
@@ -95,34 +96,21 @@
         )
         _openssl_assert(self.lib, self.lib._fips_provider != self.ffi.NULL)
 
         res = self.lib.EVP_default_properties_enable_fips(self.ffi.NULL, 1)
         _openssl_assert(self.lib, res == 1)
 
     @classmethod
-    def _register_osrandom_engine(cls) -> None:
-        # Clear any errors extant in the queue before we start. In many
-        # scenarios other things may be interacting with OpenSSL in the same
-        # process space and it has proven untenable to assume that they will
-        # reliably clear the error queue. Once we clear it here we will
-        # error on any subsequent unexpected item in the stack.
-        cls.lib.ERR_clear_error()
-        if cls.lib.CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE:
-            result = cls.lib.Cryptography_add_osrandom_engine()
-            _openssl_assert(cls.lib, result in (1, 2))
-
-    @classmethod
     def _ensure_ffi_initialized(cls) -> None:
         with cls._init_lock:
             if not cls._lib_loaded:
                 cls.lib = build_conditional_library(
                     _openssl.lib, CONDITIONAL_NAMES
                 )
                 cls._lib_loaded = True
-                cls._register_osrandom_engine()
                 # As of OpenSSL 3.0.0 we must register a legacy cipher provider
                 # to get RC2 (needed for junk asymmetric private key
                 # serialization), RC4, Blowfish, IDEA, SEED, etc. These things
                 # are ugly legacy, but we aren't going to get rid of them
                 # any time soon.
                 if cls.lib.CRYPTOGRAPHY_OPENSSL_300_OR_GREATER:
                     if not os.environ.get("CRYPTOGRAPHY_OPENSSL_NO_LEGACY"):
@@ -185,24 +173,7 @@
     warnings.warn(
         "You are using cryptography on a 32-bit Python on a 64-bit Windows "
         "Operating System. Cryptography will be significantly faster if you "
         "switch to using a 64-bit Python.",
         UserWarning,
         stacklevel=2,
     )
-
-
-def _verify_openssl_version(lib):
-    if (
-        not lib.CRYPTOGRAPHY_OPENSSL_111D_OR_GREATER
-        and not lib.CRYPTOGRAPHY_IS_LIBRESSL
-        and not lib.CRYPTOGRAPHY_IS_BORINGSSL
-    ):
-        warnings.warn(
-            "Support for OpenSSL less than version 1.1.1d is deprecated and "
-            "the next release of cryptography will drop support. Please "
-            "upgrade your OpenSSL to version 1.1.1d or newer.",
-            utils.DeprecatedIn40,
-        )
-
-
-_verify_openssl_version(Binding.lib)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/_cipheralgorithm.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/_cipheralgorithm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import abc
 import typing
 
 # This exists to break an import cycle. It is normally accessible from the
 # ciphers module.
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/_serialization.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import abc
 import typing
 
 from cryptography import utils
 from cryptography.hazmat.primitives.hashes import HashAlgorithm
 
 # This exists to break an import cycle. These classes are normally accessible
@@ -29,15 +31,15 @@
 class PrivateFormat(utils.Enum):
     PKCS8 = "PKCS8"
     TraditionalOpenSSL = "TraditionalOpenSSL"
     Raw = "Raw"
     OpenSSH = "OpenSSH"
     PKCS12 = "PKCS12"
 
-    def encryption_builder(self) -> "KeySerializationEncryptionBuilder":
+    def encryption_builder(self) -> KeySerializationEncryptionBuilder:
         if self not in (PrivateFormat.OpenSSH, PrivateFormat.PKCS12):
             raise ValueError(
                 "encryption_builder only supported with PrivateFormat.OpenSSH"
                 " and PrivateFormat.PKCS12"
             )
         return KeySerializationEncryptionBuilder(self)
 
@@ -82,15 +84,15 @@
     ) -> None:
         self._format = format
 
         self._kdf_rounds = _kdf_rounds
         self._hmac_hash = _hmac_hash
         self._key_cert_algorithm = _key_cert_algorithm
 
-    def kdf_rounds(self, rounds: int) -> "KeySerializationEncryptionBuilder":
+    def kdf_rounds(self, rounds: int) -> KeySerializationEncryptionBuilder:
         if self._kdf_rounds is not None:
             raise ValueError("kdf_rounds already set")
 
         if not isinstance(rounds, int):
             raise TypeError("kdf_rounds must be an integer")
 
         if rounds < 1:
@@ -101,15 +103,15 @@
             _kdf_rounds=rounds,
             _hmac_hash=self._hmac_hash,
             _key_cert_algorithm=self._key_cert_algorithm,
         )
 
     def hmac_hash(
         self, algorithm: HashAlgorithm
-    ) -> "KeySerializationEncryptionBuilder":
+    ) -> KeySerializationEncryptionBuilder:
         if self._format is not PrivateFormat.PKCS12:
             raise TypeError(
                 "hmac_hash only supported with PrivateFormat.PKCS12"
             )
 
         if self._hmac_hash is not None:
             raise ValueError("hmac_hash already set")
@@ -118,15 +120,15 @@
             _kdf_rounds=self._kdf_rounds,
             _hmac_hash=algorithm,
             _key_cert_algorithm=self._key_cert_algorithm,
         )
 
     def key_cert_algorithm(
         self, algorithm: PBES
-    ) -> "KeySerializationEncryptionBuilder":
+    ) -> KeySerializationEncryptionBuilder:
         if self._format is not PrivateFormat.PKCS12:
             raise TypeError(
                 "key_cert_algorithm only supported with "
                 "PrivateFormat.PKCS12"
             )
         if self._key_cert_algorithm is not None:
             raise ValueError("key_cert_algorithm already set")
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/dh.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dh.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 
+from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 from cryptography.hazmat.primitives import _serialization
 
-_MIN_MODULUS_SIZE = 512
-
 
 def generate_parameters(
     generator: int, key_size: int, backend: typing.Any = None
-) -> "DHParameters":
+) -> DHParameters:
     from cryptography.hazmat.backends.openssl.backend import backend as ossl
 
     return ossl.generate_dh_parameters(generator, key_size)
 
 
 class DHParameterNumbers:
     def __init__(self, p: int, g: int, q: typing.Optional[int] = None) -> None:
@@ -25,32 +25,33 @@
             raise TypeError("p and g must be integers")
         if q is not None and not isinstance(q, int):
             raise TypeError("q must be integer or None")
 
         if g < 2:
             raise ValueError("DH generator must be 2 or greater")
 
-        if p.bit_length() < _MIN_MODULUS_SIZE:
+        if p.bit_length() < rust_openssl.dh.MIN_MODULUS_SIZE:
             raise ValueError(
-                f"p (modulus) must be at least {_MIN_MODULUS_SIZE}-bit"
+                f"p (modulus) must be at least "
+                f"{rust_openssl.dh.MIN_MODULUS_SIZE}-bit"
             )
 
         self._p = p
         self._g = g
         self._q = q
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, DHParameterNumbers):
             return NotImplemented
 
         return (
             self._p == other._p and self._g == other._g and self._q == other._q
         )
 
-    def parameters(self, backend: typing.Any = None) -> "DHParameters":
+    def parameters(self, backend: typing.Any = None) -> DHParameters:
         from cryptography.hazmat.backends.openssl.backend import (
             backend as ossl,
         )
 
         return ossl.load_dh_parameter_numbers(self)
 
     @property
@@ -84,15 +85,15 @@
             return NotImplemented
 
         return (
             self._y == other._y
             and self._parameter_numbers == other._parameter_numbers
         )
 
-    def public_key(self, backend: typing.Any = None) -> "DHPublicKey":
+    def public_key(self, backend: typing.Any = None) -> DHPublicKey:
         from cryptography.hazmat.backends.openssl.backend import (
             backend as ossl,
         )
 
         return ossl.load_dh_public_numbers(self)
 
     @property
@@ -122,15 +123,15 @@
             return NotImplemented
 
         return (
             self._x == other._x
             and self._public_numbers == other._public_numbers
         )
 
-    def private_key(self, backend: typing.Any = None) -> "DHPrivateKey":
+    def private_key(self, backend: typing.Any = None) -> DHPrivateKey:
         from cryptography.hazmat.backends.openssl.backend import (
             backend as ossl,
         )
 
         return ossl.load_dh_private_numbers(self)
 
     @property
@@ -140,15 +141,15 @@
     @property
     def x(self) -> int:
         return self._x
 
 
 class DHParameters(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def generate_private_key(self) -> "DHPrivateKey":
+    def generate_private_key(self) -> DHPrivateKey:
         """
         Generates and returns a DHPrivateKey.
         """
 
     @abc.abstractmethod
     def parameter_bytes(
         self,
@@ -163,14 +164,15 @@
     def parameter_numbers(self) -> DHParameterNumbers:
         """
         Returns a DHParameterNumbers.
         """
 
 
 DHParametersWithSerialization = DHParameters
+DHParameters.register(rust_openssl.dh.DHParameters)
 
 
 class DHPublicKey(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
     def key_size(self) -> int:
         """
@@ -195,16 +197,23 @@
         encoding: _serialization.Encoding,
         format: _serialization.PublicFormat,
     ) -> bytes:
         """
         Returns the key serialized as bytes.
         """
 
+    @abc.abstractmethod
+    def __eq__(self, other: object) -> bool:
+        """
+        Checks equality.
+        """
+
 
 DHPublicKeyWithSerialization = DHPublicKey
+DHPublicKey.register(rust_openssl.dh.DHPublicKey)
 
 
 class DHPrivateKey(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
     def key_size(self) -> int:
         """
@@ -245,7 +254,8 @@
     ) -> bytes:
         """
         Returns the key serialized as bytes.
         """
 
 
 DHPrivateKeyWithSerialization = DHPrivateKey
+DHPrivateKey.register(rust_openssl.dh.DHPrivateKey)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/dsa.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/dsa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 
+from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 from cryptography.hazmat.primitives import _serialization, hashes
 from cryptography.hazmat.primitives.asymmetric import utils as asym_utils
 
 
 class DSAParameters(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def generate_private_key(self) -> "DSAPrivateKey":
+    def generate_private_key(self) -> DSAPrivateKey:
         """
         Generates and returns a DSAPrivateKey.
         """
 
     @abc.abstractmethod
-    def parameter_numbers(self) -> "DSAParameterNumbers":
+    def parameter_numbers(self) -> DSAParameterNumbers:
         """
         Returns a DSAParameterNumbers.
         """
 
 
 DSAParametersWithNumbers = DSAParameters
+DSAParameters.register(rust_openssl.dsa.DSAParameters)
 
 
 class DSAPrivateKey(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
     def key_size(self) -> int:
         """
         The bit length of the prime modulus.
         """
 
     @abc.abstractmethod
-    def public_key(self) -> "DSAPublicKey":
+    def public_key(self) -> DSAPublicKey:
         """
         The DSAPublicKey associated with this private key.
         """
 
     @abc.abstractmethod
     def parameters(self) -> DSAParameters:
         """
@@ -54,15 +57,15 @@
         algorithm: typing.Union[asym_utils.Prehashed, hashes.HashAlgorithm],
     ) -> bytes:
         """
         Signs the data
         """
 
     @abc.abstractmethod
-    def private_numbers(self) -> "DSAPrivateNumbers":
+    def private_numbers(self) -> DSAPrivateNumbers:
         """
         Returns a DSAPrivateNumbers.
         """
 
     @abc.abstractmethod
     def private_bytes(
         self,
@@ -72,14 +75,15 @@
     ) -> bytes:
         """
         Returns the key serialized as bytes.
         """
 
 
 DSAPrivateKeyWithSerialization = DSAPrivateKey
+DSAPrivateKey.register(rust_openssl.dsa.DSAPrivateKey)
 
 
 class DSAPublicKey(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
     def key_size(self) -> int:
         """
@@ -89,15 +93,15 @@
     @abc.abstractmethod
     def parameters(self) -> DSAParameters:
         """
         The DSAParameters object associated with this public key.
         """
 
     @abc.abstractmethod
-    def public_numbers(self) -> "DSAPublicNumbers":
+    def public_numbers(self) -> DSAPublicNumbers:
         """
         Returns a DSAPublicNumbers.
         """
 
     @abc.abstractmethod
     def public_bytes(
         self,
@@ -115,16 +119,23 @@
         data: bytes,
         algorithm: typing.Union[asym_utils.Prehashed, hashes.HashAlgorithm],
     ) -> None:
         """
         Verifies the signature of the data.
         """
 
+    @abc.abstractmethod
+    def __eq__(self, other: object) -> bool:
+        """
+        Checks equality.
+        """
+
 
 DSAPublicKeyWithSerialization = DSAPublicKey
+DSAPublicKey.register(rust_openssl.dsa.DSAPublicKey)
 
 
 class DSAParameterNumbers:
     def __init__(self, p: int, q: int, g: int):
         if (
             not isinstance(p, int)
             or not isinstance(q, int)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/ec.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 
 from cryptography import utils
 from cryptography.hazmat._oid import ObjectIdentifier
 from cryptography.hazmat.primitives import _serialization, hashes
@@ -60,23 +61,23 @@
         The digest algorithm used with this signature.
         """
 
 
 class EllipticCurvePrivateKey(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def exchange(
-        self, algorithm: "ECDH", peer_public_key: "EllipticCurvePublicKey"
+        self, algorithm: ECDH, peer_public_key: EllipticCurvePublicKey
     ) -> bytes:
         """
         Performs a key exchange operation using the provided algorithm with the
         provided peer's public key.
         """
 
     @abc.abstractmethod
-    def public_key(self) -> "EllipticCurvePublicKey":
+    def public_key(self) -> EllipticCurvePublicKey:
         """
         The EllipticCurvePublicKey for this private key.
         """
 
     @property
     @abc.abstractmethod
     def curve(self) -> EllipticCurve:
@@ -98,15 +99,15 @@
         signature_algorithm: EllipticCurveSignatureAlgorithm,
     ) -> bytes:
         """
         Signs the data
         """
 
     @abc.abstractmethod
-    def private_numbers(self) -> "EllipticCurvePrivateNumbers":
+    def private_numbers(self) -> EllipticCurvePrivateNumbers:
         """
         Returns an EllipticCurvePrivateNumbers.
         """
 
     @abc.abstractmethod
     def private_bytes(
         self,
@@ -134,15 +135,15 @@
     @abc.abstractmethod
     def key_size(self) -> int:
         """
         Bit size of a secret scalar for the curve.
         """
 
     @abc.abstractmethod
-    def public_numbers(self) -> "EllipticCurvePublicNumbers":
+    def public_numbers(self) -> EllipticCurvePublicNumbers:
         """
         Returns an EllipticCurvePublicNumbers.
         """
 
     @abc.abstractmethod
     def public_bytes(
         self,
@@ -163,15 +164,15 @@
         """
         Verifies the signature of the data.
         """
 
     @classmethod
     def from_encoded_point(
         cls, curve: EllipticCurve, data: bytes
-    ) -> "EllipticCurvePublicKey":
+    ) -> EllipticCurvePublicKey:
         utils._check_bytes("data", data)
 
         if not isinstance(curve, EllipticCurve):
             raise TypeError("curve must be an EllipticCurve instance")
 
         if len(data) == 0:
             raise ValueError("data must not be an empty byte string")
@@ -179,14 +180,20 @@
         if data[0] not in [0x02, 0x03, 0x04]:
             raise ValueError("Unsupported elliptic curve point type")
 
         from cryptography.hazmat.backends.openssl.backend import backend
 
         return backend.load_elliptic_curve_public_bytes(curve, data)
 
+    @abc.abstractmethod
+    def __eq__(self, other: object) -> bool:
+        """
+        Checks equality.
+        """
+
 
 EllipticCurvePublicKeyWithSerialization = EllipticCurvePublicKey
 
 
 class SECT571R1(EllipticCurve):
     name = "sect571r1"
     key_size = 570
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/ed25519.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x25519.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,113 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 
 from cryptography.exceptions import UnsupportedAlgorithm, _Reasons
+from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 from cryptography.hazmat.primitives import _serialization
 
-_ED25519_KEY_SIZE = 32
-_ED25519_SIG_SIZE = 64
 
-
-class Ed25519PublicKey(metaclass=abc.ABCMeta):
+class X25519PublicKey(metaclass=abc.ABCMeta):
     @classmethod
-    def from_public_bytes(cls, data: bytes) -> "Ed25519PublicKey":
+    def from_public_bytes(cls, data: bytes) -> X25519PublicKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.ed25519_supported():
+        if not backend.x25519_supported():
             raise UnsupportedAlgorithm(
-                "ed25519 is not supported by this version of OpenSSL.",
-                _Reasons.UNSUPPORTED_PUBLIC_KEY_ALGORITHM,
+                "X25519 is not supported by this version of OpenSSL.",
+                _Reasons.UNSUPPORTED_EXCHANGE_ALGORITHM,
             )
 
-        return backend.ed25519_load_public_bytes(data)
+        return backend.x25519_load_public_bytes(data)
 
     @abc.abstractmethod
     def public_bytes(
         self,
         encoding: _serialization.Encoding,
         format: _serialization.PublicFormat,
     ) -> bytes:
         """
         The serialized bytes of the public key.
         """
 
+    @abc.abstractmethod
     def public_bytes_raw(self) -> bytes:
         """
         The raw bytes of the public key.
         Equivalent to public_bytes(Raw, Raw).
         """
-        return self.public_bytes(
-            _serialization.Encoding.Raw, _serialization.PublicFormat.Raw
-        )
 
     @abc.abstractmethod
-    def verify(self, signature: bytes, data: bytes) -> None:
+    def __eq__(self, other: object) -> bool:
         """
-        Verify the signature.
+        Checks equality.
         """
 
 
-class Ed25519PrivateKey(metaclass=abc.ABCMeta):
+# For LibreSSL
+if hasattr(rust_openssl, "x25519"):
+    X25519PublicKey.register(rust_openssl.x25519.X25519PublicKey)
+
+
+class X25519PrivateKey(metaclass=abc.ABCMeta):
     @classmethod
-    def generate(cls) -> "Ed25519PrivateKey":
+    def generate(cls) -> X25519PrivateKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.ed25519_supported():
+        if not backend.x25519_supported():
             raise UnsupportedAlgorithm(
-                "ed25519 is not supported by this version of OpenSSL.",
-                _Reasons.UNSUPPORTED_PUBLIC_KEY_ALGORITHM,
+                "X25519 is not supported by this version of OpenSSL.",
+                _Reasons.UNSUPPORTED_EXCHANGE_ALGORITHM,
             )
-
-        return backend.ed25519_generate_key()
+        return backend.x25519_generate_key()
 
     @classmethod
-    def from_private_bytes(cls, data: bytes) -> "Ed25519PrivateKey":
+    def from_private_bytes(cls, data: bytes) -> X25519PrivateKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.ed25519_supported():
+        if not backend.x25519_supported():
             raise UnsupportedAlgorithm(
-                "ed25519 is not supported by this version of OpenSSL.",
-                _Reasons.UNSUPPORTED_PUBLIC_KEY_ALGORITHM,
+                "X25519 is not supported by this version of OpenSSL.",
+                _Reasons.UNSUPPORTED_EXCHANGE_ALGORITHM,
             )
 
-        return backend.ed25519_load_private_bytes(data)
+        return backend.x25519_load_private_bytes(data)
 
     @abc.abstractmethod
-    def public_key(self) -> Ed25519PublicKey:
+    def public_key(self) -> X25519PublicKey:
         """
-        The Ed25519PublicKey derived from the private key.
+        Returns the public key assosciated with this private key
         """
 
     @abc.abstractmethod
     def private_bytes(
         self,
         encoding: _serialization.Encoding,
         format: _serialization.PrivateFormat,
         encryption_algorithm: _serialization.KeySerializationEncryption,
     ) -> bytes:
         """
         The serialized bytes of the private key.
         """
 
+    @abc.abstractmethod
     def private_bytes_raw(self) -> bytes:
         """
         The raw bytes of the private key.
         Equivalent to private_bytes(Raw, Raw, NoEncryption()).
         """
-        return self.private_bytes(
-            _serialization.Encoding.Raw,
-            _serialization.PrivateFormat.Raw,
-            _serialization.NoEncryption(),
-        )
 
     @abc.abstractmethod
-    def sign(self, data: bytes) -> bytes:
+    def exchange(self, peer_public_key: X25519PublicKey) -> bytes:
         """
-        Signs the data.
+        Performs a key exchange operation using the provided peer's public key.
         """
+
+
+# For LibreSSL
+if hasattr(rust_openssl, "x25519"):
+    X25519PrivateKey.register(rust_openssl.x25519.X25519PrivateKey)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/ed448.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/ed25519.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,107 +1,118 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 
 from cryptography.exceptions import UnsupportedAlgorithm, _Reasons
+from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 from cryptography.hazmat.primitives import _serialization
 
 
-class Ed448PublicKey(metaclass=abc.ABCMeta):
+class Ed25519PublicKey(metaclass=abc.ABCMeta):
     @classmethod
-    def from_public_bytes(cls, data: bytes) -> "Ed448PublicKey":
+    def from_public_bytes(cls, data: bytes) -> Ed25519PublicKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.ed448_supported():
+        if not backend.ed25519_supported():
             raise UnsupportedAlgorithm(
-                "ed448 is not supported by this version of OpenSSL.",
+                "ed25519 is not supported by this version of OpenSSL.",
                 _Reasons.UNSUPPORTED_PUBLIC_KEY_ALGORITHM,
             )
 
-        return backend.ed448_load_public_bytes(data)
+        return backend.ed25519_load_public_bytes(data)
 
     @abc.abstractmethod
     def public_bytes(
         self,
         encoding: _serialization.Encoding,
         format: _serialization.PublicFormat,
     ) -> bytes:
         """
         The serialized bytes of the public key.
         """
 
+    @abc.abstractmethod
     def public_bytes_raw(self) -> bytes:
         """
         The raw bytes of the public key.
         Equivalent to public_bytes(Raw, Raw).
         """
-        return self.public_bytes(
-            _serialization.Encoding.Raw, _serialization.PublicFormat.Raw
-        )
 
     @abc.abstractmethod
     def verify(self, signature: bytes, data: bytes) -> None:
         """
         Verify the signature.
         """
 
+    @abc.abstractmethod
+    def __eq__(self, other: object) -> bool:
+        """
+        Checks equality.
+        """
+
+
+if hasattr(rust_openssl, "ed25519"):
+    Ed25519PublicKey.register(rust_openssl.ed25519.Ed25519PublicKey)
 
-class Ed448PrivateKey(metaclass=abc.ABCMeta):
+
+class Ed25519PrivateKey(metaclass=abc.ABCMeta):
     @classmethod
-    def generate(cls) -> "Ed448PrivateKey":
+    def generate(cls) -> Ed25519PrivateKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.ed448_supported():
+        if not backend.ed25519_supported():
             raise UnsupportedAlgorithm(
-                "ed448 is not supported by this version of OpenSSL.",
+                "ed25519 is not supported by this version of OpenSSL.",
                 _Reasons.UNSUPPORTED_PUBLIC_KEY_ALGORITHM,
             )
-        return backend.ed448_generate_key()
+
+        return backend.ed25519_generate_key()
 
     @classmethod
-    def from_private_bytes(cls, data: bytes) -> "Ed448PrivateKey":
+    def from_private_bytes(cls, data: bytes) -> Ed25519PrivateKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.ed448_supported():
+        if not backend.ed25519_supported():
             raise UnsupportedAlgorithm(
-                "ed448 is not supported by this version of OpenSSL.",
+                "ed25519 is not supported by this version of OpenSSL.",
                 _Reasons.UNSUPPORTED_PUBLIC_KEY_ALGORITHM,
             )
 
-        return backend.ed448_load_private_bytes(data)
+        return backend.ed25519_load_private_bytes(data)
 
     @abc.abstractmethod
-    def public_key(self) -> Ed448PublicKey:
+    def public_key(self) -> Ed25519PublicKey:
         """
-        The Ed448PublicKey derived from the private key.
-        """
-
-    @abc.abstractmethod
-    def sign(self, data: bytes) -> bytes:
-        """
-        Signs the data.
+        The Ed25519PublicKey derived from the private key.
         """
 
     @abc.abstractmethod
     def private_bytes(
         self,
         encoding: _serialization.Encoding,
         format: _serialization.PrivateFormat,
         encryption_algorithm: _serialization.KeySerializationEncryption,
     ) -> bytes:
         """
         The serialized bytes of the private key.
         """
 
+    @abc.abstractmethod
     def private_bytes_raw(self) -> bytes:
         """
         The raw bytes of the private key.
         Equivalent to private_bytes(Raw, Raw, NoEncryption()).
         """
-        return self.private_bytes(
-            _serialization.Encoding.Raw,
-            _serialization.PrivateFormat.Raw,
-            _serialization.NoEncryption(),
-        )
+
+    @abc.abstractmethod
+    def sign(self, data: bytes) -> bytes:
+        """
+        Signs the data.
+        """
+
+
+if hasattr(rust_openssl, "x25519"):
+    Ed25519PrivateKey.register(rust_openssl.ed25519.Ed25519PrivateKey)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/padding.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/padding.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives._asymmetric import (
     AsymmetricPadding as AsymmetricPadding,
@@ -34,15 +35,15 @@
     AUTO = _Auto()
     DIGEST_LENGTH = _DigestLength()
     name = "EMSA-PSS"
     _salt_length: typing.Union[int, _MaxLength, _Auto, _DigestLength]
 
     def __init__(
         self,
-        mgf: "MGF",
+        mgf: MGF,
         salt_length: typing.Union[int, _MaxLength, _Auto, _DigestLength],
     ) -> None:
         self._mgf = mgf
 
         if not isinstance(
             salt_length, (int, _MaxLength, _Auto, _DigestLength)
         ):
@@ -58,15 +59,15 @@
 
 
 class OAEP(AsymmetricPadding):
     name = "EME-OAEP"
 
     def __init__(
         self,
-        mgf: "MGF",
+        mgf: MGF,
         algorithm: hashes.HashAlgorithm,
         label: typing.Optional[bytes],
     ):
         if not isinstance(algorithm, hashes.HashAlgorithm):
             raise TypeError("Expected instance of hashes.HashAlgorithm.")
 
         self._mgf = mgf
@@ -85,15 +86,15 @@
         if not isinstance(algorithm, hashes.HashAlgorithm):
             raise TypeError("Expected instance of hashes.HashAlgorithm.")
 
         self._algorithm = algorithm
 
 
 def calculate_max_pss_salt_length(
-    key: typing.Union["rsa.RSAPrivateKey", "rsa.RSAPublicKey"],
+    key: typing.Union[rsa.RSAPrivateKey, rsa.RSAPublicKey],
     hash_algorithm: hashes.HashAlgorithm,
 ) -> int:
     if not isinstance(key, (rsa.RSAPrivateKey, rsa.RSAPublicKey)):
         raise TypeError("key must be an RSA public or private key")
     # bit length - 1 per RFC 3447
     emlen = (key.key_size + 6) // 8
     salt_length = emlen - hash_algorithm.digest_size - 2
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/rsa.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 from math import gcd
 
 from cryptography.hazmat.primitives import _serialization, hashes
 from cryptography.hazmat.primitives._asymmetric import AsymmetricPadding
@@ -23,15 +24,15 @@
     @abc.abstractmethod
     def key_size(self) -> int:
         """
         The bit length of the public modulus.
         """
 
     @abc.abstractmethod
-    def public_key(self) -> "RSAPublicKey":
+    def public_key(self) -> RSAPublicKey:
         """
         The RSAPublicKey associated with this private key.
         """
 
     @abc.abstractmethod
     def sign(
         self,
@@ -40,15 +41,15 @@
         algorithm: typing.Union[asym_utils.Prehashed, hashes.HashAlgorithm],
     ) -> bytes:
         """
         Signs the data.
         """
 
     @abc.abstractmethod
-    def private_numbers(self) -> "RSAPrivateNumbers":
+    def private_numbers(self) -> RSAPrivateNumbers:
         """
         Returns an RSAPrivateNumbers.
         """
 
     @abc.abstractmethod
     def private_bytes(
         self,
@@ -75,15 +76,15 @@
     @abc.abstractmethod
     def key_size(self) -> int:
         """
         The bit length of the public modulus.
         """
 
     @abc.abstractmethod
-    def public_numbers(self) -> "RSAPublicNumbers":
+    def public_numbers(self) -> RSAPublicNumbers:
         """
         Returns an RSAPublicNumbers
         """
 
     @abc.abstractmethod
     def public_bytes(
         self,
@@ -113,14 +114,20 @@
         padding: AsymmetricPadding,
         algorithm: typing.Optional[hashes.HashAlgorithm],
     ) -> bytes:
         """
         Recovers the original data from the signature.
         """
 
+    @abc.abstractmethod
+    def __eq__(self, other: object) -> bool:
+        """
+        Checks equality.
+        """
+
 
 RSAPublicKeyWithSerialization = RSAPublicKey
 
 
 def generate_private_key(
     public_exponent: int,
     key_size: int,
@@ -293,15 +300,15 @@
         self,
         p: int,
         q: int,
         d: int,
         dmp1: int,
         dmq1: int,
         iqmp: int,
-        public_numbers: "RSAPublicNumbers",
+        public_numbers: RSAPublicNumbers,
     ):
         if (
             not isinstance(p, int)
             or not isinstance(q, int)
             or not isinstance(d, int)
             or not isinstance(dmp1, int)
             or not isinstance(dmq1, int)
@@ -347,15 +354,15 @@
         return self._dmq1
 
     @property
     def iqmp(self) -> int:
         return self._iqmp
 
     @property
-    def public_numbers(self) -> "RSAPublicNumbers":
+    def public_numbers(self) -> RSAPublicNumbers:
         return self._public_numbers
 
     def private_key(
         self,
         backend: typing.Any = None,
         *,
         unsafe_skip_rsa_key_validation: bool = False,
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/types.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography import utils
 from cryptography.hazmat.primitives.asymmetric import (
     dh,
     dsa,
     ec,
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/utils.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 from cryptography.hazmat.bindings._rust import asn1
 from cryptography.hazmat.primitives import hashes
 
 decode_dss_signature = asn1.decode_dss_signature
 encode_dss_signature = asn1.encode_dss_signature
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/asymmetric/x25519.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/asymmetric/x448.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 
 from cryptography.exceptions import UnsupportedAlgorithm, _Reasons
 from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 from cryptography.hazmat.primitives import _serialization
 
 
-class X25519PublicKey(metaclass=abc.ABCMeta):
+class X448PublicKey(metaclass=abc.ABCMeta):
     @classmethod
-    def from_public_bytes(cls, data: bytes) -> "X25519PublicKey":
+    def from_public_bytes(cls, data: bytes) -> X448PublicKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.x25519_supported():
+        if not backend.x448_supported():
             raise UnsupportedAlgorithm(
-                "X25519 is not supported by this version of OpenSSL.",
+                "X448 is not supported by this version of OpenSSL.",
                 _Reasons.UNSUPPORTED_EXCHANGE_ALGORITHM,
             )
 
-        return backend.x25519_load_public_bytes(data)
+        return backend.x448_load_public_bytes(data)
 
     @abc.abstractmethod
     def public_bytes(
         self,
         encoding: _serialization.Encoding,
         format: _serialization.PublicFormat,
     ) -> bytes:
@@ -36,48 +37,53 @@
     @abc.abstractmethod
     def public_bytes_raw(self) -> bytes:
         """
         The raw bytes of the public key.
         Equivalent to public_bytes(Raw, Raw).
         """
 
+    @abc.abstractmethod
+    def __eq__(self, other: object) -> bool:
+        """
+        Checks equality.
+        """
+
 
-# For LibreSSL
-if hasattr(rust_openssl, "x25519"):
-    X25519PublicKey.register(rust_openssl.x25519.X25519PublicKey)
+if hasattr(rust_openssl, "x448"):
+    X448PublicKey.register(rust_openssl.x448.X448PublicKey)
 
 
-class X25519PrivateKey(metaclass=abc.ABCMeta):
+class X448PrivateKey(metaclass=abc.ABCMeta):
     @classmethod
-    def generate(cls) -> "X25519PrivateKey":
+    def generate(cls) -> X448PrivateKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.x25519_supported():
+        if not backend.x448_supported():
             raise UnsupportedAlgorithm(
-                "X25519 is not supported by this version of OpenSSL.",
+                "X448 is not supported by this version of OpenSSL.",
                 _Reasons.UNSUPPORTED_EXCHANGE_ALGORITHM,
             )
-        return backend.x25519_generate_key()
+        return backend.x448_generate_key()
 
     @classmethod
-    def from_private_bytes(cls, data: bytes) -> "X25519PrivateKey":
+    def from_private_bytes(cls, data: bytes) -> X448PrivateKey:
         from cryptography.hazmat.backends.openssl.backend import backend
 
-        if not backend.x25519_supported():
+        if not backend.x448_supported():
             raise UnsupportedAlgorithm(
-                "X25519 is not supported by this version of OpenSSL.",
+                "X448 is not supported by this version of OpenSSL.",
                 _Reasons.UNSUPPORTED_EXCHANGE_ALGORITHM,
             )
 
-        return backend.x25519_load_private_bytes(data)
+        return backend.x448_load_private_bytes(data)
 
     @abc.abstractmethod
-    def public_key(self) -> X25519PublicKey:
+    def public_key(self) -> X448PublicKey:
         """
-        Returns the public key assosciated with this private key
+        Returns the public key associated with this private key
         """
 
     @abc.abstractmethod
     def private_bytes(
         self,
         encoding: _serialization.Encoding,
         format: _serialization.PrivateFormat,
@@ -91,16 +97,15 @@
     def private_bytes_raw(self) -> bytes:
         """
         The raw bytes of the private key.
         Equivalent to private_bytes(Raw, Raw, NoEncryption()).
         """
 
     @abc.abstractmethod
-    def exchange(self, peer_public_key: X25519PublicKey) -> bytes:
+    def exchange(self, peer_public_key: X448PublicKey) -> bytes:
         """
         Performs a key exchange operation using the provided peer's public key.
         """
 
 
-# For LibreSSL
-if hasattr(rust_openssl, "x25519"):
-    X25519PrivateKey.register(rust_openssl.x25519.X25519PrivateKey)
+if hasattr(rust_openssl, "x448"):
+    X448PrivateKey.register(rust_openssl.x448.X448PrivateKey)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/__init__.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 from cryptography.hazmat.primitives._cipheralgorithm import (
     BlockCipherAlgorithm,
     CipherAlgorithm,
 )
 from cryptography.hazmat.primitives.ciphers.base import (
     AEADCipherContext,
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/aead.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/aead.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import os
 import typing
 
 from cryptography import exceptions, utils
 from cryptography.hazmat.backends.openssl import aead
 from cryptography.hazmat.backends.openssl.backend import backend
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/algorithms.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 from cryptography import utils
 from cryptography.hazmat.primitives.ciphers import (
     BlockCipherAlgorithm,
     CipherAlgorithm,
 )
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/base.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 
 from cryptography.exceptions import (
     AlreadyFinalized,
     AlreadyUpdated,
@@ -91,21 +92,21 @@
             mode.validate_for_algorithm(algorithm)
 
         self.algorithm = algorithm
         self.mode = mode
 
     @typing.overload
     def encryptor(
-        self: "Cipher[modes.ModeWithAuthenticationTag]",
+        self: Cipher[modes.ModeWithAuthenticationTag],
     ) -> AEADEncryptionContext:
         ...
 
     @typing.overload
     def encryptor(
-        self: "_CIPHER_TYPE",
+        self: _CIPHER_TYPE,
     ) -> CipherContext:
         ...
 
     def encryptor(self):
         if isinstance(self.mode, modes.ModeWithAuthenticationTag):
             if self.mode.tag is not None:
                 raise ValueError(
@@ -116,34 +117,34 @@
         ctx = backend.create_symmetric_encryption_ctx(
             self.algorithm, self.mode
         )
         return self._wrap_ctx(ctx, encrypt=True)
 
     @typing.overload
     def decryptor(
-        self: "Cipher[modes.ModeWithAuthenticationTag]",
+        self: Cipher[modes.ModeWithAuthenticationTag],
     ) -> AEADDecryptionContext:
         ...
 
     @typing.overload
     def decryptor(
-        self: "_CIPHER_TYPE",
+        self: _CIPHER_TYPE,
     ) -> CipherContext:
         ...
 
     def decryptor(self):
         from cryptography.hazmat.backends.openssl.backend import backend
 
         ctx = backend.create_symmetric_decryption_ctx(
             self.algorithm, self.mode
         )
         return self._wrap_ctx(ctx, encrypt=False)
 
     def _wrap_ctx(
-        self, ctx: "_BackendCipherContext", encrypt: bool
+        self, ctx: _BackendCipherContext, encrypt: bool
     ) -> typing.Union[
         AEADEncryptionContext, AEADDecryptionContext, CipherContext
     ]:
         if isinstance(self.mode, modes.ModeWithAuthenticationTag):
             if encrypt:
                 return _AEADEncryptionContext(ctx)
             else:
@@ -160,17 +161,17 @@
         modes.ECB,
         modes.ModeWithInitializationVector,
     ]
 ]
 
 
 class _CipherContext(CipherContext):
-    _ctx: typing.Optional["_BackendCipherContext"]
+    _ctx: typing.Optional[_BackendCipherContext]
 
-    def __init__(self, ctx: "_BackendCipherContext") -> None:
+    def __init__(self, ctx: _BackendCipherContext) -> None:
         self._ctx = ctx
 
     def update(self, data: bytes) -> bytes:
         if self._ctx is None:
             raise AlreadyFinalized("Context was already finalized.")
         return self._ctx.update(data)
 
@@ -184,18 +185,18 @@
             raise AlreadyFinalized("Context was already finalized.")
         data = self._ctx.finalize()
         self._ctx = None
         return data
 
 
 class _AEADCipherContext(AEADCipherContext):
-    _ctx: typing.Optional["_BackendCipherContext"]
+    _ctx: typing.Optional[_BackendCipherContext]
     _tag: typing.Optional[bytes]
 
-    def __init__(self, ctx: "_BackendCipherContext") -> None:
+    def __init__(self, ctx: _BackendCipherContext) -> None:
         self._ctx = ctx
         self._bytes_processed = 0
         self._aad_bytes_processed = 0
         self._tag = None
         self._updated = False
 
     def _check_limit(self, data_size: int) -> None:
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/ciphers/modes.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/ciphers/modes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import UnsupportedAlgorithm, _Reasons
 from cryptography.hazmat.primitives._cipheralgorithm import (
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/cmac.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/cmac.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import AlreadyFinalized
 from cryptography.hazmat.primitives import ciphers
 
 if typing.TYPE_CHECKING:
     from cryptography.hazmat.backends.openssl.cmac import _CMACContext
 
 
 class CMAC:
-    _ctx: typing.Optional["_CMACContext"]
+    _ctx: typing.Optional[_CMACContext]
     _algorithm: ciphers.BlockCipherAlgorithm
 
     def __init__(
         self,
         algorithm: ciphers.BlockCipherAlgorithm,
         backend: typing.Any = None,
-        ctx: typing.Optional["_CMACContext"] = None,
+        ctx: typing.Optional[_CMACContext] = None,
     ) -> None:
         if not isinstance(algorithm, ciphers.BlockCipherAlgorithm):
             raise TypeError("Expected instance of BlockCipherAlgorithm.")
         self._algorithm = algorithm
 
         if ctx is None:
             from cryptography.hazmat.backends.openssl.backend import (
@@ -54,11 +55,11 @@
         utils._check_bytes("signature", signature)
         if self._ctx is None:
             raise AlreadyFinalized("Context was already finalized.")
 
         ctx, self._ctx = self._ctx, None
         ctx.verify(signature)
 
-    def copy(self) -> "CMAC":
+    def copy(self) -> CMAC:
         if self._ctx is None:
             raise AlreadyFinalized("Context was already finalized.")
         return CMAC(self._algorithm, ctx=self._ctx.copy())
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/hashes.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/hashes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,41 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import abc
 import typing
 
-from cryptography import utils
-from cryptography.exceptions import AlreadyFinalized
+from cryptography.hazmat.bindings._rust import openssl as rust_openssl
+
+__all__ = [
+    "HashAlgorithm",
+    "HashContext",
+    "Hash",
+    "ExtendableOutputFunction",
+    "SHA1",
+    "SHA512_224",
+    "SHA512_256",
+    "SHA224",
+    "SHA256",
+    "SHA384",
+    "SHA512",
+    "SHA3_224",
+    "SHA3_256",
+    "SHA3_384",
+    "SHA3_512",
+    "SHAKE128",
+    "SHAKE256",
+    "MD5",
+    "BLAKE2b",
+    "BLAKE2s",
+    "SM3",
+]
 
 
 class HashAlgorithm(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
     def name(self) -> str:
         """
@@ -50,71 +75,30 @@
     @abc.abstractmethod
     def finalize(self) -> bytes:
         """
         Finalizes the hash context and returns the hash digest as bytes.
         """
 
     @abc.abstractmethod
-    def copy(self) -> "HashContext":
+    def copy(self) -> HashContext:
         """
         Return a HashContext that is a copy of the current context.
         """
 
 
+Hash = rust_openssl.hashes.Hash
+HashContext.register(Hash)
+
+
 class ExtendableOutputFunction(metaclass=abc.ABCMeta):
     """
     An interface for extendable output functions.
     """
 
 
-class Hash(HashContext):
-    _ctx: typing.Optional[HashContext]
-
-    def __init__(
-        self,
-        algorithm: HashAlgorithm,
-        backend: typing.Any = None,
-        ctx: typing.Optional["HashContext"] = None,
-    ) -> None:
-        if not isinstance(algorithm, HashAlgorithm):
-            raise TypeError("Expected instance of hashes.HashAlgorithm.")
-        self._algorithm = algorithm
-
-        if ctx is None:
-            from cryptography.hazmat.backends.openssl.backend import (
-                backend as ossl,
-            )
-
-            self._ctx = ossl.create_hash_ctx(self.algorithm)
-        else:
-            self._ctx = ctx
-
-    @property
-    def algorithm(self) -> HashAlgorithm:
-        return self._algorithm
-
-    def update(self, data: bytes) -> None:
-        if self._ctx is None:
-            raise AlreadyFinalized("Context was already finalized.")
-        utils._check_byteslike("data", data)
-        self._ctx.update(data)
-
-    def copy(self) -> "Hash":
-        if self._ctx is None:
-            raise AlreadyFinalized("Context was already finalized.")
-        return Hash(self.algorithm, ctx=self._ctx.copy())
-
-    def finalize(self) -> bytes:
-        if self._ctx is None:
-            raise AlreadyFinalized("Context was already finalized.")
-        digest = self._ctx.finalize()
-        self._ctx = None
-        return digest
-
-
 class SHA1(HashAlgorithm):
     name = "sha1"
     digest_size = 20
     block_size = 64
 
 
 class SHA512_224(HashAlgorithm):  # noqa: N801
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/__init__.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 
 
 class KeyDerivationFunction(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def derive(self, key_material: bytes) -> bytes:
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/concatkdf.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/concatkdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import AlreadyFinalized, InvalidKey
 from cryptography.hazmat.primitives import constant_time, hashes, hmac
 from cryptography.hazmat.primitives.kdf import KeyDerivationFunction
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/hkdf.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/hkdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import AlreadyFinalized, InvalidKey
 from cryptography.hazmat.primitives import constant_time, hashes, hmac
 from cryptography.hazmat.primitives.kdf import KeyDerivationFunction
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/kbkdf.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/kbkdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import (
     AlreadyFinalized,
     InvalidKey,
     UnsupportedAlgorithm,
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/pbkdf2.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/pbkdf2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import (
     AlreadyFinalized,
     InvalidKey,
     UnsupportedAlgorithm,
     _Reasons,
 )
+from cryptography.hazmat.bindings._rust import openssl as rust_openssl
 from cryptography.hazmat.primitives import constant_time, hashes
 from cryptography.hazmat.primitives.kdf import KeyDerivationFunction
 
 
 class PBKDF2HMAC(KeyDerivationFunction):
     def __init__(
         self,
@@ -44,22 +46,19 @@
         self._iterations = iterations
 
     def derive(self, key_material: bytes) -> bytes:
         if self._used:
             raise AlreadyFinalized("PBKDF2 instances can only be used once.")
         self._used = True
 
-        utils._check_byteslike("key_material", key_material)
-        from cryptography.hazmat.backends.openssl.backend import backend
-
-        return backend.derive_pbkdf2_hmac(
+        return rust_openssl.kdf.derive_pbkdf2_hmac(
+            key_material,
             self._algorithm,
-            self._length,
             self._salt,
             self._iterations,
-            key_material,
+            self._length,
         )
 
     def verify(self, key_material: bytes, expected_key: bytes) -> None:
         derived_key = self.derive(key_material)
         if not constant_time.bytes_eq(derived_key, expected_key):
             raise InvalidKey("Keys do not match.")
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/kdf/x963kdf.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/kdf/x963kdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import AlreadyFinalized, InvalidKey
 from cryptography.hazmat.primitives import constant_time, hashes
 from cryptography.hazmat.primitives.kdf import KeyDerivationFunction
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/keywrap.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/keywrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import ECB
 from cryptography.hazmat.primitives.constant_time import bytes_eq
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/padding.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/padding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import typing
 
 from cryptography import utils
 from cryptography.exceptions import AlreadyFinalized
 from cryptography.hazmat.bindings._rust import (
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/__init__.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 from cryptography.hazmat.primitives._serialization import (
     BestAvailableEncryption,
     Encoding,
     KeySerializationEncryption,
     NoEncryption,
     ParameterFormat,
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/base.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import typing
 
 from cryptography.hazmat.primitives.asymmetric import dh
 from cryptography.hazmat.primitives.asymmetric.types import (
     PrivateKeyTypes,
     PublicKeyTypes,
@@ -32,15 +33,15 @@
     from cryptography.hazmat.backends.openssl.backend import backend as ossl
 
     return ossl.load_pem_public_key(data)
 
 
 def load_pem_parameters(
     data: bytes, backend: typing.Any = None
-) -> "dh.DHParameters":
+) -> dh.DHParameters:
     from cryptography.hazmat.backends.openssl.backend import backend as ossl
 
     return ossl.load_pem_parameters(data)
 
 
 def load_der_private_key(
     data: bytes,
@@ -62,11 +63,11 @@
     from cryptography.hazmat.backends.openssl.backend import backend as ossl
 
     return ossl.load_der_public_key(data)
 
 
 def load_der_parameters(
     data: bytes, backend: typing.Any = None
-) -> "dh.DHParameters":
+) -> dh.DHParameters:
     from cryptography.hazmat.backends.openssl.backend import backend as ossl
 
     return ossl.load_der_parameters(data)
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/pkcs12.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs12.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography import x509
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives._serialization import PBES as PBES
 from cryptography.hazmat.primitives.asymmetric import (
     dsa,
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/pkcs7.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/pkcs7.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import email.base64mime
 import email.generator
 import email.message
 import email.policy
 import io
 import typing
 
@@ -69,27 +71,27 @@
         ] = [],
         additional_certs: typing.List[x509.Certificate] = [],
     ):
         self._data = data
         self._signers = signers
         self._additional_certs = additional_certs
 
-    def set_data(self, data: bytes) -> "PKCS7SignatureBuilder":
+    def set_data(self, data: bytes) -> PKCS7SignatureBuilder:
         _check_byteslike("data", data)
         if self._data is not None:
             raise ValueError("data may only be set once")
 
         return PKCS7SignatureBuilder(data, self._signers)
 
     def add_signer(
         self,
         certificate: x509.Certificate,
         private_key: PKCS7PrivateKeyTypes,
         hash_algorithm: PKCS7HashTypes,
-    ) -> "PKCS7SignatureBuilder":
+    ) -> PKCS7SignatureBuilder:
         if not isinstance(
             hash_algorithm,
             (
                 hashes.SHA224,
                 hashes.SHA256,
                 hashes.SHA384,
                 hashes.SHA512,
@@ -110,15 +112,15 @@
         return PKCS7SignatureBuilder(
             self._data,
             self._signers + [(certificate, private_key, hash_algorithm)],
         )
 
     def add_certificate(
         self, certificate: x509.Certificate
-    ) -> "PKCS7SignatureBuilder":
+    ) -> PKCS7SignatureBuilder:
         if not isinstance(certificate, x509.Certificate):
             raise TypeError("certificate must be a x509.Certificate")
 
         return PKCS7SignatureBuilder(
             self._data, self._signers, self._additional_certs + [certificate]
         )
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/serialization/ssh.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/serialization/ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import binascii
 import enum
 import os
 import re
 import typing
 import warnings
 from base64 import encodebytes as _base64_encode
+from dataclasses import dataclass
 
 from cryptography import utils
 from cryptography.exceptions import UnsupportedAlgorithm
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import (
     dsa,
     ec,
     ed25519,
     padding,
     rsa,
 )
 from cryptography.hazmat.primitives.asymmetric import utils as asym_utils
-from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.primitives.ciphers import (
+    AEADDecryptionContext,
+    Cipher,
+    algorithms,
+    modes,
+)
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     KeySerializationEncryption,
     NoEncryption,
     PrivateFormat,
     PublicFormat,
     _KeySerializationEncryption,
@@ -73,38 +80,71 @@
 
 # re is only way to work on bytes-like data
 _PEM_RC = re.compile(_SK_START + b"(.*?)" + _SK_END, re.DOTALL)
 
 # padding for max blocksize
 _PADDING = memoryview(bytearray(range(1, 1 + 16)))
 
+
+@dataclass
+class _SSHCipher:
+    alg: typing.Type[algorithms.AES]
+    key_len: int
+    mode: typing.Union[
+        typing.Type[modes.CTR],
+        typing.Type[modes.CBC],
+        typing.Type[modes.GCM],
+    ]
+    block_len: int
+    iv_len: int
+    tag_len: typing.Optional[int]
+    is_aead: bool
+
+
 # ciphers that are actually used in key wrapping
-_SSH_CIPHERS: typing.Dict[
-    bytes,
-    typing.Tuple[
-        typing.Type[algorithms.AES],
-        int,
-        typing.Union[typing.Type[modes.CTR], typing.Type[modes.CBC]],
-        int,
-    ],
-] = {
-    b"aes256-ctr": (algorithms.AES, 32, modes.CTR, 16),
-    b"aes256-cbc": (algorithms.AES, 32, modes.CBC, 16),
+_SSH_CIPHERS: typing.Dict[bytes, _SSHCipher] = {
+    b"aes256-ctr": _SSHCipher(
+        alg=algorithms.AES,
+        key_len=32,
+        mode=modes.CTR,
+        block_len=16,
+        iv_len=16,
+        tag_len=None,
+        is_aead=False,
+    ),
+    b"aes256-cbc": _SSHCipher(
+        alg=algorithms.AES,
+        key_len=32,
+        mode=modes.CBC,
+        block_len=16,
+        iv_len=16,
+        tag_len=None,
+        is_aead=False,
+    ),
+    b"aes256-gcm@openssh.com": _SSHCipher(
+        alg=algorithms.AES,
+        key_len=32,
+        mode=modes.GCM,
+        block_len=16,
+        iv_len=12,
+        tag_len=16,
+        is_aead=True,
+    ),
 }
 
 # map local curve name to key type
 _ECDSA_KEY_TYPE = {
     "secp256r1": _ECDSA_NISTP256,
     "secp384r1": _ECDSA_NISTP384,
     "secp521r1": _ECDSA_NISTP521,
 }
 
 
 def _get_ssh_key_type(
-    key: typing.Union["SSHPrivateKeyTypes", "SSHPublicKeyTypes"]
+    key: typing.Union[SSHPrivateKeyTypes, SSHPublicKeyTypes]
 ) -> bytes:
     if isinstance(key, ec.EllipticCurvePrivateKey):
         key_type = _ecdsa_key_type(key.public_key())
     elif isinstance(key, ec.EllipticCurvePublicKey):
         key_type = _ecdsa_key_type(key)
     elif isinstance(key, (rsa.RSAPrivateKey, rsa.RSAPublicKey)):
         key_type = _SSH_RSA
@@ -151,22 +191,27 @@
 
 
 def _init_cipher(
     ciphername: bytes,
     password: typing.Optional[bytes],
     salt: bytes,
     rounds: int,
-) -> Cipher[typing.Union[modes.CBC, modes.CTR]]:
+) -> Cipher[typing.Union[modes.CBC, modes.CTR, modes.GCM]]:
     """Generate key + iv and return cipher."""
     if not password:
         raise ValueError("Key is password-protected.")
 
-    algo, key_len, mode, iv_len = _SSH_CIPHERS[ciphername]
-    seed = _bcrypt_kdf(password, salt, key_len + iv_len, rounds, True)
-    return Cipher(algo(seed[:key_len]), mode(seed[key_len:]))
+    ciph = _SSH_CIPHERS[ciphername]
+    seed = _bcrypt_kdf(
+        password, salt, ciph.key_len + ciph.iv_len, rounds, True
+    )
+    return Cipher(
+        ciph.alg(seed[: ciph.key_len]),
+        ciph.mode(seed[ciph.key_len :]),
+    )
 
 
 def _get_u32(data: memoryview) -> typing.Tuple[int, memoryview]:
     """Uint32"""
     if len(data) < 4:
         raise ValueError("Invalid data")
     return int.from_bytes(data[:4], byteorder="big"), data[4:]
@@ -225,15 +270,15 @@
         """Big-endian uint32"""
         self.flist.append(val.to_bytes(length=4, byteorder="big"))
 
     def put_u64(self, val: int) -> None:
         """Big-endian uint64"""
         self.flist.append(val.to_bytes(length=8, byteorder="big"))
 
-    def put_sshstr(self, val: typing.Union[bytes, "_FragList"]) -> None:
+    def put_sshstr(self, val: typing.Union[bytes, _FragList]) -> None:
         """Bytes prefixed with u32 length"""
         if isinstance(val, (bytes, memoryview, bytearray)):
             self.put_u32(len(val))
             self.flist.append(val)
         else:
             self.put_u32(val.size())
             self.flist.extend(val.flist)
@@ -599,34 +644,52 @@
     # load public key data
     pubdata, data = _get_sshstr(data)
     pub_key_type, pubdata = _get_sshstr(pubdata)
     kformat = _lookup_kformat(pub_key_type)
     pubfields, pubdata = kformat.get_public(pubdata)
     _check_empty(pubdata)
 
-    # load secret data
-    edata, data = _get_sshstr(data)
-    _check_empty(data)
-
     if (ciphername, kdfname) != (_NONE, _NONE):
         ciphername_bytes = ciphername.tobytes()
         if ciphername_bytes not in _SSH_CIPHERS:
             raise UnsupportedAlgorithm(
                 f"Unsupported cipher: {ciphername_bytes!r}"
             )
         if kdfname != _BCRYPT:
             raise UnsupportedAlgorithm(f"Unsupported KDF: {kdfname!r}")
-        blklen = _SSH_CIPHERS[ciphername_bytes][3]
+        blklen = _SSH_CIPHERS[ciphername_bytes].block_len
+        tag_len = _SSH_CIPHERS[ciphername_bytes].tag_len
+        # load secret data
+        edata, data = _get_sshstr(data)
+        # see https://bugzilla.mindrot.org/show_bug.cgi?id=3553 for
+        # information about how OpenSSH handles AEAD tags
+        if _SSH_CIPHERS[ciphername_bytes].is_aead:
+            tag = bytes(data)
+            if len(tag) != tag_len:
+                raise ValueError("Corrupt data: invalid tag length for cipher")
+        else:
+            _check_empty(data)
         _check_block_size(edata, blklen)
         salt, kbuf = _get_sshstr(kdfoptions)
         rounds, kbuf = _get_u32(kbuf)
         _check_empty(kbuf)
         ciph = _init_cipher(ciphername_bytes, password, salt.tobytes(), rounds)
-        edata = memoryview(ciph.decryptor().update(edata))
+        dec = ciph.decryptor()
+        edata = memoryview(dec.update(edata))
+        if _SSH_CIPHERS[ciphername_bytes].is_aead:
+            assert isinstance(dec, AEADDecryptionContext)
+            _check_empty(dec.finalize_with_tag(tag))
+        else:
+            # _check_block_size requires data to be a full block so there
+            # should be no output from finalize
+            _check_empty(dec.finalize())
     else:
+        # load secret data
+        edata, data = _get_sshstr(data)
+        _check_empty(data)
         blklen = 8
         _check_block_size(edata, blklen)
     ck1, edata = _get_u32(edata)
     ck2, edata = _get_u32(edata)
     if ck1 != ck2:
         raise ValueError("Corrupt data: broken checksum")
 
@@ -671,15 +734,15 @@
     key_type = _get_ssh_key_type(private_key)
     kformat = _lookup_kformat(key_type)
 
     # setup parameters
     f_kdfoptions = _FragList()
     if password:
         ciphername = _DEFAULT_CIPHER
-        blklen = _SSH_CIPHERS[ciphername][3]
+        blklen = _SSH_CIPHERS[ciphername].block_len
         kdfname = _BCRYPT
         rounds = _DEFAULT_ROUNDS
         if (
             isinstance(encryption_algorithm, _KeySerializationEncryption)
             and encryption_algorithm._kdf_rounds is not None
         ):
             rounds = encryption_algorithm._kdf_rounds
@@ -1080,15 +1143,15 @@
         self._valid_before = _valid_before
         self._valid_after = _valid_after
         self._critical_options = _critical_options
         self._extensions = _extensions
 
     def public_key(
         self, public_key: SSHCertPublicKeyTypes
-    ) -> "SSHCertificateBuilder":
+    ) -> SSHCertificateBuilder:
         if not isinstance(
             public_key,
             (
                 ec.EllipticCurvePublicKey,
                 rsa.RSAPublicKey,
                 ed25519.Ed25519PublicKey,
             ),
@@ -1106,15 +1169,15 @@
             _valid_for_all_principals=self._valid_for_all_principals,
             _valid_before=self._valid_before,
             _valid_after=self._valid_after,
             _critical_options=self._critical_options,
             _extensions=self._extensions,
         )
 
-    def serial(self, serial: int) -> "SSHCertificateBuilder":
+    def serial(self, serial: int) -> SSHCertificateBuilder:
         if not isinstance(serial, int):
             raise TypeError("serial must be an integer")
         if not 0 <= serial < 2**64:
             raise ValueError("serial must be between 0 and 2**64")
         if self._serial is not None:
             raise ValueError("serial already set")
 
@@ -1127,15 +1190,15 @@
             _valid_for_all_principals=self._valid_for_all_principals,
             _valid_before=self._valid_before,
             _valid_after=self._valid_after,
             _critical_options=self._critical_options,
             _extensions=self._extensions,
         )
 
-    def type(self, type: SSHCertificateType) -> "SSHCertificateBuilder":
+    def type(self, type: SSHCertificateType) -> SSHCertificateBuilder:
         if not isinstance(type, SSHCertificateType):
             raise TypeError("type must be an SSHCertificateType")
         if self._type is not None:
             raise ValueError("type already set")
 
         return SSHCertificateBuilder(
             _public_key=self._public_key,
@@ -1146,15 +1209,15 @@
             _valid_for_all_principals=self._valid_for_all_principals,
             _valid_before=self._valid_before,
             _valid_after=self._valid_after,
             _critical_options=self._critical_options,
             _extensions=self._extensions,
         )
 
-    def key_id(self, key_id: bytes) -> "SSHCertificateBuilder":
+    def key_id(self, key_id: bytes) -> SSHCertificateBuilder:
         if not isinstance(key_id, bytes):
             raise TypeError("key_id must be bytes")
         if self._key_id is not None:
             raise ValueError("key_id already set")
 
         return SSHCertificateBuilder(
             _public_key=self._public_key,
@@ -1167,15 +1230,15 @@
             _valid_after=self._valid_after,
             _critical_options=self._critical_options,
             _extensions=self._extensions,
         )
 
     def valid_principals(
         self, valid_principals: typing.List[bytes]
-    ) -> "SSHCertificateBuilder":
+    ) -> SSHCertificateBuilder:
         if self._valid_for_all_principals:
             raise ValueError(
                 "Principals can't be set because the cert is valid "
                 "for all principals"
             )
         if (
             not all(isinstance(x, bytes) for x in valid_principals)
@@ -1225,15 +1288,15 @@
             _valid_after=self._valid_after,
             _critical_options=self._critical_options,
             _extensions=self._extensions,
         )
 
     def valid_before(
         self, valid_before: typing.Union[int, float]
-    ) -> "SSHCertificateBuilder":
+    ) -> SSHCertificateBuilder:
         if not isinstance(valid_before, (int, float)):
             raise TypeError("valid_before must be an int or float")
         valid_before = int(valid_before)
         if valid_before < 0 or valid_before >= 2**64:
             raise ValueError("valid_before must [0, 2**64)")
         if self._valid_before is not None:
             raise ValueError("valid_before already set")
@@ -1249,15 +1312,15 @@
             _valid_after=self._valid_after,
             _critical_options=self._critical_options,
             _extensions=self._extensions,
         )
 
     def valid_after(
         self, valid_after: typing.Union[int, float]
-    ) -> "SSHCertificateBuilder":
+    ) -> SSHCertificateBuilder:
         if not isinstance(valid_after, (int, float)):
             raise TypeError("valid_after must be an int or float")
         valid_after = int(valid_after)
         if valid_after < 0 or valid_after >= 2**64:
             raise ValueError("valid_after must [0, 2**64)")
         if self._valid_after is not None:
             raise ValueError("valid_after already set")
@@ -1273,15 +1336,15 @@
             _valid_after=valid_after,
             _critical_options=self._critical_options,
             _extensions=self._extensions,
         )
 
     def add_critical_option(
         self, name: bytes, value: bytes
-    ) -> "SSHCertificateBuilder":
+    ) -> SSHCertificateBuilder:
         if not isinstance(name, bytes) or not isinstance(value, bytes):
             raise TypeError("name and value must be bytes")
         # This is O(n**2)
         if name in [name for name, _ in self._critical_options]:
             raise ValueError("Duplicate critical option name")
 
         return SSHCertificateBuilder(
@@ -1295,15 +1358,15 @@
             _valid_after=self._valid_after,
             _critical_options=self._critical_options + [(name, value)],
             _extensions=self._extensions,
         )
 
     def add_extension(
         self, name: bytes, value: bytes
-    ) -> "SSHCertificateBuilder":
+    ) -> SSHCertificateBuilder:
         if not isinstance(name, bytes) or not isinstance(value, bytes):
             raise TypeError("name and value must be bytes")
         # This is O(n**2)
         if name in [name for name, _ in self._extensions]:
             raise ValueError("Duplicate extension name")
 
         return SSHCertificateBuilder(
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/twofactor/hotp.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/hotp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import base64
 import typing
 from urllib.parse import quote, urlencode
 
 from cryptography.hazmat.primitives import constant_time, hmac
 from cryptography.hazmat.primitives.hashes import SHA1, SHA256, SHA512
 from cryptography.hazmat.primitives.twofactor import InvalidToken
 
 HOTPHashTypes = typing.Union[SHA1, SHA256, SHA512]
 
 
 def _generate_uri(
-    hotp: "HOTP",
+    hotp: HOTP,
     type_name: str,
     account_name: str,
     issuer: typing.Optional[str],
     extra_parameters: typing.List[typing.Tuple[str, int]],
 ) -> str:
     parameters = [
         ("digits", hotp._length),
```

### Comparing `cryptography-40.0.2/src/cryptography/hazmat/primitives/twofactor/totp.py` & `cryptography-41.0.0/src/cryptography/hazmat/primitives/twofactor/totp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import typing
 
 from cryptography.hazmat.primitives import constant_time
 from cryptography.hazmat.primitives.twofactor import InvalidToken
 from cryptography.hazmat.primitives.twofactor.hotp import (
     HOTP,
     HOTPHashTypes,
```

### Comparing `cryptography-40.0.2/src/cryptography/utils.py` & `cryptography-41.0.0/src/cryptography/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import enum
 import sys
 import types
 import typing
 import warnings
 
@@ -17,16 +18,16 @@
 
 
 # Several APIs were deprecated with no specific end-of-life date because of the
 # ubiquity of their use. They should not be removed until we agree on when that
 # cycle ends.
 DeprecatedIn36 = CryptographyDeprecationWarning
 DeprecatedIn37 = CryptographyDeprecationWarning
-DeprecatedIn39 = CryptographyDeprecationWarning
 DeprecatedIn40 = CryptographyDeprecationWarning
+DeprecatedIn41 = CryptographyDeprecationWarning
 
 
 def _check_bytes(name: str, value: bytes) -> None:
     if not isinstance(value, bytes):
         raise TypeError(f"{name} must be bytes")
 
 
@@ -39,19 +40,19 @@
 
 def int_to_bytes(integer: int, length: typing.Optional[int] = None) -> bytes:
     return integer.to_bytes(
         length or (integer.bit_length() + 7) // 8 or 1, "big"
     )
 
 
-def _extract_buffer_length(obj: typing.Any) -> typing.Tuple[int, int]:
+def _extract_buffer_length(obj: typing.Any) -> typing.Tuple[typing.Any, int]:
     from cryptography.hazmat.bindings._rust import _openssl
 
     buf = _openssl.ffi.from_buffer(obj)
-    return int(_openssl.ffi.cast("uintptr_t", buf)), len(buf)
+    return buf, int(_openssl.ffi.cast("uintptr_t", buf))
 
 
 class InterfaceNotImplemented(Exception):
     pass
 
 
 class _DeprecatedValue:
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/__init__.py` & `cryptography-41.0.0/src/cryptography/x509/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 from cryptography.x509 import certificate_transparency
 from cryptography.x509.base import (
     Attribute,
     AttributeNotFound,
     Attributes,
     Certificate,
@@ -48,16 +49,18 @@
     FreshestCRL,
     GeneralNames,
     InhibitAnyPolicy,
     InvalidityDate,
     IssuerAlternativeName,
     IssuingDistributionPoint,
     KeyUsage,
+    MSCertificateTemplate,
     NameConstraints,
     NoticeReference,
+    OCSPAcceptableResponses,
     OCSPNoCheck,
     OCSPNonce,
     PolicyConstraints,
     PolicyInformation,
     PrecertificateSignedCertificateTimestamps,
     PrecertPoison,
     ReasonFlags,
@@ -192,14 +195,15 @@
     "Extensions",
     "Extension",
     "ExtendedKeyUsage",
     "FreshestCRL",
     "IssuingDistributionPoint",
     "TLSFeature",
     "TLSFeatureType",
+    "OCSPAcceptableResponses",
     "OCSPNoCheck",
     "BasicConstraints",
     "CRLNumber",
     "KeyUsage",
     "AuthorityInformationAccess",
     "SubjectInformationAccess",
     "AccessDescription",
@@ -243,8 +247,9 @@
     "PolicyConstraints",
     "PrecertificateSignedCertificateTimestamps",
     "PrecertPoison",
     "OCSPNonce",
     "SignedCertificateTimestamps",
     "SignatureAlgorithmOID",
     "NameOID",
+    "MSCertificateTemplate",
 ]
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/base.py` & `cryptography-41.0.0/src/cryptography/x509/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import datetime
 import os
 import typing
 
 from cryptography import utils
 from cryptography.hazmat.bindings._rust import x509 as rust_x509
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import (
     dsa,
     ec,
     ed448,
     ed25519,
+    padding,
     rsa,
     x448,
     x25519,
 )
 from cryptography.hazmat.primitives.asymmetric.types import (
     CertificateIssuerPrivateKeyTypes,
     CertificateIssuerPublicKeyTypes,
@@ -229,14 +231,23 @@
     def signature_algorithm_oid(self) -> ObjectIdentifier:
         """
         Returns the ObjectIdentifier of the signature algorithm.
         """
 
     @property
     @abc.abstractmethod
+    def signature_algorithm_parameters(
+        self,
+    ) -> typing.Union[None, padding.PSS, padding.PKCS1v15, ec.ECDSA]:
+        """
+        Returns the signature algorithm parameters.
+        """
+
+    @property
+    @abc.abstractmethod
     def extensions(self) -> Extensions:
         """
         Returns an Extensions object.
         """
 
     @property
     @abc.abstractmethod
@@ -275,15 +286,15 @@
     @abc.abstractmethod
     def public_bytes(self, encoding: serialization.Encoding) -> bytes:
         """
         Serializes the certificate to PEM or DER format.
         """
 
     @abc.abstractmethod
-    def verify_directly_issued_by(self, issuer: "Certificate") -> None:
+    def verify_directly_issued_by(self, issuer: Certificate) -> None:
         """
         This method verifies that certificate issuer name matches the
         issuer subject name and that the certificate is signed by the
         issuer's private key. No other validation is performed.
         """
 
 
@@ -623,29 +634,29 @@
         """
         Creates an empty X.509 certificate request (v1).
         """
         self._subject_name = subject_name
         self._extensions = extensions
         self._attributes = attributes
 
-    def subject_name(self, name: Name) -> "CertificateSigningRequestBuilder":
+    def subject_name(self, name: Name) -> CertificateSigningRequestBuilder:
         """
         Sets the certificate requestor's distinguished name.
         """
         if not isinstance(name, Name):
             raise TypeError("Expecting x509.Name object.")
         if self._subject_name is not None:
             raise ValueError("The subject name may only be set once.")
         return CertificateSigningRequestBuilder(
             name, self._extensions, self._attributes
         )
 
     def add_extension(
         self, extval: ExtensionType, critical: bool
-    ) -> "CertificateSigningRequestBuilder":
+    ) -> CertificateSigningRequestBuilder:
         """
         Adds an X.509 extension to the certificate request.
         """
         if not isinstance(extval, ExtensionType):
             raise TypeError("extension must be an ExtensionType")
 
         extension = Extension(extval.oid, critical, extval)
@@ -659,15 +670,15 @@
 
     def add_attribute(
         self,
         oid: ObjectIdentifier,
         value: bytes,
         *,
         _tag: typing.Optional[_ASN1Type] = None,
-    ) -> "CertificateSigningRequestBuilder":
+    ) -> CertificateSigningRequestBuilder:
         """
         Adds an X.509 attribute with an OID and associated value.
         """
         if not isinstance(oid, ObjectIdentifier):
             raise TypeError("oid must be an ObjectIdentifier")
 
         if not isinstance(value, bytes):
@@ -721,15 +732,15 @@
         self._subject_name = subject_name
         self._public_key = public_key
         self._serial_number = serial_number
         self._not_valid_before = not_valid_before
         self._not_valid_after = not_valid_after
         self._extensions = extensions
 
-    def issuer_name(self, name: Name) -> "CertificateBuilder":
+    def issuer_name(self, name: Name) -> CertificateBuilder:
         """
         Sets the CA's distinguished name.
         """
         if not isinstance(name, Name):
             raise TypeError("Expecting x509.Name object.")
         if self._issuer_name is not None:
             raise ValueError("The issuer name may only be set once.")
@@ -739,15 +750,15 @@
             self._public_key,
             self._serial_number,
             self._not_valid_before,
             self._not_valid_after,
             self._extensions,
         )
 
-    def subject_name(self, name: Name) -> "CertificateBuilder":
+    def subject_name(self, name: Name) -> CertificateBuilder:
         """
         Sets the requestor's distinguished name.
         """
         if not isinstance(name, Name):
             raise TypeError("Expecting x509.Name object.")
         if self._subject_name is not None:
             raise ValueError("The subject name may only be set once.")
@@ -760,15 +771,15 @@
             self._not_valid_after,
             self._extensions,
         )
 
     def public_key(
         self,
         key: CertificatePublicKeyTypes,
-    ) -> "CertificateBuilder":
+    ) -> CertificateBuilder:
         """
         Sets the requestor's public key (as found in the signing request).
         """
         if not isinstance(
             key,
             (
                 dsa.DSAPublicKey,
@@ -794,15 +805,15 @@
             key,
             self._serial_number,
             self._not_valid_before,
             self._not_valid_after,
             self._extensions,
         )
 
-    def serial_number(self, number: int) -> "CertificateBuilder":
+    def serial_number(self, number: int) -> CertificateBuilder:
         """
         Sets the certificate serial number.
         """
         if not isinstance(number, int):
             raise TypeError("Serial number must be of integral type.")
         if self._serial_number is not None:
             raise ValueError("The serial number may only be set once.")
@@ -821,17 +832,15 @@
             self._public_key,
             number,
             self._not_valid_before,
             self._not_valid_after,
             self._extensions,
         )
 
-    def not_valid_before(
-        self, time: datetime.datetime
-    ) -> "CertificateBuilder":
+    def not_valid_before(self, time: datetime.datetime) -> CertificateBuilder:
         """
         Sets the certificate activation time.
         """
         if not isinstance(time, datetime.datetime):
             raise TypeError("Expecting datetime object.")
         if self._not_valid_before is not None:
             raise ValueError("The not valid before may only be set once.")
@@ -852,15 +861,15 @@
             self._public_key,
             self._serial_number,
             time,
             self._not_valid_after,
             self._extensions,
         )
 
-    def not_valid_after(self, time: datetime.datetime) -> "CertificateBuilder":
+    def not_valid_after(self, time: datetime.datetime) -> CertificateBuilder:
         """
         Sets the certificate expiration time.
         """
         if not isinstance(time, datetime.datetime):
             raise TypeError("Expecting datetime object.")
         if self._not_valid_after is not None:
             raise ValueError("The not valid after may only be set once.")
@@ -886,15 +895,15 @@
             self._not_valid_before,
             time,
             self._extensions,
         )
 
     def add_extension(
         self, extval: ExtensionType, critical: bool
-    ) -> "CertificateBuilder":
+    ) -> CertificateBuilder:
         """
         Adds an X.509 extension to the certificate.
         """
         if not isinstance(extval, ExtensionType):
             raise TypeError("extension must be an ExtensionType")
 
         extension = Extension(extval.oid, critical, extval)
@@ -911,14 +920,18 @@
         )
 
     def sign(
         self,
         private_key: CertificateIssuerPrivateKeyTypes,
         algorithm: typing.Optional[_AllowedHashTypes],
         backend: typing.Any = None,
+        *,
+        rsa_padding: typing.Optional[
+            typing.Union[padding.PSS, padding.PKCS1v15]
+        ] = None,
     ) -> Certificate:
         """
         Signs the certificate using the CA's private key.
         """
         if self._subject_name is None:
             raise ValueError("A certificate must have a subject name")
 
@@ -933,15 +946,23 @@
 
         if self._not_valid_after is None:
             raise ValueError("A certificate must have a not valid after time")
 
         if self._public_key is None:
             raise ValueError("A certificate must have a public key")
 
-        return rust_x509.create_x509_certificate(self, private_key, algorithm)
+        if rsa_padding is not None:
+            if not isinstance(rsa_padding, (padding.PSS, padding.PKCS1v15)):
+                raise TypeError("Padding must be PSS or PKCS1v15")
+            if not isinstance(private_key, rsa.RSAPrivateKey):
+                raise TypeError("Padding is only supported for RSA keys")
+
+        return rust_x509.create_x509_certificate(
+            self, private_key, algorithm, rsa_padding
+        )
 
 
 class CertificateRevocationListBuilder:
     _extensions: typing.List[Extension[ExtensionType]]
     _revoked_certificates: typing.List[RevokedCertificate]
 
     def __init__(
@@ -956,30 +977,30 @@
         self._last_update = last_update
         self._next_update = next_update
         self._extensions = extensions
         self._revoked_certificates = revoked_certificates
 
     def issuer_name(
         self, issuer_name: Name
-    ) -> "CertificateRevocationListBuilder":
+    ) -> CertificateRevocationListBuilder:
         if not isinstance(issuer_name, Name):
             raise TypeError("Expecting x509.Name object.")
         if self._issuer_name is not None:
             raise ValueError("The issuer name may only be set once.")
         return CertificateRevocationListBuilder(
             issuer_name,
             self._last_update,
             self._next_update,
             self._extensions,
             self._revoked_certificates,
         )
 
     def last_update(
         self, last_update: datetime.datetime
-    ) -> "CertificateRevocationListBuilder":
+    ) -> CertificateRevocationListBuilder:
         if not isinstance(last_update, datetime.datetime):
             raise TypeError("Expecting datetime object.")
         if self._last_update is not None:
             raise ValueError("Last update may only be set once.")
         last_update = _convert_to_naive_utc_time(last_update)
         if last_update < _EARLIEST_UTC_TIME:
             raise ValueError(
@@ -995,15 +1016,15 @@
             self._next_update,
             self._extensions,
             self._revoked_certificates,
         )
 
     def next_update(
         self, next_update: datetime.datetime
-    ) -> "CertificateRevocationListBuilder":
+    ) -> CertificateRevocationListBuilder:
         if not isinstance(next_update, datetime.datetime):
             raise TypeError("Expecting datetime object.")
         if self._next_update is not None:
             raise ValueError("Last update may only be set once.")
         next_update = _convert_to_naive_utc_time(next_update)
         if next_update < _EARLIEST_UTC_TIME:
             raise ValueError(
@@ -1019,15 +1040,15 @@
             next_update,
             self._extensions,
             self._revoked_certificates,
         )
 
     def add_extension(
         self, extval: ExtensionType, critical: bool
-    ) -> "CertificateRevocationListBuilder":
+    ) -> CertificateRevocationListBuilder:
         """
         Adds an X.509 extension to the certificate revocation list.
         """
         if not isinstance(extval, ExtensionType):
             raise TypeError("extension must be an ExtensionType")
 
         extension = Extension(extval.oid, critical, extval)
@@ -1038,15 +1059,15 @@
             self._next_update,
             self._extensions + [extension],
             self._revoked_certificates,
         )
 
     def add_revoked_certificate(
         self, revoked_certificate: RevokedCertificate
-    ) -> "CertificateRevocationListBuilder":
+    ) -> CertificateRevocationListBuilder:
         """
         Adds a revoked certificate to the CRL.
         """
         if not isinstance(revoked_certificate, RevokedCertificate):
             raise TypeError("Must be an instance of RevokedCertificate")
 
         return CertificateRevocationListBuilder(
@@ -1082,15 +1103,15 @@
         revocation_date: typing.Optional[datetime.datetime] = None,
         extensions: typing.List[Extension[ExtensionType]] = [],
     ):
         self._serial_number = serial_number
         self._revocation_date = revocation_date
         self._extensions = extensions
 
-    def serial_number(self, number: int) -> "RevokedCertificateBuilder":
+    def serial_number(self, number: int) -> RevokedCertificateBuilder:
         if not isinstance(number, int):
             raise TypeError("Serial number must be of integral type.")
         if self._serial_number is not None:
             raise ValueError("The serial number may only be set once.")
         if number <= 0:
             raise ValueError("The serial number should be positive")
 
@@ -1102,15 +1123,15 @@
             )
         return RevokedCertificateBuilder(
             number, self._revocation_date, self._extensions
         )
 
     def revocation_date(
         self, time: datetime.datetime
-    ) -> "RevokedCertificateBuilder":
+    ) -> RevokedCertificateBuilder:
         if not isinstance(time, datetime.datetime):
             raise TypeError("Expecting datetime object.")
         if self._revocation_date is not None:
             raise ValueError("The revocation date may only be set once.")
         time = _convert_to_naive_utc_time(time)
         if time < _EARLIEST_UTC_TIME:
             raise ValueError(
@@ -1118,15 +1139,15 @@
             )
         return RevokedCertificateBuilder(
             self._serial_number, time, self._extensions
         )
 
     def add_extension(
         self, extval: ExtensionType, critical: bool
-    ) -> "RevokedCertificateBuilder":
+    ) -> RevokedCertificateBuilder:
         if not isinstance(extval, ExtensionType):
             raise TypeError("extension must be an ExtensionType")
 
         extension = Extension(extval.oid, critical, extval)
         _reject_duplicate_extension(extension, self._extensions)
         return RevokedCertificateBuilder(
             self._serial_number,
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/certificate_transparency.py` & `cryptography-41.0.0/src/cryptography/x509/certificate_transparency.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import datetime
 
 from cryptography import utils
 from cryptography.hazmat.bindings._rust import x509 as rust_x509
 from cryptography.hazmat.primitives.hashes import HashAlgorithm
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/extensions.py` & `cryptography-41.0.0/src/cryptography/x509/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import datetime
 import hashlib
 import ipaddress
 import typing
 
@@ -107,30 +108,30 @@
                 self
             )
         )
 
 
 class Extensions:
     def __init__(
-        self, extensions: typing.Iterable["Extension[ExtensionType]"]
+        self, extensions: typing.Iterable[Extension[ExtensionType]]
     ) -> None:
         self._extensions = list(extensions)
 
     def get_extension_for_oid(
         self, oid: ObjectIdentifier
-    ) -> "Extension[ExtensionType]":
+    ) -> Extension[ExtensionType]:
         for ext in self:
             if ext.oid == oid:
                 return ext
 
         raise ExtensionNotFound(f"No {oid} extension was found", oid)
 
     def get_extension_for_class(
         self, extclass: typing.Type[ExtensionTypeVar]
-    ) -> "Extension[ExtensionTypeVar]":
+    ) -> Extension[ExtensionTypeVar]:
         if extclass is UnrecognizedExtension:
             raise TypeError(
                 "UnrecognizedExtension can't be used with "
                 "get_extension_for_class because more than one instance of the"
                 " class may be present."
             )
 
@@ -217,26 +218,26 @@
     # cannot have an X25519/X448 key. This introduces some unfortunate
     # asymmetry that requires typing users to explicitly
     # narrow their type, but we should make this accurate and not just
     # convenient.
     @classmethod
     def from_issuer_public_key(
         cls, public_key: CertificateIssuerPublicKeyTypes
-    ) -> "AuthorityKeyIdentifier":
+    ) -> AuthorityKeyIdentifier:
         digest = _key_identifier_from_public_key(public_key)
         return cls(
             key_identifier=digest,
             authority_cert_issuer=None,
             authority_cert_serial_number=None,
         )
 
     @classmethod
     def from_issuer_subject_key_identifier(
-        cls, ski: "SubjectKeyIdentifier"
-    ) -> "AuthorityKeyIdentifier":
+        cls, ski: SubjectKeyIdentifier
+    ) -> AuthorityKeyIdentifier:
         return cls(
             key_identifier=ski.digest,
             authority_cert_issuer=None,
             authority_cert_serial_number=None,
         )
 
     def __repr__(self) -> str:
@@ -290,15 +291,15 @@
 
     def __init__(self, digest: bytes) -> None:
         self._digest = digest
 
     @classmethod
     def from_public_key(
         cls, public_key: CertificatePublicKeyTypes
-    ) -> "SubjectKeyIdentifier":
+    ) -> SubjectKeyIdentifier:
         return cls(_key_identifier_from_public_key(public_key))
 
     @property
     def digest(self) -> bytes:
         return self._digest
 
     @property
@@ -321,15 +322,15 @@
         return rust_x509.encode_extension_value(self)
 
 
 class AuthorityInformationAccess(ExtensionType):
     oid = ExtensionOID.AUTHORITY_INFORMATION_ACCESS
 
     def __init__(
-        self, descriptions: typing.Iterable["AccessDescription"]
+        self, descriptions: typing.Iterable[AccessDescription]
     ) -> None:
         descriptions = list(descriptions)
         if not all(isinstance(x, AccessDescription) for x in descriptions):
             raise TypeError(
                 "Every item in the descriptions list must be an "
                 "AccessDescription"
             )
@@ -354,15 +355,15 @@
         return rust_x509.encode_extension_value(self)
 
 
 class SubjectInformationAccess(ExtensionType):
     oid = ExtensionOID.SUBJECT_INFORMATION_ACCESS
 
     def __init__(
-        self, descriptions: typing.Iterable["AccessDescription"]
+        self, descriptions: typing.Iterable[AccessDescription]
     ) -> None:
         descriptions = list(descriptions)
         if not all(isinstance(x, AccessDescription) for x in descriptions):
             raise TypeError(
                 "Every item in the descriptions list must be an "
                 "AccessDescription"
             )
@@ -502,15 +503,15 @@
         return rust_x509.encode_extension_value(self)
 
 
 class CRLDistributionPoints(ExtensionType):
     oid = ExtensionOID.CRL_DISTRIBUTION_POINTS
 
     def __init__(
-        self, distribution_points: typing.Iterable["DistributionPoint"]
+        self, distribution_points: typing.Iterable[DistributionPoint]
     ) -> None:
         distribution_points = list(distribution_points)
         if not all(
             isinstance(x, DistributionPoint) for x in distribution_points
         ):
             raise TypeError(
                 "distribution_points must be a list of DistributionPoint "
@@ -539,15 +540,15 @@
         return rust_x509.encode_extension_value(self)
 
 
 class FreshestCRL(ExtensionType):
     oid = ExtensionOID.FRESHEST_CRL
 
     def __init__(
-        self, distribution_points: typing.Iterable["DistributionPoint"]
+        self, distribution_points: typing.Iterable[DistributionPoint]
     ) -> None:
         distribution_points = list(distribution_points)
         if not all(
             isinstance(x, DistributionPoint) for x in distribution_points
         ):
             raise TypeError(
                 "distribution_points must be a list of DistributionPoint "
@@ -577,15 +578,15 @@
 
 
 class DistributionPoint:
     def __init__(
         self,
         full_name: typing.Optional[typing.Iterable[GeneralName]],
         relative_name: typing.Optional[RelativeDistinguishedName],
-        reasons: typing.Optional[typing.FrozenSet["ReasonFlags"]],
+        reasons: typing.Optional[typing.FrozenSet[ReasonFlags]],
         crl_issuer: typing.Optional[typing.Iterable[GeneralName]],
     ) -> None:
         if full_name and relative_name:
             raise ValueError(
                 "You cannot provide both full_name and relative_name, at "
                 "least one must be None."
             )
@@ -675,15 +676,15 @@
         return self._full_name
 
     @property
     def relative_name(self) -> typing.Optional[RelativeDistinguishedName]:
         return self._relative_name
 
     @property
-    def reasons(self) -> typing.Optional[typing.FrozenSet["ReasonFlags"]]:
+    def reasons(self) -> typing.Optional[typing.FrozenSet[ReasonFlags]]:
         return self._reasons
 
     @property
     def crl_issuer(self) -> typing.Optional[typing.List[GeneralName]]:
         return self._crl_issuer
 
 
@@ -799,15 +800,15 @@
     def public_bytes(self) -> bytes:
         return rust_x509.encode_extension_value(self)
 
 
 class CertificatePolicies(ExtensionType):
     oid = ExtensionOID.CERTIFICATE_POLICIES
 
-    def __init__(self, policies: typing.Iterable["PolicyInformation"]) -> None:
+    def __init__(self, policies: typing.Iterable[PolicyInformation]) -> None:
         policies = list(policies)
         if not all(isinstance(x, PolicyInformation) for x in policies):
             raise TypeError(
                 "Every item in the policies list must be a "
                 "PolicyInformation"
             )
 
@@ -832,15 +833,15 @@
 
 
 class PolicyInformation:
     def __init__(
         self,
         policy_identifier: ObjectIdentifier,
         policy_qualifiers: typing.Optional[
-            typing.Iterable[typing.Union[str, "UserNotice"]]
+            typing.Iterable[typing.Union[str, UserNotice]]
         ],
     ) -> None:
         if not isinstance(policy_identifier, ObjectIdentifier):
             raise TypeError("policy_identifier must be an ObjectIdentifier")
 
         self._policy_identifier = policy_identifier
 
@@ -870,36 +871,36 @@
             self.policy_identifier == other.policy_identifier
             and self.policy_qualifiers == other.policy_qualifiers
         )
 
     def __hash__(self) -> int:
         if self.policy_qualifiers is not None:
             pq: typing.Optional[
-                typing.Tuple[typing.Union[str, "UserNotice"], ...]
+                typing.Tuple[typing.Union[str, UserNotice], ...]
             ] = tuple(self.policy_qualifiers)
         else:
             pq = None
 
         return hash((self.policy_identifier, pq))
 
     @property
     def policy_identifier(self) -> ObjectIdentifier:
         return self._policy_identifier
 
     @property
     def policy_qualifiers(
         self,
-    ) -> typing.Optional[typing.List[typing.Union[str, "UserNotice"]]]:
+    ) -> typing.Optional[typing.List[typing.Union[str, UserNotice]]]:
         return self._policy_qualifiers
 
 
 class UserNotice:
     def __init__(
         self,
-        notice_reference: typing.Optional["NoticeReference"],
+        notice_reference: typing.Optional[NoticeReference],
         explicit_text: typing.Optional[str],
     ) -> None:
         if notice_reference and not isinstance(
             notice_reference, NoticeReference
         ):
             raise TypeError(
                 "notice_reference must be None or a NoticeReference"
@@ -923,15 +924,15 @@
             and self.explicit_text == other.explicit_text
         )
 
     def __hash__(self) -> int:
         return hash((self.notice_reference, self.explicit_text))
 
     @property
-    def notice_reference(self) -> typing.Optional["NoticeReference"]:
+    def notice_reference(self) -> typing.Optional[NoticeReference]:
         return self._notice_reference
 
     @property
     def explicit_text(self) -> typing.Optional[str]:
         return self._explicit_text
 
 
@@ -1042,15 +1043,15 @@
     def public_bytes(self) -> bytes:
         return rust_x509.encode_extension_value(self)
 
 
 class TLSFeature(ExtensionType):
     oid = ExtensionOID.TLS_FEATURE
 
-    def __init__(self, features: typing.Iterable["TLSFeatureType"]) -> None:
+    def __init__(self, features: typing.Iterable[TLSFeatureType]) -> None:
         features = list(features)
         if (
             not all(isinstance(x, TLSFeatureType) for x in features)
             or len(features) == 0
         ):
             raise TypeError(
                 "features must be a list of elements from the TLSFeatureType "
@@ -1928,14 +1929,43 @@
     def nonce(self) -> bytes:
         return self._nonce
 
     def public_bytes(self) -> bytes:
         return rust_x509.encode_extension_value(self)
 
 
+class OCSPAcceptableResponses(ExtensionType):
+    oid = OCSPExtensionOID.ACCEPTABLE_RESPONSES
+
+    def __init__(self, responses: typing.Iterable[ObjectIdentifier]) -> None:
+        responses = list(responses)
+        if any(not isinstance(r, ObjectIdentifier) for r in responses):
+            raise TypeError("All responses must be ObjectIdentifiers")
+
+        self._responses = responses
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, OCSPAcceptableResponses):
+            return NotImplemented
+
+        return self._responses == other._responses
+
+    def __hash__(self) -> int:
+        return hash(tuple(self._responses))
+
+    def __repr__(self) -> str:
+        return f"<OCSPAcceptableResponses(responses={self._responses})>"
+
+    def __iter__(self) -> typing.Iterator[ObjectIdentifier]:
+        return iter(self._responses)
+
+    def public_bytes(self) -> bytes:
+        return rust_x509.encode_extension_value(self)
+
+
 class IssuingDistributionPoint(ExtensionType):
     oid = ExtensionOID.ISSUING_DISTRIBUTION_POINT
 
     def __init__(
         self,
         full_name: typing.Optional[typing.Iterable[GeneralName]],
         relative_name: typing.Optional[RelativeDistinguishedName],
@@ -2088,14 +2118,73 @@
     def only_contains_attribute_certs(self) -> bool:
         return self._only_contains_attribute_certs
 
     def public_bytes(self) -> bytes:
         return rust_x509.encode_extension_value(self)
 
 
+class MSCertificateTemplate(ExtensionType):
+    oid = ExtensionOID.MS_CERTIFICATE_TEMPLATE
+
+    def __init__(
+        self,
+        template_id: ObjectIdentifier,
+        major_version: typing.Optional[int],
+        minor_version: typing.Optional[int],
+    ) -> None:
+        if not isinstance(template_id, ObjectIdentifier):
+            raise TypeError("oid must be an ObjectIdentifier")
+        self._template_id = template_id
+        if (
+            major_version is not None and not isinstance(major_version, int)
+        ) or (
+            minor_version is not None and not isinstance(minor_version, int)
+        ):
+            raise TypeError(
+                "major_version and minor_version must be integers or None"
+            )
+        self._major_version = major_version
+        self._minor_version = minor_version
+
+    @property
+    def template_id(self) -> ObjectIdentifier:
+        return self._template_id
+
+    @property
+    def major_version(self) -> typing.Optional[int]:
+        return self._major_version
+
+    @property
+    def minor_version(self) -> typing.Optional[int]:
+        return self._minor_version
+
+    def __repr__(self) -> str:
+        return (
+            f"<MSCertificateTemplate(template_id={self.template_id}, "
+            f"major_version={self.major_version}, "
+            f"minor_version={self.minor_version})>"
+        )
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, MSCertificateTemplate):
+            return NotImplemented
+
+        return (
+            self.template_id == other.template_id
+            and self.major_version == other.major_version
+            and self.minor_version == other.minor_version
+        )
+
+    def __hash__(self) -> int:
+        return hash((self.template_id, self.major_version, self.minor_version))
+
+    def public_bytes(self) -> bytes:
+        return rust_x509.encode_extension_value(self)
+
+
 class UnrecognizedExtension(ExtensionType):
     def __init__(self, oid: ObjectIdentifier, value: bytes) -> None:
         if not isinstance(oid, ObjectIdentifier):
             raise TypeError("oid must be an ObjectIdentifier")
         self._oid = oid
         self._value = value
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/general_name.py` & `cryptography-41.0.0/src/cryptography/x509/general_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import ipaddress
 import typing
 from email.utils import parseaddr
 
 from cryptography.x509.name import Name
@@ -55,15 +56,15 @@
         self._value = value
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
-    def _init_without_validation(cls, value: str) -> "RFC822Name":
+    def _init_without_validation(cls, value: str) -> RFC822Name:
         instance = cls.__new__(cls)
         instance._value = value
         return instance
 
     def __repr__(self) -> str:
         return f"<RFC822Name(value={self.value!r})>"
 
@@ -94,15 +95,15 @@
         self._value = value
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
-    def _init_without_validation(cls, value: str) -> "DNSName":
+    def _init_without_validation(cls, value: str) -> DNSName:
         instance = cls.__new__(cls)
         instance._value = value
         return instance
 
     def __repr__(self) -> str:
         return f"<DNSName(value={self.value!r})>"
 
@@ -133,17 +134,15 @@
         self._value = value
 
     @property
     def value(self) -> str:
         return self._value
 
     @classmethod
-    def _init_without_validation(
-        cls, value: str
-    ) -> "UniformResourceIdentifier":
+    def _init_without_validation(cls, value: str) -> UniformResourceIdentifier:
         instance = cls.__new__(cls)
         instance._value = value
         return instance
 
     def __repr__(self) -> str:
         return f"<UniformResourceIdentifier(value={self.value!r})>"
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/name.py` & `cryptography-41.0.0/src/cryptography/x509/name.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 import binascii
 import re
 import sys
 import typing
 import warnings
 
 from cryptography import utils
@@ -296,15 +298,15 @@
             )
 
     @classmethod
     def from_rfc4514_string(
         cls,
         data: str,
         attr_name_overrides: typing.Optional[_NameOidMap] = None,
-    ) -> "Name":
+    ) -> Name:
         return _RFC4514NameParser(data, attr_name_overrides or {}).parse()
 
     def rfc4514_string(
         self, attr_name_overrides: typing.Optional[_OidNameMap] = None
     ) -> str:
         """
         Format as RFC4514 Distinguished Name string.
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/ocsp.py` & `cryptography-41.0.0/src/cryptography/x509/ocsp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
 
 import abc
 import datetime
 import typing
 
 from cryptography import utils, x509
 from cryptography.hazmat.bindings._rust import ocsp
@@ -419,15 +420,15 @@
         self._extensions = extensions
 
     def add_certificate(
         self,
         cert: x509.Certificate,
         issuer: x509.Certificate,
         algorithm: hashes.HashAlgorithm,
-    ) -> "OCSPRequestBuilder":
+    ) -> OCSPRequestBuilder:
         if self._request is not None or self._request_hash is not None:
             raise ValueError("Only one certificate can be added to a request")
 
         _verify_algorithm(algorithm)
         if not isinstance(cert, x509.Certificate) or not isinstance(
             issuer, x509.Certificate
         ):
@@ -439,15 +440,15 @@
 
     def add_certificate_by_hash(
         self,
         issuer_name_hash: bytes,
         issuer_key_hash: bytes,
         serial_number: int,
         algorithm: hashes.HashAlgorithm,
-    ) -> "OCSPRequestBuilder":
+    ) -> OCSPRequestBuilder:
         if self._request is not None or self._request_hash is not None:
             raise ValueError("Only one certificate can be added to a request")
 
         if not isinstance(serial_number, int):
             raise TypeError("serial_number must be an integer")
 
         _verify_algorithm(algorithm)
@@ -465,15 +466,15 @@
             self._request,
             (issuer_name_hash, issuer_key_hash, serial_number, algorithm),
             self._extensions,
         )
 
     def add_extension(
         self, extval: x509.ExtensionType, critical: bool
-    ) -> "OCSPRequestBuilder":
+    ) -> OCSPRequestBuilder:
         if not isinstance(extval, x509.ExtensionType):
             raise TypeError("extension must be an ExtensionType")
 
         extension = x509.Extension(extval.oid, critical, extval)
         _reject_duplicate_extension(extension, self._extensions)
 
         return OCSPRequestBuilder(
@@ -508,15 +509,15 @@
         issuer: x509.Certificate,
         algorithm: hashes.HashAlgorithm,
         cert_status: OCSPCertStatus,
         this_update: datetime.datetime,
         next_update: typing.Optional[datetime.datetime],
         revocation_time: typing.Optional[datetime.datetime],
         revocation_reason: typing.Optional[x509.ReasonFlags],
-    ) -> "OCSPResponseBuilder":
+    ) -> OCSPResponseBuilder:
         if self._response is not None:
             raise ValueError("Only one response per OCSPResponse.")
 
         singleresp = _SingleResponse(
             cert,
             issuer,
             algorithm,
@@ -531,15 +532,15 @@
             self._responder_id,
             self._certs,
             self._extensions,
         )
 
     def responder_id(
         self, encoding: OCSPResponderEncoding, responder_cert: x509.Certificate
-    ) -> "OCSPResponseBuilder":
+    ) -> OCSPResponseBuilder:
         if self._responder_id is not None:
             raise ValueError("responder_id can only be set once")
         if not isinstance(responder_cert, x509.Certificate):
             raise TypeError("responder_cert must be a Certificate")
         if not isinstance(encoding, OCSPResponderEncoding):
             raise TypeError(
                 "encoding must be an element from OCSPResponderEncoding"
@@ -550,15 +551,15 @@
             (responder_cert, encoding),
             self._certs,
             self._extensions,
         )
 
     def certificates(
         self, certs: typing.Iterable[x509.Certificate]
-    ) -> "OCSPResponseBuilder":
+    ) -> OCSPResponseBuilder:
         if self._certs is not None:
             raise ValueError("certificates may only be set once")
         certs = list(certs)
         if len(certs) == 0:
             raise ValueError("certs must not be an empty list")
         if not all(isinstance(x, x509.Certificate) for x in certs):
             raise TypeError("certs must be a list of Certificates")
@@ -567,15 +568,15 @@
             self._responder_id,
             certs,
             self._extensions,
         )
 
     def add_extension(
         self, extval: x509.ExtensionType, critical: bool
-    ) -> "OCSPResponseBuilder":
+    ) -> OCSPResponseBuilder:
         if not isinstance(extval, x509.ExtensionType):
             raise TypeError("extension must be an ExtensionType")
 
         extension = x509.Extension(extval.oid, critical, extval)
         _reject_duplicate_extension(extension, self._extensions)
 
         return OCSPResponseBuilder(
```

### Comparing `cryptography-40.0.2/src/cryptography/x509/oid.py` & `cryptography-41.0.0/src/cryptography/x509/oid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
+from __future__ import annotations
+
 from cryptography.hazmat._oid import (
     AttributeOID,
     AuthorityInformationAccessOID,
     CertificatePoliciesOID,
     CRLEntryExtensionOID,
     ExtendedKeyUsageOID,
     ExtensionOID,
```

### Comparing `cryptography-40.0.2/src/cryptography.egg-info/PKG-INFO` & `cryptography-41.0.0/src/cryptography.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 Metadata-Version: 2.1
 Name: cryptography
-Version: 40.0.2
+Version: 41.0.0
 Summary: cryptography is a package which provides cryptographic recipes and primitives to Python developers.
-Home-page: https://github.com/pyca/cryptography
-Author: The Python Cryptographic Authority and individual contributors
-Author-email: cryptography-dev@python.org
-License: (Apache-2.0 OR BSD-3-Clause) AND PSF-2.0
-Project-URL: Documentation, https://cryptography.io/
-Project-URL: Source, https://github.com/pyca/cryptography/
-Project-URL: Issues, https://github.com/pyca/cryptography/issues
-Project-URL: Changelog, https://cryptography.io/en/latest/changelog/
+Author-email: The Python Cryptographic Authority and individual contributors <cryptography-dev@python.org>
+License: Apache-2.0 OR BSD-3-Clause
+Project-URL: homepage, https://github.com/pyca/cryptography
+Project-URL: documentation, https://cryptography.io/
+Project-URL: source, https://github.com/pyca/cryptography/
+Project-URL: issues, https://github.com/pyca/cryptography/issues
+Project-URL: changelog, https://cryptography.io/en/latest/changelog/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: tox
+Provides-Extra: ssh
+Provides-Extra: nox
 Provides-Extra: test
 Provides-Extra: test-randomorder
 Provides-Extra: docs
 Provides-Extra: docstest
 Provides-Extra: sdist
 Provides-Extra: pep8test
-Provides-Extra: ssh
 License-File: LICENSE
 License-File: LICENSE.APACHE
 License-File: LICENSE.BSD
-License-File: LICENSE.PSF
 
 pyca/cryptography
 =================
 
 .. image:: https://img.shields.io/pypi/v/cryptography.svg
     :target: https://pypi.org/project/cryptography/
     :alt: Latest Version
@@ -60,15 +57,15 @@
 
 .. image:: https://github.com/pyca/cryptography/workflows/CI/badge.svg?branch=main
     :target: https://github.com/pyca/cryptography/actions?query=workflow%3ACI+branch%3Amain
 
 
 ``cryptography`` is a package which provides cryptographic recipes and
 primitives to Python developers. Our goal is for it to be your "cryptographic
-standard library". It supports Python 3.6+ and PyPy3 7.3.10+.
+standard library". It supports Python 3.7+ and PyPy3 7.3.10+.
 
 ``cryptography`` includes both high level recipes and low level interfaces to
 common cryptographic algorithms such as symmetric ciphers, message digests, and
 key derivation functions. For example, to encrypt something with
 ``cryptography``'s high level symmetric encryption recipe:
 
 .. code-block:: pycon
```

### Comparing `cryptography-40.0.2/src/cryptography.egg-info/SOURCES.txt` & `cryptography-41.0.0/src/cryptography.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 LICENSE.APACHE
 LICENSE.BSD
-LICENSE.PSF
 MANIFEST.in
 README.rst
+noxfile.py
 pyproject.toml
-setup.cfg
 setup.py
-tox.ini
 docs/Makefile
 docs/api-stability.rst
 docs/changelog.rst
 docs/community.rst
 docs/conf.py
 docs/doing-a-release.rst
 docs/exceptions.rst
@@ -101,33 +99,30 @@
 src/_cffi_src/openssl/dh.py
 src/_cffi_src/openssl/dsa.py
 src/_cffi_src/openssl/ec.py
 src/_cffi_src/openssl/ecdsa.py
 src/_cffi_src/openssl/engine.py
 src/_cffi_src/openssl/err.py
 src/_cffi_src/openssl/evp.py
+src/_cffi_src/openssl/evp_aead.py
 src/_cffi_src/openssl/fips.py
-src/_cffi_src/openssl/hmac.py
 src/_cffi_src/openssl/nid.py
 src/_cffi_src/openssl/objects.py
 src/_cffi_src/openssl/opensslv.py
-src/_cffi_src/openssl/osrandom_engine.py
 src/_cffi_src/openssl/pem.py
 src/_cffi_src/openssl/pkcs12.py
 src/_cffi_src/openssl/pkcs7.py
 src/_cffi_src/openssl/provider.py
 src/_cffi_src/openssl/rand.py
 src/_cffi_src/openssl/rsa.py
 src/_cffi_src/openssl/ssl.py
 src/_cffi_src/openssl/x509.py
 src/_cffi_src/openssl/x509_vfy.py
 src/_cffi_src/openssl/x509name.py
 src/_cffi_src/openssl/x509v3.py
-src/_cffi_src/openssl/src/osrandom_engine.c
-src/_cffi_src/openssl/src/osrandom_engine.h
 src/cryptography/__about__.py
 src/cryptography/__init__.py
 src/cryptography/exceptions.py
 src/cryptography/fernet.py
 src/cryptography/py.typed
 src/cryptography/utils.py
 src/cryptography.egg-info/PKG-INFO
@@ -141,34 +136,36 @@
 src/cryptography/hazmat/backends/__init__.py
 src/cryptography/hazmat/backends/openssl/__init__.py
 src/cryptography/hazmat/backends/openssl/aead.py
 src/cryptography/hazmat/backends/openssl/backend.py
 src/cryptography/hazmat/backends/openssl/ciphers.py
 src/cryptography/hazmat/backends/openssl/cmac.py
 src/cryptography/hazmat/backends/openssl/decode_asn1.py
-src/cryptography/hazmat/backends/openssl/dh.py
-src/cryptography/hazmat/backends/openssl/dsa.py
 src/cryptography/hazmat/backends/openssl/ec.py
-src/cryptography/hazmat/backends/openssl/ed25519.py
-src/cryptography/hazmat/backends/openssl/ed448.py
-src/cryptography/hazmat/backends/openssl/hashes.py
-src/cryptography/hazmat/backends/openssl/hmac.py
-src/cryptography/hazmat/backends/openssl/poly1305.py
 src/cryptography/hazmat/backends/openssl/rsa.py
 src/cryptography/hazmat/backends/openssl/utils.py
-src/cryptography/hazmat/backends/openssl/x448.py
 src/cryptography/hazmat/bindings/__init__.py
 src/cryptography/hazmat/bindings/_rust/__init__.pyi
 src/cryptography/hazmat/bindings/_rust/_openssl.pyi
 src/cryptography/hazmat/bindings/_rust/asn1.pyi
+src/cryptography/hazmat/bindings/_rust/exceptions.pyi
 src/cryptography/hazmat/bindings/_rust/ocsp.pyi
 src/cryptography/hazmat/bindings/_rust/pkcs7.pyi
 src/cryptography/hazmat/bindings/_rust/x509.pyi
 src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
 src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
+src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
 src/cryptography/hazmat/bindings/openssl/__init__.py
 src/cryptography/hazmat/bindings/openssl/_conditional.py
 src/cryptography/hazmat/bindings/openssl/binding.py
 src/cryptography/hazmat/primitives/__init__.py
 src/cryptography/hazmat/primitives/_asymmetric.py
 src/cryptography/hazmat/primitives/_cipheralgorithm.py
 src/cryptography/hazmat/primitives/_serialization.py
@@ -218,34 +215,63 @@
 src/cryptography/x509/general_name.py
 src/cryptography/x509/name.py
 src/cryptography/x509/ocsp.py
 src/cryptography/x509/oid.py
 src/rust/Cargo.lock
 src/rust/Cargo.toml
 src/rust/build.rs
+src/rust/cryptography-cffi/Cargo.toml
+src/rust/cryptography-cffi/build.rs
+src/rust/cryptography-cffi/src/lib.rs
+src/rust/cryptography-openssl/Cargo.toml
+src/rust/cryptography-openssl/build.rs
+src/rust/cryptography-openssl/src/fips.rs
+src/rust/cryptography-openssl/src/hmac.rs
+src/rust/cryptography-openssl/src/lib.rs
+src/rust/cryptography-x509/Cargo.toml
+src/rust/cryptography-x509/src/certificate.rs
+src/rust/cryptography-x509/src/common.rs
+src/rust/cryptography-x509/src/crl.rs
+src/rust/cryptography-x509/src/csr.rs
+src/rust/cryptography-x509/src/extensions.rs
+src/rust/cryptography-x509/src/lib.rs
+src/rust/cryptography-x509/src/name.rs
+src/rust/cryptography-x509/src/ocsp_req.rs
+src/rust/cryptography-x509/src/ocsp_resp.rs
+src/rust/cryptography-x509/src/oid.rs
+src/rust/cryptography-x509/src/pkcs7.rs
 src/rust/src/asn1.rs
 src/rust/src/buf.rs
 src/rust/src/error.rs
-src/rust/src/intern.rs
+src/rust/src/exceptions.rs
 src/rust/src/lib.rs
 src/rust/src/oid.rs
 src/rust/src/pkcs7.rs
 src/rust/src/pool.rs
+src/rust/src/backend/dh.rs
+src/rust/src/backend/dsa.rs
+src/rust/src/backend/ed25519.rs
+src/rust/src/backend/ed448.rs
+src/rust/src/backend/hashes.rs
+src/rust/src/backend/hmac.rs
+src/rust/src/backend/kdf.rs
 src/rust/src/backend/mod.rs
+src/rust/src/backend/poly1305.rs
+src/rust/src/backend/utils.rs
 src/rust/src/backend/x25519.rs
+src/rust/src/backend/x448.rs
 src/rust/src/x509/certificate.rs
 src/rust/src/x509/common.rs
 src/rust/src/x509/crl.rs
 src/rust/src/x509/csr.rs
 src/rust/src/x509/extensions.rs
 src/rust/src/x509/mod.rs
 src/rust/src/x509/ocsp.rs
 src/rust/src/x509/ocsp_req.rs
 src/rust/src/x509/ocsp_resp.rs
-src/rust/src/x509/oid.rs
 src/rust/src/x509/sct.rs
 src/rust/src/x509/sign.rs
 tests/__init__.py
 tests/conftest.py
 tests/deprecated_module.py
 tests/doubles.py
 tests/test_cryptography_utils.py
@@ -254,14 +280,16 @@
 tests/test_rust_utils.py
 tests/test_utils.py
 tests/test_warnings.py
 tests/utils.py
 tests/bench/__init__.py
 tests/bench/test_aead.py
 tests/bench/test_ec_load.py
+tests/bench/test_hashes.py
+tests/bench/test_hmac.py
 tests/bench/test_x509.py
 tests/hazmat/__init__.py
 tests/hazmat/test_oid.py
 tests/hazmat/backends/__init__.py
 tests/hazmat/backends/test_openssl.py
 tests/hazmat/backends/test_openssl_memleak.py
 tests/hazmat/bindings/test_openssl.py
```

### Comparing `cryptography-40.0.2/src/rust/Cargo.lock` & `cryptography-41.0.0/src/rust/Cargo.lock`

 * *Files 21% similar despite different names*

```diff
@@ -11,41 +11,31 @@
 [[package]]
 name = "aliasable"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "250f629c0161ad8107cf89319e990051fae62832fd343083bea452d93e2205fd"
 
 [[package]]
-name = "android_system_properties"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
-dependencies = [
- "libc",
-]
-
-[[package]]
 name = "asn1"
-version = "0.13.0"
+version = "0.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2affba5e62ee09eeba078f01a00c4aed45ac4287e091298eccbb0d4802efbdc5"
+checksum = "28c19b9324de5b815b6487e0f8098312791b09de0dbf3d5c2db1fe2d95bab973"
 dependencies = [
  "asn1_derive",
- "chrono",
 ]
 
 [[package]]
 name = "asn1_derive"
-version = "0.13.0"
+version = "0.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfab79c195875e5aef2bd20b4c8ed8d43ef9610bcffefbbcf66f88f555cc78af"
+checksum = "a045c3ccad89f244a86bd1e6cf1a7bf645296e7692698b056399b6efd4639407"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -59,117 +49,67 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "bumpalo"
-version = "3.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "37ccbd214614c6783386c1af30caf03192f17891059cecc394b4fb119e363de3"
-
-[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "chrono"
-version = "0.4.24"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+name = "cryptography-cffi"
+version = "0.1.0"
 dependencies = [
- "iana-time-zone",
- "num-integer",
- "num-traits",
- "winapi",
+ "cc",
+ "openssl-sys",
+ "pyo3",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
+name = "cryptography-openssl"
+version = "0.1.0"
 dependencies = [
- "termcolor",
- "unicode-width",
+ "foreign-types",
+ "foreign-types-shared",
+ "openssl",
+ "openssl-sys",
 ]
 
 [[package]]
-name = "core-foundation-sys"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
-
-[[package]]
 name = "cryptography-rust"
 version = "0.1.0"
 dependencies = [
  "asn1",
  "cc",
- "chrono",
+ "cryptography-cffi",
+ "cryptography-openssl",
+ "cryptography-x509",
  "foreign-types-shared",
  "once_cell",
  "openssl",
  "openssl-sys",
  "ouroboros",
  "pem",
  "pyo3",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.86"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "51d1075c37807dcf850c379432f0df05ba52cc30f279c5cfc43cc221ce7f8579"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.86"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5044281f61b27bc598f2f6647d480aed48d2bf52d6eb0b627d84c0361b17aa70"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.86"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61b50bc93ba22c27b0d31128d2d130a0a6b3d267ae27ef7e4fae2167dfe8781c"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.86"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e61fda7e62115119469c7b3591fd913ecca96fb766cfd3f2e2502ab7bc87a5"
+name = "cryptography-x509"
+version = "0.1.0"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn",
+ "asn1",
 ]
 
 [[package]]
 name = "foreign-types"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
@@ -180,168 +120,81 @@
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
-name = "iana-time-zone"
-version = "0.1.54"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
-dependencies = [
- "android_system_properties",
- "core-foundation-sys",
- "iana-time-zone-haiku",
- "js-sys",
- "wasm-bindgen",
- "windows",
-]
-
-[[package]]
-name = "iana-time-zone-haiku"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
-dependencies = [
- "cxx",
- "cxx-build",
-]
-
-[[package]]
 name = "indoc"
-version = "0.3.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "47741a8bc60fb26eb8d6e0238bbb26d8575ff623fdc97b1a2c00c050b9684ed8"
-dependencies = [
- "indoc-impl",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "indoc-impl"
-version = "0.3.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce046d161f000fffde5f432a0d034d0341dc152643b2598ed5bfce44c4f3a8f0"
-dependencies = [
- "proc-macro-hack",
- "proc-macro2",
- "quote",
- "syn",
- "unindent",
-]
-
-[[package]]
-name = "instant"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
-name = "js-sys"
-version = "0.3.61"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
-dependencies = [
- "wasm-bindgen",
-]
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
-name = "log"
-version = "0.4.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
-
-[[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
-name = "num-traits"
-version = "0.2.15"
+name = "memoffset"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.14.0"
+version = "1.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f7254b99e31cad77da24b08ebf628882739a608578bb1bcdfc1f9c21260d7c0"
+checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
 
 [[package]]
 name = "openssl"
-version = "0.10.50"
+version = "0.10.53"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e30d8bc91859781f0a943411186324d580f2bbeb71b452fe91ae344806af3f1"
+checksum = "12df40a956736488b7b44fe79fe12d4f245bb5b3f5a1f6095e499760015be392"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.85"
+version = "0.9.88"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d3d193fb1488ad46ffe3aaabc912cc931d02ee8518fe2959aea8ef52718b0c0"
+checksum = "c2ce0f250f34a308dcfdbb351f511359857d4ed2134ba715a4eadd46e1ffd617"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -361,86 +214,65 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5f7d21ccd03305a674437ee1248f3ab5d4b1db095cf1caf49f1713ddf61956b7"
 dependencies = [
  "Inflector",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.11.2"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
- "instant",
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.8.6"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
- "instant",
  "libc",
  "redox_syscall",
  "smallvec",
- "winapi",
-]
-
-[[package]]
-name = "paste"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45ca20c77d80be666aef2b45486da86238fabe33e38306bd3118fe4af33fa880"
-dependencies = [
- "paste-impl",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "paste-impl"
-version = "0.1.18"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d95a7db200b97ef370c8e6de0088252f7e0dfff7d047a28528e47456c0fc98b6"
-dependencies = [
- "proc-macro-hack",
+ "windows-sys",
 ]
 
 [[package]]
 name = "pem"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8835c273a76a90455d7344889b0964598e3316e2a79ede8e36f16bdcf2228b8"
 dependencies = [
  "base64",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -448,81 +280,87 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.53"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba466839c78239c09faf015484e5cc04860f88242cff4d03eb038f04b4699b73"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.15.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d41d50a7271e08c7c8a54cd24af5d62f73ee3a6f6a314215281ebdec421d5752"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
+ "memoffset",
  "parking_lot",
- "paste",
  "pyo3-build-config",
+ "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.15.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "779239fc40b8e18bc8416d3a37d280ca9b9fb04bda54b98037bb6748595c2410"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-ffi"
+version = "0.18.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+dependencies = [
+ "libc",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.15.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00b247e8c664be87998d8628e86f282c25066165f1f8dda66100c48202fdb93a"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
+ "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.15.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a8c2812c412e00e641d99eeb79dd478317d981d938aa60325dfa7157b607095"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
- "pyo3-build-config",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
@@ -535,20 +373,14 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
-
-[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
@@ -558,33 +390,35 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
+name = "syn"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
- "winapi-util",
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
 ]
 
 [[package]]
-name = "unicode-ident"
-version = "1.0.8"
+name = "target-lexicon"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
+name = "unicode-ident"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -597,103 +431,18 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
-name = "wasm-bindgen"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
-dependencies = [
- "cfg-if",
- "wasm-bindgen-macro",
-]
-
-[[package]]
-name = "wasm-bindgen-backend"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
-dependencies = [
- "bumpalo",
- "log",
- "once_cell",
- "proc-macro2",
- "quote",
- "syn",
- "wasm-bindgen-shared",
-]
-
-[[package]]
-name = "wasm-bindgen-macro"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
-dependencies = [
- "quote",
- "wasm-bindgen-macro-support",
-]
-
-[[package]]
-name = "wasm-bindgen-macro-support"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
- "wasm-bindgen-backend",
- "wasm-bindgen-shared",
-]
-
-[[package]]
-name = "wasm-bindgen-shared"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
-
-[[package]]
-name = "winapi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
-
-[[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
-name = "winapi-util"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
-dependencies = [
- "winapi",
-]
-
-[[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
-name = "windows"
-version = "0.46.0"
+name = "windows-sys"
+version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
```

### Comparing `cryptography-40.0.2/src/rust/build.rs` & `cryptography-41.0.0/src/rust/cryptography-cffi/build.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+// This file is dual licensed under the terms of the Apache License, Version
+// 2.0, and the BSD License. See the LICENSE file in the root of this repository
+// for complete details.
+
 use std::env;
-use std::io::Write;
 use std::path::Path;
-use std::process::{Command, Stdio};
+use std::process::Command;
 
-#[allow(clippy::unusual_byte_groupings)]
 fn main() {
     let target = env::var("TARGET").unwrap();
     let openssl_static = env::var("OPENSSL_STATIC")
         .map(|x| x == "1")
         .unwrap_or(false);
     if target.contains("apple") && openssl_static {
         // On (older) OSX we need to link against the clang runtime,
@@ -19,18 +21,19 @@
             println!("cargo:rustc-link-search={}", path);
         }
     }
 
     let out_dir = env::var("OUT_DIR").unwrap();
     // FIXME: maybe pyo3-build-config should provide a way to do this?
     let python = env::var("PYO3_PYTHON").unwrap_or_else(|_| "python3".to_string());
-    println!("cargo:rerun-if-changed=../_cffi_src/");
+    println!("cargo:rerun-if-env-changed=PYO3_PYTHON");
+    println!("cargo:rerun-if-changed=../../_cffi_src/");
     let output = Command::new(&python)
         .env("OUT_DIR", &out_dir)
-        .arg("../_cffi_src/build_openssl.py")
+        .arg("../../_cffi_src/build_openssl.py")
         .output()
         .expect("failed to execute build_openssl.py");
     if !output.status.success() {
         panic!(
             "failed to run build_openssl.py, stdout: \n{}\nstderr: \n{}\n",
             String::from_utf8(output.stdout).unwrap(),
             String::from_utf8(output.stderr).unwrap()
@@ -59,51 +62,33 @@
         .include(openssl_include)
         .flag_if_supported("-Wconversion")
         .flag_if_supported("-Wno-error=sign-conversion")
         .flag_if_supported("-Wno-unused-parameter");
 
     // Enable abi3 mode if we're not using PyPy.
     if python_impl != "PyPy" {
-        // cp36
-        build.define("Py_LIMITED_API", "0x030600f0");
+        // cp37 (Python 3.7 to help our grep when we some day drop 3.7 support)
+        build.define("Py_LIMITED_API", "0x030700f0");
     }
 
     if cfg!(windows) {
         build.define("WIN32_LEAN_AND_MEAN", None);
     }
 
     build.compile("_openssl.a");
-
-    if let Ok(version) = env::var("DEP_OPENSSL_LIBRESSL_VERSION_NUMBER") {
-        let version = u64::from_str_radix(&version, 16).unwrap();
-
-        println!("cargo:rustc-cfg=CRYPTOGRAPHY_IS_LIBRESSL");
-        if version >= 0x3_07_00_00_0 {
-            println!("cargo:rustc-cfg=CRYPTOGRAPHY_LIBRESSL_370_OR_GREATER")
-        }
-    }
 }
 
 /// Run a python script using the specified interpreter binary.
 fn run_python_script(interpreter: impl AsRef<Path>, script: &str) -> Result<String, String> {
     let interpreter = interpreter.as_ref();
     let out = Command::new(interpreter)
         .env("PYTHONIOENCODING", "utf-8")
-        .stdin(Stdio::piped())
-        .stdout(Stdio::piped())
-        .stderr(Stdio::inherit())
-        .spawn()
-        .and_then(|mut child| {
-            child
-                .stdin
-                .as_mut()
-                .expect("piped stdin")
-                .write_all(script.as_bytes())?;
-            child.wait_with_output()
-        });
+        .arg("-c")
+        .arg(script)
+        .output();
 
     match out {
         Err(err) => Err(format!(
             "failed to run the Python interpreter at {}: {}",
             interpreter.display(),
             err
         )),
```

### Comparing `cryptography-40.0.2/src/rust/src/asn1.rs` & `cryptography-41.0.0/src/rust/src/asn1.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::error::{CryptographyError, CryptographyResult};
-use crate::x509::Name;
+use asn1::SimpleAsn1Readable;
+use cryptography_x509::certificate::Certificate;
+use cryptography_x509::common::{DssSignature, SubjectPublicKeyInfo, Time};
+use cryptography_x509::name::Name;
 use pyo3::basic::CompareOp;
 use pyo3::types::IntoPyDict;
 use pyo3::ToPyObject;
 
 pub(crate) fn py_oid_to_oid(py_oid: &pyo3::PyAny) -> pyo3::PyResult<asn1::ObjectIdentifier> {
     Ok(py_oid
         .downcast::<pyo3::PyCell<crate::oid::ObjectIdentifier>>()?
@@ -19,52 +22,34 @@
 pub(crate) fn oid_to_py_oid<'p>(
     py: pyo3::Python<'p>,
     oid: &asn1::ObjectIdentifier,
 ) -> pyo3::PyResult<&'p pyo3::PyAny> {
     Ok(pyo3::Py::new(py, crate::oid::ObjectIdentifier { oid: oid.clone() })?.into_ref(py))
 }
 
-#[derive(asn1::Asn1Read)]
-struct AlgorithmIdentifier<'a> {
-    _oid: asn1::ObjectIdentifier,
-    _params: Option<asn1::Tlv<'a>>,
-}
-
-#[derive(asn1::Asn1Read)]
-struct Spki<'a> {
-    _algorithm: AlgorithmIdentifier<'a>,
-    data: asn1::BitString<'a>,
-}
-
 #[pyo3::prelude::pyfunction]
 fn parse_spki_for_data(
     py: pyo3::Python<'_>,
     data: &[u8],
 ) -> Result<pyo3::PyObject, CryptographyError> {
-    let spki = asn1::parse_single::<Spki<'_>>(data)?;
-    if spki.data.padding_bits() != 0 {
+    let spki = asn1::parse_single::<SubjectPublicKeyInfo<'_>>(data)?;
+    if spki.subject_public_key.padding_bits() != 0 {
         return Err(pyo3::exceptions::PyValueError::new_err("Invalid public key encoding").into());
     }
 
-    Ok(pyo3::types::PyBytes::new(py, spki.data.as_bytes()).to_object(py))
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct DssSignature<'a> {
-    r: asn1::BigUint<'a>,
-    s: asn1::BigUint<'a>,
+    Ok(pyo3::types::PyBytes::new(py, spki.subject_public_key.as_bytes()).to_object(py))
 }
 
 pub(crate) fn big_byte_slice_to_py_int<'p>(
     py: pyo3::Python<'p>,
     v: &'_ [u8],
 ) -> pyo3::PyResult<&'p pyo3::PyAny> {
     let int_type = py.get_type::<pyo3::types::PyLong>();
     let kwargs = [("signed", true)].into_py_dict(py);
-    int_type.call_method("from_bytes", (v, "big"), Some(kwargs))
+    int_type.call_method(pyo3::intern!(py, "from_bytes"), (v, "big"), Some(kwargs))
 }
 
 #[pyo3::prelude::pyfunction]
 fn decode_dss_signature(
     py: pyo3::Python<'_>,
     data: &[u8],
 ) -> Result<pyo3::PyObject, CryptographyError> {
@@ -87,31 +72,39 @@
             "Negative integers are not supported",
         ));
     }
 
     // Round the length up so that we prefix an extra \x00. This ensures that
     // integers that'd have the high bit set in their first octet are not
     // encoded as negative in DER.
-    let n = v.call_method0("bit_length")?.extract::<usize>()? / 8 + 1;
-    v.call_method1("to_bytes", (n, "big"))?.extract()
+    let n = v
+        .call_method0(pyo3::intern!(py, "bit_length"))?
+        .extract::<usize>()?
+        / 8
+        + 1;
+    v.call_method1(pyo3::intern!(py, "to_bytes"), (n, "big"))?
+        .extract()
 }
 
 pub(crate) fn encode_der_data<'p>(
     py: pyo3::Python<'p>,
     pem_tag: String,
     data: Vec<u8>,
     encoding: &'p pyo3::PyAny,
 ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
     let encoding_class = py
-        .import("cryptography.hazmat.primitives.serialization")?
-        .getattr(crate::intern!(py, "Encoding"))?;
+        .import(pyo3::intern!(
+            py,
+            "cryptography.hazmat.primitives.serialization"
+        ))?
+        .getattr(pyo3::intern!(py, "Encoding"))?;
 
-    if encoding == encoding_class.getattr(crate::intern!(py, "DER"))? {
+    if encoding.is(encoding_class.getattr(pyo3::intern!(py, "DER"))?) {
         Ok(pyo3::types::PyBytes::new(py, &data))
-    } else if encoding == encoding_class.getattr(crate::intern!(py, "PEM"))? {
+    } else if encoding.is(encoding_class.getattr(pyo3::intern!(py, "PEM"))?) {
         Ok(pyo3::types::PyBytes::new(
             py,
             &pem::encode_config(
                 &pem::Pem {
                     tag: pem_tag,
                     contents: data,
                 },
@@ -139,92 +132,60 @@
         r: asn1::BigUint::new(py_uint_to_big_endian_bytes(py, r)?).unwrap(),
         s: asn1::BigUint::new(py_uint_to_big_endian_bytes(py, s)?).unwrap(),
     };
     let result = asn1::write_single(&sig)?;
     Ok(pyo3::types::PyBytes::new(py, &result).to_object(py))
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.asn1")]
 struct TestCertificate {
     #[pyo3(get)]
     not_before_tag: u8,
     #[pyo3(get)]
     not_after_tag: u8,
     #[pyo3(get)]
     issuer_value_tags: Vec<u8>,
     #[pyo3(get)]
     subject_value_tags: Vec<u8>,
 }
 
-#[derive(asn1::Asn1Read)]
-struct Asn1Certificate<'a> {
-    tbs_cert: TbsCertificate<'a>,
-    _signature_alg: asn1::Sequence<'a>,
-    _signature: asn1::BitString<'a>,
-}
-
-#[derive(asn1::Asn1Read)]
-struct TbsCertificate<'a> {
-    #[explicit(0)]
-    _version: Option<u8>,
-    _serial: asn1::BigUint<'a>,
-    _signature_alg: asn1::Sequence<'a>,
-
-    issuer: Name<'a>,
-    validity: Validity<'a>,
-    subject: Name<'a>,
-
-    _spki: asn1::Sequence<'a>,
-    #[implicit(1)]
-    _issuer_unique_id: Option<asn1::BitString<'a>>,
-    #[implicit(2)]
-    _subject_unique_id: Option<asn1::BitString<'a>>,
-    #[explicit(3)]
-    _extensions: Option<asn1::Sequence<'a>>,
-}
-
-#[derive(asn1::Asn1Read)]
-struct Validity<'a> {
-    not_before: asn1::Tlv<'a>,
-    not_after: asn1::Tlv<'a>,
-}
-
 fn parse_name_value_tags(rdns: &mut Name<'_>) -> Vec<u8> {
     let mut tags = vec![];
     for rdn in rdns.unwrap_read().clone() {
         let mut attributes = rdn.collect::<Vec<_>>();
         assert_eq!(attributes.len(), 1);
 
         tags.push(attributes.pop().unwrap().value.tag().as_u8().unwrap());
     }
     tags
 }
 
+fn time_tag(t: &Time) -> u8 {
+    match t {
+        Time::UtcTime(_) => asn1::UtcTime::TAG.as_u8().unwrap(),
+        Time::GeneralizedTime(_) => asn1::GeneralizedTime::TAG.as_u8().unwrap(),
+    }
+}
+
 #[pyo3::prelude::pyfunction]
 fn test_parse_certificate(data: &[u8]) -> Result<TestCertificate, CryptographyError> {
-    let mut asn1_cert = asn1::parse_single::<Asn1Certificate<'_>>(data)?;
+    let mut cert = asn1::parse_single::<Certificate<'_>>(data)?;
 
     Ok(TestCertificate {
-        not_before_tag: asn1_cert
-            .tbs_cert
-            .validity
-            .not_before
-            .tag()
-            .as_u8()
-            .unwrap(),
-        not_after_tag: asn1_cert.tbs_cert.validity.not_after.tag().as_u8().unwrap(),
-        issuer_value_tags: parse_name_value_tags(&mut asn1_cert.tbs_cert.issuer),
-        subject_value_tags: parse_name_value_tags(&mut asn1_cert.tbs_cert.subject),
+        not_before_tag: time_tag(&cert.tbs_cert.validity.not_before),
+        not_after_tag: time_tag(&cert.tbs_cert.validity.not_after),
+        issuer_value_tags: parse_name_value_tags(&mut cert.tbs_cert.issuer),
+        subject_value_tags: parse_name_value_tags(&mut cert.tbs_cert.subject),
     })
 }
 
 pub(crate) fn create_submodule(py: pyo3::Python<'_>) -> pyo3::PyResult<&pyo3::prelude::PyModule> {
     let submod = pyo3::prelude::PyModule::new(py, "asn1")?;
-    submod.add_wrapped(pyo3::wrap_pyfunction!(parse_spki_for_data))?;
+    submod.add_function(pyo3::wrap_pyfunction!(parse_spki_for_data, submod)?)?;
 
-    submod.add_wrapped(pyo3::wrap_pyfunction!(decode_dss_signature))?;
-    submod.add_wrapped(pyo3::wrap_pyfunction!(encode_dss_signature))?;
+    submod.add_function(pyo3::wrap_pyfunction!(decode_dss_signature, submod)?)?;
+    submod.add_function(pyo3::wrap_pyfunction!(encode_dss_signature, submod)?)?;
 
-    submod.add_wrapped(pyo3::wrap_pyfunction!(test_parse_certificate))?;
+    submod.add_function(pyo3::wrap_pyfunction!(test_parse_certificate, submod)?)?;
 
     Ok(submod)
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/backend/x25519.rs` & `cryptography-41.0.0/src/rust/src/backend/utils.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,297 +1,302 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
-use crate::buf::CffiBuf;
 use crate::error::{CryptographyError, CryptographyResult};
-use foreign_types_shared::ForeignTypeRef;
 
-#[pyo3::prelude::pyclass]
-struct X25519PrivateKey {
-    pkey: openssl::pkey::PKey<openssl::pkey::Private>,
-}
+pub(crate) fn py_int_to_bn(
+    py: pyo3::Python<'_>,
+    v: &pyo3::PyAny,
+) -> CryptographyResult<openssl::bn::BigNum> {
+    let n = v
+        .call_method0(pyo3::intern!(py, "bit_length"))?
+        .extract::<usize>()?
+        / 8
+        + 1;
+    let bytes: &[u8] = v
+        .call_method1(pyo3::intern!(py, "to_bytes"), (n, pyo3::intern!(py, "big")))?
+        .extract()?;
 
-#[pyo3::prelude::pyclass]
-struct X25519PublicKey {
-    pkey: openssl::pkey::PKey<openssl::pkey::Public>,
+    Ok(openssl::bn::BigNum::from_slice(bytes)?)
 }
 
-#[pyo3::prelude::pyfunction]
-fn generate_key() -> CryptographyResult<X25519PrivateKey> {
-    Ok(X25519PrivateKey {
-        pkey: openssl::pkey::PKey::generate_x25519()?,
-    })
+pub(crate) fn bn_to_py_int<'p>(
+    py: pyo3::Python<'p>,
+    b: &openssl::bn::BigNumRef,
+) -> CryptographyResult<&'p pyo3::PyAny> {
+    assert!(!b.is_negative());
+
+    let int_type = py.get_type::<pyo3::types::PyLong>();
+    Ok(int_type.call_method1(
+        pyo3::intern!(py, "from_bytes"),
+        (b.to_vec(), pyo3::intern!(py, "big")),
+    )?)
 }
 
-#[pyo3::prelude::pyfunction]
-fn private_key_from_ptr(ptr: usize) -> X25519PrivateKey {
-    let pkey = unsafe { openssl::pkey::PKeyRef::from_ptr(ptr as *mut _) };
-    X25519PrivateKey {
-        pkey: pkey.to_owned(),
-    }
+pub(crate) fn bn_to_big_endian_bytes(b: &openssl::bn::BigNumRef) -> CryptographyResult<Vec<u8>> {
+    Ok(b.to_vec_padded(b.num_bits() / 8 + 1)?)
 }
 
-#[pyo3::prelude::pyfunction]
-fn public_key_from_ptr(ptr: usize) -> X25519PublicKey {
-    let pkey = unsafe { openssl::pkey::PKeyRef::from_ptr(ptr as *mut _) };
-    X25519PublicKey {
-        pkey: pkey.to_owned(),
+#[allow(clippy::too_many_arguments)]
+pub(crate) fn pkey_private_bytes<'p>(
+    py: pyo3::Python<'p>,
+    key_obj: &pyo3::PyAny,
+    pkey: &openssl::pkey::PKey<openssl::pkey::Private>,
+    encoding: &pyo3::PyAny,
+    format: &pyo3::PyAny,
+    encryption_algorithm: &pyo3::PyAny,
+    openssh_allowed: bool,
+    raw_allowed: bool,
+) -> CryptographyResult<&'p pyo3::types::PyBytes> {
+    let serialization_mod = py.import(pyo3::intern!(
+        py,
+        "cryptography.hazmat.primitives.serialization"
+    ))?;
+    let encoding_class: &pyo3::types::PyType = serialization_mod
+        .getattr(pyo3::intern!(py, "Encoding"))?
+        .extract()?;
+    let private_format_class: &pyo3::types::PyType = serialization_mod
+        .getattr(pyo3::intern!(py, "PrivateFormat"))?
+        .extract()?;
+    let key_serialization_encryption_class: &pyo3::types::PyType = serialization_mod
+        .getattr(pyo3::intern!(py, "KeySerializationEncryption"))?
+        .extract()?;
+    let no_encryption_class: &pyo3::types::PyType = serialization_mod
+        .getattr(pyo3::intern!(py, "NoEncryption"))?
+        .extract()?;
+    let best_available_encryption_class: &pyo3::types::PyType = serialization_mod
+        .getattr(pyo3::intern!(py, "BestAvailableEncryption"))?
+        .extract()?;
+
+    if !encoding.is_instance(encoding_class)? {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyTypeError::new_err(
+                "encoding must be an item from the Encoding enum",
+            ),
+        ));
+    }
+    if !format.is_instance(private_format_class)? {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyTypeError::new_err(
+                "format must be an item from the PrivateFormat enum",
+            ),
+        ));
+    }
+    if !encryption_algorithm.is_instance(key_serialization_encryption_class)? {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyTypeError::new_err(
+                "Encryption algorithm must be a KeySerializationEncryption instance",
+            ),
+        ));
     }
-}
-
-#[pyo3::prelude::pyfunction]
-fn from_private_bytes(data: CffiBuf<'_>) -> pyo3::PyResult<X25519PrivateKey> {
-    let pkey =
-        openssl::pkey::PKey::private_key_from_raw_bytes(data.as_bytes(), openssl::pkey::Id::X25519)
-            .map_err(|e| {
-                pyo3::exceptions::PyValueError::new_err(format!(
-                    "An X25519 private key is 32 bytes long: {}",
-                    e
-                ))
-            })?;
-    Ok(X25519PrivateKey { pkey })
-}
-#[pyo3::prelude::pyfunction]
-fn from_public_bytes(data: &[u8]) -> pyo3::PyResult<X25519PublicKey> {
-    let pkey = openssl::pkey::PKey::public_key_from_raw_bytes(data, openssl::pkey::Id::X25519)
-        .map_err(|_| {
-            pyo3::exceptions::PyValueError::new_err("An X25519 public key is 32 bytes long")
-        })?;
-    Ok(X25519PublicKey { pkey })
-}
-
-#[pyo3::prelude::pymethods]
-impl X25519PrivateKey {
-    fn exchange<'p>(
-        &self,
-        py: pyo3::Python<'p>,
-        public_key: &X25519PublicKey,
-    ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
-        let mut deriver = openssl::derive::Deriver::new(&self.pkey)?;
-        deriver.set_peer(&public_key.pkey)?;
-
-        Ok(pyo3::types::PyBytes::new_with(py, deriver.len()?, |b| {
-            let n = deriver.derive(b).map_err(|_| {
-                pyo3::exceptions::PyValueError::new_err("Error computing shared key.")
-            })?;
-            assert_eq!(n, b.len());
-            Ok(())
-        })?)
-    }
-
-    fn public_key(&self) -> CryptographyResult<X25519PublicKey> {
-        let raw_bytes = self.pkey.raw_public_key()?;
-        Ok(X25519PublicKey {
-            pkey: openssl::pkey::PKey::public_key_from_raw_bytes(
-                &raw_bytes,
-                openssl::pkey::Id::X25519,
-            )?,
-        })
-    }
-
-    fn private_bytes_raw<'p>(
-        &self,
-        py: pyo3::Python<'p>,
-    ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
-        let raw_bytes = self.pkey.raw_private_key()?;
-        Ok(pyo3::types::PyBytes::new(py, &raw_bytes))
-    }
-
-    fn private_bytes<'p>(
-        &self,
-        py: pyo3::Python<'p>,
-        encoding: &pyo3::PyAny,
-        format: &pyo3::PyAny,
-        encryption_algorithm: &pyo3::PyAny,
-    ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
-        let serialization_mod = py.import("cryptography.hazmat.primitives.serialization")?;
-        let encoding_class: &pyo3::types::PyType = serialization_mod
-            .getattr(crate::intern!(py, "Encoding"))?
-            .extract()?;
-        let private_format_class: &pyo3::types::PyType = serialization_mod
-            .getattr(crate::intern!(py, "PrivateFormat"))?
-            .extract()?;
-        let no_encryption_class: &pyo3::types::PyType = serialization_mod
-            .getattr(crate::intern!(py, "NoEncryption"))?
-            .extract()?;
-        let best_available_encryption_class: &pyo3::types::PyType = serialization_mod
-            .getattr(crate::intern!(py, "BestAvailableEncryption"))?
-            .extract()?;
-
-        if !encoding_class.is_instance(encoding)? {
-            return Err(CryptographyError::from(
-                pyo3::exceptions::PyTypeError::new_err(
-                    "encoding must be an item from the Encoding enum",
-                ),
-            ));
-        }
-        if !private_format_class.is_instance(format)? {
-            return Err(CryptographyError::from(
-                pyo3::exceptions::PyTypeError::new_err(
-                    "format must be an item from the PrivateFormat enum",
-                ),
-            ));
-        }
 
-        if encoding == encoding_class.getattr(crate::intern!(py, "Raw"))?
-            || format == private_format_class.getattr(crate::intern!(py, "Raw"))?
+    #[cfg(any(not(CRYPTOGRAPHY_IS_LIBRESSL), CRYPTOGRAPHY_LIBRESSL_370_OR_GREATER))]
+    if raw_allowed
+        && (encoding.is(encoding_class.getattr(pyo3::intern!(py, "Raw"))?)
+            || format.is(private_format_class.getattr(pyo3::intern!(py, "Raw"))?))
+    {
+        if !encoding.is(encoding_class.getattr(pyo3::intern!(py, "Raw"))?)
+            || !format.is(private_format_class.getattr(pyo3::intern!(py, "Raw"))?)
+            || !encryption_algorithm.is_instance(no_encryption_class)?
         {
-            if encoding != encoding_class.getattr(crate::intern!(py, "Raw"))?
-                || format != private_format_class.getattr(crate::intern!(py, "Raw"))?
-                || !no_encryption_class.is_instance(encryption_algorithm)?
-            {
-                return Err(CryptographyError::from(pyo3::exceptions::PyValueError::new_err(
+            return Err(CryptographyError::from(pyo3::exceptions::PyValueError::new_err(
                     "When using Raw both encoding and format must be Raw and encryption_algorithm must be NoEncryption()"
                 )));
-            }
-            let raw_bytes = self.pkey.raw_private_key()?;
-            return Ok(pyo3::types::PyBytes::new(py, &raw_bytes));
         }
+        let raw_bytes = pkey.raw_private_key()?;
+        return Ok(pyo3::types::PyBytes::new(py, &raw_bytes));
+    }
 
-        let password = if no_encryption_class.is_instance(encryption_algorithm)? {
-            b""
-        } else if best_available_encryption_class.is_instance(encryption_algorithm)? {
-            encryption_algorithm
-                .getattr(crate::intern!(py, "password"))?
-                .extract::<&[u8]>()?
-        } else {
-            return Err(CryptographyError::from(
-                pyo3::exceptions::PyTypeError::new_err(
-                    "Encryption algorithm must be a KeySerializationEncryption instance",
-                ),
-            ));
-        };
+    let password = if encryption_algorithm.is_instance(no_encryption_class)? {
+        b""
+    } else if encryption_algorithm.is_instance(best_available_encryption_class)? {
+        encryption_algorithm
+            .getattr(pyo3::intern!(py, "password"))?
+            .extract::<&[u8]>()?
+    } else {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyValueError::new_err("Unsupported encryption type"),
+        ));
+    };
+
+    if password.len() > 1023 {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyValueError::new_err(
+                "Passwords longer than 1023 bytes are not supported by this backend",
+            ),
+        ));
+    }
 
-        if password.len() > 1023 {
-            return Err(CryptographyError::from(
-                pyo3::exceptions::PyValueError::new_err(
-                    "Passwords longer than 1023 bytes are not supported by this backend",
-                ),
-            ));
+    if format.is(private_format_class.getattr(pyo3::intern!(py, "PKCS8"))?) {
+        if encoding.is(encoding_class.getattr(pyo3::intern!(py, "PEM"))?) {
+            let pem_bytes = if password.is_empty() {
+                pkey.private_key_to_pem_pkcs8()?
+            } else {
+                pkey.private_key_to_pem_pkcs8_passphrase(
+                    openssl::symm::Cipher::aes_256_cbc(),
+                    password,
+                )?
+            };
+            return Ok(pyo3::types::PyBytes::new(py, &pem_bytes));
+        } else if encoding.is(encoding_class.getattr(pyo3::intern!(py, "DER"))?) {
+            let der_bytes = if password.is_empty() {
+                pkey.private_key_to_pkcs8()?
+            } else {
+                pkey.private_key_to_pkcs8_passphrase(
+                    openssl::symm::Cipher::aes_256_cbc(),
+                    password,
+                )?
+            };
+            return Ok(pyo3::types::PyBytes::new(py, &der_bytes));
         }
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyValueError::new_err("Unsupported encoding for PKCS8"),
+        ));
+    }
 
-        if format == private_format_class.getattr(crate::intern!(py, "PKCS8"))? {
-            if encoding == encoding_class.getattr(crate::intern!(py, "PEM"))? {
+    if format.is(private_format_class.getattr(pyo3::intern!(py, "TraditionalOpenSSL"))?) {
+        if let Ok(dsa) = pkey.dsa() {
+            if encoding.is(encoding_class.getattr(pyo3::intern!(py, "PEM"))?) {
                 let pem_bytes = if password.is_empty() {
-                    self.pkey.private_key_to_pem_pkcs8()?
+                    dsa.private_key_to_pem()?
                 } else {
-                    self.pkey.private_key_to_pem_pkcs8_passphrase(
+                    dsa.private_key_to_pem_passphrase(
                         openssl::symm::Cipher::aes_256_cbc(),
                         password,
                     )?
                 };
                 return Ok(pyo3::types::PyBytes::new(py, &pem_bytes));
-            } else if encoding == encoding_class.getattr(crate::intern!(py, "DER"))? {
-                let der_bytes = if password.is_empty() {
-                    self.pkey.private_key_to_pkcs8()?
-                } else {
-                    self.pkey.private_key_to_pkcs8_passphrase(
-                        openssl::symm::Cipher::aes_256_cbc(),
-                        password,
-                    )?
-                };
+            } else if encoding.is(encoding_class.getattr(pyo3::intern!(py, "DER"))?) {
+                if !password.is_empty() {
+                    return Err(CryptographyError::from(
+                        pyo3::exceptions::PyValueError::new_err(
+                            "Encryption is not supported for DER encoded traditional OpenSSL keys",
+                        ),
+                    ));
+                }
+
+                let der_bytes = dsa.private_key_to_der()?;
                 return Ok(pyo3::types::PyBytes::new(py, &der_bytes));
-            } else {
-                return Err(CryptographyError::from(
-                    pyo3::exceptions::PyValueError::new_err("Unsupported encoding for PKCS8"),
-                ));
             }
         }
+    }
 
-        Err(CryptographyError::from(
-            pyo3::exceptions::PyValueError::new_err("format is invalid with this key"),
-        ))
+    // OpenSSH + PEM
+    if openssh_allowed && format.is(private_format_class.getattr(pyo3::intern!(py, "OpenSSH"))?) {
+        if encoding.is(encoding_class.getattr(pyo3::intern!(py, "PEM"))?) {
+            return Ok(py
+                .import(pyo3::intern!(
+                    py,
+                    "cryptography.hazmat.primitives.serialization.ssh"
+                ))?
+                .call_method1(
+                    pyo3::intern!(py, "_serialize_ssh_private_key"),
+                    (key_obj, password, encryption_algorithm),
+                )?
+                .extract()?);
+        }
+
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyValueError::new_err(
+                "OpenSSH private key format can only be used with PEM encoding",
+            ),
+        ));
     }
+
+    Err(CryptographyError::from(
+        pyo3::exceptions::PyValueError::new_err("format is invalid with this key"),
+    ))
 }
 
-#[pyo3::prelude::pymethods]
-impl X25519PublicKey {
-    fn public_bytes_raw<'p>(
-        &self,
-        py: pyo3::Python<'p>,
-    ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
-        let raw_bytes = self.pkey.raw_public_key()?;
-        Ok(pyo3::types::PyBytes::new(py, &raw_bytes))
-    }
-
-    fn public_bytes<'p>(
-        &self,
-        py: pyo3::Python<'p>,
-        encoding: &pyo3::PyAny,
-        format: &pyo3::PyAny,
-    ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
-        let serialization_mod = py.import("cryptography.hazmat.primitives.serialization")?;
-        let encoding_class: &pyo3::types::PyType = serialization_mod
-            .getattr(crate::intern!(py, "Encoding"))?
-            .extract()?;
-        let public_format_class: &pyo3::types::PyType = serialization_mod
-            .getattr(crate::intern!(py, "PublicFormat"))?
-            .extract()?;
+pub(crate) fn pkey_public_bytes<'p>(
+    py: pyo3::Python<'p>,
+    key_obj: &pyo3::PyAny,
+    pkey: &openssl::pkey::PKey<openssl::pkey::Public>,
+    encoding: &pyo3::PyAny,
+    format: &pyo3::PyAny,
+    openssh_allowed: bool,
+    raw_allowed: bool,
+) -> CryptographyResult<&'p pyo3::types::PyBytes> {
+    let serialization_mod = py.import(pyo3::intern!(
+        py,
+        "cryptography.hazmat.primitives.serialization"
+    ))?;
+    let encoding_class: &pyo3::types::PyType = serialization_mod
+        .getattr(pyo3::intern!(py, "Encoding"))?
+        .extract()?;
+    let public_format_class: &pyo3::types::PyType = serialization_mod
+        .getattr(pyo3::intern!(py, "PublicFormat"))?
+        .extract()?;
+
+    if !encoding.is_instance(encoding_class)? {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyTypeError::new_err(
+                "encoding must be an item from the Encoding enum",
+            ),
+        ));
+    }
+    if !format.is_instance(public_format_class)? {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyTypeError::new_err(
+                "format must be an item from the PublicFormat enum",
+            ),
+        ));
+    }
 
-        if !encoding_class.is_instance(encoding)? {
-            return Err(CryptographyError::from(
-                pyo3::exceptions::PyTypeError::new_err(
-                    "encoding must be an item from the Encoding enum",
-                ),
-            ));
-        }
-        if !public_format_class.is_instance(format)? {
+    #[cfg(any(not(CRYPTOGRAPHY_IS_LIBRESSL), CRYPTOGRAPHY_LIBRESSL_370_OR_GREATER))]
+    if raw_allowed
+        && (encoding.is(encoding_class.getattr(pyo3::intern!(py, "Raw"))?)
+            || format.is(public_format_class.getattr(pyo3::intern!(py, "Raw"))?))
+    {
+        if !encoding.is(encoding_class.getattr(pyo3::intern!(py, "Raw"))?)
+            || !format.is(public_format_class.getattr(pyo3::intern!(py, "Raw"))?)
+        {
             return Err(CryptographyError::from(
-                pyo3::exceptions::PyTypeError::new_err(
-                    "format must be an item from the PublicFormat enum",
+                pyo3::exceptions::PyValueError::new_err(
+                    "When using Raw both encoding and format must be Raw",
                 ),
             ));
         }
+        let raw_bytes = pkey.raw_public_key()?;
+        return Ok(pyo3::types::PyBytes::new(py, &raw_bytes));
+    }
 
-        if encoding == encoding_class.getattr(crate::intern!(py, "Raw"))?
-            || format == public_format_class.getattr(crate::intern!(py, "Raw"))?
-        {
-            if encoding != encoding_class.getattr(crate::intern!(py, "Raw"))?
-                || format != public_format_class.getattr(crate::intern!(py, "Raw"))?
-            {
-                return Err(CryptographyError::from(
-                    pyo3::exceptions::PyValueError::new_err(
-                        "When using Raw both encoding and format must be Raw",
-                    ),
-                ));
-            }
-            let raw_bytes = self.pkey.raw_public_key()?;
-            return Ok(pyo3::types::PyBytes::new(py, &raw_bytes));
+    // SubjectPublicKeyInfo + PEM/DER
+    if format.is(public_format_class.getattr(pyo3::intern!(py, "SubjectPublicKeyInfo"))?) {
+        if encoding.is(encoding_class.getattr(pyo3::intern!(py, "PEM"))?) {
+            let pem_bytes = pkey.public_key_to_pem()?;
+            return Ok(pyo3::types::PyBytes::new(py, &pem_bytes));
+        } else if encoding.is(encoding_class.getattr(pyo3::intern!(py, "DER"))?) {
+            let der_bytes = pkey.public_key_to_der()?;
+            return Ok(pyo3::types::PyBytes::new(py, &der_bytes));
         }
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyValueError::new_err(
+                "SubjectPublicKeyInfo works only with PEM or DER encoding",
+            ),
+        ));
+    }
 
-        // SubjectPublicKeyInfo + PEM/DER
-        if format == public_format_class.getattr(crate::intern!(py, "SubjectPublicKeyInfo"))? {
-            if encoding == encoding_class.getattr(crate::intern!(py, "PEM"))? {
-                let pem_bytes = self.pkey.public_key_to_pem()?;
-                return Ok(pyo3::types::PyBytes::new(py, &pem_bytes));
-            } else if encoding == encoding_class.getattr(crate::intern!(py, "DER"))? {
-                let der_bytes = self.pkey.public_key_to_der()?;
-                return Ok(pyo3::types::PyBytes::new(py, &der_bytes));
-            } else {
-                return Err(CryptographyError::from(
-                    pyo3::exceptions::PyValueError::new_err(
-                        "SubjectPublicKeyInfo works only with PEM or DER encoding",
-                    ),
-                ));
-            }
+    // OpenSSH + OpenSSH
+    if openssh_allowed && format.is(public_format_class.getattr(pyo3::intern!(py, "OpenSSH"))?) {
+        if encoding.is(encoding_class.getattr(pyo3::intern!(py, "OpenSSH"))?) {
+            return Ok(py
+                .import(pyo3::intern!(
+                    py,
+                    "cryptography.hazmat.primitives.serialization.ssh"
+                ))?
+                .call_method1(pyo3::intern!(py, "serialize_ssh_public_key"), (key_obj,))?
+                .extract()?);
         }
 
-        Err(CryptographyError::from(
-            pyo3::exceptions::PyValueError::new_err("format is invalid with this key"),
-        ))
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyValueError::new_err(
+                "OpenSSH format must be used with OpenSSH encoding",
+            ),
+        ));
     }
-}
-
-pub(crate) fn create_module(py: pyo3::Python<'_>) -> pyo3::PyResult<&pyo3::prelude::PyModule> {
-    let m = pyo3::prelude::PyModule::new(py, "x25519")?;
-    m.add_wrapped(pyo3::wrap_pyfunction!(generate_key))?;
-    m.add_wrapped(pyo3::wrap_pyfunction!(private_key_from_ptr))?;
-    m.add_wrapped(pyo3::wrap_pyfunction!(public_key_from_ptr))?;
-    m.add_wrapped(pyo3::wrap_pyfunction!(from_private_bytes))?;
-    m.add_wrapped(pyo3::wrap_pyfunction!(from_public_bytes))?;
-
-    m.add_class::<X25519PrivateKey>()?;
-    m.add_class::<X25519PublicKey>()?;
 
-    Ok(m)
+    Err(CryptographyError::from(
+        pyo3::exceptions::PyValueError::new_err("format is invalid with this key"),
+    ))
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/buf.rs` & `cryptography-41.0.0/src/rust/src/buf.rs`

 * *Files 12% similar despite different names*

```diff
@@ -2,39 +2,43 @@
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use std::{ptr, slice};
 
 pub(crate) struct CffiBuf<'p> {
     _pyobj: &'p pyo3::PyAny,
+    _bufobj: &'p pyo3::PyAny,
     buf: &'p [u8],
 }
 
 impl CffiBuf<'_> {
     pub(crate) fn as_bytes(&self) -> &[u8] {
         self.buf
     }
 }
 
 impl<'a> pyo3::conversion::FromPyObject<'a> for CffiBuf<'a> {
     fn extract(pyobj: &'a pyo3::PyAny) -> pyo3::PyResult<Self> {
         let py = pyobj.py();
 
-        let (ptrval, len): (usize, usize) = py
-            .import("cryptography.utils")?
-            .call_method1("_extract_buffer_length", (pyobj,))?
+        let (bufobj, ptrval): (&pyo3::PyAny, usize) = py
+            .import(pyo3::intern!(py, "cryptography.utils"))?
+            .call_method1(pyo3::intern!(py, "_extract_buffer_length"), (pyobj,))?
             .extract()?;
+
+        let len = bufobj.len()?;
         let ptr = if len == 0 {
             ptr::NonNull::dangling().as_ptr()
         } else {
             ptrval as *const u8
         };
 
         Ok(CffiBuf {
             _pyobj: pyobj,
+            _bufobj: bufobj,
             // SAFETY: _extract_buffer_length ensures that we have a valid ptr
             // and length (and we ensure we meet slice's requirements for
             // 0-length slices above), we're keeping pyobj alive which ensures
             // the buffer is valid. But! There is no actually guarantee
             // against concurrent mutation. See
             // https://alexgaynor.net/2022/oct/23/buffers-on-the-edge/
             // for details. This is the same as our cffi status quo ante, so
```

### Comparing `cryptography-40.0.2/src/rust/src/error.rs` & `cryptography-41.0.0/src/rust/src/error.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
-use crate::OpenSSLError;
+use crate::{exceptions, OpenSSLError};
+use pyo3::ToPyObject;
 
 pub enum CryptographyError {
     Asn1Parse(asn1::ParseError),
     Asn1Write(asn1::WriteError),
     Py(pyo3::PyErr),
     OpenSSL(openssl::error::ErrorStack),
 }
@@ -58,48 +59,38 @@
             ),
             CryptographyError::Asn1Write(asn1::WriteError::AllocationError) => {
                 pyo3::exceptions::PyMemoryError::new_err(
                     "failed to allocate memory while performing ASN.1 serialization",
                 )
             }
             CryptographyError::Py(py_error) => py_error,
-            CryptographyError::OpenSSL(error_stack) => {
-                let gil = pyo3::Python::acquire_gil();
-                let py = gil.python();
-
-                let internal_error = py
-                    .import("cryptography.exceptions")
-                    .expect("Failed to import cryptography module")
-                    .getattr(crate::intern!(py, "InternalError"))
-                    .expect("Failed to get InternalError attribute");
-
+            CryptographyError::OpenSSL(error_stack) => pyo3::Python::with_gil(|py| {
                 let errors = pyo3::types::PyList::empty(py);
                 for e in error_stack.errors() {
                     errors
                         .append(
                             pyo3::PyCell::new(py, OpenSSLError { e: e.clone() })
                                 .expect("Failed to create OpenSSLError"),
                         )
                         .expect("Failed to append to list");
                 }
-                pyo3::PyErr::from_instance(
-                    internal_error
-                        .call1((
-                            "Unknown OpenSSL error. This error is commonly encountered
-                    when another library is not cleaning up the OpenSSL error
-                    stack. If you are using cryptography with another library
-                    that uses OpenSSL try disabling it before reporting a bug.
-                    Otherwise please file an issue at
-                    https://github.com/pyca/cryptography/issues with
-                    information on how to reproduce this.",
-                            errors,
-                        ))
-                        .expect("Failed to create InternalError"),
-                )
-            }
+                exceptions::InternalError::new_err((
+                    format!(
+                        "Unknown OpenSSL error. This error is commonly encountered
+                        when another library is not cleaning up the OpenSSL error
+                        stack. If you are using cryptography with another library
+                        that uses OpenSSL try disabling it before reporting a bug.
+                        Otherwise please file an issue at
+                        https://github.com/pyca/cryptography/issues with
+                        information on how to reproduce this. ({:?})",
+                        errors
+                    ),
+                    errors.to_object(py),
+                ))
+            }),
         }
     }
 }
 
 impl CryptographyError {
     pub(crate) fn add_location(self, loc: asn1::ParseLocation) -> Self {
         match self {
@@ -126,15 +117,15 @@
         pyo3::Python::with_gil(|py| {
             let e: CryptographyError = asn1::WriteError::AllocationError.into();
             assert!(matches!(
                 e,
                 CryptographyError::Asn1Write(asn1::WriteError::AllocationError)
             ));
             let py_e: pyo3::PyErr = e.into();
-            assert!(py_e.is_instance::<pyo3::exceptions::PyMemoryError>(py));
+            assert!(py_e.is_instance_of::<pyo3::exceptions::PyMemoryError>(py));
 
             let e: CryptographyError =
                 pyo3::PyDowncastError::new(py.None().as_ref(py), "abc").into();
             assert!(matches!(e, CryptographyError::Py(_)));
         })
     }
```

### Comparing `cryptography-40.0.2/src/rust/src/lib.rs` & `cryptography-41.0.0/src/rust/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,23 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 #![deny(rust_2018_idioms)]
-// Temporarily allow `clippy::borrow_deref_ref` until we can upgrade to the
-// latest pyo3: https://github.com/PyO3/pyo3/pull/2503
-//
-// `unknown_lints` is required until GHA upgrades their rustc.
-#![allow(unknown_lints, clippy::borrow_deref_ref)]
 
 mod asn1;
 mod backend;
 mod buf;
 mod error;
-mod intern;
+mod exceptions;
 pub(crate) mod oid;
 mod pkcs7;
 mod pool;
 mod x509;
 
-#[cfg(not(python_implementation = "PyPy"))]
-use pyo3::FromPyPointer;
-use std::convert::TryInto;
-
-#[cfg(python_implementation = "PyPy")]
-extern "C" {
-    fn Cryptography_make_openssl_module() -> std::os::raw::c_int;
-}
-#[cfg(not(python_implementation = "PyPy"))]
-extern "C" {
-    fn PyInit__openssl() -> *mut pyo3::ffi::PyObject;
-}
-
 /// Returns the value of the input with the most-significant-bit copied to all
 /// of the bits.
 fn duplicate_msb_to_all(a: u8) -> u8 {
     0u8.wrapping_sub(a >> 7)
 }
 
 /// This returns 0xFF if a < b else 0x00, but does so in a constant time
@@ -99,15 +81,15 @@
 }
 
 #[pyo3::prelude::pyfunction]
 fn raise_openssl_error() -> crate::error::CryptographyResult<()> {
     Err(openssl::error::ErrorStack::get().into())
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.openssl")]
 struct OpenSSLError {
     e: openssl::error::Error,
 }
 
 #[pyo3::pymethods]
 impl OpenSSLError {
     #[getter]
@@ -124,18 +106,15 @@
     fn reason_text(&self) -> &[u8] {
         self.e.reason().unwrap_or("").as_bytes()
     }
 
     fn _lib_reason_match(&self, lib: i32, reason: i32) -> bool {
         self.e.library_code() == lib && self.e.reason_code() == reason
     }
-}
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyObjectProtocol for OpenSSLError {
     fn __repr__(&self) -> pyo3::PyResult<String> {
         Ok(format!(
             "<OpenSSLError(code={}, lib={}, reason={}, reason_text={})>",
             self.e.code(),
             self.e.library_code(),
             self.e.reason_code(),
             self.e.reason().unwrap_or("")
@@ -148,54 +127,50 @@
     let errs = pyo3::types::PyList::empty(py);
     for e in openssl::error::ErrorStack::get().errors() {
         errs.append(pyo3::PyCell::new(py, OpenSSLError { e: e.clone() })?)?;
     }
     Ok(errs)
 }
 
+#[pyo3::prelude::pyfunction]
+fn is_fips_enabled() -> bool {
+    cryptography_openssl::fips::is_enabled()
+}
+
 #[pyo3::prelude::pymodule]
 fn _rust(py: pyo3::Python<'_>, m: &pyo3::types::PyModule) -> pyo3::PyResult<()> {
     m.add_function(pyo3::wrap_pyfunction!(check_pkcs7_padding, m)?)?;
     m.add_function(pyo3::wrap_pyfunction!(check_ansix923_padding, m)?)?;
     m.add_class::<oid::ObjectIdentifier>()?;
     m.add_class::<pool::FixedPool>()?;
 
     m.add_submodule(asn1::create_submodule(py)?)?;
     m.add_submodule(pkcs7::create_submodule(py)?)?;
+    m.add_submodule(exceptions::create_submodule(py)?)?;
 
     let x509_mod = pyo3::prelude::PyModule::new(py, "x509")?;
     crate::x509::certificate::add_to_module(x509_mod)?;
     crate::x509::common::add_to_module(x509_mod)?;
     crate::x509::crl::add_to_module(x509_mod)?;
     crate::x509::csr::add_to_module(x509_mod)?;
     crate::x509::sct::add_to_module(x509_mod)?;
     m.add_submodule(x509_mod)?;
 
     let ocsp_mod = pyo3::prelude::PyModule::new(py, "ocsp")?;
     crate::x509::ocsp_req::add_to_module(ocsp_mod)?;
     crate::x509::ocsp_resp::add_to_module(ocsp_mod)?;
     m.add_submodule(ocsp_mod)?;
 
-    #[cfg(python_implementation = "PyPy")]
-    let openssl_mod = unsafe {
-        let res = Cryptography_make_openssl_module();
-        assert_eq!(res, 0);
-        pyo3::types::PyModule::import(py, "_openssl")?
-    };
-    #[cfg(not(python_implementation = "PyPy"))]
-    let openssl_mod = unsafe {
-        let ptr = PyInit__openssl();
-        pyo3::types::PyModule::from_owned_ptr(py, ptr)
-    };
-    m.add_submodule(openssl_mod)?;
+    m.add_submodule(cryptography_cffi::create_module(py)?)?;
 
     let openssl_mod = pyo3::prelude::PyModule::new(py, "openssl")?;
     openssl_mod.add_function(pyo3::wrap_pyfunction!(openssl_version, m)?)?;
     openssl_mod.add_function(pyo3::wrap_pyfunction!(raise_openssl_error, m)?)?;
     openssl_mod.add_function(pyo3::wrap_pyfunction!(capture_error_stack, m)?)?;
+    openssl_mod.add_function(pyo3::wrap_pyfunction!(is_fips_enabled, m)?)?;
     openssl_mod.add_class::<OpenSSLError>()?;
     crate::backend::add_to_module(openssl_mod)?;
     m.add_submodule(openssl_mod)?;
 
     Ok(())
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/oid.rs` & `cryptography-41.0.0/src/rust/src/oid.rs`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::error::CryptographyResult;
 use std::collections::hash_map::DefaultHasher;
 use std::hash::{Hash, Hasher};
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust")]
 pub(crate) struct ObjectIdentifier {
     pub(crate) oid: asn1::ObjectIdentifier,
 }
 
 #[pyo3::pymethods]
 impl ObjectIdentifier {
     #[new]
@@ -27,30 +27,24 @@
 
     #[getter]
     fn _name<'p>(
         slf: pyo3::PyRef<'_, Self>,
         py: pyo3::Python<'p>,
     ) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let oid_names = py
-            .import("cryptography.hazmat._oid")?
-            .getattr(crate::intern!(py, "_OID_NAMES"))?;
-        oid_names.call_method1("get", (slf, "Unknown OID"))
+            .import(pyo3::intern!(py, "cryptography.hazmat._oid"))?
+            .getattr(pyo3::intern!(py, "_OID_NAMES"))?;
+        oid_names.call_method1(pyo3::intern!(py, "get"), (slf, "Unknown OID"))
     }
 
     fn __deepcopy__(slf: pyo3::PyRef<'_, Self>, _memo: pyo3::PyObject) -> pyo3::PyRef<'_, Self> {
         slf
     }
-}
-
-#[pyo3::prelude::pyproto]
-impl pyo3::PyObjectProtocol for ObjectIdentifier {
-    fn __repr__(&self) -> pyo3::PyResult<String> {
-        let gil = pyo3::Python::acquire_gil();
-        let py = gil.python();
 
+    fn __repr__(&self, py: pyo3::Python<'_>) -> pyo3::PyResult<String> {
         let self_clone = pyo3::PyCell::new(
             py,
             ObjectIdentifier {
                 oid: self.oid.clone(),
             },
         )?;
         let name = ObjectIdentifier::_name(self_clone.borrow(), py)?.extract::<&str>()?;
@@ -58,15 +52,15 @@
             "<ObjectIdentifier(oid={}, name={})>",
             self.oid, name
         ))
     }
 
     fn __richcmp__(
         &self,
-        other: pyo3::PyRef<ObjectIdentifier>,
+        other: pyo3::PyRef<'_, ObjectIdentifier>,
         op: pyo3::basic::CompareOp,
     ) -> pyo3::PyResult<bool> {
         match op {
             pyo3::basic::CompareOp::Eq => Ok(self.oid == other.oid),
             pyo3::basic::CompareOp::Ne => Ok(self.oid != other.oid),
             _ => Err(pyo3::exceptions::PyTypeError::new_err(
                 "ObjectIdentifiers cannot be ordered",
```

### Comparing `cryptography-40.0.2/src/rust/src/pkcs7.rs` & `cryptography-41.0.0/src/rust/src/pkcs7.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,317 +2,278 @@
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::asn1::encode_der_data;
 use crate::buf::CffiBuf;
 use crate::error::CryptographyResult;
 use crate::x509;
-
-use chrono::Timelike;
+use cryptography_x509::csr::Attribute;
+use cryptography_x509::{common, oid, pkcs7};
 use once_cell::sync::Lazy;
 use std::borrow::Cow;
 use std::collections::HashMap;
 use std::ops::Deref;
 
-const PKCS7_DATA_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 7, 1);
-const PKCS7_SIGNED_DATA_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 7, 2);
-
 const PKCS7_CONTENT_TYPE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 9, 3);
 const PKCS7_MESSAGE_DIGEST_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 9, 4);
 const PKCS7_SIGNING_TIME_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 9, 5);
 const PKCS7_SMIME_CAP_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 9, 15);
 
 const AES_256_CBC_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 1, 42);
 const AES_192_CBC_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 1, 22);
 const AES_128_CBC_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 1, 2);
 
-static EMPTY_STRING_DER: Lazy<Vec<u8>> = Lazy::new(|| {
-    // TODO: kind of verbose way to say "\x04\x00".
-    asn1::write_single(&(&[] as &[u8])).unwrap()
-});
-static EMPTY_STRING_TLV: Lazy<asn1::Tlv<'static>> =
-    Lazy::new(|| asn1::parse_single(&EMPTY_STRING_DER).unwrap());
-
 static OIDS_TO_MIC_NAME: Lazy<HashMap<&asn1::ObjectIdentifier, &str>> = Lazy::new(|| {
     let mut h = HashMap::new();
-    h.insert(&x509::oid::SHA224_OID, "sha-224");
-    h.insert(&x509::oid::SHA256_OID, "sha-256");
-    h.insert(&x509::oid::SHA384_OID, "sha-384");
-    h.insert(&x509::oid::SHA512_OID, "sha-512");
+    h.insert(&oid::SHA224_OID, "sha-224");
+    h.insert(&oid::SHA256_OID, "sha-256");
+    h.insert(&oid::SHA384_OID, "sha-384");
+    h.insert(&oid::SHA512_OID, "sha-512");
     h
 });
 
-#[derive(asn1::Asn1Write)]
-struct ContentInfo<'a> {
-    content_type: asn1::ObjectIdentifier,
-    #[explicit(0)]
-    content: Option<asn1::Tlv<'a>>,
-}
-
-#[derive(asn1::Asn1Write)]
-struct SignedData<'a> {
-    version: u8,
-    digest_algorithms: asn1::SetOfWriter<'a, x509::AlgorithmIdentifier<'a>>,
-    content_info: ContentInfo<'a>,
-    #[implicit(0)]
-    certificates: Option<asn1::SetOfWriter<'a, &'a x509::certificate::RawCertificate<'a>>>,
-
-    // We don't ever supply any of these, so for now, don't fill out the fields.
-    #[implicit(1)]
-    crls: Option<asn1::SetOfWriter<'a, asn1::Sequence<'a>>>,
-
-    signer_infos: asn1::SetOfWriter<'a, SignerInfo<'a>>,
-}
-
-#[derive(asn1::Asn1Write)]
-struct SignerInfo<'a> {
-    version: u8,
-    issuer_and_serial_number: IssuerAndSerialNumber<'a>,
-    digest_algorithm: x509::AlgorithmIdentifier<'a>,
-    #[implicit(0)]
-    authenticated_attributes: Option<x509::csr::Attributes<'a>>,
-
-    digest_encryption_algorithm: x509::AlgorithmIdentifier<'a>,
-    encrypted_digest: &'a [u8],
-
-    #[implicit(1)]
-    unauthenticated_attributes: Option<x509::csr::Attributes<'a>>,
-}
-
-#[derive(asn1::Asn1Write)]
-struct IssuerAndSerialNumber<'a> {
-    issuer: x509::Name<'a>,
-    serial_number: asn1::BigInt<'a>,
-}
-
 #[pyo3::prelude::pyfunction]
 fn serialize_certificates<'p>(
     py: pyo3::Python<'p>,
-    py_certs: Vec<pyo3::PyRef<'p, x509::Certificate>>,
+    py_certs: Vec<pyo3::PyRef<'p, x509::certificate::Certificate>>,
     encoding: &'p pyo3::PyAny,
 ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
     if py_certs.is_empty() {
         return Err(pyo3::exceptions::PyTypeError::new_err(
             "certs must be a list of certs with length >= 1",
         )
         .into());
     }
 
     let raw_certs = py_certs
         .iter()
         .map(|c| c.raw.borrow_value_public())
         .collect::<Vec<_>>();
 
-    let signed_data = SignedData {
+    let signed_data = pkcs7::SignedData {
         version: 1,
         digest_algorithms: asn1::SetOfWriter::new(&[]),
-        content_info: ContentInfo {
-            content_type: PKCS7_DATA_OID,
-            content: Some(*EMPTY_STRING_TLV),
+        content_info: pkcs7::ContentInfo {
+            _content_type: asn1::DefinedByMarker::marker(),
+            content: pkcs7::Content::Data(Some(asn1::Explicit::new(b""))),
         },
         certificates: Some(asn1::SetOfWriter::new(&raw_certs)),
         crls: None,
         signer_infos: asn1::SetOfWriter::new(&[]),
     };
 
-    let signed_data_bytes = asn1::write_single(&signed_data)?;
-
-    let content_info = ContentInfo {
-        content_type: PKCS7_SIGNED_DATA_OID,
-        content: Some(asn1::parse_single(&signed_data_bytes).unwrap()),
+    let content_info = pkcs7::ContentInfo {
+        _content_type: asn1::DefinedByMarker::marker(),
+        content: pkcs7::Content::SignedData(asn1::Explicit::new(Box::new(signed_data))),
     };
     let content_info_bytes = asn1::write_single(&content_info)?;
 
     encode_der_data(py, "PKCS7".to_string(), content_info_bytes, encoding)
 }
 
 #[pyo3::prelude::pyfunction]
 fn sign_and_serialize<'p>(
     py: pyo3::Python<'p>,
     builder: &'p pyo3::PyAny,
     encoding: &'p pyo3::PyAny,
     options: &'p pyo3::types::PyList,
 ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
     let pkcs7_options = py
-        .import("cryptography.hazmat.primitives.serialization.pkcs7")?
-        .getattr(crate::intern!(py, "PKCS7Options"))?;
+        .import(pyo3::intern!(
+            py,
+            "cryptography.hazmat.primitives.serialization.pkcs7"
+        ))?
+        .getattr(pyo3::intern!(py, "PKCS7Options"))?;
 
-    let raw_data: CffiBuf<'p> = builder.getattr(crate::intern!(py, "_data"))?.extract()?;
-    let text_mode = options.contains(pkcs7_options.getattr(crate::intern!(py, "Text"))?)?;
+    let raw_data: CffiBuf<'p> = builder.getattr(pyo3::intern!(py, "_data"))?.extract()?;
+    let text_mode = options.contains(pkcs7_options.getattr(pyo3::intern!(py, "Text"))?)?;
     let (data_with_header, data_without_header) =
-        if options.contains(pkcs7_options.getattr(crate::intern!(py, "Binary"))?)? {
+        if options.contains(pkcs7_options.getattr(pyo3::intern!(py, "Binary"))?)? {
             (
                 Cow::Borrowed(raw_data.as_bytes()),
                 Cow::Borrowed(raw_data.as_bytes()),
             )
         } else {
             smime_canonicalize(raw_data.as_bytes(), text_mode)
         };
 
-    let content_type_bytes = asn1::write_single(&PKCS7_DATA_OID)?;
-    let signing_time_bytes = asn1::write_single(&x509::certificate::time_from_chrono(
-        chrono::Utc::now().with_nanosecond(0).unwrap(),
-    )?)?;
+    let content_type_bytes = asn1::write_single(&pkcs7::PKCS7_DATA_OID)?;
+    let now = x509::common::datetime_now(py)?;
+    let signing_time_bytes = asn1::write_single(&x509::certificate::time_from_datetime(now)?)?;
     let smime_cap_bytes = asn1::write_single(&asn1::SequenceOfWriter::new([
         // Subset of values OpenSSL provides:
         // https://github.com/openssl/openssl/blob/667a8501f0b6e5705fd611d5bb3ca24848b07154/crypto/pkcs7/pk7_smime.c#L150
         // removing all the ones that are bad cryptography
         AES_256_CBC_OID,
         AES_192_CBC_OID,
         AES_128_CBC_OID,
     ]))?;
 
     let py_signers: Vec<(
-        pyo3::PyRef<'p, x509::Certificate>,
+        pyo3::PyRef<'p, x509::certificate::Certificate>,
         &pyo3::PyAny,
         &pyo3::PyAny,
-    )> = builder.getattr(crate::intern!(py, "_signers"))?.extract()?;
+    )> = builder.getattr(pyo3::intern!(py, "_signers"))?.extract()?;
 
-    let py_certs: Vec<pyo3::PyRef<'p, x509::Certificate>> = builder
-        .getattr(crate::intern!(py, "_additional_certs"))?
+    let py_certs: Vec<pyo3::PyRef<'p, x509::certificate::Certificate>> = builder
+        .getattr(pyo3::intern!(py, "_additional_certs"))?
         .extract()?;
 
     let mut signer_infos = vec![];
     let mut digest_algs = vec![];
     let mut certs = py_certs
         .iter()
         .map(|p| p.raw.borrow_value_public())
         .collect::<Vec<_>>();
     for (cert, py_private_key, py_hash_alg) in &py_signers {
         let (authenticated_attrs, signature) = if options
-            .contains(pkcs7_options.getattr(crate::intern!(py, "NoAttributes"))?)?
+            .contains(pkcs7_options.getattr(pyo3::intern!(py, "NoAttributes"))?)?
         {
             (
                 None,
-                x509::sign::sign_data(py, py_private_key, py_hash_alg, &data_with_header)?,
+                x509::sign::sign_data(
+                    py,
+                    py_private_key,
+                    py_hash_alg,
+                    py.None().into_ref(py),
+                    &data_with_header,
+                )?,
             )
         } else {
-            let mut authenticated_attrs = vec![];
-
-            authenticated_attrs.push(x509::csr::Attribute {
-                type_id: PKCS7_CONTENT_TYPE_OID,
-                values: x509::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
-                    asn1::parse_single(&content_type_bytes).unwrap(),
-                ])),
-            });
-            authenticated_attrs.push(x509::csr::Attribute {
-                type_id: PKCS7_SIGNING_TIME_OID,
-                values: x509::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
-                    asn1::parse_single(&signing_time_bytes).unwrap(),
-                ])),
-            });
+            let mut authenticated_attrs = vec![
+                Attribute {
+                    type_id: PKCS7_CONTENT_TYPE_OID,
+                    values: common::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
+                        asn1::parse_single(&content_type_bytes).unwrap(),
+                    ])),
+                },
+                Attribute {
+                    type_id: PKCS7_SIGNING_TIME_OID,
+                    values: common::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
+                        asn1::parse_single(&signing_time_bytes).unwrap(),
+                    ])),
+                },
+            ];
 
             let digest =
                 asn1::write_single(&x509::ocsp::hash_data(py, py_hash_alg, &data_with_header)?)?;
             // Gross hack: copy to PyBytes to extend the lifetime to 'p
             let digest_bytes = pyo3::types::PyBytes::new(py, &digest);
-            authenticated_attrs.push(x509::csr::Attribute {
+            authenticated_attrs.push(Attribute {
                 type_id: PKCS7_MESSAGE_DIGEST_OID,
-                values: x509::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
+                values: common::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
                     asn1::parse_single(digest_bytes.as_bytes()).unwrap(),
                 ])),
             });
 
-            if !options.contains(pkcs7_options.getattr(crate::intern!(py, "NoCapabilities"))?)? {
-                authenticated_attrs.push(x509::csr::Attribute {
+            if !options.contains(pkcs7_options.getattr(pyo3::intern!(py, "NoCapabilities"))?)? {
+                authenticated_attrs.push(Attribute {
                     type_id: PKCS7_SMIME_CAP_OID,
-                    values: x509::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
+                    values: common::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
                         asn1::parse_single(&smime_cap_bytes).unwrap(),
                     ])),
                 });
             }
 
             let signed_data =
                 asn1::write_single(&asn1::SetOfWriter::new(authenticated_attrs.as_slice()))?;
 
             (
-                Some(x509::Asn1ReadableOrWritable::new_write(
+                Some(common::Asn1ReadableOrWritable::new_write(
                     asn1::SetOfWriter::new(authenticated_attrs),
                 )),
-                x509::sign::sign_data(py, py_private_key, py_hash_alg, &signed_data)?,
+                x509::sign::sign_data(
+                    py,
+                    py_private_key,
+                    py_hash_alg,
+                    py.None().into_ref(py),
+                    &signed_data,
+                )?,
             )
         };
 
-        let digest_alg = x509::AlgorithmIdentifier {
-            oid: x509::ocsp::HASH_NAME_TO_OIDS[py_hash_alg
-                .getattr(crate::intern!(py, "name"))?
-                .extract::<&str>()?]
-            .clone(),
-            params: Some(*x509::sign::NULL_TLV),
-        };
+        let digest_alg = x509::ocsp::HASH_NAME_TO_ALGORITHM_IDENTIFIERS[py_hash_alg
+            .getattr(pyo3::intern!(py, "name"))?
+            .extract::<&str>()?]
+        .clone();
         // Technically O(n^2), but no one will have that many signers.
         if !digest_algs.contains(&digest_alg) {
             digest_algs.push(digest_alg.clone());
         }
         certs.push(cert.raw.borrow_value_public());
 
-        signer_infos.push(SignerInfo {
+        signer_infos.push(pkcs7::SignerInfo {
             version: 1,
-            issuer_and_serial_number: IssuerAndSerialNumber {
+            issuer_and_serial_number: pkcs7::IssuerAndSerialNumber {
                 issuer: cert.raw.borrow_value_public().tbs_cert.issuer.clone(),
                 serial_number: cert.raw.borrow_value_public().tbs_cert.serial,
             },
             digest_algorithm: digest_alg,
             authenticated_attributes: authenticated_attrs,
             digest_encryption_algorithm: x509::sign::compute_signature_algorithm(
                 py,
                 py_private_key,
                 py_hash_alg,
+                py.None().into_ref(py),
             )?,
             encrypted_digest: signature,
             unauthenticated_attributes: None,
         });
     }
 
     let data_tlv_bytes;
     let content =
-        if options.contains(pkcs7_options.getattr(crate::intern!(py, "DetachedSignature"))?)? {
+        if options.contains(pkcs7_options.getattr(pyo3::intern!(py, "DetachedSignature"))?)? {
             None
         } else {
             data_tlv_bytes = asn1::write_single(&data_with_header.deref())?;
             Some(asn1::parse_single(&data_tlv_bytes).unwrap())
         };
 
-    let signed_data = SignedData {
+    let signed_data = pkcs7::SignedData {
         version: 1,
         digest_algorithms: asn1::SetOfWriter::new(&digest_algs),
-        content_info: ContentInfo {
-            content_type: PKCS7_DATA_OID,
-            content,
+        content_info: pkcs7::ContentInfo {
+            _content_type: asn1::DefinedByMarker::marker(),
+            content: pkcs7::Content::Data(content.map(asn1::Explicit::new)),
         },
-        certificates: if options.contains(pkcs7_options.getattr(crate::intern!(py, "NoCerts"))?)? {
+        certificates: if options.contains(pkcs7_options.getattr(pyo3::intern!(py, "NoCerts"))?)? {
             None
         } else {
             Some(asn1::SetOfWriter::new(&certs))
         },
         crls: None,
         signer_infos: asn1::SetOfWriter::new(&signer_infos),
     };
 
-    let signed_data_bytes = asn1::write_single(&signed_data)?;
-
-    let content_info = ContentInfo {
-        content_type: PKCS7_SIGNED_DATA_OID,
-        content: Some(asn1::parse_single(&signed_data_bytes).unwrap()),
+    let content_info = pkcs7::ContentInfo {
+        _content_type: asn1::DefinedByMarker::marker(),
+        content: pkcs7::Content::SignedData(asn1::Explicit::new(Box::new(signed_data))),
     };
     let ci_bytes = asn1::write_single(&content_info)?;
 
     let encoding_class = py
-        .import("cryptography.hazmat.primitives.serialization")?
-        .getattr(crate::intern!(py, "Encoding"))?;
+        .import(pyo3::intern!(
+            py,
+            "cryptography.hazmat.primitives.serialization"
+        ))?
+        .getattr(pyo3::intern!(py, "Encoding"))?;
 
-    if encoding == encoding_class.getattr(crate::intern!(py, "SMIME"))? {
+    if encoding.is(encoding_class.getattr(pyo3::intern!(py, "SMIME"))?) {
         let mic_algs = digest_algs
             .iter()
-            .map(|d| OIDS_TO_MIC_NAME[&d.oid])
+            .map(|d| OIDS_TO_MIC_NAME[&d.oid()])
             .collect::<Vec<_>>()
             .join(",");
         let smime_encode = py
-            .import("cryptography.hazmat.primitives.serialization.pkcs7")?
-            .getattr(crate::intern!(py, "_smime_encode"))?;
+            .import(pyo3::intern!(
+                py,
+                "cryptography.hazmat.primitives.serialization.pkcs7"
+            ))?
+            .getattr(pyo3::intern!(py, "_smime_encode"))?;
         Ok(smime_encode
             .call1((&*data_without_header, &*ci_bytes, mic_algs, text_mode))?
             .extract()?)
     } else {
         // Handles the DER, PEM, and error cases
         encode_der_data(py, "PKCS7".to_string(), ci_bytes, encoding)
     }
@@ -351,16 +312,16 @@
         (Cow::Borrowed(data), Cow::Borrowed(data))
     }
 }
 
 pub(crate) fn create_submodule(py: pyo3::Python<'_>) -> pyo3::PyResult<&pyo3::prelude::PyModule> {
     let submod = pyo3::prelude::PyModule::new(py, "pkcs7")?;
 
-    submod.add_wrapped(pyo3::wrap_pyfunction!(serialize_certificates))?;
-    submod.add_wrapped(pyo3::wrap_pyfunction!(sign_and_serialize))?;
+    submod.add_function(pyo3::wrap_pyfunction!(serialize_certificates, submod)?)?;
+    submod.add_function(pyo3::wrap_pyfunction!(sign_and_serialize, submod)?)?;
 
     Ok(submod)
 }
 
 #[cfg(test)]
 mod tests {
     use super::smime_canonicalize;
```

### Comparing `cryptography-40.0.2/src/rust/src/pool.rs` & `cryptography-41.0.0/src/rust/src/pool.rs`

 * *Files 27% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 // for complete details.
 
 use std::cell::Cell;
 
 // An object pool that can contain a single object and will dynamically
 // allocate new objects to fulfill requests if the pool'd object is already in
 // use.
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust")]
 pub(crate) struct FixedPool {
     create_fn: pyo3::PyObject,
 
     value: Cell<Option<pyo3::PyObject>>,
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust")]
 struct PoolAcquisition {
     pool: pyo3::Py<FixedPool>,
 
     value: pyo3::PyObject,
     fresh: bool,
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/certificate.rs` & `cryptography-41.0.0/src/rust/src/x509/certificate.rs`

 * *Files 15% similar despite different names*

```diff
@@ -2,155 +2,122 @@
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::asn1::{
     big_byte_slice_to_py_int, encode_der_data, oid_to_py_oid, py_uint_to_big_endian_bytes,
 };
 use crate::error::{CryptographyError, CryptographyResult};
-use crate::x509;
-use crate::x509::{crl, extensions, oid, sct, sign, Asn1ReadableOrWritable};
-use chrono::Datelike;
-use pyo3::ToPyObject;
+use crate::x509::{extensions, sct, sign};
+use crate::{exceptions, x509};
+use cryptography_x509::common::Asn1ReadableOrWritable;
+use cryptography_x509::extensions::Extension;
+use cryptography_x509::extensions::{
+    AuthorityKeyIdentifier, BasicConstraints, DisplayText, DistributionPoint,
+    DistributionPointName, MSCertificateTemplate, NameConstraints, PolicyConstraints,
+    PolicyInformation, PolicyQualifierInfo, Qualifier, RawExtensions, SequenceOfAccessDescriptions,
+    SequenceOfSubtrees, UserNotice,
+};
+use cryptography_x509::{common, name, oid};
+use pyo3::{IntoPy, ToPyObject};
 use std::collections::hash_map::DefaultHasher;
 use std::hash::{Hash, Hasher};
-use std::sync::Arc;
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write, Hash, PartialEq, Clone)]
-pub(crate) struct RawCertificate<'a> {
-    pub(crate) tbs_cert: TbsCertificate<'a>,
-    signature_alg: x509::AlgorithmIdentifier<'a>,
-    signature: asn1::BitString<'a>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write, Hash, PartialEq, Clone)]
-pub(crate) struct TbsCertificate<'a> {
-    #[explicit(0)]
-    #[default(0)]
-    version: u8,
-    pub(crate) serial: asn1::BigInt<'a>,
-    signature_alg: x509::AlgorithmIdentifier<'a>,
-
-    pub(crate) issuer: x509::Name<'a>,
-    validity: Validity,
-    pub(crate) subject: x509::Name<'a>,
-
-    pub(crate) spki: SubjectPublicKeyInfo<'a>,
-    #[implicit(1)]
-    issuer_unique_id: Option<asn1::BitString<'a>>,
-    #[implicit(2)]
-    subject_unique_id: Option<asn1::BitString<'a>>,
-    #[explicit(3)]
-    extensions: Option<x509::Extensions<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write, Hash, PartialEq, Clone)]
-pub(crate) struct Validity {
-    not_before: x509::Time,
-    not_after: x509::Time,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write, Hash, PartialEq, Clone)]
-pub(crate) struct SubjectPublicKeyInfo<'a> {
-    _algorithm: x509::AlgorithmIdentifier<'a>,
-    pub(crate) subject_public_key: asn1::BitString<'a>,
-}
 
 #[ouroboros::self_referencing]
-pub(crate) struct OwnedRawCertificate {
-    data: Arc<[u8]>,
+pub(crate) struct OwnedCertificate {
+    data: pyo3::Py<pyo3::types::PyBytes>,
 
     #[borrows(data)]
     #[covariant]
-    value: RawCertificate<'this>,
+    value: cryptography_x509::certificate::Certificate<'this>,
 }
 
-impl OwnedRawCertificate {
+impl OwnedCertificate {
     // Re-expose ::new with `pub(crate)` visibility.
     pub(crate) fn new_public(
-        data: Arc<[u8]>,
-        value_ref_builder: impl for<'this> FnOnce(&'this Arc<[u8]>) -> RawCertificate<'this>,
-    ) -> OwnedRawCertificate {
-        OwnedRawCertificate::new(data, value_ref_builder)
+        data: pyo3::Py<pyo3::types::PyBytes>,
+        value_ref_builder: impl for<'this> FnOnce(
+            &'this pyo3::Py<pyo3::types::PyBytes>,
+        )
+            -> cryptography_x509::certificate::Certificate<'this>,
+    ) -> OwnedCertificate {
+        OwnedCertificate::new(data, value_ref_builder)
     }
 
-    pub(crate) fn borrow_value_public(&self) -> &RawCertificate<'_> {
+    pub(crate) fn borrow_value_public(&self) -> &cryptography_x509::certificate::Certificate<'_> {
         self.borrow_value()
     }
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.x509")]
 pub(crate) struct Certificate {
-    pub(crate) raw: OwnedRawCertificate,
+    pub(crate) raw: OwnedCertificate,
     pub(crate) cached_extensions: Option<pyo3::PyObject>,
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyObjectProtocol for Certificate {
+#[pyo3::prelude::pymethods]
+impl Certificate {
     fn __hash__(&self) -> u64 {
         let mut hasher = DefaultHasher::new();
         self.raw.borrow_value().hash(&mut hasher);
         hasher.finish()
     }
 
     fn __richcmp__(
         &self,
-        other: pyo3::PyRef<Certificate>,
+        other: pyo3::PyRef<'_, Certificate>,
         op: pyo3::basic::CompareOp,
     ) -> pyo3::PyResult<bool> {
         match op {
             pyo3::basic::CompareOp::Eq => Ok(self.raw.borrow_value() == other.raw.borrow_value()),
             pyo3::basic::CompareOp::Ne => Ok(self.raw.borrow_value() != other.raw.borrow_value()),
             _ => Err(pyo3::exceptions::PyTypeError::new_err(
                 "Certificates cannot be ordered",
             )),
         }
     }
 
-    fn __repr__(&self) -> pyo3::PyResult<String> {
-        let gil = pyo3::Python::acquire_gil();
-        let py = gil.python();
-
+    fn __repr__(&self, py: pyo3::Python<'_>) -> pyo3::PyResult<String> {
         let subject = self.subject(py)?;
         let subject_repr = subject.repr()?.extract::<&str>()?;
         Ok(format!("<Certificate(subject={}, ...)>", subject_repr))
     }
-}
 
-#[pyo3::prelude::pymethods]
-impl Certificate {
     fn __deepcopy__(slf: pyo3::PyRef<'_, Self>, _memo: pyo3::PyObject) -> pyo3::PyRef<'_, Self> {
         slf
     }
 
     fn public_key<'p>(&self, py: pyo3::Python<'p>) -> CryptographyResult<&'p pyo3::PyAny> {
         // This makes an unnecessary copy. It'd be nice to get rid of it.
         let serialized = pyo3::types::PyBytes::new(
             py,
             &asn1::write_single(&self.raw.borrow_value().tbs_cert.spki)?,
         );
         Ok(py
-            .import("cryptography.hazmat.primitives.serialization")?
-            .getattr(crate::intern!(py, "load_der_public_key"))?
+            .import(pyo3::intern!(
+                py,
+                "cryptography.hazmat.primitives.serialization"
+            ))?
+            .getattr(pyo3::intern!(py, "load_der_public_key"))?
             .call1((serialized,))?)
     }
 
     fn fingerprint<'p>(
         &self,
         py: pyo3::Python<'p>,
         algorithm: pyo3::PyObject,
     ) -> CryptographyResult<&'p pyo3::PyAny> {
         let hasher = py
-            .import("cryptography.hazmat.primitives.hashes")?
-            .getattr(crate::intern!(py, "Hash"))?
+            .import(pyo3::intern!(py, "cryptography.hazmat.primitives.hashes"))?
+            .getattr(pyo3::intern!(py, "Hash"))?
             .call1((algorithm,))?;
         // This makes an unnecessary copy. It'd be nice to get rid of it.
         let serialized =
             pyo3::types::PyBytes::new(py, &asn1::write_single(&self.raw.borrow_value())?);
-        hasher.call_method1("update", (serialized,))?;
-        Ok(hasher.call_method0("finalize")?)
+        hasher.call_method1(pyo3::intern!(py, "update"), (serialized,))?;
+        Ok(hasher.call_method0(pyo3::intern!(py, "finalize"))?)
     }
 
     fn public_bytes<'p>(
         &self,
         py: pyo3::Python<'p>,
         encoding: &'p pyo3::PyAny,
     ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
@@ -204,122 +171,128 @@
     fn tbs_precertificate_bytes<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
         let val = self.raw.borrow_value();
         let mut tbs_precert = val.tbs_cert.clone();
         // Remove the SCT list extension
-        match tbs_precert.extensions {
-            Some(extensions) => {
-                let readable_extensions = extensions.unwrap_read().clone();
+        match val.tbs_cert.extensions() {
+            Ok(extensions) => {
+                let readable_extensions = match extensions.as_raw() {
+                    Some(raw_exts) => raw_exts.unwrap_read().clone(),
+                    None => {
+                        return Err(CryptographyError::from(
+                            pyo3::exceptions::PyValueError::new_err(
+                                "Could not find any extensions in TBS certificate",
+                            ),
+                        ))
+                    }
+                };
                 let ext_count = readable_extensions.len();
-                let filtered_extensions: Vec<x509::common::Extension<'_>> = readable_extensions
+                let filtered_extensions: Vec<Extension<'_>> = readable_extensions
                     .filter(|x| x.extn_id != oid::PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS_OID)
                     .collect();
                 if filtered_extensions.len() == ext_count {
                     return Err(CryptographyError::from(
                         pyo3::exceptions::PyValueError::new_err(
                             "Could not find pre-certificate SCT list extension",
                         ),
                     ));
                 }
-                let filtered_extensions: x509::Extensions<'_> = Asn1ReadableOrWritable::new_write(
+                let filtered_extensions: RawExtensions<'_> = Asn1ReadableOrWritable::new_write(
                     asn1::SequenceOfWriter::new(filtered_extensions),
                 );
-                tbs_precert.extensions = Some(filtered_extensions);
+
+                tbs_precert.raw_extensions = Some(filtered_extensions);
                 let result = asn1::write_single(&tbs_precert)?;
                 Ok(pyo3::types::PyBytes::new(py, &result))
             }
-            None => Err(CryptographyError::from(
-                pyo3::exceptions::PyValueError::new_err(
-                    "Could not find any extensions in TBS certificate",
-                ),
-            )),
+            Err(oid) => {
+                let oid_obj = oid_to_py_oid(py, &oid)?;
+                Err(exceptions::DuplicateExtension::new_err((
+                    format!("Duplicate {} extension found", oid),
+                    oid_obj.into_py(py),
+                ))
+                .into())
+            }
         }
     }
 
     #[getter]
     fn signature<'p>(&self, py: pyo3::Python<'p>) -> &'p pyo3::types::PyBytes {
         pyo3::types::PyBytes::new(py, self.raw.borrow_value().signature.as_bytes())
     }
 
     #[getter]
     fn not_valid_before<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        let chrono = &self
+        let dt = &self
             .raw
             .borrow_value()
             .tbs_cert
             .validity
             .not_before
-            .as_chrono();
-        x509::chrono_to_py(py, chrono)
+            .as_datetime();
+        x509::datetime_to_py(py, dt)
     }
 
     #[getter]
     fn not_valid_after<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        let chrono = &self
+        let dt = &self
             .raw
             .borrow_value()
             .tbs_cert
             .validity
             .not_after
-            .as_chrono();
-        x509::chrono_to_py(py, chrono)
+            .as_datetime();
+        x509::datetime_to_py(py, dt)
     }
 
     #[getter]
     fn signature_hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> Result<&'p pyo3::PyAny, CryptographyError> {
-        let sig_oids_to_hash = py
-            .import("cryptography.hazmat._oid")?
-            .getattr(crate::intern!(py, "_SIG_OIDS_TO_HASH"))?;
-        let hash_alg = sig_oids_to_hash.get_item(self.signature_algorithm_oid(py)?);
-        match hash_alg {
-            Ok(data) => Ok(data),
-            Err(_) => Err(CryptographyError::from(pyo3::PyErr::from_instance(
-                py.import("cryptography.exceptions")?.call_method1(
-                    "UnsupportedAlgorithm",
-                    (format!(
-                        "Signature algorithm OID: {} not recognized",
-                        self.raw.borrow_value().signature_alg.oid
-                    ),),
-                )?,
-            ))),
-        }
+        sign::identify_signature_hash_algorithm(py, &self.raw.borrow_value().signature_alg)
     }
 
     #[getter]
     fn signature_algorithm_oid<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        oid_to_py_oid(py, &self.raw.borrow_value().signature_alg.oid)
+        oid_to_py_oid(py, self.raw.borrow_value().signature_alg.oid())
+    }
+
+    #[getter]
+    fn signature_algorithm_parameters<'p>(
+        &'p self,
+        py: pyo3::Python<'p>,
+    ) -> CryptographyResult<&'p pyo3::PyAny> {
+        sign::identify_signature_algorithm_parameters(py, &self.raw.borrow_value().signature_alg)
     }
 
     #[getter]
     fn extensions(&mut self, py: pyo3::Python<'_>) -> pyo3::PyResult<pyo3::PyObject> {
-        let x509_module = py.import("cryptography.x509")?;
+        let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
         x509::parse_and_cache_extensions(
             py,
             &mut self.cached_extensions,
-            &self.raw.borrow_value().tbs_cert.extensions,
+            &self.raw.borrow_value().tbs_cert.raw_extensions,
             |oid, ext_data| match *oid {
                 oid::PRECERT_POISON_OID => {
                     asn1::parse_single::<()>(ext_data)?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "PrecertPoison"))?
+                            .getattr(pyo3::intern!(py, "PrecertPoison"))?
                             .call0()?,
                     ))
                 }
                 oid::PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS_OID => {
                     let contents = asn1::parse_single::<&[u8]>(ext_data)?;
                     let scts = sct::parse_scts(py, contents, sct::LogEntryType::PreCertificate)?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(
+                            .getattr(pyo3::intern!(
                                 py,
                                 "PrecertificateSignedCertificateTimestamps"
                             ))?
                             .call1((scts,))?,
                     ))
                 }
                 _ => parse_cert_ext(py, oid.clone(), ext_data),
@@ -340,74 +313,83 @@
         if self.raw.borrow_value().tbs_cert.issuer != issuer.raw.borrow_value().tbs_cert.subject {
             return Err(CryptographyError::from(
                 pyo3::exceptions::PyValueError::new_err(
                     "Issuer certificate subject does not match certificate issuer.",
                 ),
             ));
         };
-        sign::verify_signature_with_oid(
+        sign::verify_signature_with_signature_algorithm(
             py,
             issuer.public_key(py)?,
-            &self.raw.borrow_value().signature_alg.oid,
+            &self.raw.borrow_value().signature_alg,
             self.raw.borrow_value().signature.as_bytes(),
             &asn1::write_single(&self.raw.borrow_value().tbs_cert)?,
         )
     }
 }
 
 fn cert_version(py: pyo3::Python<'_>, version: u8) -> Result<&pyo3::PyAny, CryptographyError> {
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     match version {
         0 => Ok(x509_module
-            .getattr(crate::intern!(py, "Version"))?
-            .get_item("v1")?),
+            .getattr(pyo3::intern!(py, "Version"))?
+            .get_item(pyo3::intern!(py, "v1"))?),
         2 => Ok(x509_module
-            .getattr(crate::intern!(py, "Version"))?
-            .get_item("v3")?),
-        _ => Err(CryptographyError::from(pyo3::PyErr::from_instance(
-            x509_module
-                .getattr(crate::intern!(py, "InvalidVersion"))?
-                .call1((format!("{} is not a valid X509 version", version), version))?,
-        ))),
+            .getattr(pyo3::intern!(py, "Version"))?
+            .get_item(pyo3::intern!(py, "v3"))?),
+        _ => Err(CryptographyError::from(
+            exceptions::InvalidVersion::new_err((
+                format!("{} is not a valid X509 version", version),
+                version,
+            )),
+        )),
     }
 }
 
 #[pyo3::prelude::pyfunction]
 fn load_pem_x509_certificate(py: pyo3::Python<'_>, data: &[u8]) -> CryptographyResult<Certificate> {
     // We support both PEM header strings that OpenSSL does
     // https://github.com/openssl/openssl/blob/5e2d22d53ed322a7124e26a4fbd116a8210eb77a/include/openssl/pem.h#L32-L33
     let parsed = x509::find_in_pem(
         data,
         |p| p.tag == "CERTIFICATE" || p.tag == "X509 CERTIFICATE",
         "Valid PEM but no BEGIN CERTIFICATE/END CERTIFICATE delimiters. Are you sure this is a certificate?",
     )?;
-    load_der_x509_certificate(py, &parsed.contents)
+    load_der_x509_certificate(
+        py,
+        pyo3::types::PyBytes::new(py, &parsed.contents).into_py(py),
+    )
 }
 
 #[pyo3::prelude::pyfunction]
 fn load_pem_x509_certificates(
     py: pyo3::Python<'_>,
     data: &[u8],
 ) -> CryptographyResult<Vec<Certificate>> {
     let certs = pem::parse_many(data)?
         .iter()
         .filter(|p| p.tag == "CERTIFICATE" || p.tag == "X509 CERTIFICATE")
-        .map(|p| load_der_x509_certificate(py, &p.contents))
+        .map(|p| {
+            load_der_x509_certificate(py, pyo3::types::PyBytes::new(py, &p.contents).into_py(py))
+        })
         .collect::<Result<Vec<_>, _>>()?;
 
     if certs.is_empty() {
         return Err(CryptographyError::from(pem::PemError::MalformedFraming));
     }
 
     Ok(certs)
 }
 
 #[pyo3::prelude::pyfunction]
-fn load_der_x509_certificate(py: pyo3::Python<'_>, data: &[u8]) -> CryptographyResult<Certificate> {
-    let raw = OwnedRawCertificate::try_new(Arc::from(data), |data| asn1::parse_single(data))?;
+fn load_der_x509_certificate(
+    py: pyo3::Python<'_>,
+    data: pyo3::Py<pyo3::types::PyBytes>,
+) -> CryptographyResult<Certificate> {
+    let raw = OwnedCertificate::try_new(data, |data| asn1::parse_single(data.as_bytes(py)))?;
     // Parse cert version immediately so we can raise error on parse if it is invalid.
     cert_version(py, raw.borrow_value().tbs_cert.version)?;
     // determine if the serial is negative and raise a warning if it is. We want to drop support
     // for this sort of invalid encoding eventually.
     warn_if_negative_serial(py, raw.borrow_value().tbs_cert.serial.as_bytes())?;
 
     Ok(Certificate {
@@ -415,121 +397,84 @@
         cached_extensions: None,
     })
 }
 
 fn warn_if_negative_serial(py: pyo3::Python<'_>, bytes: &'_ [u8]) -> pyo3::PyResult<()> {
     if bytes[0] & 0x80 != 0 {
         let cryptography_warning = py
-            .import("cryptography.utils")?
-            .getattr(crate::intern!(py, "DeprecatedIn36"))?;
+            .import(pyo3::intern!(py, "cryptography.utils"))?
+            .getattr(pyo3::intern!(py, "DeprecatedIn36"))?;
         pyo3::PyErr::warn(
             py,
             cryptography_warning,
             "Parsed a negative serial number, which is disallowed by RFC 5280.",
             1,
         )?;
     }
     Ok(())
 }
 
-// Needed due to clippy type complexity warning.
-type SequenceOfPolicyQualifiers<'a> = x509::Asn1ReadableOrWritable<
-    'a,
-    asn1::SequenceOf<'a, PolicyQualifierInfo<'a>>,
-    asn1::SequenceOfWriter<'a, PolicyQualifierInfo<'a>, Vec<PolicyQualifierInfo<'a>>>,
->;
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct PolicyInformation<'a> {
-    pub policy_identifier: asn1::ObjectIdentifier,
-    pub policy_qualifiers: Option<SequenceOfPolicyQualifiers<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct PolicyQualifierInfo<'a> {
-    pub policy_qualifier_id: asn1::ObjectIdentifier,
-    pub qualifier: Qualifier<'a>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) enum Qualifier<'a> {
-    CpsUri(asn1::IA5String<'a>),
-    UserNotice(UserNotice<'a>),
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct UserNotice<'a> {
-    pub notice_ref: Option<NoticeReference<'a>>,
-    pub explicit_text: Option<DisplayText<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct NoticeReference<'a> {
-    pub organization: DisplayText<'a>,
-    pub notice_numbers: x509::Asn1ReadableOrWritable<
-        'a,
-        asn1::SequenceOf<'a, asn1::BigUint<'a>>,
-        asn1::SequenceOfWriter<'a, asn1::BigUint<'a>, Vec<asn1::BigUint<'a>>>,
-    >,
-}
-
-// DisplayText also allows BMPString, which we currently do not support.
-#[allow(clippy::enum_variant_names)]
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) enum DisplayText<'a> {
-    IA5String(asn1::IA5String<'a>),
-    Utf8String(asn1::Utf8String<'a>),
-    VisibleString(asn1::VisibleString<'a>),
-    BmpString(asn1::BMPString<'a>),
-}
-
 fn parse_display_text(
     py: pyo3::Python<'_>,
     text: DisplayText<'_>,
 ) -> pyo3::PyResult<pyo3::PyObject> {
     match text {
         DisplayText::IA5String(o) => Ok(pyo3::types::PyString::new(py, o.as_str()).to_object(py)),
         DisplayText::Utf8String(o) => Ok(pyo3::types::PyString::new(py, o.as_str()).to_object(py)),
         DisplayText::VisibleString(o) => {
+            if asn1::VisibleString::new(o.as_str()).is_none() {
+                let cryptography_warning = py
+                    .import(pyo3::intern!(py, "cryptography.utils"))?
+                    .getattr(pyo3::intern!(py, "DeprecatedIn41"))?;
+                pyo3::PyErr::warn(
+                    py,
+                    cryptography_warning,
+                    "Invalid ASN.1 (UTF-8 characters in a VisibleString) in the explicit text and/or notice reference of the certificate policies extension. In a future version of cryptography, an exception will be raised.",
+                    1,
+                )?;
+            }
             Ok(pyo3::types::PyString::new(py, o.as_str()).to_object(py))
         }
         DisplayText::BmpString(o) => {
             let py_bytes = pyo3::types::PyBytes::new(py, o.as_utf16_be_bytes());
             // TODO: do the string conversion in rust perhaps
             Ok(py_bytes
-                .call_method1("decode", ("utf_16_be",))?
+                .call_method1(
+                    pyo3::intern!(py, "decode"),
+                    (pyo3::intern!(py, "utf_16_be"),),
+                )?
                 .to_object(py))
         }
     }
 }
 
 fn parse_user_notice(
     py: pyo3::Python<'_>,
     un: UserNotice<'_>,
 ) -> Result<pyo3::PyObject, CryptographyError> {
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     let et = match un.explicit_text {
         Some(data) => parse_display_text(py, data)?,
         None => py.None(),
     };
     let nr = match un.notice_ref {
         Some(data) => {
             let org = parse_display_text(py, data.organization)?;
             let numbers = pyo3::types::PyList::empty(py);
             for num in data.notice_numbers.unwrap_read().clone() {
                 numbers.append(big_byte_slice_to_py_int(py, num.as_bytes())?.to_object(py))?;
             }
             x509_module
-                .call_method1("NoticeReference", (org, numbers))?
+                .call_method1(pyo3::intern!(py, "NoticeReference"), (org, numbers))?
                 .to_object(py)
         }
         None => py.None(),
     };
     Ok(x509_module
-        .call_method1("UserNotice", (nr, et))?
+        .call_method1(pyo3::intern!(py, "UserNotice"), (nr, et))?
         .to_object(py))
 }
 
 fn parse_policy_qualifiers<'a>(
     py: pyo3::Python<'_>,
     policy_qualifiers: &asn1::SequenceOf<'a, PolicyQualifierInfo<'a>>,
 ) -> Result<pyo3::PyObject, CryptographyError> {
@@ -561,108 +506,43 @@
         py_pq.append(qualifier)?;
     }
     Ok(py_pq.to_object(py))
 }
 
 fn parse_cp(py: pyo3::Python<'_>, ext_data: &[u8]) -> Result<pyo3::PyObject, CryptographyError> {
     let cp = asn1::parse_single::<asn1::SequenceOf<'_, PolicyInformation<'_>>>(ext_data)?;
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     let certificate_policies = pyo3::types::PyList::empty(py);
     for policyinfo in cp {
         let pi_oid = oid_to_py_oid(py, &policyinfo.policy_identifier)?.to_object(py);
         let py_pqis = match policyinfo.policy_qualifiers {
             Some(policy_qualifiers) => {
                 parse_policy_qualifiers(py, policy_qualifiers.unwrap_read())?
             }
             None => py.None(),
         };
         let pi = x509_module
-            .call_method1("PolicyInformation", (pi_oid, py_pqis))?
+            .call_method1(pyo3::intern!(py, "PolicyInformation"), (pi_oid, py_pqis))?
             .to_object(py);
         certificate_policies.append(pi)?;
     }
     Ok(certificate_policies.to_object(py))
 }
 
-// Needed due to clippy type complexity warning.
-pub(crate) type SequenceOfSubtrees<'a> = x509::Asn1ReadableOrWritable<
-    'a,
-    asn1::SequenceOf<'a, GeneralSubtree<'a>>,
-    asn1::SequenceOfWriter<'a, GeneralSubtree<'a>, Vec<GeneralSubtree<'a>>>,
->;
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct NameConstraints<'a> {
-    #[implicit(0)]
-    pub permitted_subtrees: Option<SequenceOfSubtrees<'a>>,
-
-    #[implicit(1)]
-    pub excluded_subtrees: Option<SequenceOfSubtrees<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct GeneralSubtree<'a> {
-    pub base: x509::GeneralName<'a>,
-
-    #[implicit(0)]
-    #[default(0u64)]
-    pub minimum: u64,
-
-    #[implicit(1)]
-    pub maximum: Option<u64>,
-}
-
 fn parse_general_subtrees(
     py: pyo3::Python<'_>,
     subtrees: SequenceOfSubtrees<'_>,
 ) -> Result<pyo3::PyObject, CryptographyError> {
     let gns = pyo3::types::PyList::empty(py);
     for gs in subtrees.unwrap_read().clone() {
         gns.append(x509::parse_general_name(py, gs.base)?)?;
     }
     Ok(gns.to_object(py))
 }
 
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct DistributionPoint<'a> {
-    #[explicit(0)]
-    pub distribution_point: Option<DistributionPointName<'a>>,
-
-    #[implicit(1)]
-    pub reasons: crl::ReasonFlags<'a>,
-
-    #[implicit(2)]
-    pub crl_issuer: Option<x509::common::SequenceOfGeneralName<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) enum DistributionPointName<'a> {
-    #[implicit(0)]
-    FullName(x509::common::SequenceOfGeneralName<'a>),
-
-    #[implicit(1)]
-    NameRelativeToCRLIssuer(
-        x509::Asn1ReadableOrWritable<
-            'a,
-            asn1::SetOf<'a, x509::AttributeTypeValue<'a>>,
-            asn1::SetOfWriter<'a, x509::AttributeTypeValue<'a>, Vec<x509::AttributeTypeValue<'a>>>,
-        >,
-    ),
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct AuthorityKeyIdentifier<'a> {
-    #[implicit(0)]
-    pub key_identifier: Option<&'a [u8]>,
-    #[implicit(1)]
-    pub authority_cert_issuer: Option<x509::common::SequenceOfGeneralName<'a>>,
-    #[implicit(2)]
-    pub authority_cert_serial_number: Option<asn1::BigUint<'a>>,
-}
-
 pub(crate) fn parse_distribution_point_name(
     py: pyo3::Python<'_>,
     dp: DistributionPointName<'_>,
 ) -> Result<(pyo3::PyObject, pyo3::PyObject), CryptographyError> {
     Ok(match dp {
         DistributionPointName::FullName(data) => (
             x509::parse_general_names(py, data.unwrap_read())?,
@@ -684,17 +564,17 @@
     };
     let reasons =
         parse_distribution_point_reasons(py, dp.reasons.as_ref().map(|v| v.unwrap_read()))?;
     let crl_issuer = match dp.crl_issuer {
         Some(aci) => x509::parse_general_names(py, aci.unwrap_read())?,
         None => py.None(),
     };
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     Ok(x509_module
-        .getattr(crate::intern!(py, "DistributionPoint"))?
+        .getattr(pyo3::intern!(py, "DistributionPoint"))?
         .call1((full_name, relative_name, reasons, crl_issuer))?
         .to_object(py))
 }
 
 pub(crate) fn parse_distribution_points(
     py: pyo3::Python<'_>,
     data: &[u8],
@@ -709,16 +589,16 @@
 }
 
 pub(crate) fn parse_distribution_point_reasons(
     py: pyo3::Python<'_>,
     reasons: Option<&asn1::BitString<'_>>,
 ) -> Result<pyo3::PyObject, CryptographyError> {
     let reason_bit_mapping = py
-        .import("cryptography.x509.extensions")?
-        .getattr(crate::intern!(py, "_REASON_BIT_MAPPING"))?;
+        .import(pyo3::intern!(py, "cryptography.x509.extensions"))?
+        .getattr(pyo3::intern!(py, "_REASON_BIT_MAPPING"))?;
     Ok(match reasons {
         Some(bs) => {
             let mut vec = Vec::new();
             for i in 1..=8 {
                 if bs.has_bit_set(i) {
                     vec.push(reason_bit_mapping.get_item(i)?);
                 }
@@ -730,16 +610,16 @@
 }
 
 pub(crate) fn encode_distribution_point_reasons(
     py: pyo3::Python<'_>,
     py_reasons: &pyo3::PyAny,
 ) -> pyo3::PyResult<asn1::OwnedBitString> {
     let reason_flag_mapping = py
-        .import("cryptography.x509.extensions")?
-        .getattr(crate::intern!(py, "_CRLREASONFLAGS"))?;
+        .import(pyo3::intern!(py, "cryptography.x509.extensions"))?
+        .getattr(pyo3::intern!(py, "_CRLREASONFLAGS"))?;
 
     let mut bits = vec![0, 0];
     for py_reason in py_reasons.iter()? {
         let bit = reason_flag_mapping
             .get_item(py_reason?)?
             .extract::<usize>()?;
         set_bit(&mut bits, bit, true)
@@ -747,128 +627,113 @@
     if bits[1] == 0 {
         bits.truncate(1);
     }
     let unused_bits = bits.last().unwrap().trailing_zeros() as u8;
     Ok(asn1::OwnedBitString::new(bits, unused_bits).unwrap())
 }
 
-#[derive(asn1::Asn1Read, asn1::Asn1Write, pyo3::prelude::FromPyObject)]
-pub(crate) struct BasicConstraints {
-    #[default(false)]
-    pub ca: bool,
-    pub path_length: Option<u64>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct PolicyConstraints {
-    #[implicit(0)]
-    pub require_explicit_policy: Option<u64>,
-    #[implicit(1)]
-    pub inhibit_policy_mapping: Option<u64>,
-}
-
 pub(crate) fn parse_authority_key_identifier<'p>(
     py: pyo3::Python<'p>,
     ext_data: &[u8],
 ) -> Result<&'p pyo3::PyAny, CryptographyError> {
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     let aki = asn1::parse_single::<AuthorityKeyIdentifier<'_>>(ext_data)?;
     let serial = match aki.authority_cert_serial_number {
         Some(biguint) => big_byte_slice_to_py_int(py, biguint.as_bytes())?.to_object(py),
         None => py.None(),
     };
     let issuer = match aki.authority_cert_issuer {
         Some(aci) => x509::parse_general_names(py, aci.unwrap_read())?,
         None => py.None(),
     };
     Ok(x509_module
-        .getattr(crate::intern!(py, "AuthorityKeyIdentifier"))?
+        .getattr(pyo3::intern!(py, "AuthorityKeyIdentifier"))?
         .call1((aki.key_identifier, issuer, serial))?)
 }
 
 pub(crate) fn parse_access_descriptions(
     py: pyo3::Python<'_>,
     ext_data: &[u8],
 ) -> Result<pyo3::PyObject, CryptographyError> {
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     let ads = pyo3::types::PyList::empty(py);
-    let parsed = asn1::parse_single::<x509::common::SequenceOfAccessDescriptions<'_>>(ext_data)?;
+    let parsed = asn1::parse_single::<SequenceOfAccessDescriptions<'_>>(ext_data)?;
     for access in parsed.unwrap_read().clone() {
         let py_oid = oid_to_py_oid(py, &access.access_method)?.to_object(py);
         let gn = x509::parse_general_name(py, access.access_location)?;
         let ad = x509_module
-            .getattr(crate::intern!(py, "AccessDescription"))?
+            .getattr(pyo3::intern!(py, "AccessDescription"))?
             .call1((py_oid, gn))?
             .to_object(py);
         ads.append(ad)?;
     }
     Ok(ads.to_object(py))
 }
 
 pub fn parse_cert_ext<'p>(
     py: pyo3::Python<'p>,
     oid: asn1::ObjectIdentifier,
     ext_data: &[u8],
 ) -> CryptographyResult<Option<&'p pyo3::PyAny>> {
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     match oid {
         oid::SUBJECT_ALTERNATIVE_NAME_OID => {
             let gn_seq =
-                asn1::parse_single::<asn1::SequenceOf<'_, x509::GeneralName<'_>>>(ext_data)?;
+                asn1::parse_single::<asn1::SequenceOf<'_, name::GeneralName<'_>>>(ext_data)?;
             let sans = x509::parse_general_names(py, &gn_seq)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "SubjectAlternativeName"))?
+                    .getattr(pyo3::intern!(py, "SubjectAlternativeName"))?
                     .call1((sans,))?,
             ))
         }
         oid::ISSUER_ALTERNATIVE_NAME_OID => {
             let gn_seq =
-                asn1::parse_single::<asn1::SequenceOf<'_, x509::GeneralName<'_>>>(ext_data)?;
+                asn1::parse_single::<asn1::SequenceOf<'_, name::GeneralName<'_>>>(ext_data)?;
             let ians = x509::parse_general_names(py, &gn_seq)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "IssuerAlternativeName"))?
+                    .getattr(pyo3::intern!(py, "IssuerAlternativeName"))?
                     .call1((ians,))?,
             ))
         }
         oid::TLS_FEATURE_OID => {
             let tls_feature_type_to_enum = py
-                .import("cryptography.x509.extensions")?
-                .getattr(crate::intern!(py, "_TLS_FEATURE_TYPE_TO_ENUM"))?;
+                .import(pyo3::intern!(py, "cryptography.x509.extensions"))?
+                .getattr(pyo3::intern!(py, "_TLS_FEATURE_TYPE_TO_ENUM"))?;
 
             let features = pyo3::types::PyList::empty(py);
             for feature in asn1::parse_single::<asn1::SequenceOf<'_, u64>>(ext_data)? {
                 let py_feature = tls_feature_type_to_enum.get_item(feature.to_object(py))?;
                 features.append(py_feature)?;
             }
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "TLSFeature"))?
+                    .getattr(pyo3::intern!(py, "TLSFeature"))?
                     .call1((features,))?,
             ))
         }
         oid::SUBJECT_KEY_IDENTIFIER_OID => {
             let identifier = asn1::parse_single::<&[u8]>(ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "SubjectKeyIdentifier"))?
+                    .getattr(pyo3::intern!(py, "SubjectKeyIdentifier"))?
                     .call1((identifier,))?,
             ))
         }
         oid::EXTENDED_KEY_USAGE_OID => {
             let ekus = pyo3::types::PyList::empty(py);
             for oid in asn1::parse_single::<asn1::SequenceOf<'_, asn1::ObjectIdentifier>>(ext_data)?
             {
                 let oid_obj = oid_to_py_oid(py, &oid)?;
                 ekus.append(oid_obj)?;
             }
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "ExtendedKeyUsage"))?
+                    .getattr(pyo3::intern!(py, "ExtendedKeyUsage"))?
                     .call1((ekus,))?,
             ))
         }
         oid::KEY_USAGE_OID => {
             let kus = asn1::parse_single::<asn1::BitString<'_>>(ext_data)?;
             let digital_signature = kus.has_bit_set(0);
             let content_comitment = kus.has_bit_set(1);
@@ -876,100 +741,99 @@
             let data_encipherment = kus.has_bit_set(3);
             let key_agreement = kus.has_bit_set(4);
             let key_cert_sign = kus.has_bit_set(5);
             let crl_sign = kus.has_bit_set(6);
             let encipher_only = kus.has_bit_set(7);
             let decipher_only = kus.has_bit_set(8);
             Ok(Some(
-                x509_module
-                    .getattr(crate::intern!(py, "KeyUsage"))?
-                    .call1((
-                        digital_signature,
-                        content_comitment,
-                        key_encipherment,
-                        data_encipherment,
-                        key_agreement,
-                        key_cert_sign,
-                        crl_sign,
-                        encipher_only,
-                        decipher_only,
-                    ))?,
+                x509_module.getattr(pyo3::intern!(py, "KeyUsage"))?.call1((
+                    digital_signature,
+                    content_comitment,
+                    key_encipherment,
+                    data_encipherment,
+                    key_agreement,
+                    key_cert_sign,
+                    crl_sign,
+                    encipher_only,
+                    decipher_only,
+                ))?,
             ))
         }
         oid::AUTHORITY_INFORMATION_ACCESS_OID => {
             let ads = parse_access_descriptions(py, ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "AuthorityInformationAccess"))?
+                    .getattr(pyo3::intern!(py, "AuthorityInformationAccess"))?
                     .call1((ads,))?,
             ))
         }
         oid::SUBJECT_INFORMATION_ACCESS_OID => {
             let ads = parse_access_descriptions(py, ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "SubjectInformationAccess"))?
+                    .getattr(pyo3::intern!(py, "SubjectInformationAccess"))?
                     .call1((ads,))?,
             ))
         }
         oid::CERTIFICATE_POLICIES_OID => {
             let cp = parse_cp(py, ext_data)?;
-            Ok(Some(
-                x509_module.call_method1("CertificatePolicies", (cp,))?,
-            ))
+            Ok(Some(x509_module.call_method1(
+                pyo3::intern!(py, "CertificatePolicies"),
+                (cp,),
+            )?))
         }
         oid::POLICY_CONSTRAINTS_OID => {
             let pc = asn1::parse_single::<PolicyConstraints>(ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "PolicyConstraints"))?
+                    .getattr(pyo3::intern!(py, "PolicyConstraints"))?
                     .call1((pc.require_explicit_policy, pc.inhibit_policy_mapping))?,
             ))
         }
         oid::OCSP_NO_CHECK_OID => {
             asn1::parse_single::<()>(ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "OCSPNoCheck"))?
+                    .getattr(pyo3::intern!(py, "OCSPNoCheck"))?
                     .call0()?,
             ))
         }
         oid::INHIBIT_ANY_POLICY_OID => {
             let bignum = asn1::parse_single::<asn1::BigUint<'_>>(ext_data)?;
             let pynum = big_byte_slice_to_py_int(py, bignum.as_bytes())?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "InhibitAnyPolicy"))?
+                    .getattr(pyo3::intern!(py, "InhibitAnyPolicy"))?
                     .call1((pynum,))?,
             ))
         }
         oid::BASIC_CONSTRAINTS_OID => {
             let bc = asn1::parse_single::<BasicConstraints>(ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "BasicConstraints"))?
+                    .getattr(pyo3::intern!(py, "BasicConstraints"))?
                     .call1((bc.ca, bc.path_length))?,
             ))
         }
         oid::AUTHORITY_KEY_IDENTIFIER_OID => {
             Ok(Some(parse_authority_key_identifier(py, ext_data)?))
         }
         oid::CRL_DISTRIBUTION_POINTS_OID => {
             let dp = parse_distribution_points(py, ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "CRLDistributionPoints"))?
+                    .getattr(pyo3::intern!(py, "CRLDistributionPoints"))?
                     .call1((dp,))?,
             ))
         }
         oid::FRESHEST_CRL_OID => {
             let dp = parse_distribution_points(py, ext_data)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "FreshestCRL"))?
+                    .getattr(pyo3::intern!(py, "FreshestCRL"))?
                     .call1((dp,))?,
             ))
         }
         oid::NAME_CONSTRAINTS_OID => {
             let nc = asn1::parse_single::<NameConstraints<'_>>(ext_data)?;
             let permitted_subtrees = match nc.permitted_subtrees {
                 Some(data) => parse_general_subtrees(py, data)?,
@@ -977,115 +841,132 @@
             };
             let excluded_subtrees = match nc.excluded_subtrees {
                 Some(data) => parse_general_subtrees(py, data)?,
                 None => py.None(),
             };
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "NameConstraints"))?
+                    .getattr(pyo3::intern!(py, "NameConstraints"))?
                     .call1((permitted_subtrees, excluded_subtrees))?,
             ))
         }
+        oid::MS_CERTIFICATE_TEMPLATE => {
+            let ms_cert_tpl = asn1::parse_single::<MSCertificateTemplate>(ext_data)?;
+            let py_oid = oid_to_py_oid(py, &ms_cert_tpl.template_id)?;
+            Ok(Some(
+                x509_module
+                    .getattr(pyo3::intern!(py, "MSCertificateTemplate"))?
+                    .call1((py_oid, ms_cert_tpl.major_version, ms_cert_tpl.minor_version))?,
+            ))
+        }
         _ => Ok(None),
     }
 }
 
 pub(crate) fn time_from_py(
     py: pyo3::Python<'_>,
     val: &pyo3::PyAny,
-) -> CryptographyResult<x509::Time> {
-    let dt = x509::py_to_chrono(py, val)?;
-    time_from_chrono(dt)
+) -> CryptographyResult<common::Time> {
+    let dt = x509::py_to_datetime(py, val)?;
+    time_from_datetime(dt)
 }
 
-pub(crate) fn time_from_chrono(
-    dt: chrono::DateTime<chrono::Utc>,
-) -> CryptographyResult<x509::Time> {
+pub(crate) fn time_from_datetime(dt: asn1::DateTime) -> CryptographyResult<common::Time> {
     if dt.year() >= 2050 {
-        Ok(x509::Time::GeneralizedTime(asn1::GeneralizedTime::new(dt)?))
+        Ok(common::Time::GeneralizedTime(asn1::GeneralizedTime::new(
+            dt,
+        )?))
     } else {
-        Ok(x509::Time::UtcTime(asn1::UtcTime::new(dt).unwrap()))
+        Ok(common::Time::UtcTime(asn1::UtcTime::new(dt).unwrap()))
     }
 }
 
 #[pyo3::prelude::pyfunction]
 fn create_x509_certificate(
     py: pyo3::Python<'_>,
     builder: &pyo3::PyAny,
     private_key: &pyo3::PyAny,
     hash_algorithm: &pyo3::PyAny,
+    rsa_padding: &pyo3::PyAny,
 ) -> CryptographyResult<Certificate> {
-    let sigalg = x509::sign::compute_signature_algorithm(py, private_key, hash_algorithm)?;
-    let serialization_mod = py.import("cryptography.hazmat.primitives.serialization")?;
+    let sigalg =
+        x509::sign::compute_signature_algorithm(py, private_key, hash_algorithm, rsa_padding)?;
+    let serialization_mod = py.import(pyo3::intern!(
+        py,
+        "cryptography.hazmat.primitives.serialization"
+    ))?;
     let der_encoding = serialization_mod
-        .getattr(crate::intern!(py, "Encoding"))?
-        .getattr(crate::intern!(py, "DER"))?;
+        .getattr(pyo3::intern!(py, "Encoding"))?
+        .getattr(pyo3::intern!(py, "DER"))?;
     let spki_format = serialization_mod
-        .getattr(crate::intern!(py, "PublicFormat"))?
-        .getattr(crate::intern!(py, "SubjectPublicKeyInfo"))?;
+        .getattr(pyo3::intern!(py, "PublicFormat"))?
+        .getattr(pyo3::intern!(py, "SubjectPublicKeyInfo"))?;
 
     let spki_bytes = builder
-        .getattr(crate::intern!(py, "_public_key"))?
-        .call_method1("public_bytes", (der_encoding, spki_format))?
+        .getattr(pyo3::intern!(py, "_public_key"))?
+        .call_method1(
+            pyo3::intern!(py, "public_bytes"),
+            (der_encoding, spki_format),
+        )?
         .extract::<&[u8]>()?;
 
     let py_serial = builder
-        .getattr(crate::intern!(py, "_serial_number"))?
+        .getattr(pyo3::intern!(py, "_serial_number"))?
         .extract()?;
 
-    let py_issuer_name = builder.getattr(crate::intern!(py, "_issuer_name"))?;
-    let py_subject_name = builder.getattr(crate::intern!(py, "_subject_name"))?;
-    let py_not_before = builder.getattr(crate::intern!(py, "_not_valid_before"))?;
-    let py_not_after = builder.getattr(crate::intern!(py, "_not_valid_after"))?;
+    let py_issuer_name = builder.getattr(pyo3::intern!(py, "_issuer_name"))?;
+    let py_subject_name = builder.getattr(pyo3::intern!(py, "_subject_name"))?;
+    let py_not_before = builder.getattr(pyo3::intern!(py, "_not_valid_before"))?;
+    let py_not_after = builder.getattr(pyo3::intern!(py, "_not_valid_after"))?;
 
-    let tbs_cert = TbsCertificate {
+    let tbs_cert = cryptography_x509::certificate::TbsCertificate {
         version: builder
-            .getattr(crate::intern!(py, "_version"))?
-            .getattr(crate::intern!(py, "value"))?
+            .getattr(pyo3::intern!(py, "_version"))?
+            .getattr(pyo3::intern!(py, "value"))?
             .extract()?,
         serial: asn1::BigInt::new(py_uint_to_big_endian_bytes(py, py_serial)?).unwrap(),
         signature_alg: sigalg.clone(),
         issuer: x509::common::encode_name(py, py_issuer_name)?,
-        validity: Validity {
+        validity: cryptography_x509::certificate::Validity {
             not_before: time_from_py(py, py_not_before)?,
             not_after: time_from_py(py, py_not_after)?,
         },
         subject: x509::common::encode_name(py, py_subject_name)?,
         spki: asn1::parse_single(spki_bytes)?,
         issuer_unique_id: None,
         subject_unique_id: None,
-        extensions: x509::common::encode_extensions(
+        raw_extensions: x509::common::encode_extensions(
             py,
-            builder.getattr(crate::intern!(py, "_extensions"))?,
+            builder.getattr(pyo3::intern!(py, "_extensions"))?,
             extensions::encode_extension,
         )?,
     };
 
     let tbs_bytes = asn1::write_single(&tbs_cert)?;
-    let signature = x509::sign::sign_data(py, private_key, hash_algorithm, &tbs_bytes)?;
-    let data = asn1::write_single(&RawCertificate {
+    let signature =
+        x509::sign::sign_data(py, private_key, hash_algorithm, rsa_padding, &tbs_bytes)?;
+    let data = asn1::write_single(&cryptography_x509::certificate::Certificate {
         tbs_cert,
         signature_alg: sigalg,
         signature: asn1::BitString::new(signature, 0).unwrap(),
     })?;
-    // TODO: extra copy as we round-trip through a slice
-    load_der_x509_certificate(py, &data)
+    load_der_x509_certificate(py, pyo3::types::PyBytes::new(py, &data).into_py(py))
 }
 
 pub(crate) fn set_bit(vals: &mut [u8], n: usize, set: bool) {
     let idx = n / 8;
     let v = 1 << (7 - (n & 0x07));
     if set {
         vals[idx] |= v;
     }
 }
 
 pub(crate) fn add_to_module(module: &pyo3::prelude::PyModule) -> pyo3::PyResult<()> {
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_der_x509_certificate))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_pem_x509_certificate))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_pem_x509_certificates))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(create_x509_certificate))?;
+    module.add_function(pyo3::wrap_pyfunction!(load_der_x509_certificate, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(load_pem_x509_certificate, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(load_pem_x509_certificates, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(create_x509_certificate, module)?)?;
 
     module.add_class::<Certificate>()?;
 
     Ok(())
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/crl.rs` & `cryptography-41.0.0/src/rust/src/x509/crl.rs`

 * *Files 10% similar despite different names*

```diff
@@ -2,324 +2,333 @@
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::asn1::{
     big_byte_slice_to_py_int, encode_der_data, oid_to_py_oid, py_uint_to_big_endian_bytes,
 };
 use crate::error::{CryptographyError, CryptographyResult};
-use crate::x509;
-use crate::x509::{certificate, extensions, oid, sign};
-use pyo3::ToPyObject;
-use std::convert::TryInto;
+use crate::x509::{certificate, extensions, sign};
+use crate::{exceptions, x509};
+use cryptography_x509::{common, crl, name, oid};
+use pyo3::{IntoPy, ToPyObject};
 use std::sync::Arc;
 
 #[pyo3::prelude::pyfunction]
 fn load_der_x509_crl(
     py: pyo3::Python<'_>,
-    data: &[u8],
+    data: pyo3::Py<pyo3::types::PyBytes>,
 ) -> Result<CertificateRevocationList, CryptographyError> {
-    let raw = OwnedRawCertificateRevocationList::try_new(
-        Arc::from(data),
-        |data| asn1::parse_single(data),
-        |_| Ok(pyo3::once_cell::GILOnceCell::new()),
-    )?;
+    let owned = OwnedCertificateRevocationList::try_new(data, |data| {
+        asn1::parse_single(data.as_bytes(py))
+    })?;
 
-    let version = raw.borrow_value().tbs_cert_list.version.unwrap_or(1);
+    let version = owned.borrow_value().tbs_cert_list.version.unwrap_or(1);
     if version != 1 {
-        let x509_module = py.import("cryptography.x509")?;
-        return Err(CryptographyError::from(pyo3::PyErr::from_instance(
-            x509_module
-                .getattr(crate::intern!(py, "InvalidVersion"))?
-                .call1((format!("{} is not a valid CRL version", version), version))?,
-        )));
+        return Err(CryptographyError::from(
+            exceptions::InvalidVersion::new_err((
+                format!("{} is not a valid CRL version", version),
+                version,
+            )),
+        ));
     }
 
     Ok(CertificateRevocationList {
-        raw: Arc::new(raw),
+        owned: Arc::new(owned),
+        revoked_certs: pyo3::once_cell::GILOnceCell::new(),
         cached_extensions: None,
     })
 }
 
 #[pyo3::prelude::pyfunction]
 fn load_pem_x509_crl(
     py: pyo3::Python<'_>,
     data: &[u8],
 ) -> Result<CertificateRevocationList, CryptographyError> {
     let block = x509::find_in_pem(
         data,
         |p| p.tag == "X509 CRL",
         "Valid PEM but no BEGIN X509 CRL/END X509 delimiters. Are you sure this is a CRL?",
     )?;
-    // TODO: Produces an extra copy
-    load_der_x509_crl(py, &block.contents)
+    load_der_x509_crl(
+        py,
+        pyo3::types::PyBytes::new(py, &block.contents).into_py(py),
+    )
 }
 
 #[ouroboros::self_referencing]
-struct OwnedRawCertificateRevocationList {
-    data: Arc<[u8]>,
+struct OwnedCertificateRevocationList {
+    data: pyo3::Py<pyo3::types::PyBytes>,
     #[borrows(data)]
     #[covariant]
-    value: RawCertificateRevocationList<'this>,
-    #[borrows(data)]
-    #[not_covariant]
-    revoked_certs: pyo3::once_cell::GILOnceCell<Vec<RawRevokedCertificate<'this>>>,
+    value: crl::CertificateRevocationList<'this>,
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.x509")]
 struct CertificateRevocationList {
-    raw: Arc<OwnedRawCertificateRevocationList>,
+    owned: Arc<OwnedCertificateRevocationList>,
 
+    revoked_certs: pyo3::once_cell::GILOnceCell<Vec<OwnedRevokedCertificate>>,
     cached_extensions: Option<pyo3::PyObject>,
 }
 
 impl CertificateRevocationList {
     fn public_bytes_der(&self) -> CryptographyResult<Vec<u8>> {
-        Ok(asn1::write_single(self.raw.borrow_value())?)
+        Ok(asn1::write_single(self.owned.borrow_value())?)
     }
 
-    fn revoked_cert(&self, py: pyo3::Python<'_>, idx: usize) -> pyo3::PyResult<RevokedCertificate> {
-        let raw = try_map_arc_data_crl(&self.raw, |_crl, revoked_certs| {
-            let revoked_certs = revoked_certs.get(py).unwrap();
-            Ok::<_, pyo3::PyErr>(revoked_certs[idx].clone())
-        })?;
-        Ok(RevokedCertificate {
-            raw,
+    fn revoked_cert(&self, py: pyo3::Python<'_>, idx: usize) -> RevokedCertificate {
+        RevokedCertificate {
+            owned: self.revoked_certs.get(py).unwrap()[idx].clone(),
             cached_extensions: None,
-        })
+        }
     }
 
     fn len(&self) -> usize {
-        self.raw
+        self.owned
             .borrow_value()
             .tbs_cert_list
             .revoked_certificates
             .as_ref()
             .map_or(0, |v| v.unwrap_read().len())
     }
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyObjectProtocol for CertificateRevocationList {
+#[pyo3::prelude::pymethods]
+impl CertificateRevocationList {
     fn __richcmp__(
         &self,
-        other: pyo3::PyRef<CertificateRevocationList>,
+        other: pyo3::PyRef<'_, CertificateRevocationList>,
         op: pyo3::basic::CompareOp,
     ) -> pyo3::PyResult<bool> {
         match op {
-            pyo3::basic::CompareOp::Eq => Ok(self.raw.borrow_value() == other.raw.borrow_value()),
-            pyo3::basic::CompareOp::Ne => Ok(self.raw.borrow_value() != other.raw.borrow_value()),
+            pyo3::basic::CompareOp::Eq => {
+                Ok(self.owned.borrow_value() == other.owned.borrow_value())
+            }
+            pyo3::basic::CompareOp::Ne => {
+                Ok(self.owned.borrow_value() != other.owned.borrow_value())
+            }
             _ => Err(pyo3::exceptions::PyTypeError::new_err(
                 "CRLs cannot be ordered",
             )),
         }
     }
-}
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyMappingProtocol for CertificateRevocationList {
     fn __len__(&self) -> usize {
         self.len()
     }
 
-    fn __getitem__(&self, idx: &pyo3::PyAny) -> pyo3::PyResult<pyo3::PyObject> {
-        let gil = pyo3::Python::acquire_gil();
-        let py = gil.python();
-
-        self.raw.with(|val| {
-            val.revoked_certs.get_or_init(py, || {
-                match &val.value.tbs_cert_list.revoked_certificates {
-                    Some(c) => c.unwrap_read().clone().collect(),
-                    None => vec![],
-                }
-            });
+    fn __iter__(&self) -> CRLIterator {
+        CRLIterator {
+            contents: OwnedCRLIteratorData::try_new(Arc::clone(&self.owned), |v| {
+                Ok::<_, ()>(
+                    v.borrow_value()
+                        .tbs_cert_list
+                        .revoked_certificates
+                        .as_ref()
+                        .map(|v| v.unwrap_read().clone()),
+                )
+            })
+            .unwrap(),
+        }
+    }
+
+    fn __getitem__(
+        &self,
+        py: pyo3::Python<'_>,
+        idx: &pyo3::PyAny,
+    ) -> pyo3::PyResult<pyo3::PyObject> {
+        self.revoked_certs.get_or_init(py, || {
+            let mut revoked_certs = vec![];
+            let mut it = self.__iter__();
+            while let Some(c) = it.__next__() {
+                revoked_certs.push(c.owned);
+            }
+            revoked_certs
         });
 
-        if idx.is_instance::<pyo3::types::PySlice>()? {
+        if idx.is_instance_of::<pyo3::types::PySlice>()? {
             let indices = idx
                 .downcast::<pyo3::types::PySlice>()?
                 .indices(self.len().try_into().unwrap())?;
             let result = pyo3::types::PyList::empty(py);
             for i in (indices.start..indices.stop).step_by(indices.step.try_into().unwrap()) {
-                let revoked_cert = pyo3::PyCell::new(py, self.revoked_cert(py, i as usize)?)?;
+                let revoked_cert = pyo3::PyCell::new(py, self.revoked_cert(py, i as usize))?;
                 result.append(revoked_cert)?;
             }
             Ok(result.to_object(py))
         } else {
             let mut idx = idx.extract::<isize>()?;
             if idx < 0 {
                 idx += self.len() as isize;
             }
             if idx >= (self.len() as isize) || idx < 0 {
                 return Err(pyo3::exceptions::PyIndexError::new_err(()));
             }
-            Ok(pyo3::PyCell::new(py, self.revoked_cert(py, idx as usize)?)?.to_object(py))
+            Ok(pyo3::PyCell::new(py, self.revoked_cert(py, idx as usize))?.to_object(py))
         }
     }
-}
 
-#[pyo3::prelude::pymethods]
-impl CertificateRevocationList {
     fn fingerprint<'p>(
         &self,
         py: pyo3::Python<'p>,
         algorithm: pyo3::PyObject,
     ) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        let hashes_mod = py.import("cryptography.hazmat.primitives.hashes")?;
+        let hashes_mod = py.import(pyo3::intern!(py, "cryptography.hazmat.primitives.hashes"))?;
         let h = hashes_mod
-            .getattr(crate::intern!(py, "Hash"))?
+            .getattr(pyo3::intern!(py, "Hash"))?
             .call1((algorithm,))?;
-        h.call_method1("update", (self.public_bytes_der()?.as_slice(),))?;
-        h.call_method0("finalize")
+
+        let data = self.public_bytes_der()?;
+        h.call_method1(pyo3::intern!(py, "update"), (data.as_slice(),))?;
+        h.call_method0(pyo3::intern!(py, "finalize"))
     }
 
     #[getter]
     fn signature_algorithm_oid<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        oid_to_py_oid(py, &self.raw.borrow_value().signature_algorithm.oid)
+        oid_to_py_oid(py, self.owned.borrow_value().signature_algorithm.oid())
     }
 
     #[getter]
     fn signature_hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let oid = self.signature_algorithm_oid(py)?;
-        let oid_module = py.import("cryptography.hazmat._oid")?;
-        let exceptions_module = py.import("cryptography.exceptions")?;
+        let oid_module = py.import(pyo3::intern!(py, "cryptography.hazmat._oid"))?;
         match oid_module
-            .getattr(crate::intern!(py, "_SIG_OIDS_TO_HASH"))?
+            .getattr(pyo3::intern!(py, "_SIG_OIDS_TO_HASH"))?
             .get_item(oid)
         {
             Ok(v) => Ok(v),
-            Err(_) => Err(pyo3::PyErr::from_instance(exceptions_module.call_method1(
-                "UnsupportedAlgorithm",
-                (format!(
-                    "Signature algorithm OID:{} not recognized",
-                    self.raw.borrow_value().signature_algorithm.oid
-                ),),
-            )?)),
+            Err(_) => Err(exceptions::UnsupportedAlgorithm::new_err(format!(
+                "Signature algorithm OID: {} not recognized",
+                self.owned.borrow_value().signature_algorithm.oid(),
+            ))),
         }
     }
 
     #[getter]
     fn signature(&self) -> &[u8] {
-        self.raw.borrow_value().signature_value.as_bytes()
+        self.owned.borrow_value().signature_value.as_bytes()
     }
 
     #[getter]
     fn tbs_certlist_bytes<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
-        let b = asn1::write_single(&self.raw.borrow_value().tbs_cert_list)?;
+        let b = asn1::write_single(&self.owned.borrow_value().tbs_cert_list)?;
         Ok(pyo3::types::PyBytes::new(py, &b))
     }
 
     fn public_bytes<'p>(
         &self,
         py: pyo3::Python<'p>,
         encoding: &'p pyo3::PyAny,
     ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
-        let result = asn1::write_single(self.raw.borrow_value())?;
+        let result = asn1::write_single(self.owned.borrow_value())?;
 
         encode_der_data(py, "X509 CRL".to_string(), result, encoding)
     }
 
     #[getter]
     fn issuer<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         Ok(x509::parse_name(
             py,
-            &self.raw.borrow_value().tbs_cert_list.issuer,
+            &self.owned.borrow_value().tbs_cert_list.issuer,
         )?)
     }
 
     #[getter]
     fn next_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        match &self.raw.borrow_value().tbs_cert_list.next_update {
-            Some(t) => x509::chrono_to_py(py, t.as_chrono()),
+        match &self.owned.borrow_value().tbs_cert_list.next_update {
+            Some(t) => x509::datetime_to_py(py, t.as_datetime()),
             None => Ok(py.None().into_ref(py)),
         }
     }
 
     #[getter]
     fn last_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        x509::chrono_to_py(
+        x509::datetime_to_py(
             py,
-            self.raw
+            self.owned
                 .borrow_value()
                 .tbs_cert_list
                 .this_update
-                .as_chrono(),
+                .as_datetime(),
         )
     }
 
     #[getter]
     fn extensions(&mut self, py: pyo3::Python<'_>) -> pyo3::PyResult<pyo3::PyObject> {
-        let x509_module = py.import("cryptography.x509")?;
+        let tbs_cert_list = &self.owned.borrow_value().tbs_cert_list;
+
+        let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
         x509::parse_and_cache_extensions(
             py,
             &mut self.cached_extensions,
-            &self.raw.borrow_value().tbs_cert_list.crl_extensions,
+            &tbs_cert_list.raw_crl_extensions,
             |oid, ext_data| match *oid {
                 oid::CRL_NUMBER_OID => {
                     let bignum = asn1::parse_single::<asn1::BigUint<'_>>(ext_data)?;
                     let pynum = big_byte_slice_to_py_int(py, bignum.as_bytes())?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "CRLNumber"))?
+                            .getattr(pyo3::intern!(py, "CRLNumber"))?
                             .call1((pynum,))?,
                     ))
                 }
                 oid::DELTA_CRL_INDICATOR_OID => {
                     let bignum = asn1::parse_single::<asn1::BigUint<'_>>(ext_data)?;
                     let pynum = big_byte_slice_to_py_int(py, bignum.as_bytes())?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "DeltaCRLIndicator"))?
+                            .getattr(pyo3::intern!(py, "DeltaCRLIndicator"))?
                             .call1((pynum,))?,
                     ))
                 }
                 oid::ISSUER_ALTERNATIVE_NAME_OID => {
-                    let gn_seq = asn1::parse_single::<asn1::SequenceOf<'_, x509::GeneralName<'_>>>(
+                    let gn_seq = asn1::parse_single::<asn1::SequenceOf<'_, name::GeneralName<'_>>>(
                         ext_data,
                     )?;
                     let ians = x509::parse_general_names(py, &gn_seq)?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "IssuerAlternativeName"))?
+                            .getattr(pyo3::intern!(py, "IssuerAlternativeName"))?
                             .call1((ians,))?,
                     ))
                 }
                 oid::AUTHORITY_INFORMATION_ACCESS_OID => {
                     let ads = certificate::parse_access_descriptions(py, ext_data)?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "AuthorityInformationAccess"))?
+                            .getattr(pyo3::intern!(py, "AuthorityInformationAccess"))?
                             .call1((ads,))?,
                     ))
                 }
                 oid::AUTHORITY_KEY_IDENTIFIER_OID => Ok(Some(
                     certificate::parse_authority_key_identifier(py, ext_data)?,
                 )),
                 oid::ISSUING_DISTRIBUTION_POINT_OID => {
-                    let idp = asn1::parse_single::<IssuingDistributionPoint<'_>>(ext_data)?;
+                    let idp = asn1::parse_single::<crl::IssuingDistributionPoint<'_>>(ext_data)?;
                     let (full_name, relative_name) = match idp.distribution_point {
                         Some(data) => certificate::parse_distribution_point_name(py, data)?,
                         None => (py.None(), py.None()),
                     };
                     let py_reasons = if let Some(reasons) = idp.only_some_reasons {
                         certificate::parse_distribution_point_reasons(
                             py,
                             Some(reasons.unwrap_read()),
                         )?
                     } else {
                         py.None()
                     };
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "IssuingDistributionPoint"))?
+                            .getattr(pyo3::intern!(py, "IssuingDistributionPoint"))?
                             .call1((
                                 full_name,
                                 relative_name,
                                 idp.only_contains_user_certs,
                                 idp.only_contains_ca_certs,
                                 py_reasons,
                                 idp.indirect_crl,
@@ -327,30 +336,30 @@
                             ))?,
                     ))
                 }
                 oid::FRESHEST_CRL_OID => {
                     let dp = certificate::parse_distribution_points(py, ext_data)?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "FreshestCRL"))?
+                            .getattr(pyo3::intern!(py, "FreshestCRL"))?
                             .call1((dp,))?,
                     ))
                 }
                 _ => Ok(None),
             },
         )
     }
 
     fn get_revoked_certificate_by_serial_number(
         &mut self,
         py: pyo3::Python<'_>,
         serial: &pyo3::types::PyLong,
     ) -> pyo3::PyResult<Option<RevokedCertificate>> {
         let serial_bytes = py_uint_to_big_endian_bytes(py, serial)?;
-        let owned = OwnedRawRevokedCertificate::try_new(Arc::clone(&self.raw), |v| {
+        let owned = OwnedRevokedCertificate::try_new(Arc::clone(&self.owned), |v| {
             let certs = match &v.borrow_value().tbs_cert_list.revoked_certificates {
                 Some(certs) => certs.unwrap_read().clone(),
                 None => return Err(()),
             };
 
             // TODO: linear scan. Make a hash or bisect!
             for cert in certs {
@@ -358,242 +367,154 @@
                     return Ok(cert);
                 }
             }
             Err(())
         });
         match owned {
             Ok(o) => Ok(Some(RevokedCertificate {
-                raw: o,
+                owned: o,
                 cached_extensions: None,
             })),
             Err(()) => Ok(None),
         }
     }
 
     fn is_signature_valid<'p>(
         slf: pyo3::PyRef<'_, Self>,
         py: pyo3::Python<'p>,
         public_key: &'p pyo3::PyAny,
     ) -> CryptographyResult<bool> {
-        if slf.raw.borrow_value().tbs_cert_list.signature
-            != slf.raw.borrow_value().signature_algorithm
+        if slf.owned.borrow_value().tbs_cert_list.signature
+            != slf.owned.borrow_value().signature_algorithm
         {
             return Ok(false);
         };
 
         // Error on invalid public key -- below we treat any error as just
         // being an invalid signature.
         sign::identify_public_key_type(py, public_key)?;
 
-        Ok(sign::verify_signature_with_oid(
+        Ok(sign::verify_signature_with_signature_algorithm(
             py,
             public_key,
-            &slf.raw.borrow_value().signature_algorithm.oid,
-            slf.raw.borrow_value().signature_value.as_bytes(),
-            &asn1::write_single(&slf.raw.borrow_value().tbs_cert_list)?,
+            &slf.owned.borrow_value().signature_algorithm,
+            slf.owned.borrow_value().signature_value.as_bytes(),
+            &asn1::write_single(&slf.owned.borrow_value().tbs_cert_list)?,
         )
         .is_ok())
     }
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyIterProtocol<'_> for CertificateRevocationList {
-    fn __iter__(slf: pyo3::PyRef<'p, Self>) -> CRLIterator {
-        CRLIterator {
-            contents: OwnedCRLIteratorData::try_new(Arc::clone(&slf.raw), |v| {
-                Ok::<_, ()>(
-                    v.borrow_value()
-                        .tbs_cert_list
-                        .revoked_certificates
-                        .as_ref()
-                        .map(|v| v.unwrap_read().clone()),
-                )
-            })
-            .unwrap(),
-        }
-    }
-}
-
 #[ouroboros::self_referencing]
 struct OwnedCRLIteratorData {
-    data: Arc<OwnedRawCertificateRevocationList>,
+    data: Arc<OwnedCertificateRevocationList>,
     #[borrows(data)]
     #[covariant]
-    value: Option<asn1::SequenceOf<'this, RawRevokedCertificate<'this>>>,
+    value: Option<asn1::SequenceOf<'this, crl::RevokedCertificate<'this>>>,
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.x509")]
 struct CRLIterator {
     contents: OwnedCRLIteratorData,
 }
 
 // Open-coded implementation of the API discussed in
 // https://github.com/joshua-maros/ouroboros/issues/38
-fn try_map_arc_data_crl<E>(
-    crl: &Arc<OwnedRawCertificateRevocationList>,
-    f: impl for<'this> FnOnce(
-        &'this OwnedRawCertificateRevocationList,
-        &pyo3::once_cell::GILOnceCell<Vec<RawRevokedCertificate<'this>>>,
-    ) -> Result<RawRevokedCertificate<'this>, E>,
-) -> Result<OwnedRawRevokedCertificate, E> {
-    OwnedRawRevokedCertificate::try_new(Arc::clone(crl), |inner_crl| {
-        crl.with(|value| {
-            f(inner_crl, unsafe {
-                std::mem::transmute(value.revoked_certs)
-            })
-        })
-    })
-}
 fn try_map_arc_data_mut_crl_iterator<E>(
     it: &mut OwnedCRLIteratorData,
     f: impl for<'this> FnOnce(
-        &'this OwnedRawCertificateRevocationList,
-        &mut Option<asn1::SequenceOf<'this, RawRevokedCertificate<'this>>>,
-    ) -> Result<RawRevokedCertificate<'this>, E>,
-) -> Result<OwnedRawRevokedCertificate, E> {
-    OwnedRawRevokedCertificate::try_new(Arc::clone(it.borrow_data()), |inner_it| {
+        &'this OwnedCertificateRevocationList,
+        &mut Option<asn1::SequenceOf<'this, crl::RevokedCertificate<'this>>>,
+    ) -> Result<crl::RevokedCertificate<'this>, E>,
+) -> Result<OwnedRevokedCertificate, E> {
+    OwnedRevokedCertificate::try_new(Arc::clone(it.borrow_data()), |inner_it| {
         it.with_value_mut(|value| f(inner_it, unsafe { std::mem::transmute(value) }))
     })
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyIterProtocol<'_> for CRLIterator {
-    fn __iter__(slf: pyo3::PyRef<'p, Self>) -> pyo3::PyRef<'p, Self> {
+#[pyo3::prelude::pymethods]
+impl CRLIterator {
+    fn __len__(&self) -> usize {
+        self.contents.borrow_value().clone().map_or(0, |v| v.len())
+    }
+
+    fn __iter__(slf: pyo3::PyRef<'_, Self>) -> pyo3::PyRef<'_, Self> {
         slf
     }
 
-    fn __next__(mut slf: pyo3::PyRefMut<'p, Self>) -> Option<RevokedCertificate> {
-        let revoked = try_map_arc_data_mut_crl_iterator(&mut slf.contents, |_data, v| match v {
+    fn __next__(&mut self) -> Option<RevokedCertificate> {
+        let revoked = try_map_arc_data_mut_crl_iterator(&mut self.contents, |_data, v| match v {
             Some(v) => match v.next() {
                 Some(revoked) => Ok(revoked),
                 None => Err(()),
             },
             None => Err(()),
         })
         .ok()?;
         Some(RevokedCertificate {
-            raw: revoked,
+            owned: revoked,
             cached_extensions: None,
         })
     }
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PySequenceProtocol<'_> for CRLIterator {
-    fn __len__(&self) -> usize {
-        self.contents.borrow_value().clone().map_or(0, |v| v.len())
-    }
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write, PartialEq, Hash)]
-struct RawCertificateRevocationList<'a> {
-    tbs_cert_list: TBSCertList<'a>,
-    signature_algorithm: x509::AlgorithmIdentifier<'a>,
-    signature_value: asn1::BitString<'a>,
-}
-
-type RevokedCertificates<'a> = Option<
-    x509::Asn1ReadableOrWritable<
-        'a,
-        asn1::SequenceOf<'a, RawRevokedCertificate<'a>>,
-        asn1::SequenceOfWriter<'a, RawRevokedCertificate<'a>, Vec<RawRevokedCertificate<'a>>>,
-    >,
->;
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write, PartialEq, Hash)]
-struct TBSCertList<'a> {
-    version: Option<u8>,
-    signature: x509::AlgorithmIdentifier<'a>,
-    issuer: x509::Name<'a>,
-    this_update: x509::Time,
-    next_update: Option<x509::Time>,
-    revoked_certificates: RevokedCertificates<'a>,
-    #[explicit(0)]
-    crl_extensions: Option<x509::Extensions<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write, PartialEq, Hash, Clone)]
-struct RawRevokedCertificate<'a> {
-    user_certificate: asn1::BigUint<'a>,
-    revocation_date: x509::Time,
-    crl_entry_extensions: Option<x509::Extensions<'a>>,
-}
-
 #[ouroboros::self_referencing]
-struct OwnedRawRevokedCertificate {
-    data: Arc<OwnedRawCertificateRevocationList>,
+struct OwnedRevokedCertificate {
+    data: Arc<OwnedCertificateRevocationList>,
     #[borrows(data)]
     #[covariant]
-    value: RawRevokedCertificate<'this>,
+    value: crl::RevokedCertificate<'this>,
+}
+
+impl Clone for OwnedRevokedCertificate {
+    fn clone(&self) -> OwnedRevokedCertificate {
+        // This is safe because `Arc::clone` ensures the data is alive, but
+        // Rust doesn't understand the lifetime relationship it produces.
+        // Open-coded implementation of the API discussed in
+        // https://github.com/joshua-maros/ouroboros/issues/38
+        OwnedRevokedCertificate::new(Arc::clone(self.borrow_data()), |_| unsafe {
+            std::mem::transmute(self.borrow_value().clone())
+        })
+    }
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.x509")]
 struct RevokedCertificate {
-    raw: OwnedRawRevokedCertificate,
+    owned: OwnedRevokedCertificate,
     cached_extensions: Option<pyo3::PyObject>,
 }
 
 #[pyo3::prelude::pymethods]
 impl RevokedCertificate {
     #[getter]
     fn serial_number<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        big_byte_slice_to_py_int(py, self.raw.borrow_value().user_certificate.as_bytes())
+        big_byte_slice_to_py_int(py, self.owned.borrow_value().user_certificate.as_bytes())
     }
 
     #[getter]
     fn revocation_date<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        x509::chrono_to_py(py, self.raw.borrow_value().revocation_date.as_chrono())
+        x509::datetime_to_py(py, self.owned.borrow_value().revocation_date.as_datetime())
     }
 
     #[getter]
     fn extensions(&mut self, py: pyo3::Python<'_>) -> pyo3::PyResult<pyo3::PyObject> {
         x509::parse_and_cache_extensions(
             py,
             &mut self.cached_extensions,
-            &self.raw.borrow_value().crl_entry_extensions,
+            &self.owned.borrow_value().raw_crl_entry_extensions,
             |oid, ext_data| parse_crl_entry_ext(py, oid.clone(), ext_data),
         )
     }
 }
 
-pub(crate) type ReasonFlags<'a> =
-    Option<x509::Asn1ReadableOrWritable<'a, asn1::BitString<'a>, asn1::OwnedBitString>>;
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct IssuingDistributionPoint<'a> {
-    #[explicit(0)]
-    pub distribution_point: Option<certificate::DistributionPointName<'a>>,
-
-    #[implicit(1)]
-    #[default(false)]
-    pub only_contains_user_certs: bool,
-
-    #[implicit(2)]
-    #[default(false)]
-    pub only_contains_ca_certs: bool,
-
-    #[implicit(3)]
-    pub only_some_reasons: ReasonFlags<'a>,
-
-    #[implicit(4)]
-    #[default(false)]
-    pub indirect_crl: bool,
-
-    #[implicit(5)]
-    #[default(false)]
-    pub only_contains_attribute_certs: bool,
-}
-
-pub(crate) type CRLReason = asn1::Enumerated;
-
 pub(crate) fn parse_crl_reason_flags<'p>(
     py: pyo3::Python<'p>,
-    reason: &CRLReason,
+    reason: &crl::CRLReason,
 ) -> CryptographyResult<&'p pyo3::PyAny> {
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     let flag_name = match reason.value() {
         0 => "unspecified",
         1 => "key_compromise",
         2 => "ca_compromise",
         3 => "affiliation_changed",
         4 => "superseded",
         5 => "cessation_of_operation",
@@ -607,123 +528,132 @@
                     "Unsupported reason code: {}",
                     value
                 )),
             ))
         }
     };
     Ok(x509_module
-        .getattr(crate::intern!(py, "ReasonFlags"))?
+        .getattr(pyo3::intern!(py, "ReasonFlags"))?
         .getattr(flag_name)?)
 }
 
 pub fn parse_crl_entry_ext<'p>(
     py: pyo3::Python<'p>,
     oid: asn1::ObjectIdentifier,
     data: &[u8],
 ) -> CryptographyResult<Option<&'p pyo3::PyAny>> {
-    let x509_module = py.import("cryptography.x509")?;
+    let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
     match oid {
         oid::CRL_REASON_OID => {
-            let flags = parse_crl_reason_flags(py, &asn1::parse_single::<CRLReason>(data)?)?;
+            let flags = parse_crl_reason_flags(py, &asn1::parse_single::<crl::CRLReason>(data)?)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "CRLReason"))?
+                    .getattr(pyo3::intern!(py, "CRLReason"))?
                     .call1((flags,))?,
             ))
         }
         oid::CERTIFICATE_ISSUER_OID => {
-            let gn_seq = asn1::parse_single::<asn1::SequenceOf<'_, x509::GeneralName<'_>>>(data)?;
+            let gn_seq = asn1::parse_single::<asn1::SequenceOf<'_, name::GeneralName<'_>>>(data)?;
             let gns = x509::parse_general_names(py, &gn_seq)?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "CertificateIssuer"))?
+                    .getattr(pyo3::intern!(py, "CertificateIssuer"))?
                     .call1((gns,))?,
             ))
         }
         oid::INVALIDITY_DATE_OID => {
             let time = asn1::parse_single::<asn1::GeneralizedTime>(data)?;
-            let py_dt = x509::chrono_to_py(py, time.as_chrono())?;
+            let py_dt = x509::datetime_to_py(py, time.as_datetime())?;
             Ok(Some(
                 x509_module
-                    .getattr(crate::intern!(py, "InvalidityDate"))?
+                    .getattr(pyo3::intern!(py, "InvalidityDate"))?
                     .call1((py_dt,))?,
             ))
         }
         _ => Ok(None),
     }
 }
 
 #[pyo3::prelude::pyfunction]
 fn create_x509_crl(
     py: pyo3::Python<'_>,
     builder: &pyo3::PyAny,
     private_key: &pyo3::PyAny,
     hash_algorithm: &pyo3::PyAny,
 ) -> CryptographyResult<CertificateRevocationList> {
-    let sigalg = x509::sign::compute_signature_algorithm(py, private_key, hash_algorithm)?;
-
+    let sigalg = x509::sign::compute_signature_algorithm(
+        py,
+        private_key,
+        hash_algorithm,
+        py.None().into_ref(py),
+    )?;
     let mut revoked_certs = vec![];
     for py_revoked_cert in builder
-        .getattr(crate::intern!(py, "_revoked_certificates"))?
+        .getattr(pyo3::intern!(py, "_revoked_certificates"))?
         .iter()?
     {
         let py_revoked_cert = py_revoked_cert?;
         let serial_number = py_revoked_cert
-            .getattr(crate::intern!(py, "serial_number"))?
+            .getattr(pyo3::intern!(py, "serial_number"))?
             .extract()?;
-        let py_revocation_date = py_revoked_cert.getattr(crate::intern!(py, "revocation_date"))?;
-        revoked_certs.push(RawRevokedCertificate {
+        let py_revocation_date = py_revoked_cert.getattr(pyo3::intern!(py, "revocation_date"))?;
+        revoked_certs.push(crl::RevokedCertificate {
             user_certificate: asn1::BigUint::new(py_uint_to_big_endian_bytes(py, serial_number)?)
                 .unwrap(),
             revocation_date: x509::certificate::time_from_py(py, py_revocation_date)?,
-            crl_entry_extensions: x509::common::encode_extensions(
+            raw_crl_entry_extensions: x509::common::encode_extensions(
                 py,
-                py_revoked_cert.getattr(crate::intern!(py, "extensions"))?,
+                py_revoked_cert.getattr(pyo3::intern!(py, "extensions"))?,
                 extensions::encode_extension,
             )?,
         });
     }
 
-    let py_issuer_name = builder.getattr(crate::intern!(py, "_issuer_name"))?;
-    let py_this_update = builder.getattr(crate::intern!(py, "_last_update"))?;
-    let py_next_update = builder.getattr(crate::intern!(py, "_next_update"))?;
-    let tbs_cert_list = TBSCertList {
+    let py_issuer_name = builder.getattr(pyo3::intern!(py, "_issuer_name"))?;
+    let py_this_update = builder.getattr(pyo3::intern!(py, "_last_update"))?;
+    let py_next_update = builder.getattr(pyo3::intern!(py, "_next_update"))?;
+    let tbs_cert_list = crl::TBSCertList {
         version: Some(1),
         signature: sigalg.clone(),
         issuer: x509::common::encode_name(py, py_issuer_name)?,
         this_update: x509::certificate::time_from_py(py, py_this_update)?,
         next_update: Some(x509::certificate::time_from_py(py, py_next_update)?),
         revoked_certificates: if revoked_certs.is_empty() {
             None
         } else {
-            Some(x509::Asn1ReadableOrWritable::new_write(
+            Some(common::Asn1ReadableOrWritable::new_write(
                 asn1::SequenceOfWriter::new(revoked_certs),
             ))
         },
-        crl_extensions: x509::common::encode_extensions(
+        raw_crl_extensions: x509::common::encode_extensions(
             py,
-            builder.getattr(crate::intern!(py, "_extensions"))?,
+            builder.getattr(pyo3::intern!(py, "_extensions"))?,
             extensions::encode_extension,
         )?,
     };
 
     let tbs_bytes = asn1::write_single(&tbs_cert_list)?;
-    let signature = x509::sign::sign_data(py, private_key, hash_algorithm, &tbs_bytes)?;
-    let data = asn1::write_single(&RawCertificateRevocationList {
+    let signature = x509::sign::sign_data(
+        py,
+        private_key,
+        hash_algorithm,
+        py.None().into_ref(py),
+        &tbs_bytes,
+    )?;
+    let data = asn1::write_single(&crl::CertificateRevocationList {
         tbs_cert_list,
         signature_algorithm: sigalg,
         signature_value: asn1::BitString::new(signature, 0).unwrap(),
     })?;
-    // TODO: extra copy as we round-trip through a slice
-    load_der_x509_crl(py, &data)
+    load_der_x509_crl(py, pyo3::types::PyBytes::new(py, &data).into_py(py))
 }
 
 pub(crate) fn add_to_module(module: &pyo3::prelude::PyModule) -> pyo3::PyResult<()> {
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_der_x509_crl))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_pem_x509_crl))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(create_x509_crl))?;
+    module.add_function(pyo3::wrap_pyfunction!(load_der_x509_crl, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(load_pem_x509_crl, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(create_x509_crl, module)?)?;
 
     module.add_class::<CertificateRevocationList>()?;
     module.add_class::<RevokedCertificate>()?;
 
     Ok(())
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/csr.rs` & `cryptography-41.0.0/src/rust/src/x509/csr.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,127 +1,75 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::asn1::{encode_der_data, oid_to_py_oid, py_oid_to_oid};
 use crate::error::{CryptographyError, CryptographyResult};
-use crate::x509;
-use crate::x509::{certificate, oid, sign};
+use crate::x509::{certificate, sign};
+use crate::{exceptions, x509};
 use asn1::SimpleAsn1Readable;
+use cryptography_x509::csr::{check_attribute_length, Attribute, CertificationRequestInfo, Csr};
+use cryptography_x509::{common, oid};
+use pyo3::IntoPy;
 use std::collections::hash_map::DefaultHasher;
 use std::hash::{Hash, Hasher};
 
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct RawCsr<'a> {
-    csr_info: CertificationRequestInfo<'a>,
-    signature_alg: x509::AlgorithmIdentifier<'a>,
-    signature: asn1::BitString<'a>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct CertificationRequestInfo<'a> {
-    version: u8,
-    subject: x509::Name<'a>,
-    spki: certificate::SubjectPublicKeyInfo<'a>,
-    #[implicit(0, required)]
-    attributes: Attributes<'a>,
-}
-
-pub(crate) type Attributes<'a> = x509::Asn1ReadableOrWritable<
-    'a,
-    asn1::SetOf<'a, Attribute<'a>>,
-    asn1::SetOfWriter<'a, Attribute<'a>, Vec<Attribute<'a>>>,
->;
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct Attribute<'a> {
-    pub(crate) type_id: asn1::ObjectIdentifier,
-    pub(crate) values: x509::Asn1ReadableOrWritable<
-        'a,
-        asn1::SetOf<'a, asn1::Tlv<'a>>,
-        asn1::SetOfWriter<'a, x509::common::RawTlv<'a>, [x509::common::RawTlv<'a>; 1]>,
-    >,
-}
-
-fn check_attribute_length<'a>(
-    values: asn1::SetOf<'a, asn1::Tlv<'a>>,
-) -> Result<(), CryptographyError> {
-    if values.count() > 1 {
-        Err(CryptographyError::from(
-            pyo3::exceptions::PyValueError::new_err("Only single-valued attributes are supported"),
-        ))
-    } else {
-        Ok(())
-    }
-}
-
-impl CertificationRequestInfo<'_> {
-    fn get_extension_attribute(&self) -> Result<Option<x509::Extensions<'_>>, CryptographyError> {
-        for attribute in self.attributes.unwrap_read().clone() {
-            if attribute.type_id == oid::EXTENSION_REQUEST
-                || attribute.type_id == oid::MS_EXTENSION_REQUEST
-            {
-                check_attribute_length(attribute.values.unwrap_read().clone())?;
-                let val = attribute.values.unwrap_read().clone().next().unwrap();
-                let exts = asn1::parse_single(val.full_data())?;
-                return Ok(Some(exts));
-            }
-        }
-        Ok(None)
-    }
-}
-
 #[ouroboros::self_referencing]
-struct OwnedRawCsr {
-    data: Vec<u8>,
+struct OwnedCsr {
+    data: pyo3::Py<pyo3::types::PyBytes>,
     #[borrows(data)]
     #[covariant]
-    value: RawCsr<'this>,
+    value: Csr<'this>,
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.x509")]
 struct CertificateSigningRequest {
-    raw: OwnedRawCsr,
+    raw: OwnedCsr,
     cached_extensions: Option<pyo3::PyObject>,
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::basic::PyObjectProtocol for CertificateSigningRequest {
-    fn __hash__(&self) -> u64 {
+#[pyo3::prelude::pymethods]
+impl CertificateSigningRequest {
+    fn __hash__(&self, py: pyo3::Python<'_>) -> u64 {
         let mut hasher = DefaultHasher::new();
-        self.raw.borrow_data().hash(&mut hasher);
+        self.raw.borrow_data().as_bytes(py).hash(&mut hasher);
         hasher.finish()
     }
 
     fn __richcmp__(
         &self,
-        other: pyo3::PyRef<CertificateSigningRequest>,
+        py: pyo3::Python<'_>,
+        other: pyo3::PyRef<'_, CertificateSigningRequest>,
         op: pyo3::basic::CompareOp,
     ) -> pyo3::PyResult<bool> {
         match op {
-            pyo3::basic::CompareOp::Eq => Ok(self.raw.borrow_data() == other.raw.borrow_data()),
-            pyo3::basic::CompareOp::Ne => Ok(self.raw.borrow_data() != other.raw.borrow_data()),
+            pyo3::basic::CompareOp::Eq => {
+                Ok(self.raw.borrow_data().as_bytes(py) == other.raw.borrow_data().as_bytes(py))
+            }
+            pyo3::basic::CompareOp::Ne => {
+                Ok(self.raw.borrow_data().as_bytes(py) != other.raw.borrow_data().as_bytes(py))
+            }
             _ => Err(pyo3::exceptions::PyTypeError::new_err(
                 "CSRs cannot be ordered",
             )),
         }
     }
-}
 
-#[pyo3::prelude::pymethods]
-impl CertificateSigningRequest {
     fn public_key<'p>(&self, py: pyo3::Python<'p>) -> CryptographyResult<&'p pyo3::PyAny> {
         // This makes an unnecessary copy. It'd be nice to get rid of it.
         let serialized = pyo3::types::PyBytes::new(
             py,
             &asn1::write_single(&self.raw.borrow_value().csr_info.spki)?,
         );
         Ok(py
-            .import("cryptography.hazmat.primitives.serialization")?
-            .getattr(crate::intern!(py, "load_der_public_key"))?
+            .import(pyo3::intern!(
+                py,
+                "cryptography.hazmat.primitives.serialization"
+            ))?
+            .getattr(pyo3::intern!(py, "load_der_public_key"))?
             .call1((serialized,))?)
     }
 
     #[getter]
     fn subject<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         Ok(x509::parse_name(
             py,
@@ -145,34 +93,31 @@
 
     #[getter]
     fn signature_hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> Result<&'p pyo3::PyAny, CryptographyError> {
         let sig_oids_to_hash = py
-            .import("cryptography.hazmat._oid")?
-            .getattr(crate::intern!(py, "_SIG_OIDS_TO_HASH"))?;
+            .import(pyo3::intern!(py, "cryptography.hazmat._oid"))?
+            .getattr(pyo3::intern!(py, "_SIG_OIDS_TO_HASH"))?;
         let hash_alg = sig_oids_to_hash.get_item(self.signature_algorithm_oid(py)?);
         match hash_alg {
             Ok(data) => Ok(data),
-            Err(_) => Err(CryptographyError::from(pyo3::PyErr::from_instance(
-                py.import("cryptography.exceptions")?.call_method1(
-                    "UnsupportedAlgorithm",
-                    (format!(
-                        "Signature algorithm OID: {} not recognized",
-                        self.raw.borrow_value().signature_alg.oid
-                    ),),
-                )?,
-            ))),
+            Err(_) => Err(CryptographyError::from(
+                exceptions::UnsupportedAlgorithm::new_err(format!(
+                    "Signature algorithm OID: {} not recognized",
+                    self.raw.borrow_value().signature_alg.oid()
+                )),
+            )),
         }
     }
 
     #[getter]
     fn signature_algorithm_oid<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        oid_to_py_oid(py, &self.raw.borrow_value().signature_alg.oid)
+        oid_to_py_oid(py, self.raw.borrow_value().signature_alg.oid())
     }
 
     fn public_bytes<'p>(
         &self,
         py: pyo3::Python<'p>,
         encoding: &'p pyo3::PyAny,
     ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
@@ -183,16 +128,16 @@
 
     fn get_attribute_for_oid<'p>(
         &self,
         py: pyo3::Python<'p>,
         oid: &pyo3::PyAny,
     ) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let cryptography_warning = py
-            .import("cryptography.utils")?
-            .getattr(crate::intern!(py, "DeprecatedIn36"))?;
+            .import(pyo3::intern!(py, "cryptography.utils"))?
+            .getattr(pyo3::intern!(py, "DeprecatedIn36"))?;
         pyo3::PyErr::warn(
             py,
             cryptography_warning,
             "CertificateSigningRequest.get_attribute_for_oid has been deprecated. Please switch to request.attributes.get_attribute_for_oid.",
             1,
         )?;
         let rust_oid = py_oid_to_oid(oid)?;
@@ -201,86 +146,104 @@
             .borrow_value()
             .csr_info
             .attributes
             .unwrap_read()
             .clone()
         {
             if rust_oid == attribute.type_id {
-                check_attribute_length(attribute.values.unwrap_read().clone())?;
+                check_attribute_length(attribute.values.unwrap_read().clone()).map_err(|_| {
+                    pyo3::exceptions::PyValueError::new_err(
+                        "Only single-valued attributes are supported",
+                    )
+                })?;
                 let val = attribute.values.unwrap_read().clone().next().unwrap();
                 // We allow utf8string, printablestring, and ia5string at this time
                 if val.tag() == asn1::Utf8String::TAG
                     || val.tag() == asn1::PrintableString::TAG
                     || val.tag() == asn1::IA5String::TAG
                 {
                     return Ok(pyo3::types::PyBytes::new(py, val.data()));
-                } else {
-                    return Err(pyo3::exceptions::PyValueError::new_err(format!(
-                        "OID {} has a disallowed ASN.1 type: {:?}",
-                        oid,
-                        val.tag()
-                    )));
                 }
+                return Err(pyo3::exceptions::PyValueError::new_err(format!(
+                    "OID {} has a disallowed ASN.1 type: {:?}",
+                    oid,
+                    val.tag()
+                )));
             }
         }
-        Err(pyo3::PyErr::from_instance(
-            py.import("cryptography.x509")?.call_method1(
-                "AttributeNotFound",
-                (format!("No {} attribute was found", oid), oid),
-            )?,
-        ))
+        Err(exceptions::AttributeNotFound::new_err((
+            format!("No {} attribute was found", oid),
+            oid.into_py(py),
+        )))
     }
 
     #[getter]
     fn attributes<'p>(&mut self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let pyattrs = pyo3::types::PyList::empty(py);
         for attribute in self
             .raw
             .borrow_value()
             .csr_info
             .attributes
             .unwrap_read()
             .clone()
         {
-            check_attribute_length(attribute.values.unwrap_read().clone())?;
+            check_attribute_length(attribute.values.unwrap_read().clone()).map_err(|_| {
+                pyo3::exceptions::PyValueError::new_err(
+                    "Only single-valued attributes are supported",
+                )
+            })?;
             let oid = oid_to_py_oid(py, &attribute.type_id)?;
             let val = attribute.values.unwrap_read().clone().next().unwrap();
             let serialized = pyo3::types::PyBytes::new(py, val.data());
             let tag = val.tag().as_u8().ok_or_else(|| {
                 CryptographyError::from(pyo3::exceptions::PyValueError::new_err(
                     "Long-form tags are not supported in CSR attribute values",
                 ))
             })?;
             let pyattr = py
-                .import("cryptography.x509")?
-                .call_method1("Attribute", (oid, serialized, tag))?;
+                .import(pyo3::intern!(py, "cryptography.x509"))?
+                .call_method1(pyo3::intern!(py, "Attribute"), (oid, serialized, tag))?;
             pyattrs.append(pyattr)?;
         }
-        py.import("cryptography.x509")?
-            .call_method1("Attributes", (pyattrs,))
+        py.import(pyo3::intern!(py, "cryptography.x509"))?
+            .call_method1(pyo3::intern!(py, "Attributes"), (pyattrs,))
     }
 
     #[getter]
     fn extensions(&mut self, py: pyo3::Python<'_>) -> pyo3::PyResult<pyo3::PyObject> {
-        let exts = self.raw.borrow_value().csr_info.get_extension_attribute()?;
+        let raw_exts = self
+            .raw
+            .borrow_value()
+            .csr_info
+            .get_extension_attribute()
+            .map_err(|_| {
+                pyo3::exceptions::PyValueError::new_err(
+                    "Only single-valued attributes are supported",
+                )
+            })?;
 
-        x509::parse_and_cache_extensions(py, &mut self.cached_extensions, &exts, |oid, ext_data| {
-            certificate::parse_cert_ext(py, oid.clone(), ext_data)
-        })
+        x509::parse_and_cache_extensions(
+            py,
+            &mut self.cached_extensions,
+            &raw_exts,
+            |oid, ext_data| certificate::parse_cert_ext(py, oid.clone(), ext_data),
+        )
     }
 
     #[getter]
     fn is_signature_valid(
         slf: pyo3::PyRef<'_, Self>,
         py: pyo3::Python<'_>,
     ) -> CryptographyResult<bool> {
-        Ok(sign::verify_signature_with_oid(
+        let public_key = slf.public_key(py)?;
+        Ok(sign::verify_signature_with_signature_algorithm(
             py,
-            slf.public_key(py)?,
-            &slf.raw.borrow_value().signature_alg.oid,
+            public_key,
+            &slf.raw.borrow_value().signature_alg,
             slf.raw.borrow_value().signature.as_bytes(),
             &asn1::write_single(&slf.raw.borrow_value().csr_info)?,
         )
         .is_ok())
     }
 }
 
@@ -292,32 +255,35 @@
     // We support both PEM header strings that OpenSSL does
     // https://github.com/openssl/openssl/blob/5e2d22d53ed322a7124e26a4fbd116a8210eb77a/include/openssl/pem.h#L35-L36
     let parsed = x509::find_in_pem(
         data,
         |p| p.tag == "CERTIFICATE REQUEST" || p.tag == "NEW CERTIFICATE REQUEST",
         "Valid PEM but no BEGIN CERTIFICATE REQUEST/END CERTIFICATE REQUEST delimiters. Are you sure this is a CSR?",
     )?;
-    load_der_x509_csr(py, &parsed.contents)
+    load_der_x509_csr(
+        py,
+        pyo3::types::PyBytes::new(py, &parsed.contents).into_py(py),
+    )
 }
 
 #[pyo3::prelude::pyfunction]
 fn load_der_x509_csr(
     py: pyo3::Python<'_>,
-    data: &[u8],
+    data: pyo3::Py<pyo3::types::PyBytes>,
 ) -> CryptographyResult<CertificateSigningRequest> {
-    let raw = OwnedRawCsr::try_new(data.to_vec(), |data| asn1::parse_single(data))?;
+    let raw = OwnedCsr::try_new(data, |data| asn1::parse_single(data.as_bytes(py)))?;
 
     let version = raw.borrow_value().csr_info.version;
     if version != 0 {
-        let x509_module = py.import("cryptography.x509")?;
-        return Err(CryptographyError::from(pyo3::PyErr::from_instance(
-            x509_module
-                .getattr(crate::intern!(py, "InvalidVersion"))?
-                .call1((format!("{} is not a valid CSR version", version), version))?,
-        )));
+        return Err(CryptographyError::from(
+            exceptions::InvalidVersion::new_err((
+                format!("{} is not a valid CSR version", version),
+                version,
+            )),
+        ));
     }
 
     Ok(CertificateSigningRequest {
         raw,
         cached_extensions: None,
     })
 }
@@ -325,45 +291,56 @@
 #[pyo3::prelude::pyfunction]
 fn create_x509_csr(
     py: pyo3::Python<'_>,
     builder: &pyo3::PyAny,
     private_key: &pyo3::PyAny,
     hash_algorithm: &pyo3::PyAny,
 ) -> CryptographyResult<CertificateSigningRequest> {
-    let sigalg = x509::sign::compute_signature_algorithm(py, private_key, hash_algorithm)?;
-    let serialization_mod = py.import("cryptography.hazmat.primitives.serialization")?;
+    let sigalg = x509::sign::compute_signature_algorithm(
+        py,
+        private_key,
+        hash_algorithm,
+        py.None().into_ref(py),
+    )?;
+    let serialization_mod = py.import(pyo3::intern!(
+        py,
+        "cryptography.hazmat.primitives.serialization"
+    ))?;
     let der_encoding = serialization_mod
-        .getattr(crate::intern!(py, "Encoding"))?
-        .getattr(crate::intern!(py, "DER"))?;
+        .getattr(pyo3::intern!(py, "Encoding"))?
+        .getattr(pyo3::intern!(py, "DER"))?;
     let spki_format = serialization_mod
-        .getattr(crate::intern!(py, "PublicFormat"))?
-        .getattr(crate::intern!(py, "SubjectPublicKeyInfo"))?;
+        .getattr(pyo3::intern!(py, "PublicFormat"))?
+        .getattr(pyo3::intern!(py, "SubjectPublicKeyInfo"))?;
 
     let spki_bytes = private_key
-        .call_method0("public_key")?
-        .call_method1("public_bytes", (der_encoding, spki_format))?
+        .call_method0(pyo3::intern!(py, "public_key"))?
+        .call_method1(
+            pyo3::intern!(py, "public_bytes"),
+            (der_encoding, spki_format),
+        )?
         .extract::<&[u8]>()?;
 
     let mut attrs = vec![];
     let ext_bytes;
     if let Some(exts) = x509::common::encode_extensions(
         py,
-        builder.getattr(crate::intern!(py, "_extensions"))?,
+        builder.getattr(pyo3::intern!(py, "_extensions"))?,
         x509::extensions::encode_extension,
     )? {
         ext_bytes = asn1::write_single(&exts)?;
         attrs.push(Attribute {
             type_id: (oid::EXTENSION_REQUEST).clone(),
-            values: x509::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
+            values: common::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
                 asn1::parse_single(&ext_bytes)?,
             ])),
         })
     }
 
-    for py_attr in builder.getattr(crate::intern!(py, "_attributes"))?.iter()? {
+    for py_attr in builder.getattr(pyo3::intern!(py, "_attributes"))?.iter()? {
         let (py_oid, value, tag): (&pyo3::PyAny, &[u8], Option<u8>) = py_attr?.extract()?;
         let oid = py_oid_to_oid(py_oid)?;
         let tag = if let Some(tag) = tag {
             asn1::Tag::from_bytes(&[tag])?.0
         } else {
             if std::str::from_utf8(value).is_err() {
                 return Err(CryptographyError::from(
@@ -373,42 +350,47 @@
                 ));
             }
             asn1::Utf8String::TAG
         };
 
         attrs.push(Attribute {
             type_id: oid,
-            values: x509::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
-                x509::common::RawTlv::new(tag, value),
+            values: common::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new([
+                common::RawTlv::new(tag, value),
             ])),
         })
     }
 
-    let py_subject_name = builder.getattr(crate::intern!(py, "_subject_name"))?;
+    let py_subject_name = builder.getattr(pyo3::intern!(py, "_subject_name"))?;
 
     let csr_info = CertificationRequestInfo {
         version: 0,
         subject: x509::common::encode_name(py, py_subject_name)?,
         spki: asn1::parse_single(spki_bytes)?,
-        attributes: x509::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new(attrs)),
+        attributes: common::Asn1ReadableOrWritable::new_write(asn1::SetOfWriter::new(attrs)),
     };
 
     let tbs_bytes = asn1::write_single(&csr_info)?;
-    let signature = x509::sign::sign_data(py, private_key, hash_algorithm, &tbs_bytes)?;
-    let data = asn1::write_single(&RawCsr {
+    let signature = x509::sign::sign_data(
+        py,
+        private_key,
+        hash_algorithm,
+        py.None().into_ref(py),
+        &tbs_bytes,
+    )?;
+    let data = asn1::write_single(&Csr {
         csr_info,
         signature_alg: sigalg,
         signature: asn1::BitString::new(signature, 0).unwrap(),
     })?;
-    // TODO: extra copy as we round-trip through a slice
-    load_der_x509_csr(py, &data)
+    load_der_x509_csr(py, pyo3::types::PyBytes::new(py, &data).into_py(py))
 }
 
 pub(crate) fn add_to_module(module: &pyo3::prelude::PyModule) -> pyo3::PyResult<()> {
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_der_x509_csr))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_pem_x509_csr))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(create_x509_csr))?;
+    module.add_function(pyo3::wrap_pyfunction!(load_der_x509_csr, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(load_pem_x509_csr, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(create_x509_csr, module)?)?;
 
     module.add_class::<CertificateSigningRequest>()?;
 
     Ok(())
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/mod.rs` & `cryptography-41.0.0/src/rust/src/x509/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 pub(crate) mod common;
 pub(crate) mod crl;
 pub(crate) mod csr;
 pub(crate) mod extensions;
 pub(crate) mod ocsp;
 pub(crate) mod ocsp_req;
 pub(crate) mod ocsp_resp;
-pub(crate) mod oid;
 pub(crate) mod sct;
 pub(crate) mod sign;
 
-pub(crate) use certificate::Certificate;
 pub(crate) use common::{
-    chrono_to_py, find_in_pem, parse_and_cache_extensions, parse_general_name, parse_general_names,
-    parse_name, parse_rdn, py_to_chrono, AlgorithmIdentifier, Asn1ReadableOrWritable,
-    AttributeTypeValue, Extensions, GeneralName, Name, Time,
+    datetime_to_py, find_in_pem, parse_and_cache_extensions, parse_general_name,
+    parse_general_names, parse_name, parse_rdn, py_to_datetime,
 };
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/ocsp.rs` & `cryptography-41.0.0/src/rust/src/x509/ocsp.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,127 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::error::CryptographyResult;
 use crate::x509;
-use crate::x509::oid;
+use crate::x509::certificate::Certificate;
+use cryptography_x509::common;
+use cryptography_x509::ocsp_req::CertID;
 use once_cell::sync::Lazy;
 use std::collections::HashMap;
 
-pub(crate) static OIDS_TO_HASH: Lazy<HashMap<&asn1::ObjectIdentifier, &str>> = Lazy::new(|| {
+pub(crate) static ALGORITHM_PARAMETERS_TO_HASH: Lazy<
+    HashMap<common::AlgorithmParameters<'_>, &str>,
+> = Lazy::new(|| {
     let mut h = HashMap::new();
-    h.insert(&oid::SHA1_OID, "SHA1");
-    h.insert(&oid::SHA224_OID, "SHA224");
-    h.insert(&oid::SHA256_OID, "SHA256");
-    h.insert(&oid::SHA384_OID, "SHA384");
-    h.insert(&oid::SHA512_OID, "SHA512");
+    h.insert(common::AlgorithmParameters::Sha1(Some(())), "SHA1");
+    h.insert(common::AlgorithmParameters::Sha224(Some(())), "SHA224");
+    h.insert(common::AlgorithmParameters::Sha256(Some(())), "SHA256");
+    h.insert(common::AlgorithmParameters::Sha384(Some(())), "SHA384");
+    h.insert(common::AlgorithmParameters::Sha512(Some(())), "SHA512");
     h
 });
-pub(crate) static HASH_NAME_TO_OIDS: Lazy<HashMap<&str, &asn1::ObjectIdentifier>> =
-    Lazy::new(|| {
-        let mut h = HashMap::new();
-        h.insert("sha1", &oid::SHA1_OID);
-        h.insert("sha224", &oid::SHA224_OID);
-        h.insert("sha256", &oid::SHA256_OID);
-        h.insert("sha384", &oid::SHA384_OID);
-        h.insert("sha512", &oid::SHA512_OID);
-        h
-    });
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-pub(crate) struct CertID<'a> {
-    pub(crate) hash_algorithm: x509::AlgorithmIdentifier<'a>,
-    pub(crate) issuer_name_hash: &'a [u8],
-    pub(crate) issuer_key_hash: &'a [u8],
-    pub(crate) serial_number: asn1::BigInt<'a>,
+
+pub(crate) static HASH_NAME_TO_ALGORITHM_IDENTIFIERS: Lazy<
+    HashMap<&str, common::AlgorithmIdentifier<'_>>,
+> = Lazy::new(|| {
+    let mut h = HashMap::new();
+    h.insert(
+        "sha1",
+        common::AlgorithmIdentifier {
+            oid: asn1::DefinedByMarker::marker(),
+            params: common::AlgorithmParameters::Sha1(Some(())),
+        },
+    );
+    h.insert(
+        "sha224",
+        common::AlgorithmIdentifier {
+            oid: asn1::DefinedByMarker::marker(),
+            params: common::AlgorithmParameters::Sha224(Some(())),
+        },
+    );
+    h.insert(
+        "sha256",
+        common::AlgorithmIdentifier {
+            oid: asn1::DefinedByMarker::marker(),
+            params: common::AlgorithmParameters::Sha256(Some(())),
+        },
+    );
+    h.insert(
+        "sha384",
+        common::AlgorithmIdentifier {
+            oid: asn1::DefinedByMarker::marker(),
+            params: common::AlgorithmParameters::Sha384(Some(())),
+        },
+    );
+    h.insert(
+        "sha512",
+        common::AlgorithmIdentifier {
+            oid: asn1::DefinedByMarker::marker(),
+            params: common::AlgorithmParameters::Sha512(Some(())),
+        },
+    );
+    h
+});
+
+pub(crate) fn certid_new<'p>(
+    py: pyo3::Python<'p>,
+    cert: &'p Certificate,
+    issuer: &'p Certificate,
+    hash_algorithm: &'p pyo3::PyAny,
+) -> CryptographyResult<CertID<'p>> {
+    let issuer_der = asn1::write_single(&cert.raw.borrow_value_public().tbs_cert.issuer)?;
+    let issuer_name_hash = hash_data(py, hash_algorithm, &issuer_der)?;
+    let issuer_key_hash = hash_data(
+        py,
+        hash_algorithm,
+        issuer
+            .raw
+            .borrow_value_public()
+            .tbs_cert
+            .spki
+            .subject_public_key
+            .as_bytes(),
+    )?;
+
+    Ok(CertID {
+        hash_algorithm: x509::ocsp::HASH_NAME_TO_ALGORITHM_IDENTIFIERS[hash_algorithm
+            .getattr(pyo3::intern!(py, "name"))?
+            .extract::<&str>()?]
+        .clone(),
+        issuer_name_hash,
+        issuer_key_hash,
+        serial_number: cert.raw.borrow_value_public().tbs_cert.serial,
+    })
 }
 
-impl CertID<'_> {
-    pub(crate) fn new<'p>(
-        py: pyo3::Python<'p>,
-        cert: &'p x509::Certificate,
-        issuer: &'p x509::Certificate,
-        hash_algorithm: &'p pyo3::PyAny,
-    ) -> CryptographyResult<CertID<'p>> {
-        let issuer_der = asn1::write_single(&cert.raw.borrow_value_public().tbs_cert.issuer)?;
-        let issuer_name_hash = hash_data(py, hash_algorithm, &issuer_der)?;
-        let issuer_key_hash = hash_data(
-            py,
-            hash_algorithm,
-            issuer
-                .raw
-                .borrow_value_public()
-                .tbs_cert
-                .spki
-                .subject_public_key
-                .as_bytes(),
-        )?;
-
-        Ok(CertID {
-            hash_algorithm: x509::AlgorithmIdentifier {
-                oid: HASH_NAME_TO_OIDS[hash_algorithm
-                    .getattr(crate::intern!(py, "name"))?
-                    .extract::<&str>()?]
-                .clone(),
-                params: Some(*x509::sign::NULL_TLV),
-            },
-            issuer_name_hash,
-            issuer_key_hash,
-            serial_number: cert.raw.borrow_value_public().tbs_cert.serial,
-        })
-    }
-
-    pub(crate) fn new_from_hash<'p>(
-        py: pyo3::Python<'p>,
-        issuer_name_hash: &'p [u8],
-        issuer_key_hash: &'p [u8],
-        serial_number: asn1::BigInt<'p>,
-        hash_algorithm: &'p pyo3::PyAny,
-    ) -> CryptographyResult<CertID<'p>> {
-        Ok(CertID {
-            hash_algorithm: x509::AlgorithmIdentifier {
-                oid: HASH_NAME_TO_OIDS[hash_algorithm
-                    .getattr(crate::intern!(py, "name"))?
-                    .extract::<&str>()?]
-                .clone(),
-                params: Some(*x509::sign::NULL_TLV),
-            },
-            issuer_name_hash,
-            issuer_key_hash,
-            serial_number,
-        })
-    }
+pub(crate) fn certid_new_from_hash<'p>(
+    py: pyo3::Python<'p>,
+    issuer_name_hash: &'p [u8],
+    issuer_key_hash: &'p [u8],
+    serial_number: asn1::BigInt<'p>,
+    hash_algorithm: &'p pyo3::PyAny,
+) -> CryptographyResult<CertID<'p>> {
+    Ok(CertID {
+        hash_algorithm: x509::ocsp::HASH_NAME_TO_ALGORITHM_IDENTIFIERS[hash_algorithm
+            .getattr(pyo3::intern!(py, "name"))?
+            .extract::<&str>()?]
+        .clone(),
+        issuer_name_hash,
+        issuer_key_hash,
+        serial_number,
+    })
 }
 
 pub(crate) fn hash_data<'p>(
     py: pyo3::Python<'p>,
     py_hash_alg: &'p pyo3::PyAny,
     data: &[u8],
 ) -> pyo3::PyResult<&'p [u8]> {
     let hash = py
-        .import("cryptography.hazmat.primitives.hashes")?
-        .getattr(crate::intern!(py, "Hash"))?
+        .import(pyo3::intern!(py, "cryptography.hazmat.primitives.hashes"))?
+        .getattr(pyo3::intern!(py, "Hash"))?
         .call1((py_hash_alg,))?;
-    hash.call_method1("update", (data,))?;
-    hash.call_method0("finalize")?.extract()
+    hash.call_method1(pyo3::intern!(py, "update"), (data,))?;
+    hash.call_method0(pyo3::intern!(py, "finalize"))?.extract()
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/ocsp_req.rs` & `cryptography-41.0.0/src/rust/src/x509/ocsp_req.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
-use crate::asn1::{big_byte_slice_to_py_int, py_uint_to_big_endian_bytes};
+use crate::asn1::{big_byte_slice_to_py_int, oid_to_py_oid, py_uint_to_big_endian_bytes};
 use crate::error::{CryptographyError, CryptographyResult};
-use crate::x509;
-use crate::x509::{extensions, ocsp, oid};
-use std::sync::Arc;
+use crate::x509::{extensions, ocsp};
+use crate::{exceptions, x509};
+use cryptography_x509::{common, ocsp_req, oid};
+use pyo3::IntoPy;
 
 #[ouroboros::self_referencing]
-struct OwnedRawOCSPRequest {
-    data: Arc<[u8]>,
+struct OwnedOCSPRequest {
+    data: pyo3::Py<pyo3::types::PyBytes>,
     #[borrows(data)]
     #[covariant]
-    value: RawOCSPRequest<'this>,
+    value: ocsp_req::OCSPRequest<'this>,
 }
 
 #[pyo3::prelude::pyfunction]
-fn load_der_ocsp_request(_py: pyo3::Python<'_>, data: &[u8]) -> CryptographyResult<OCSPRequest> {
-    let raw = OwnedRawOCSPRequest::try_new(Arc::from(data), |data| asn1::parse_single(data))?;
+fn load_der_ocsp_request(
+    py: pyo3::Python<'_>,
+    data: pyo3::Py<pyo3::types::PyBytes>,
+) -> CryptographyResult<OCSPRequest> {
+    let raw = OwnedOCSPRequest::try_new(data, |data| asn1::parse_single(data.as_bytes(py)))?;
 
     if raw
         .borrow_value()
         .tbs_request
         .request_list
         .unwrap_read()
         .len()
@@ -37,23 +41,23 @@
 
     Ok(OCSPRequest {
         raw,
         cached_extensions: None,
     })
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.ocsp")]
 struct OCSPRequest {
-    raw: OwnedRawOCSPRequest,
+    raw: OwnedOCSPRequest,
 
     cached_extensions: Option<pyo3::PyObject>,
 }
 
 impl OCSPRequest {
-    fn cert_id(&self) -> ocsp::CertID<'_> {
+    fn cert_id(&self) -> ocsp_req::CertID<'_> {
         self.raw
             .borrow_value()
             .tbs_request
             .request_list
             .unwrap_read()
             .clone()
             .next()
@@ -77,184 +81,166 @@
     #[getter]
     fn hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> Result<&'p pyo3::PyAny, CryptographyError> {
         let cert_id = self.cert_id();
 
-        let hashes = py.import("cryptography.hazmat.primitives.hashes")?;
-        match ocsp::OIDS_TO_HASH.get(&cert_id.hash_algorithm.oid) {
-            Some(alg_name) => Ok(hashes.getattr(alg_name)?.call0()?),
-            None => {
-                let exceptions = py.import("cryptography.exceptions")?;
-                Err(CryptographyError::from(pyo3::PyErr::from_instance(
-                    exceptions
-                        .getattr(crate::intern!(py, "UnsupportedAlgorithm"))?
-                        .call1((format!(
-                            "Signature algorithm OID: {} not recognized",
-                            cert_id.hash_algorithm.oid
-                        ),))?,
-                )))
-            }
+        let hashes = py.import(pyo3::intern!(py, "cryptography.hazmat.primitives.hashes"))?;
+        match ocsp::ALGORITHM_PARAMETERS_TO_HASH.get(&cert_id.hash_algorithm.params) {
+            Some(alg_name) => Ok(hashes.getattr(*alg_name)?.call0()?),
+            None => Err(CryptographyError::from(
+                exceptions::UnsupportedAlgorithm::new_err(format!(
+                    "Signature algorithm OID: {} not recognized",
+                    cert_id.hash_algorithm.oid()
+                )),
+            )),
         }
     }
 
     #[getter]
     fn serial_number<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> Result<&'p pyo3::PyAny, CryptographyError> {
         let bytes = self.cert_id().serial_number.as_bytes();
         Ok(big_byte_slice_to_py_int(py, bytes)?)
     }
 
     #[getter]
     fn extensions(&mut self, py: pyo3::Python<'_>) -> pyo3::PyResult<pyo3::PyObject> {
-        let x509_module = py.import("cryptography.x509")?;
+        let tbs_request = &self.raw.borrow_value().tbs_request;
+
+        let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
         x509::parse_and_cache_extensions(
             py,
             &mut self.cached_extensions,
-            &self.raw.borrow_value().tbs_request.request_extensions,
+            &tbs_request.raw_request_extensions,
             |oid, value| {
-                match oid {
-                    &oid::NONCE_OID => {
+                match *oid {
+                    oid::NONCE_OID => {
                         // This is a disaster. RFC 2560 says that the contents of the nonce is
                         // just the raw extension value. This is nonsense, since they're always
                         // supposed to be ASN.1 TLVs. RFC 6960 correctly specifies that the
                         // nonce is an OCTET STRING, and so you should unwrap the TLV to get
                         // the nonce. So we try parsing as a TLV and fall back to just using
                         // the raw value.
                         let nonce = asn1::parse_single::<&[u8]>(value).unwrap_or(value);
-                        Ok(Some(x509_module.call_method1("OCSPNonce", (nonce,))?))
+                        Ok(Some(
+                            x509_module.call_method1(pyo3::intern!(py, "OCSPNonce"), (nonce,))?,
+                        ))
+                    }
+                    oid::ACCEPTABLE_RESPONSES_OID => {
+                        let oids = asn1::parse_single::<
+                            asn1::SequenceOf<'_, asn1::ObjectIdentifier>,
+                        >(value)?;
+                        let py_oids = pyo3::types::PyList::empty(py);
+                        for oid in oids {
+                            py_oids.append(oid_to_py_oid(py, &oid)?)?;
+                        }
+
+                        Ok(Some(x509_module.call_method1(
+                            pyo3::intern!(py, "OCSPAcceptableResponses"),
+                            (py_oids,),
+                        )?))
                     }
                     _ => Ok(None),
                 }
             },
         )
     }
 
     fn public_bytes<'p>(
         &self,
         py: pyo3::Python<'p>,
         encoding: &pyo3::PyAny,
     ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
         let der = py
-            .import("cryptography.hazmat.primitives.serialization")?
-            .getattr(crate::intern!(py, "Encoding"))?
-            .getattr(crate::intern!(py, "DER"))?;
-        if encoding != der {
+            .import(pyo3::intern!(
+                py,
+                "cryptography.hazmat.primitives.serialization"
+            ))?
+            .getattr(pyo3::intern!(py, "Encoding"))?
+            .getattr(pyo3::intern!(py, "DER"))?;
+        if !encoding.is(der) {
             return Err(pyo3::exceptions::PyValueError::new_err(
                 "The only allowed encoding value is Encoding.DER",
             )
             .into());
         }
         let result = asn1::write_single(self.raw.borrow_value())?;
         Ok(pyo3::types::PyBytes::new(py, &result))
     }
 }
 
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct RawOCSPRequest<'a> {
-    tbs_request: TBSRequest<'a>,
-    // Parsing out the full structure, which includes the entirety of a
-    // certificate is more trouble than it's worth, since it's not in the
-    // Python API.
-    #[explicit(0)]
-    optional_signature: Option<asn1::Sequence<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct TBSRequest<'a> {
-    #[explicit(0)]
-    #[default(0)]
-    version: u8,
-    #[explicit(1)]
-    requestor_name: Option<x509::GeneralName<'a>>,
-    request_list: x509::Asn1ReadableOrWritable<
-        'a,
-        asn1::SequenceOf<'a, Request<'a>>,
-        asn1::SequenceOfWriter<'a, Request<'a>>,
-    >,
-    #[explicit(2)]
-    request_extensions: Option<x509::Extensions<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct Request<'a> {
-    req_cert: ocsp::CertID<'a>,
-    #[explicit(0)]
-    single_request_extensions: Option<x509::Extensions<'a>>,
-}
-
 #[pyo3::prelude::pyfunction]
 fn create_ocsp_request(
     py: pyo3::Python<'_>,
     builder: &pyo3::PyAny,
 ) -> CryptographyResult<OCSPRequest> {
-    let builder_request = builder.getattr(crate::intern!(py, "_request"))?;
+    let builder_request = builder.getattr(pyo3::intern!(py, "_request"))?;
 
     // Declare outside the if-block so the lifetimes are right.
     let (py_cert, py_issuer, py_hash): (
-        pyo3::PyRef<'_, x509::Certificate>,
-        pyo3::PyRef<'_, x509::Certificate>,
+        pyo3::PyRef<'_, x509::certificate::Certificate>,
+        pyo3::PyRef<'_, x509::certificate::Certificate>,
         &pyo3::PyAny,
     );
     let req_cert = if !builder_request.is_none() {
         let tuple = builder_request.extract::<(
-            pyo3::PyRef<'_, x509::Certificate>,
-            pyo3::PyRef<'_, x509::Certificate>,
+            pyo3::PyRef<'_, x509::certificate::Certificate>,
+            pyo3::PyRef<'_, x509::certificate::Certificate>,
             &pyo3::PyAny,
         )>()?;
         py_cert = tuple.0;
         py_issuer = tuple.1;
         py_hash = tuple.2;
-        ocsp::CertID::new(py, &py_cert, &py_issuer, py_hash)?
+        ocsp::certid_new(py, &py_cert, &py_issuer, py_hash)?
     } else {
         let (issuer_name_hash, issuer_key_hash, py_serial, py_hash): (
             &[u8],
             &[u8],
             &pyo3::types::PyLong,
             &pyo3::PyAny,
         ) = builder
-            .getattr(crate::intern!(py, "_request_hash"))?
+            .getattr(pyo3::intern!(py, "_request_hash"))?
             .extract()?;
         let serial_number = asn1::BigInt::new(py_uint_to_big_endian_bytes(py, py_serial)?).unwrap();
-        ocsp::CertID::new_from_hash(
+        ocsp::certid_new_from_hash(
             py,
             issuer_name_hash,
             issuer_key_hash,
             serial_number,
             py_hash,
         )?
     };
 
     let extensions = x509::common::encode_extensions(
         py,
-        builder.getattr(crate::intern!(py, "_extensions"))?,
+        builder.getattr(pyo3::intern!(py, "_extensions"))?,
         extensions::encode_extension,
     )?;
-    let reqs = [Request {
+    let reqs = [ocsp_req::Request {
         req_cert,
         single_request_extensions: None,
     }];
-    let ocsp_req = RawOCSPRequest {
-        tbs_request: TBSRequest {
+    let ocsp_req = ocsp_req::OCSPRequest {
+        tbs_request: ocsp_req::TBSRequest {
             version: 0,
             requestor_name: None,
-            request_list: x509::Asn1ReadableOrWritable::new_write(asn1::SequenceOfWriter::new(
+            request_list: common::Asn1ReadableOrWritable::new_write(asn1::SequenceOfWriter::new(
                 &reqs,
             )),
-            request_extensions: extensions,
+            raw_request_extensions: extensions,
         },
         optional_signature: None,
     };
     let data = asn1::write_single(&ocsp_req)?;
-    // TODO: extra copy as we round-trip through a slice
-    load_der_ocsp_request(py, &data)
+    load_der_ocsp_request(py, pyo3::types::PyBytes::new(py, &data).into_py(py))
 }
 
 pub(crate) fn add_to_module(module: &pyo3::prelude::PyModule) -> pyo3::PyResult<()> {
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_der_ocsp_request))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(create_ocsp_request))?;
+    module.add_function(pyo3::wrap_pyfunction!(load_der_ocsp_request, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(create_ocsp_request, module)?)?;
 
     Ok(())
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/ocsp_resp.rs` & `cryptography-41.0.0/src/rust/src/x509/ocsp_resp.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::asn1::{big_byte_slice_to_py_int, oid_to_py_oid};
 use crate::error::{CryptographyError, CryptographyResult};
-use crate::x509;
-use crate::x509::{certificate, crl, extensions, ocsp, oid, py_to_chrono, sct};
-use chrono::Timelike;
+use crate::x509::{certificate, crl, extensions, ocsp, py_to_datetime, sct};
+use crate::{exceptions, x509};
+use cryptography_x509::ocsp_resp::SingleResponse;
+use cryptography_x509::{common, ocsp_resp, oid};
+use pyo3::IntoPy;
 use std::sync::Arc;
 
 const BASIC_RESPONSE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 48, 1, 1);
 
 #[pyo3::prelude::pyfunction]
 fn load_der_ocsp_response(
-    _py: pyo3::Python<'_>,
-    data: &[u8],
+    py: pyo3::Python<'_>,
+    data: pyo3::Py<pyo3::types::PyBytes>,
 ) -> Result<OCSPResponse, CryptographyError> {
-    let raw = OwnedRawOCSPResponse::try_new(Arc::from(data), |data| asn1::parse_single(data))?;
+    let raw = OwnedOCSPResponse::try_new(data, |data| asn1::parse_single(data.as_bytes(py)))?;
 
     let response = raw.borrow_value();
     match response.response_status.value() {
         SUCCESSFUL_RESPONSE => match response.response_bytes {
             Some(ref bytes) => {
                 if bytes.response_type != BASIC_RESPONSE_OID {
                     return Err(CryptographyError::from(
@@ -53,31 +55,31 @@
         raw: Arc::new(raw),
         cached_extensions: None,
         cached_single_extensions: None,
     })
 }
 
 #[ouroboros::self_referencing]
-struct OwnedRawOCSPResponse {
-    data: Arc<[u8]>,
+struct OwnedOCSPResponse {
+    data: pyo3::Py<pyo3::types::PyBytes>,
     #[borrows(data)]
     #[covariant]
-    value: RawOCSPResponse<'this>,
+    value: ocsp_resp::OCSPResponse<'this>,
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.ocsp")]
 struct OCSPResponse {
-    raw: Arc<OwnedRawOCSPResponse>,
+    raw: Arc<OwnedOCSPResponse>,
 
     cached_extensions: Option<pyo3::PyObject>,
     cached_single_extensions: Option<pyo3::PyObject>,
 }
 
 impl OCSPResponse {
-    fn requires_successful_response(&self) -> pyo3::PyResult<&BasicOCSPResponse<'_>> {
+    fn requires_successful_response(&self) -> pyo3::PyResult<&ocsp_resp::BasicOCSPResponse<'_>> {
         match self.raw.borrow_value().response_bytes.as_ref() {
             Some(b) => Ok(b.response.get()),
             None => Err(pyo3::exceptions::PyValueError::new_err(
                 "OCSP response status is not successful so the property has no value",
             )),
         }
     }
@@ -128,69 +130,72 @@
             "TRY_LATER"
         } else if status == SIG_REQUIRED_RESPONSE {
             "SIG_REQUIRED"
         } else {
             assert_eq!(status, UNAUTHORIZED_RESPONSE);
             "UNAUTHORIZED"
         };
-        py.import("cryptography.x509.ocsp")?
-            .getattr(crate::intern!(py, "OCSPResponseStatus"))?
+        py.import(pyo3::intern!(py, "cryptography.x509.ocsp"))?
+            .getattr(pyo3::intern!(py, "OCSPResponseStatus"))?
             .getattr(attr)
     }
 
     #[getter]
     fn responder_name<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
         match resp.tbs_response_data.responder_id {
-            ResponderId::ByName(ref name) => Ok(x509::parse_name(py, name)?),
-            ResponderId::ByKey(_) => Ok(py.None().into_ref(py)),
+            ocsp_resp::ResponderId::ByName(ref name) => Ok(x509::parse_name(py, name)?),
+            ocsp_resp::ResponderId::ByKey(_) => Ok(py.None().into_ref(py)),
         }
     }
 
     #[getter]
     fn responder_key_hash<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
         match resp.tbs_response_data.responder_id {
-            ResponderId::ByKey(key_hash) => Ok(pyo3::types::PyBytes::new(py, key_hash).as_ref()),
-            ResponderId::ByName(_) => Ok(py.None().into_ref(py)),
+            ocsp_resp::ResponderId::ByKey(key_hash) => {
+                Ok(pyo3::types::PyBytes::new(py, key_hash).as_ref())
+            }
+            ocsp_resp::ResponderId::ByName(_) => Ok(py.None().into_ref(py)),
         }
     }
 
     #[getter]
     fn produced_at<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        x509::chrono_to_py(py, resp.tbs_response_data.produced_at.as_chrono())
+        x509::datetime_to_py(py, resp.tbs_response_data.produced_at.as_datetime())
     }
 
     #[getter]
     fn signature_algorithm_oid<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        oid_to_py_oid(py, &resp.signature_algorithm.oid)
+        oid_to_py_oid(py, resp.signature_algorithm.oid())
     }
 
     #[getter]
     fn signature_hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> Result<&'p pyo3::PyAny, CryptographyError> {
         let sig_oids_to_hash = py
-            .import("cryptography.hazmat._oid")?
-            .getattr(crate::intern!(py, "_SIG_OIDS_TO_HASH"))?;
+            .import(pyo3::intern!(py, "cryptography.hazmat._oid"))?
+            .getattr(pyo3::intern!(py, "_SIG_OIDS_TO_HASH"))?;
         let hash_alg = sig_oids_to_hash.get_item(self.signature_algorithm_oid(py)?);
         match hash_alg {
             Ok(data) => Ok(data),
             Err(_) => {
                 let exc_messsage = format!(
                     "Signature algorithm OID: {} not recognized",
-                    self.requires_successful_response()?.signature_algorithm.oid
+                    self.requires_successful_response()?
+                        .signature_algorithm
+                        .oid()
                 );
-                Err(CryptographyError::from(pyo3::PyErr::from_instance(
-                    py.import("cryptography.exceptions")?
-                        .call_method1("UnsupportedAlgorithm", (exc_messsage,))?,
-                )))
+                Err(CryptographyError::from(
+                    exceptions::UnsupportedAlgorithm::new_err(exc_messsage),
+                ))
             }
         }
     }
 
     #[getter]
     fn signature<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::types::PyBytes> {
         let resp = self.requires_successful_response()?;
@@ -213,15 +218,15 @@
         let py_certs = pyo3::types::PyList::empty(py);
         let certs = match &resp.certs {
             Some(certs) => certs.unwrap_read(),
             None => return Ok(py_certs),
         };
         for i in 0..certs.len() {
             // TODO: O(n^2), don't have too many certificates!
-            let raw_cert = map_arc_data_ocsp_response(&self.raw, |_data, resp| {
+            let raw_cert = map_arc_data_ocsp_response(py, &self.raw, |_data, resp| {
                 resp.response_bytes
                     .as_ref()
                     .unwrap()
                     .response
                     .get()
                     .certs
                     .as_ref()
@@ -229,625 +234,576 @@
                     .unwrap_read()
                     .clone()
                     .nth(i)
                     .unwrap()
             });
             py_certs.append(pyo3::PyCell::new(
                 py,
-                x509::Certificate {
+                x509::certificate::Certificate {
                     raw: raw_cert,
                     cached_extensions: None,
                 },
             )?)?;
         }
         Ok(py_certs)
     }
 
     #[getter]
     fn serial_number<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
-        single_resp.py_serial_number(py)
+        let single_resp = single_response(resp)?;
+        singleresp_py_serial_number(&single_resp, py)
     }
 
     #[getter]
     fn issuer_key_hash(&self) -> Result<&[u8], CryptographyError> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
+        let single_resp = single_response(resp)?;
         Ok(single_resp.cert_id.issuer_key_hash)
     }
 
     #[getter]
     fn issuer_name_hash(&self) -> Result<&[u8], CryptographyError> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
+        let single_resp = single_response(resp)?;
         Ok(single_resp.cert_id.issuer_name_hash)
     }
 
     #[getter]
     fn hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> Result<&'p pyo3::PyAny, CryptographyError> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
-        single_resp.py_hash_algorithm(py)
+        let single_resp = single_response(resp)?;
+        singleresp_py_hash_algorithm(&single_resp, py)
     }
 
     #[getter]
     fn certificate_status<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        resp.single_response()?.py_certificate_status(py)
+        let single_resp = single_response(resp)?;
+        singleresp_py_certificate_status(&single_resp, py)
     }
 
     #[getter]
     fn revocation_time<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
-        single_resp.py_revocation_time(py)
+        let single_resp = single_response(resp)?;
+        singleresp_py_revocation_time(&single_resp, py)
     }
 
     #[getter]
     fn revocation_reason<'p>(&self, py: pyo3::Python<'p>) -> CryptographyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
-        single_resp.py_revocation_reason(py)
+        let single_resp = single_response(resp)?;
+        singleresp_py_revocation_reason(&single_resp, py)
     }
 
     #[getter]
     fn this_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
-        single_resp.py_this_update(py)
+        let single_resp = single_response(resp)?;
+        singleresp_py_this_update(&single_resp, py)
     }
 
     #[getter]
     fn next_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let resp = self.requires_successful_response()?;
-        let single_resp = resp.single_response()?;
-        single_resp.py_next_update(py)
+        let single_resp = single_response(resp)?;
+        singleresp_py_next_update(&single_resp, py)
     }
 
     #[getter]
     fn extensions(&mut self, py: pyo3::Python<'_>) -> pyo3::PyResult<pyo3::PyObject> {
         self.requires_successful_response()?;
-        let x509_module = py.import("cryptography.x509")?;
+
+        let response_data = &self
+            .raw
+            .borrow_value()
+            .response_bytes
+            .as_ref()
+            .unwrap()
+            .response
+            .get()
+            .tbs_response_data;
+
+        let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
         x509::parse_and_cache_extensions(
             py,
             &mut self.cached_extensions,
-            &self
-                .raw
-                .borrow_value()
-                .response_bytes
-                .as_ref()
-                .unwrap()
-                .response
-                .get()
-                .tbs_response_data
-                .response_extensions,
+            &response_data.raw_response_extensions,
             |oid, ext_data| {
                 match oid {
                     &oid::NONCE_OID => {
                         // This is a disaster. RFC 2560 says that the contents of the nonce is
                         // just the raw extension value. This is nonsense, since they're always
                         // supposed to be ASN.1 TLVs. RFC 6960 correctly specifies that the
                         // nonce is an OCTET STRING, and so you should unwrap the TLV to get
                         // the nonce. So we try parsing as a TLV and fall back to just using
                         // the raw value.
                         let nonce = asn1::parse_single::<&[u8]>(ext_data).unwrap_or(ext_data);
-                        Ok(Some(x509_module.call_method1("OCSPNonce", (nonce,))?))
+                        Ok(Some(
+                            x509_module.call_method1(pyo3::intern!(py, "OCSPNonce"), (nonce,))?,
+                        ))
                     }
                     _ => Ok(None),
                 }
             },
         )
     }
 
     #[getter]
     fn single_extensions(&mut self, py: pyo3::Python<'_>) -> pyo3::PyResult<pyo3::PyObject> {
         self.requires_successful_response()?;
-        let single_resp = self
-            .raw
-            .borrow_value()
-            .response_bytes
-            .as_ref()
-            .unwrap()
-            .response
-            .get()
-            .single_response()?;
-        let x509_module = py.import("cryptography.x509")?;
+        let single_resp = single_response(
+            self.raw
+                .borrow_value()
+                .response_bytes
+                .as_ref()
+                .unwrap()
+                .response
+                .get(),
+        )?;
+
+        let x509_module = py.import(pyo3::intern!(py, "cryptography.x509"))?;
         x509::parse_and_cache_extensions(
             py,
             &mut self.cached_single_extensions,
-            &single_resp.single_extensions,
+            &single_resp.raw_single_extensions,
             |oid, ext_data| match oid {
                 &oid::SIGNED_CERTIFICATE_TIMESTAMPS_OID => {
                     let contents = asn1::parse_single::<&[u8]>(ext_data)?;
                     let scts = sct::parse_scts(py, contents, sct::LogEntryType::Certificate)?;
                     Ok(Some(
                         x509_module
-                            .getattr(crate::intern!(py, "SignedCertificateTimestamps"))?
+                            .getattr(pyo3::intern!(py, "SignedCertificateTimestamps"))?
                             .call1((scts,))?,
                     ))
                 }
                 _ => crl::parse_crl_entry_ext(py, oid.clone(), ext_data),
             },
         )
     }
 
     fn public_bytes<'p>(
         &self,
         py: pyo3::Python<'p>,
         encoding: &pyo3::PyAny,
     ) -> CryptographyResult<&'p pyo3::types::PyBytes> {
         let der = py
-            .import("cryptography.hazmat.primitives.serialization")?
-            .getattr(crate::intern!(py, "Encoding"))?
-            .getattr(crate::intern!(py, "DER"))?;
-        if encoding != der {
+            .import(pyo3::intern!(
+                py,
+                "cryptography.hazmat.primitives.serialization"
+            ))?
+            .getattr(pyo3::intern!(py, "Encoding"))?
+            .getattr(pyo3::intern!(py, "DER"))?;
+        if !encoding.is(der) {
             return Err(pyo3::exceptions::PyValueError::new_err(
                 "The only allowed encoding value is Encoding.DER",
             )
             .into());
         }
         let result = asn1::write_single(self.raw.borrow_value())?;
         Ok(pyo3::types::PyBytes::new(py, &result))
     }
 }
 
 // Open-coded implementation of the API discussed in
 // https://github.com/joshua-maros/ouroboros/issues/38
 fn map_arc_data_ocsp_response(
-    it: &OwnedRawOCSPResponse,
+    py: pyo3::Python<'_>,
+    it: &OwnedOCSPResponse,
     f: impl for<'this> FnOnce(
         &'this [u8],
-        &RawOCSPResponse<'this>,
-    ) -> certificate::RawCertificate<'this>,
-) -> certificate::OwnedRawCertificate {
-    certificate::OwnedRawCertificate::new_public(Arc::clone(it.borrow_data()), |inner_it| {
-        it.with(|value| f(inner_it, unsafe { std::mem::transmute(value.value) }))
+        &ocsp_resp::OCSPResponse<'this>,
+    ) -> cryptography_x509::certificate::Certificate<'this>,
+) -> certificate::OwnedCertificate {
+    certificate::OwnedCertificate::new_public(it.borrow_data().clone_ref(py), |inner_it| {
+        it.with(|value| {
+            f(inner_it.as_bytes(py), unsafe {
+                std::mem::transmute(value.value)
+            })
+        })
     })
 }
 fn try_map_arc_data_mut_ocsp_response_iterator<E>(
     it: &mut OwnedOCSPResponseIteratorData,
     f: impl for<'this> FnOnce(
-        &'this OwnedRawOCSPResponse,
-        &mut asn1::SequenceOf<'this, SingleResponse<'this>>,
-    ) -> Result<SingleResponse<'this>, E>,
+        &'this OwnedOCSPResponse,
+        &mut asn1::SequenceOf<'this, ocsp_resp::SingleResponse<'this>>,
+    ) -> Result<ocsp_resp::SingleResponse<'this>, E>,
 ) -> Result<OwnedSingleResponse, E> {
     OwnedSingleResponse::try_new(Arc::clone(it.borrow_data()), |inner_it| {
         it.with_value_mut(|value| f(inner_it, unsafe { std::mem::transmute(value) }))
     })
 }
 
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct RawOCSPResponse<'a> {
-    response_status: asn1::Enumerated,
-    #[explicit(0)]
-    response_bytes: Option<ResponseBytes<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct ResponseBytes<'a> {
-    response_type: asn1::ObjectIdentifier,
-    response: asn1::OctetStringEncoded<BasicOCSPResponse<'a>>,
-}
-
-type OCSPCerts<'a> = Option<
-    x509::Asn1ReadableOrWritable<
-        'a,
-        asn1::SequenceOf<'a, certificate::RawCertificate<'a>>,
-        asn1::SequenceOfWriter<
-            'a,
-            certificate::RawCertificate<'a>,
-            Vec<certificate::RawCertificate<'a>>,
-        >,
-    >,
->;
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct BasicOCSPResponse<'a> {
-    tbs_response_data: ResponseData<'a>,
-    signature_algorithm: x509::AlgorithmIdentifier<'a>,
-    signature: asn1::BitString<'a>,
-    #[explicit(0)]
-    certs: OCSPCerts<'a>,
-}
-
-impl BasicOCSPResponse<'_> {
-    fn single_response(&self) -> Result<SingleResponse<'_>, CryptographyError> {
-        let responses = self.tbs_response_data.responses.unwrap_read();
-        let num_responses = responses.len();
+fn single_response<'a>(
+    resp: &ocsp_resp::BasicOCSPResponse<'a>,
+) -> Result<ocsp_resp::SingleResponse<'a>, CryptographyError> {
+    let responses = resp.tbs_response_data.responses.unwrap_read();
+    let num_responses = responses.len();
+
+    if num_responses != 1 {
+        return Err(CryptographyError::from(
+            pyo3::exceptions::PyValueError::new_err(format!(
+                "OCSP response contains {} SINGLERESP structures.  Use .response_iter to iterate through them",
+                num_responses
+            ))
+        ));
+    }
 
-        if num_responses != 1 {
-            return Err(CryptographyError::from(
-                pyo3::exceptions::PyValueError::new_err(format!(
-                    "OCSP response contains {} SINGLERESP structures.  Use .response_iter to iterate through them",
-                    num_responses
-                ))
-            ));
-        }
+    Ok(responses.clone().next().unwrap())
+}
 
-        Ok(responses.clone().next().unwrap())
-    }
+fn singleresp_py_serial_number<'p>(
+    resp: &ocsp_resp::SingleResponse<'_>,
+    py: pyo3::Python<'p>,
+) -> pyo3::PyResult<&'p pyo3::PyAny> {
+    big_byte_slice_to_py_int(py, resp.cert_id.serial_number.as_bytes())
 }
 
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct ResponseData<'a> {
-    #[explicit(0)]
-    #[default(0)]
-    version: u8,
-    responder_id: ResponderId<'a>,
-    produced_at: asn1::GeneralizedTime,
-    responses: x509::Asn1ReadableOrWritable<
-        'a,
-        asn1::SequenceOf<'a, SingleResponse<'a>>,
-        asn1::SequenceOfWriter<'a, SingleResponse<'a>, Vec<SingleResponse<'a>>>,
-    >,
-    #[explicit(1)]
-    response_extensions: Option<x509::Extensions<'a>>,
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-enum ResponderId<'a> {
-    #[explicit(1)]
-    ByName(x509::Name<'a>),
-    #[explicit(2)]
-    ByKey(&'a [u8]),
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct SingleResponse<'a> {
-    cert_id: ocsp::CertID<'a>,
-    cert_status: CertStatus,
-    this_update: asn1::GeneralizedTime,
-    #[explicit(0)]
-    next_update: Option<asn1::GeneralizedTime>,
-    #[explicit(1)]
-    single_extensions: Option<x509::Extensions<'a>>,
-}
-
-impl SingleResponse<'_> {
-    fn py_serial_number<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        big_byte_slice_to_py_int(py, self.cert_id.serial_number.as_bytes())
-    }
-
-    fn py_certificate_status<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        let attr = match self.cert_status {
-            CertStatus::Good(_) => "GOOD",
-            CertStatus::Revoked(_) => "REVOKED",
-            CertStatus::Unknown(_) => "UNKNOWN",
-        };
-        py.import("cryptography.x509.ocsp")?
-            .getattr(crate::intern!(py, "OCSPCertStatus"))?
-            .getattr(attr)
+fn singleresp_py_certificate_status<'p>(
+    resp: &ocsp_resp::SingleResponse<'_>,
+    py: pyo3::Python<'p>,
+) -> pyo3::PyResult<&'p pyo3::PyAny> {
+    let attr = match resp.cert_status {
+        ocsp_resp::CertStatus::Good(_) => pyo3::intern!(py, "GOOD"),
+        ocsp_resp::CertStatus::Revoked(_) => pyo3::intern!(py, "REVOKED"),
+        ocsp_resp::CertStatus::Unknown(_) => pyo3::intern!(py, "UNKNOWN"),
+    };
+    py.import(pyo3::intern!(py, "cryptography.x509.ocsp"))?
+        .getattr(pyo3::intern!(py, "OCSPCertStatus"))?
+        .getattr(attr)
+}
+
+fn singleresp_py_hash_algorithm<'p>(
+    resp: &ocsp_resp::SingleResponse<'_>,
+    py: pyo3::Python<'p>,
+) -> Result<&'p pyo3::PyAny, CryptographyError> {
+    let hashes = py.import(pyo3::intern!(py, "cryptography.hazmat.primitives.hashes"))?;
+    match ocsp::ALGORITHM_PARAMETERS_TO_HASH.get(&resp.cert_id.hash_algorithm.params) {
+        Some(alg_name) => Ok(hashes.getattr(*alg_name)?.call0()?),
+        None => Err(CryptographyError::from(
+            exceptions::UnsupportedAlgorithm::new_err(format!(
+                "Signature algorithm OID: {} not recognized",
+                resp.cert_id.hash_algorithm.oid()
+            )),
+        )),
     }
+}
 
-    fn py_hash_algorithm<'p>(
-        &self,
-        py: pyo3::Python<'p>,
-    ) -> Result<&'p pyo3::PyAny, CryptographyError> {
-        let hashes = py.import("cryptography.hazmat.primitives.hashes")?;
-        match ocsp::OIDS_TO_HASH.get(&self.cert_id.hash_algorithm.oid) {
-            Some(alg_name) => Ok(hashes.getattr(alg_name)?.call0()?),
-            None => {
-                let exceptions = py.import("cryptography.exceptions")?;
-                Err(CryptographyError::from(pyo3::PyErr::from_instance(
-                    exceptions
-                        .getattr(crate::intern!(py, "UnsupportedAlgorithm"))?
-                        .call1((format!(
-                            "Signature algorithm OID: {} not recognized",
-                            self.cert_id.hash_algorithm.oid
-                        ),))?,
-                )))
-            }
-        }
-    }
+fn singleresp_py_this_update<'p>(
+    resp: &ocsp_resp::SingleResponse<'_>,
+    py: pyo3::Python<'p>,
+) -> pyo3::PyResult<&'p pyo3::PyAny> {
+    x509::datetime_to_py(py, resp.this_update.as_datetime())
+}
 
-    fn py_this_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        x509::chrono_to_py(py, self.this_update.as_chrono())
+fn singleresp_py_next_update<'p>(
+    resp: &ocsp_resp::SingleResponse<'_>,
+    py: pyo3::Python<'p>,
+) -> pyo3::PyResult<&'p pyo3::PyAny> {
+    match &resp.next_update {
+        Some(v) => x509::datetime_to_py(py, v.as_datetime()),
+        None => Ok(py.None().into_ref(py)),
     }
+}
 
-    fn py_next_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        match &self.next_update {
-            Some(v) => x509::chrono_to_py(py, v.as_chrono()),
+fn singleresp_py_revocation_reason<'p>(
+    resp: &ocsp_resp::SingleResponse<'_>,
+    py: pyo3::Python<'p>,
+) -> CryptographyResult<&'p pyo3::PyAny> {
+    match &resp.cert_status {
+        ocsp_resp::CertStatus::Revoked(revoked_info) => match revoked_info.revocation_reason {
+            Some(ref v) => crl::parse_crl_reason_flags(py, v),
             None => Ok(py.None().into_ref(py)),
+        },
+        ocsp_resp::CertStatus::Good(_) | ocsp_resp::CertStatus::Unknown(_) => {
+            Ok(py.None().into_ref(py))
         }
     }
+}
 
-    fn py_revocation_reason<'p>(
-        &self,
-        py: pyo3::Python<'p>,
-    ) -> CryptographyResult<&'p pyo3::PyAny> {
-        match &self.cert_status {
-            CertStatus::Revoked(revoked_info) => match revoked_info.revocation_reason {
-                Some(ref v) => crl::parse_crl_reason_flags(py, v),
-                None => Ok(py.None().into_ref(py)),
-            },
-            CertStatus::Good(_) | CertStatus::Unknown(_) => Ok(py.None().into_ref(py)),
+fn singleresp_py_revocation_time<'p>(
+    resp: &ocsp_resp::SingleResponse<'_>,
+    py: pyo3::Python<'p>,
+) -> pyo3::PyResult<&'p pyo3::PyAny> {
+    match &resp.cert_status {
+        ocsp_resp::CertStatus::Revoked(revoked_info) => {
+            x509::datetime_to_py(py, revoked_info.revocation_time.as_datetime())
         }
-    }
-
-    fn py_revocation_time<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        match &self.cert_status {
-            CertStatus::Revoked(revoked_info) => {
-                x509::chrono_to_py(py, revoked_info.revocation_time.as_chrono())
-            }
-            CertStatus::Good(_) | CertStatus::Unknown(_) => Ok(py.None().into_ref(py)),
+        ocsp_resp::CertStatus::Good(_) | ocsp_resp::CertStatus::Unknown(_) => {
+            Ok(py.None().into_ref(py))
         }
     }
 }
 
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-enum CertStatus {
-    #[implicit(0)]
-    Good(()),
-    #[implicit(1)]
-    Revoked(RevokedInfo),
-    #[implicit(2)]
-    Unknown(()),
-}
-
-#[derive(asn1::Asn1Read, asn1::Asn1Write)]
-struct RevokedInfo {
-    revocation_time: asn1::GeneralizedTime,
-    #[explicit(0)]
-    revocation_reason: Option<crl::CRLReason>,
-}
-
 #[pyo3::prelude::pyfunction]
 fn create_ocsp_response(
     py: pyo3::Python<'_>,
     status: &pyo3::PyAny,
     builder: &pyo3::PyAny,
     private_key: &pyo3::PyAny,
     hash_algorithm: &pyo3::PyAny,
 ) -> CryptographyResult<OCSPResponse> {
     let response_status = status
-        .getattr(crate::intern!(py, "value"))?
+        .getattr(pyo3::intern!(py, "value"))?
         .extract::<u32>()?;
 
-    let py_cert: pyo3::PyRef<'_, x509::Certificate>;
-    let py_issuer: pyo3::PyRef<'_, x509::Certificate>;
+    let py_cert: pyo3::PyRef<'_, x509::certificate::Certificate>;
+    let py_issuer: pyo3::PyRef<'_, x509::certificate::Certificate>;
     let borrowed_cert;
-    let py_certs: Option<Vec<pyo3::PyRef<'_, x509::Certificate>>>;
+    let py_certs: Option<Vec<pyo3::PyRef<'_, x509::certificate::Certificate>>>;
     let response_bytes = if response_status == SUCCESSFUL_RESPONSE {
-        let ocsp_mod = py.import("cryptography.x509.ocsp")?;
+        let ocsp_mod = py.import(pyo3::intern!(py, "cryptography.x509.ocsp"))?;
 
-        let py_single_resp = builder.getattr(crate::intern!(py, "_response"))?;
+        let py_single_resp = builder.getattr(pyo3::intern!(py, "_response"))?;
         py_cert = py_single_resp
-            .getattr(crate::intern!(py, "_cert"))?
+            .getattr(pyo3::intern!(py, "_cert"))?
             .extract()?;
         py_issuer = py_single_resp
-            .getattr(crate::intern!(py, "_issuer"))?
+            .getattr(pyo3::intern!(py, "_issuer"))?
+            .extract()?;
+        let py_cert_hash_algorithm = py_single_resp.getattr(pyo3::intern!(py, "_algorithm"))?;
+        let (responder_cert, responder_encoding): (
+            &pyo3::PyCell<x509::certificate::Certificate>,
+            &pyo3::PyAny,
+        ) = builder
+            .getattr(pyo3::intern!(py, "_responder_id"))?
             .extract()?;
-        let py_cert_hash_algorithm = py_single_resp.getattr(crate::intern!(py, "_algorithm"))?;
-        let (responder_cert, responder_encoding): (&pyo3::PyCell<x509::Certificate>, &pyo3::PyAny) =
-            builder
-                .getattr(crate::intern!(py, "_responder_id"))?
-                .extract()?;
-
-        let py_cert_status = py_single_resp.getattr(crate::intern!(py, "_cert_status"))?;
-        let cert_status = if py_cert_status
-            == ocsp_mod
-                .getattr(crate::intern!(py, "OCSPCertStatus"))?
-                .getattr(crate::intern!(py, "GOOD"))?
+
+        let py_cert_status = py_single_resp.getattr(pyo3::intern!(py, "_cert_status"))?;
+        let cert_status = if py_cert_status.is(ocsp_mod
+            .getattr(pyo3::intern!(py, "OCSPCertStatus"))?
+            .getattr(pyo3::intern!(py, "GOOD"))?)
         {
-            CertStatus::Good(())
-        } else if py_cert_status
-            == ocsp_mod
-                .getattr(crate::intern!(py, "OCSPCertStatus"))?
-                .getattr(crate::intern!(py, "UNKNOWN"))?
+            ocsp_resp::CertStatus::Good(())
+        } else if py_cert_status.is(ocsp_mod
+            .getattr(pyo3::intern!(py, "OCSPCertStatus"))?
+            .getattr(pyo3::intern!(py, "UNKNOWN"))?)
         {
-            CertStatus::Unknown(())
+            ocsp_resp::CertStatus::Unknown(())
         } else {
             let revocation_reason = if !py_single_resp
-                .getattr(crate::intern!(py, "_revocation_reason"))?
+                .getattr(pyo3::intern!(py, "_revocation_reason"))?
                 .is_none()
             {
                 let value = py
-                    .import("cryptography.hazmat.backends.openssl.decode_asn1")?
-                    .getattr(crate::intern!(py, "_CRL_ENTRY_REASON_ENUM_TO_CODE"))?
-                    .get_item(py_single_resp.getattr(crate::intern!(py, "_revocation_reason"))?)?
+                    .import(pyo3::intern!(
+                        py,
+                        "cryptography.hazmat.backends.openssl.decode_asn1"
+                    ))?
+                    .getattr(pyo3::intern!(py, "_CRL_ENTRY_REASON_ENUM_TO_CODE"))?
+                    .get_item(py_single_resp.getattr(pyo3::intern!(py, "_revocation_reason"))?)?
                     .extract::<u32>()?;
                 Some(asn1::Enumerated::new(value))
             } else {
                 None
             };
             // REVOKED
             let py_revocation_time =
-                py_single_resp.getattr(crate::intern!(py, "_revocation_time"))?;
+                py_single_resp.getattr(pyo3::intern!(py, "_revocation_time"))?;
             let revocation_time =
-                asn1::GeneralizedTime::new(py_to_chrono(py, py_revocation_time)?)?;
-            CertStatus::Revoked(RevokedInfo {
+                asn1::GeneralizedTime::new(py_to_datetime(py, py_revocation_time)?)?;
+            ocsp_resp::CertStatus::Revoked(ocsp_resp::RevokedInfo {
                 revocation_time,
                 revocation_reason,
             })
         };
         let next_update = if !py_single_resp
-            .getattr(crate::intern!(py, "_next_update"))?
+            .getattr(pyo3::intern!(py, "_next_update"))?
             .is_none()
         {
-            let py_next_update = py_single_resp.getattr(crate::intern!(py, "_next_update"))?;
-            Some(asn1::GeneralizedTime::new(py_to_chrono(
+            let py_next_update = py_single_resp.getattr(pyo3::intern!(py, "_next_update"))?;
+            Some(asn1::GeneralizedTime::new(py_to_datetime(
                 py,
                 py_next_update,
             )?)?)
         } else {
             None
         };
-        let py_this_update = py_single_resp.getattr(crate::intern!(py, "_this_update"))?;
-        let this_update = asn1::GeneralizedTime::new(py_to_chrono(py, py_this_update)?)?;
+        let py_this_update = py_single_resp.getattr(pyo3::intern!(py, "_this_update"))?;
+        let this_update = asn1::GeneralizedTime::new(py_to_datetime(py, py_this_update)?)?;
 
         let responses = vec![SingleResponse {
-            cert_id: ocsp::CertID::new(py, &py_cert, &py_issuer, py_cert_hash_algorithm)?,
+            cert_id: ocsp::certid_new(py, &py_cert, &py_issuer, py_cert_hash_algorithm)?,
             cert_status,
             next_update,
             this_update,
-            single_extensions: None,
+            raw_single_extensions: None,
         }];
 
         borrowed_cert = responder_cert.borrow();
-        let responder_id = if responder_encoding
-            == ocsp_mod
-                .getattr(crate::intern!(py, "OCSPResponderEncoding"))?
-                .getattr(crate::intern!(py, "HASH"))?
+        let responder_id = if responder_encoding.is(ocsp_mod
+            .getattr(pyo3::intern!(py, "OCSPResponderEncoding"))?
+            .getattr(pyo3::intern!(py, "HASH"))?)
         {
             let sha1 = py
-                .import("cryptography.hazmat.primitives.hashes")?
-                .getattr(crate::intern!(py, "SHA1"))?
+                .import(pyo3::intern!(py, "cryptography.hazmat.primitives.hashes"))?
+                .getattr(pyo3::intern!(py, "SHA1"))?
                 .call0()?;
-            ResponderId::ByKey(ocsp::hash_data(
+            ocsp_resp::ResponderId::ByKey(ocsp::hash_data(
                 py,
                 sha1,
                 borrowed_cert
                     .raw
                     .borrow_value_public()
                     .tbs_cert
                     .spki
                     .subject_public_key
                     .as_bytes(),
             )?)
         } else {
-            ResponderId::ByName(
+            ocsp_resp::ResponderId::ByName(
                 borrowed_cert
                     .raw
                     .borrow_value_public()
                     .tbs_cert
                     .subject
                     .clone(),
             )
         };
 
-        let tbs_response_data = ResponseData {
+        let tbs_response_data = ocsp_resp::ResponseData {
             version: 0,
-            produced_at: asn1::GeneralizedTime::new(
-                chrono::Utc::now().with_nanosecond(0).unwrap(),
-            )?,
+            produced_at: asn1::GeneralizedTime::new(x509::common::datetime_now(py)?)?,
             responder_id,
-            responses: x509::Asn1ReadableOrWritable::new_write(asn1::SequenceOfWriter::new(
+            responses: common::Asn1ReadableOrWritable::new_write(asn1::SequenceOfWriter::new(
                 responses,
             )),
-            response_extensions: x509::common::encode_extensions(
+            raw_response_extensions: x509::common::encode_extensions(
                 py,
-                builder.getattr(crate::intern!(py, "_extensions"))?,
+                builder.getattr(pyo3::intern!(py, "_extensions"))?,
                 extensions::encode_extension,
             )?,
         };
 
-        let sigalg = x509::sign::compute_signature_algorithm(py, private_key, hash_algorithm)?;
+        let sigalg = x509::sign::compute_signature_algorithm(
+            py,
+            private_key,
+            hash_algorithm,
+            py.None().into_ref(py),
+        )?;
         let tbs_bytes = asn1::write_single(&tbs_response_data)?;
-        let signature = x509::sign::sign_data(py, private_key, hash_algorithm, &tbs_bytes)?;
-
-        py.import("cryptography.hazmat.backends.openssl.backend")?
-            .getattr(crate::intern!(py, "backend"))?
-            .call_method1(
-                "_check_keys_correspond",
-                (
-                    responder_cert.call_method0("public_key")?,
-                    private_key.call_method0("public_key")?,
+        let signature = x509::sign::sign_data(
+            py,
+            private_key,
+            hash_algorithm,
+            py.None().into_ref(py),
+            &tbs_bytes,
+        )?;
+
+        if !responder_cert
+            .call_method0(pyo3::intern!(py, "public_key"))?
+            .eq(private_key.call_method0(pyo3::intern!(py, "public_key"))?)?
+        {
+            return Err(CryptographyError::from(
+                pyo3::exceptions::PyValueError::new_err(
+                    "Certificate public key and provided private key do not match",
                 ),
-            )?;
+            ));
+        }
 
-        py_certs = builder.getattr(crate::intern!(py, "_certs"))?.extract()?;
+        py_certs = builder.getattr(pyo3::intern!(py, "_certs"))?.extract()?;
         let certs = py_certs.as_ref().map(|py_certs| {
-            x509::Asn1ReadableOrWritable::new_write(asn1::SequenceOfWriter::new(
+            common::Asn1ReadableOrWritable::new_write(asn1::SequenceOfWriter::new(
                 py_certs
                     .iter()
                     .map(|c| c.raw.borrow_value_public().clone())
                     .collect(),
             ))
         });
 
-        let basic_resp = BasicOCSPResponse {
+        let basic_resp = ocsp_resp::BasicOCSPResponse {
             tbs_response_data,
             signature: asn1::BitString::new(signature, 0).unwrap(),
             signature_algorithm: sigalg,
             certs,
         };
-        Some(ResponseBytes {
+        Some(ocsp_resp::ResponseBytes {
             response_type: (BASIC_RESPONSE_OID).clone(),
             response: asn1::OctetStringEncoded::new(basic_resp),
         })
     } else {
         None
     };
 
-    let resp = RawOCSPResponse {
+    let resp = ocsp_resp::OCSPResponse {
         response_status: asn1::Enumerated::new(response_status),
         response_bytes,
     };
     let data = asn1::write_single(&resp)?;
-    // TODO: extra copy as we round-trip through a slice
-    load_der_ocsp_response(py, &data)
+    load_der_ocsp_response(py, pyo3::types::PyBytes::new(py, &data).into_py(py))
 }
 
 pub(crate) fn add_to_module(module: &pyo3::prelude::PyModule) -> pyo3::PyResult<()> {
-    module.add_wrapped(pyo3::wrap_pyfunction!(load_der_ocsp_response))?;
-    module.add_wrapped(pyo3::wrap_pyfunction!(create_ocsp_response))?;
+    module.add_function(pyo3::wrap_pyfunction!(load_der_ocsp_response, module)?)?;
+    module.add_function(pyo3::wrap_pyfunction!(create_ocsp_response, module)?)?;
 
     Ok(())
 }
 
 #[ouroboros::self_referencing]
 struct OwnedOCSPResponseIteratorData {
-    data: Arc<OwnedRawOCSPResponse>,
+    data: Arc<OwnedOCSPResponse>,
     #[borrows(data)]
     #[covariant]
     value: asn1::SequenceOf<'this, SingleResponse<'this>>,
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.ocsp")]
 struct OCSPResponseIterator {
     contents: OwnedOCSPResponseIteratorData,
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyIterProtocol<'_> for OCSPResponseIterator {
-    fn __iter__(slf: pyo3::PyRef<'p, Self>) -> pyo3::PyRef<'p, Self> {
+#[pyo3::prelude::pymethods]
+impl OCSPResponseIterator {
+    fn __iter__(slf: pyo3::PyRef<'_, Self>) -> pyo3::PyRef<'_, Self> {
         slf
     }
 
-    fn __next__(mut slf: pyo3::PyRefMut<'p, Self>) -> Option<OCSPSingleResponse> {
+    fn __next__(&mut self) -> Option<OCSPSingleResponse> {
         let single_resp =
-            try_map_arc_data_mut_ocsp_response_iterator(&mut slf.contents, |_data, v| {
+            try_map_arc_data_mut_ocsp_response_iterator(&mut self.contents, |_data, v| {
                 match v.next() {
                     Some(single_resp) => Ok(single_resp),
                     None => Err(()),
                 }
             })
             .ok()?;
         Some(OCSPSingleResponse { raw: single_resp })
     }
 }
 
 #[ouroboros::self_referencing]
 struct OwnedSingleResponse {
-    data: Arc<OwnedRawOCSPResponse>,
+    data: Arc<OwnedOCSPResponse>,
     #[borrows(data)]
     #[covariant]
-    value: SingleResponse<'this>,
+    value: ocsp_resp::SingleResponse<'this>,
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.ocsp")]
 struct OCSPSingleResponse {
     raw: OwnedSingleResponse,
 }
 
 impl OCSPSingleResponse {
     fn single_response(&self) -> &SingleResponse<'_> {
         self.raw.borrow_value()
     }
 }
 
 #[pyo3::prelude::pymethods]
 impl OCSPSingleResponse {
     #[getter]
     fn serial_number<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        self.single_response().py_serial_number(py)
+        singleresp_py_serial_number(self.single_response(), py)
     }
 
     #[getter]
     fn issuer_key_hash(&self) -> &[u8] {
         let single_resp = self.single_response();
         single_resp.cert_id.issuer_key_hash
     }
@@ -859,35 +815,41 @@
     }
 
     #[getter]
     fn hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> Result<&'p pyo3::PyAny, CryptographyError> {
-        self.single_response().py_hash_algorithm(py)
+        let single_resp = self.single_response();
+        singleresp_py_hash_algorithm(single_resp, py)
     }
 
     #[getter]
     fn certificate_status<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        self.single_response().py_certificate_status(py)
+        let single_resp = self.single_response();
+        singleresp_py_certificate_status(single_resp, py)
     }
 
     #[getter]
     fn revocation_time<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        self.single_response().py_revocation_time(py)
+        let single_resp = self.single_response();
+        singleresp_py_revocation_time(single_resp, py)
     }
 
     #[getter]
     fn revocation_reason<'p>(&self, py: pyo3::Python<'p>) -> CryptographyResult<&'p pyo3::PyAny> {
-        self.single_response().py_revocation_reason(py)
+        let single_resp = self.single_response();
+        singleresp_py_revocation_reason(single_resp, py)
     }
 
     #[getter]
     fn this_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        self.single_response().py_this_update(py)
+        let single_resp = self.single_response();
+        singleresp_py_this_update(single_resp, py)
     }
 
     #[getter]
     fn next_update<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        self.single_response().py_next_update(py)
+        let single_resp = self.single_response();
+        singleresp_py_next_update(single_resp, py)
     }
 }
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/oid.rs` & `cryptography-41.0.0/src/rust/cryptography-x509/src/oid.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
-pub(crate) const EXTENSION_REQUEST: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 113549, 1, 9, 14);
-pub(crate) const MS_EXTENSION_REQUEST: asn1::ObjectIdentifier =
+pub const EXTENSION_REQUEST: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 9, 14);
+pub const MS_EXTENSION_REQUEST: asn1::ObjectIdentifier =
     asn1::oid!(1, 3, 6, 1, 4, 1, 311, 2, 1, 14);
-pub(crate) const PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS_OID: asn1::ObjectIdentifier =
+pub const MS_CERTIFICATE_TEMPLATE: asn1::ObjectIdentifier =
+    asn1::oid!(1, 3, 6, 1, 4, 1, 311, 21, 7);
+pub const PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS_OID: asn1::ObjectIdentifier =
     asn1::oid!(1, 3, 6, 1, 4, 1, 11129, 2, 4, 2);
-pub(crate) const PRECERT_POISON_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 3, 6, 1, 4, 1, 11129, 2, 4, 3);
-pub(crate) const SIGNED_CERTIFICATE_TIMESTAMPS_OID: asn1::ObjectIdentifier =
+pub const PRECERT_POISON_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 4, 1, 11129, 2, 4, 3);
+pub const SIGNED_CERTIFICATE_TIMESTAMPS_OID: asn1::ObjectIdentifier =
     asn1::oid!(1, 3, 6, 1, 4, 1, 11129, 2, 4, 5);
-pub(crate) const AUTHORITY_INFORMATION_ACCESS_OID: asn1::ObjectIdentifier =
+pub const AUTHORITY_INFORMATION_ACCESS_OID: asn1::ObjectIdentifier =
     asn1::oid!(1, 3, 6, 1, 5, 5, 7, 1, 1);
-pub(crate) const SUBJECT_INFORMATION_ACCESS_OID: asn1::ObjectIdentifier =
+pub const SUBJECT_INFORMATION_ACCESS_OID: asn1::ObjectIdentifier =
     asn1::oid!(1, 3, 6, 1, 5, 5, 7, 1, 11);
-pub(crate) const TLS_FEATURE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 1, 24);
-pub(crate) const CP_CPS_URI_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 2, 1);
-pub(crate) const CP_USER_NOTICE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 2, 2);
-pub(crate) const NONCE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 48, 1, 2);
-pub(crate) const OCSP_NO_CHECK_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 3, 6, 1, 5, 5, 7, 48, 1, 5);
-pub(crate) const SUBJECT_KEY_IDENTIFIER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 14);
-pub(crate) const KEY_USAGE_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 15);
-pub(crate) const SUBJECT_ALTERNATIVE_NAME_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 17);
-pub(crate) const ISSUER_ALTERNATIVE_NAME_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 18);
-pub(crate) const BASIC_CONSTRAINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 19);
-pub(crate) const CRL_NUMBER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 20);
-pub(crate) const CRL_REASON_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 21);
-pub(crate) const INVALIDITY_DATE_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 24);
-pub(crate) const DELTA_CRL_INDICATOR_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 27);
-pub(crate) const ISSUING_DISTRIBUTION_POINT_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 28);
-pub(crate) const CERTIFICATE_ISSUER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 29);
-pub(crate) const NAME_CONSTRAINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 30);
-pub(crate) const CRL_DISTRIBUTION_POINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 31);
-pub(crate) const CERTIFICATE_POLICIES_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 32);
-pub(crate) const AUTHORITY_KEY_IDENTIFIER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 35);
-pub(crate) const POLICY_CONSTRAINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 36);
-pub(crate) const EXTENDED_KEY_USAGE_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 37);
-pub(crate) const FRESHEST_CRL_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 46);
-pub(crate) const INHIBIT_ANY_POLICY_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 54);
+pub const TLS_FEATURE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 1, 24);
+pub const CP_CPS_URI_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 2, 1);
+pub const CP_USER_NOTICE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 2, 2);
+pub const NONCE_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 48, 1, 2);
+pub const OCSP_NO_CHECK_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 6, 1, 5, 5, 7, 48, 1, 5);
+pub const SUBJECT_KEY_IDENTIFIER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 14);
+pub const KEY_USAGE_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 15);
+pub const SUBJECT_ALTERNATIVE_NAME_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 17);
+pub const ISSUER_ALTERNATIVE_NAME_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 18);
+pub const BASIC_CONSTRAINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 19);
+pub const CRL_NUMBER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 20);
+pub const CRL_REASON_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 21);
+pub const INVALIDITY_DATE_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 24);
+pub const DELTA_CRL_INDICATOR_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 27);
+pub const ISSUING_DISTRIBUTION_POINT_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 28);
+pub const CERTIFICATE_ISSUER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 29);
+pub const NAME_CONSTRAINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 30);
+pub const CRL_DISTRIBUTION_POINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 31);
+pub const CERTIFICATE_POLICIES_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 32);
+pub const AUTHORITY_KEY_IDENTIFIER_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 35);
+pub const POLICY_CONSTRAINTS_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 36);
+pub const EXTENDED_KEY_USAGE_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 37);
+pub const FRESHEST_CRL_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 46);
+pub const INHIBIT_ANY_POLICY_OID: asn1::ObjectIdentifier = asn1::oid!(2, 5, 29, 54);
+pub const ACCEPTABLE_RESPONSES_OID: asn1::ObjectIdentifier =
+    asn1::oid!(1, 3, 6, 1, 5, 5, 7, 48, 1, 4);
 
 // Signing methods
-pub(crate) const ECDSA_WITH_SHA224_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 10045, 4, 3, 1);
-pub(crate) const ECDSA_WITH_SHA256_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 10045, 4, 3, 2);
-pub(crate) const ECDSA_WITH_SHA384_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 10045, 4, 3, 3);
-pub(crate) const ECDSA_WITH_SHA512_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 10045, 4, 3, 4);
-pub(crate) const ECDSA_WITH_SHA3_224_OID: asn1::ObjectIdentifier =
+pub const ECDSA_WITH_SHA224_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 10045, 4, 3, 1);
+pub const ECDSA_WITH_SHA256_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 10045, 4, 3, 2);
+pub const ECDSA_WITH_SHA384_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 10045, 4, 3, 3);
+pub const ECDSA_WITH_SHA512_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 10045, 4, 3, 4);
+pub const ECDSA_WITH_SHA3_224_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 9);
-pub(crate) const ECDSA_WITH_SHA3_256_OID: asn1::ObjectIdentifier =
+pub const ECDSA_WITH_SHA3_256_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 10);
-pub(crate) const ECDSA_WITH_SHA3_384_OID: asn1::ObjectIdentifier =
+pub const ECDSA_WITH_SHA3_384_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 11);
-pub(crate) const ECDSA_WITH_SHA3_512_OID: asn1::ObjectIdentifier =
+pub const ECDSA_WITH_SHA3_512_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 12);
 
-pub(crate) const RSA_WITH_SHA224_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 113549, 1, 1, 14);
-pub(crate) const RSA_WITH_SHA256_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 113549, 1, 1, 11);
-pub(crate) const RSA_WITH_SHA384_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 113549, 1, 1, 12);
-pub(crate) const RSA_WITH_SHA512_OID: asn1::ObjectIdentifier =
-    asn1::oid!(1, 2, 840, 113549, 1, 1, 13);
-pub(crate) const RSA_WITH_SHA3_224_OID: asn1::ObjectIdentifier =
+pub const RSA_WITH_SHA1_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 1, 5);
+pub const RSA_WITH_SHA1_ALT_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 14, 3, 2, 29);
+pub const RSA_WITH_SHA224_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 1, 14);
+pub const RSA_WITH_SHA256_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 1, 11);
+pub const RSA_WITH_SHA384_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 1, 12);
+pub const RSA_WITH_SHA512_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 1, 13);
+pub const RSA_WITH_SHA3_224_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 13);
-pub(crate) const RSA_WITH_SHA3_256_OID: asn1::ObjectIdentifier =
+pub const RSA_WITH_SHA3_256_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 14);
-pub(crate) const RSA_WITH_SHA3_384_OID: asn1::ObjectIdentifier =
+pub const RSA_WITH_SHA3_384_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 15);
-pub(crate) const RSA_WITH_SHA3_512_OID: asn1::ObjectIdentifier =
+pub const RSA_WITH_SHA3_512_OID: asn1::ObjectIdentifier =
     asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 16);
 
-pub(crate) const DSA_WITH_SHA224_OID: asn1::ObjectIdentifier =
-    asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 1);
-pub(crate) const DSA_WITH_SHA256_OID: asn1::ObjectIdentifier =
-    asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 2);
-pub(crate) const DSA_WITH_SHA384_OID: asn1::ObjectIdentifier =
-    asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 3);
-pub(crate) const DSA_WITH_SHA512_OID: asn1::ObjectIdentifier =
-    asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 4);
+pub const DSA_WITH_SHA224_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 1);
+pub const DSA_WITH_SHA256_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 2);
+pub const DSA_WITH_SHA384_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 3);
+pub const DSA_WITH_SHA512_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 3, 4);
 
-pub(crate) const ED25519_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 101, 112);
-pub(crate) const ED448_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 101, 113);
+pub const ED25519_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 101, 112);
+pub const ED448_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 101, 113);
 
 // Hashes
-pub(crate) const SHA1_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 14, 3, 2, 26);
-pub(crate) const SHA224_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 4);
-pub(crate) const SHA256_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 1);
-pub(crate) const SHA384_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 2);
-pub(crate) const SHA512_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 3);
+pub const SHA1_OID: asn1::ObjectIdentifier = asn1::oid!(1, 3, 14, 3, 2, 26);
+pub const SHA224_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 4);
+pub const SHA256_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 1);
+pub const SHA384_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 2);
+pub const SHA512_OID: asn1::ObjectIdentifier = asn1::oid!(2, 16, 840, 1, 101, 3, 4, 2, 3);
+pub const SHA3_224_OID: asn1::ObjectIdentifier =
+    asn1::oid!(1, 3, 6, 1, 4, 1, 37476, 3, 2, 1, 99, 7, 224);
+pub const SHA3_256_OID: asn1::ObjectIdentifier =
+    asn1::oid!(1, 3, 6, 1, 4, 1, 37476, 3, 2, 1, 99, 7, 256);
+pub const SHA3_384_OID: asn1::ObjectIdentifier =
+    asn1::oid!(1, 3, 6, 1, 4, 1, 37476, 3, 2, 1, 99, 7, 384);
+pub const SHA3_512_OID: asn1::ObjectIdentifier =
+    asn1::oid!(1, 3, 6, 1, 4, 1, 37476, 3, 2, 1, 99, 7, 512);
+
+pub const MGF1_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 1, 8);
+pub const RSASSA_PSS_OID: asn1::ObjectIdentifier = asn1::oid!(1, 2, 840, 113549, 1, 1, 10);
```

### Comparing `cryptography-40.0.2/src/rust/src/x509/sct.rs` & `cryptography-41.0.0/src/rust/src/x509/sct.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 use crate::error::CryptographyError;
 use pyo3::types::IntoPyDict;
 use pyo3::ToPyObject;
 use std::collections::hash_map::DefaultHasher;
-use std::convert::{TryFrom, TryInto};
 use std::hash::{Hash, Hasher};
 
 struct TLSReader<'a> {
     data: &'a [u8],
 }
 
 impl<'a> TLSReader<'a> {
@@ -124,118 +123,127 @@
                     value
                 )))
             }
         })
     }
 }
 
-#[pyo3::prelude::pyclass]
+#[pyo3::prelude::pyclass(module = "cryptography.hazmat.bindings._rust.x509")]
 pub(crate) struct Sct {
     log_id: [u8; 32],
     timestamp: u64,
     entry_type: LogEntryType,
     hash_algorithm: HashAlgorithm,
     signature_algorithm: SignatureAlgorithm,
     // TODO: These could be 'self references back into sct_data with ouroboros.
     signature: Vec<u8>,
     extension_bytes: Vec<u8>,
     pub(crate) sct_data: Vec<u8>,
 }
 
 #[pyo3::prelude::pymethods]
 impl Sct {
+    fn __richcmp__(
+        &self,
+        other: pyo3::PyRef<'_, Sct>,
+        op: pyo3::basic::CompareOp,
+    ) -> pyo3::PyResult<bool> {
+        match op {
+            pyo3::basic::CompareOp::Eq => Ok(self.sct_data == other.sct_data),
+            pyo3::basic::CompareOp::Ne => Ok(self.sct_data != other.sct_data),
+            _ => Err(pyo3::exceptions::PyTypeError::new_err(
+                "SCTs cannot be ordered",
+            )),
+        }
+    }
+
+    fn __hash__(&self) -> u64 {
+        let mut hasher = DefaultHasher::new();
+        self.sct_data.hash(&mut hasher);
+        hasher.finish()
+    }
+
     #[getter]
     fn version<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        py.import("cryptography.x509.certificate_transparency")?
-            .getattr(crate::intern!(py, "Version"))?
-            .getattr(crate::intern!(py, "v1"))
+        py.import(pyo3::intern!(
+            py,
+            "cryptography.x509.certificate_transparency"
+        ))?
+        .getattr(pyo3::intern!(py, "Version"))?
+        .getattr(pyo3::intern!(py, "v1"))
     }
 
     #[getter]
     fn log_id(&self) -> &[u8] {
         &self.log_id
     }
 
     #[getter]
     fn timestamp<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let datetime_class = py
-            .import("datetime")?
-            .getattr(crate::intern!(py, "datetime"))?;
+            .import(pyo3::intern!(py, "datetime"))?
+            .getattr(pyo3::intern!(py, "datetime"))?;
         datetime_class
-            .call_method1("utcfromtimestamp", (self.timestamp / 1000,))?
+            .call_method1(
+                pyo3::intern!(py, "utcfromtimestamp"),
+                (self.timestamp / 1000,),
+            )?
             .call_method(
                 "replace",
                 (),
                 Some(vec![("microsecond", self.timestamp % 1000 * 1000)].into_py_dict(py)),
             )
     }
 
     #[getter]
     fn entry_type<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let et_class = py
-            .import("cryptography.x509.certificate_transparency")?
-            .getattr(crate::intern!(py, "LogEntryType"))?;
+            .import(pyo3::intern!(
+                py,
+                "cryptography.x509.certificate_transparency"
+            ))?
+            .getattr(pyo3::intern!(py, "LogEntryType"))?;
         let attr_name = match self.entry_type {
             LogEntryType::Certificate => "X509_CERTIFICATE",
             LogEntryType::PreCertificate => "PRE_CERTIFICATE",
         };
         et_class.getattr(attr_name)
     }
 
     #[getter]
     fn signature_hash_algorithm<'p>(
         &self,
         py: pyo3::Python<'p>,
     ) -> pyo3::PyResult<&'p pyo3::PyAny> {
-        let hashes_mod = py.import("cryptography.hazmat.primitives.hashes")?;
+        let hashes_mod = py.import(pyo3::intern!(py, "cryptography.hazmat.primitives.hashes"))?;
         hashes_mod.call_method0(self.hash_algorithm.to_attr())
     }
 
     #[getter]
     fn signature_algorithm<'p>(&self, py: pyo3::Python<'p>) -> pyo3::PyResult<&'p pyo3::PyAny> {
         let sa_class = py
-            .import("cryptography.x509.certificate_transparency")?
-            .getattr(crate::intern!(py, "SignatureAlgorithm"))?;
+            .import(pyo3::intern!(
+                py,
+                "cryptography.x509.certificate_transparency"
+            ))?
+            .getattr(pyo3::intern!(py, "SignatureAlgorithm"))?;
         sa_class.getattr(self.signature_algorithm.to_attr())
     }
 
     #[getter]
     fn signature(&self) -> &[u8] {
         &self.signature
     }
 
     #[getter]
     fn extension_bytes(&self) -> &[u8] {
         &self.extension_bytes
     }
 }
 
-#[pyo3::prelude::pyproto]
-impl pyo3::PyObjectProtocol for Sct {
-    fn __richcmp__(
-        &self,
-        other: pyo3::PyRef<Sct>,
-        op: pyo3::basic::CompareOp,
-    ) -> pyo3::PyResult<bool> {
-        match op {
-            pyo3::basic::CompareOp::Eq => Ok(self.sct_data == other.sct_data),
-            pyo3::basic::CompareOp::Ne => Ok(self.sct_data != other.sct_data),
-            _ => Err(pyo3::exceptions::PyTypeError::new_err(
-                "SCTs cannot be ordered",
-            )),
-        }
-    }
-
-    fn __hash__(&self) -> u64 {
-        let mut hasher = DefaultHasher::new();
-        self.sct_data.hash(&mut hasher);
-        hasher.finish()
-    }
-}
-
 pub(crate) fn parse_scts(
     py: pyo3::Python<'_>,
     data: &[u8],
     entry_type: LogEntryType,
 ) -> Result<pyo3::PyObject, CryptographyError> {
     let mut reader = TLSReader::new(data).read_length_prefixed()?;
```

### Comparing `cryptography-40.0.2/tests/bench/test_aead.py` & `cryptography-41.0.0/tests/bench/test_aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/bench/test_x509.py` & `cryptography-41.0.0/tests/bench/test_x509.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,24 @@
         key_identifier=b"\x00" * 16,
         authority_cert_issuer=None,
         authority_cert_serial_number=None,
     )
     benchmark(aki.public_bytes)
 
 
+def test_load_der_certificate(benchmark):
+    cert_bytes = load_vectors_from_file(
+        os.path.join("x509", "PKITS_data", "certs", "GoodCACert.crt"),
+        loader=lambda pemfile: pemfile.read(),
+        mode="rb",
+    )
+
+    benchmark(x509.load_der_x509_certificate, cert_bytes)
+
+
 def test_load_pem_certificate(benchmark):
     cert_bytes = load_vectors_from_file(
         os.path.join("x509", "cryptography.io.pem"),
         loader=lambda pemfile: pemfile.read(),
         mode="rb",
     )
```

### Comparing `cryptography-40.0.2/tests/conftest.py` & `cryptography-41.0.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
-import sys
+import contextlib
 
 import pytest
 
 from cryptography.hazmat.backends.openssl import backend as openssl_backend
 
 from .utils import check_backend_support
 
@@ -24,19 +24,14 @@
         ]
     )
 
 
 def pytest_addoption(parser):
     parser.addoption("--wycheproof-root", default=None)
     parser.addoption("--enable-fips", default=False)
-    # REMOVE ME WHEN WE DROP PYTHON 3.6 SUPPORT
-    # This just adds a no-op flag so that we don't error on py36 where
-    # pytest-subtests is stuck on 0.8.0
-    if sys.version_info[:2] == (3, 6):
-        parser.addoption("--no-subtests-shortletter", action="store_true")
 
 
 def pytest_runtest_setup(item):
     if openssl_backend._fips_enabled:
         for marker in item.iter_markers(name="skip_fips"):
             pytest.skip(marker.kwargs["reason"])
 
@@ -48,7 +43,25 @@
     # Ensure the error stack is clear before the test
     errors = openssl_backend._consume_errors()
     assert not errors
     yield openssl_backend
     # Ensure the error stack is clear after the test
     errors = openssl_backend._consume_errors()
     assert not errors
+
+
+@pytest.fixture()
+def subtests():
+    # This is a miniature version of the pytest-subtests package, but
+    # optimized for lower overhead.
+    #
+    # When tests are skipped, these are not logged in the final pytest output.
+    yield SubTests()
+
+
+class SubTests:
+    @contextlib.contextmanager
+    def test(self):
+        try:
+            yield
+        except pytest.skip.Exception:
+            pass
```

### Comparing `cryptography-40.0.2/tests/doubles.py` & `cryptography-41.0.0/tests/doubles.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/backends/test_openssl.py` & `cryptography-41.0.0/tests/hazmat/backends/test_openssl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 
 import itertools
 import os
-import subprocess
-import sys
-import textwrap
 
 import pytest
 
 from cryptography.exceptions import InternalError, _Reasons
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.backends.openssl.backend import backend
 from cryptography.hazmat.backends.openssl.ec import _sn_to_elliptic_curve
 from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives.asymmetric import dh, padding
+from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives.ciphers import Cipher
 from cryptography.hazmat.primitives.ciphers.algorithms import AES
 from cryptography.hazmat.primitives.ciphers.modes import CBC
 
 from ...doubles import (
     DummyAsymmetricPadding,
     DummyBlockCipherAlgorithm,
     DummyCipherAlgorithm,
     DummyHashAlgorithm,
     DummyMode,
 )
 from ...hazmat.primitives.test_rsa import rsa_key_512, rsa_key_2048
 from ...utils import (
-    load_nist_vectors,
     load_vectors_from_file,
     raises_unsupported_algorithm,
 )
 
 # Make ruff happy since we're importing fixtures that pytest patches in as
 # func args
 __all__ = ["rsa_key_512", "rsa_key_2048"]
@@ -160,181 +156,19 @@
         bn = backend._int_to_bn(value)
         assert bn != backend._ffi.NULL
         bn = backend._ffi.gc(bn, backend._lib.BN_clear_free)
 
         assert bn
         assert backend._bn_to_int(bn) == value
 
-    def test_int_to_bn_inplace(self):
-        value = (2**4242) - 4242
-        bn_ptr = backend._lib.BN_new()
-        assert bn_ptr != backend._ffi.NULL
-        bn_ptr = backend._ffi.gc(bn_ptr, backend._lib.BN_free)
-        bn = backend._int_to_bn(value, bn_ptr)
-
-        assert bn == bn_ptr
-        assert backend._bn_to_int(bn_ptr) == value
-
     def test_bn_to_int(self):
         bn = backend._int_to_bn(0)
         assert backend._bn_to_int(bn) == 0
 
 
-@pytest.mark.skipif(
-    not backend._lib.CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE,
-    reason="Requires OpenSSL with ENGINE support and OpenSSL < 1.1.1d",
-)
-@pytest.mark.skip_fips(reason="osrandom engine disabled for FIPS")
-class TestOpenSSLRandomEngine:
-    def setup_method(self):
-        # The default RAND engine is global and shared between
-        # tests. We make sure that the default engine is osrandom
-        # before we start each test and restore the global state to
-        # that engine in teardown.
-        current_default = backend._lib.ENGINE_get_default_RAND()
-        name = backend._lib.ENGINE_get_name(current_default)
-        assert name == backend._lib.Cryptography_osrandom_engine_name
-
-    def teardown_method(self):
-        # we need to reset state to being default. backend is a shared global
-        # for all these tests.
-        backend.activate_osrandom_engine()
-        current_default = backend._lib.ENGINE_get_default_RAND()
-        name = backend._lib.ENGINE_get_name(current_default)
-        assert name == backend._lib.Cryptography_osrandom_engine_name
-
-    @pytest.mark.skipif(
-        sys.executable is None, reason="No Python interpreter available."
-    )
-    def test_osrandom_engine_is_default(self, tmpdir):
-        engine_printer = textwrap.dedent(
-            """
-            import sys
-            from cryptography.hazmat.backends.openssl.backend import backend
-
-            e = backend._lib.ENGINE_get_default_RAND()
-            name = backend._lib.ENGINE_get_name(e)
-            sys.stdout.write(backend._ffi.string(name).decode('ascii'))
-            res = backend._lib.ENGINE_free(e)
-            assert res == 1
-            """
-        )
-        engine_name = tmpdir.join("engine_name")
-
-        # If we're running tests via ``python setup.py test`` in a clean
-        # environment then all of our dependencies are going to be installed
-        # into either the current directory or the .eggs directory. However the
-        # subprocess won't know to activate these dependencies, so we'll get it
-        # to do so by passing our entire sys.path into the subprocess via the
-        # PYTHONPATH environment variable.
-        env = os.environ.copy()
-        env["PYTHONPATH"] = os.pathsep.join(sys.path)
-
-        with engine_name.open("w") as out:
-            subprocess.check_call(
-                [sys.executable, "-c", engine_printer],
-                env=env,
-                stdout=out,
-                stderr=subprocess.PIPE,
-            )
-
-        osrandom_engine_name = backend._ffi.string(
-            backend._lib.Cryptography_osrandom_engine_name
-        )
-
-        assert engine_name.read().encode("ascii") == osrandom_engine_name
-
-    def test_osrandom_sanity_check(self):
-        # This test serves as a check against catastrophic failure.
-        buf = backend._ffi.new("unsigned char[]", 500)
-        res = backend._lib.RAND_bytes(buf, 500)
-        assert res == 1
-        assert backend._ffi.buffer(buf)[:] != "\x00" * 500
-
-    def test_activate_osrandom_no_default(self):
-        backend.activate_builtin_random()
-        e = backend._lib.ENGINE_get_default_RAND()
-        assert e == backend._ffi.NULL
-        backend.activate_osrandom_engine()
-        e = backend._lib.ENGINE_get_default_RAND()
-        name = backend._lib.ENGINE_get_name(e)
-        assert name == backend._lib.Cryptography_osrandom_engine_name
-        res = backend._lib.ENGINE_free(e)
-        assert res == 1
-
-    def test_activate_builtin_random(self):
-        e = backend._lib.ENGINE_get_default_RAND()
-        assert e != backend._ffi.NULL
-        name = backend._lib.ENGINE_get_name(e)
-        assert name == backend._lib.Cryptography_osrandom_engine_name
-        res = backend._lib.ENGINE_free(e)
-        assert res == 1
-        backend.activate_builtin_random()
-        e = backend._lib.ENGINE_get_default_RAND()
-        assert e == backend._ffi.NULL
-
-    def test_activate_builtin_random_already_active(self):
-        backend.activate_builtin_random()
-        e = backend._lib.ENGINE_get_default_RAND()
-        assert e == backend._ffi.NULL
-        backend.activate_builtin_random()
-        e = backend._lib.ENGINE_get_default_RAND()
-        assert e == backend._ffi.NULL
-
-    def test_osrandom_engine_implementation(self):
-        name = backend.osrandom_engine_implementation()
-        assert name in [
-            "/dev/urandom",
-            "CryptGenRandom",
-            "getentropy",
-            "getrandom",
-        ]
-        if sys.platform.startswith("linux"):
-            assert name in ["getrandom", "/dev/urandom"]
-        if sys.platform == "darwin":
-            assert name in ["getentropy"]
-        if sys.platform == "win32":
-            assert name == "CryptGenRandom"
-
-    def test_activate_osrandom_already_default(self):
-        e = backend._lib.ENGINE_get_default_RAND()
-        name = backend._lib.ENGINE_get_name(e)
-        assert name == backend._lib.Cryptography_osrandom_engine_name
-        res = backend._lib.ENGINE_free(e)
-        assert res == 1
-        backend.activate_osrandom_engine()
-        e = backend._lib.ENGINE_get_default_RAND()
-        name = backend._lib.ENGINE_get_name(e)
-        assert name == backend._lib.Cryptography_osrandom_engine_name
-        res = backend._lib.ENGINE_free(e)
-        assert res == 1
-
-
-@pytest.mark.skipif(
-    backend._lib.CRYPTOGRAPHY_NEEDS_OSRANDOM_ENGINE,
-    reason="Requires OpenSSL without ENGINE support or OpenSSL >=1.1.1d",
-)
-class TestOpenSSLNoEngine:
-    def test_no_engine_support(self):
-        assert (
-            backend._ffi.string(backend._lib.Cryptography_osrandom_engine_id)
-            == b"no-engine-support"
-        )
-        assert (
-            backend._ffi.string(backend._lib.Cryptography_osrandom_engine_name)
-            == b"osrandom_engine disabled"
-        )
-
-    def test_activate_builtin_random_does_nothing(self):
-        backend.activate_builtin_random()
-
-    def test_activate_osrandom_does_nothing(self):
-        backend.activate_osrandom_engine()
-
-
 class TestOpenSSLRSA:
     def test_generate_rsa_parameters_supported(self):
         assert backend.generate_rsa_parameters_supported(1, 1024) is False
         assert backend.generate_rsa_parameters_supported(4, 1024) is False
         assert backend.generate_rsa_parameters_supported(3, 1024) is True
         assert backend.generate_rsa_parameters_supported(3, 511) is False
 
@@ -535,44 +369,14 @@
 )
 @pytest.mark.supported(
     only_if=lambda backend: backend.dh_supported(),
     skip_message="Requires DH support",
 )
 class TestOpenSSLDHSerialization:
     @pytest.mark.parametrize(
-        "vector",
-        load_vectors_from_file(
-            os.path.join("asymmetric", "DH", "RFC5114.txt"), load_nist_vectors
-        ),
-    )
-    def test_dh_serialization_with_q_unsupported(self, backend, vector):
-        parameters = dh.DHParameterNumbers(
-            int(vector["p"], 16), int(vector["g"], 16), int(vector["q"], 16)
-        )
-        public = dh.DHPublicNumbers(int(vector["ystatcavs"], 16), parameters)
-        private = dh.DHPrivateNumbers(int(vector["xstatcavs"], 16), public)
-        private_key = private.private_key(backend)
-        public_key = private_key.public_key()
-        with raises_unsupported_algorithm(_Reasons.UNSUPPORTED_SERIALIZATION):
-            private_key.private_bytes(
-                serialization.Encoding.PEM,
-                serialization.PrivateFormat.PKCS8,
-                serialization.NoEncryption(),
-            )
-        with raises_unsupported_algorithm(_Reasons.UNSUPPORTED_SERIALIZATION):
-            public_key.public_bytes(
-                serialization.Encoding.PEM,
-                serialization.PublicFormat.SubjectPublicKeyInfo,
-            )
-        with raises_unsupported_algorithm(_Reasons.UNSUPPORTED_SERIALIZATION):
-            parameters.parameters(backend).parameter_bytes(
-                serialization.Encoding.PEM, serialization.ParameterFormat.PKCS3
-            )
-
-    @pytest.mark.parametrize(
         ("key_path", "loader_func"),
         [
             (
                 os.path.join("asymmetric", "DH", "dhkey_rfc5114_2.pem"),
                 serialization.load_pem_private_key,
             ),
             (
```

### Comparing `cryptography-40.0.2/tests/hazmat/backends/test_openssl_memleak.py` & `cryptography-41.0.0/tests/hazmat/backends/test_openssl_memleak.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,15 @@
         gc.collect()
         gc.collect()
 
         if _openssl.lib.CRYPTOGRAPHY_OPENSSL_300_OR_GREATER:
             _openssl.lib.OSSL_PROVIDER_unload(backend._binding._legacy_provider)
             _openssl.lib.OSSL_PROVIDER_unload(backend._binding._default_provider)
 
-        if _openssl.lib.Cryptography_HAS_OPENSSL_CLEANUP:
-            _openssl.lib.OPENSSL_cleanup()
+        _openssl.lib.OPENSSL_cleanup()
 
         # Swap back to the original functions so that if OpenSSL tries to free
         # something from its atexit handle it won't be going through a Python
         # function, which will be deallocated when this function returns
         result = _openssl.lib.Cryptography_CRYPTO_set_mem_functions(
             _openssl.ffi.addressof(
                 _openssl.lib, "Cryptography_malloc_wrapper"
```

### Comparing `cryptography-40.0.2/tests/hazmat/bindings/test_openssl.py` & `cryptography-41.0.0/tests/hazmat/bindings/test_openssl.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,14 @@
 class TestOpenSSL:
     def test_binding_loads(self):
         binding = Binding()
         assert binding
         assert binding.lib
         assert binding.ffi
 
-    def test_add_engine_more_than_once(self):
-        b = Binding()
-        b._register_osrandom_engine()
-        assert b.lib.ERR_get_error() == 0
-
     def test_ssl_ctx_options(self):
         # Test that we're properly handling 32-bit unsigned on all platforms.
         b = Binding()
         # SSL_OP_ALL is 0 on BoringSSL
         if not b.lib.CRYPTOGRAPHY_IS_BORINGSSL:
             assert b.lib.SSL_OP_ALL > 0
         ctx = b.lib.SSL_CTX_new(b.lib.TLS_method())
@@ -81,26 +76,14 @@
 
         error = exc_info.value.err_code[0]
         assert error.lib == b.lib.ERR_LIB_EVP
         assert error.reason == b.lib.EVP_R_DATA_NOT_MULTIPLE_OF_BLOCK_LENGTH
         if not b.lib.CRYPTOGRAPHY_IS_BORINGSSL:
             assert b"data not multiple of block length" in error.reason_text
 
-    def test_check_startup_errors_are_allowed(self):
-        b = Binding()
-        b.lib.ERR_put_error(
-            b.lib.ERR_LIB_EVP,
-            b.lib.EVP_F_EVP_ENCRYPTFINAL_EX,
-            b.lib.EVP_R_DATA_NOT_MULTIPLE_OF_BLOCK_LENGTH,
-            b"",
-            -1,
-        )
-        b._register_osrandom_engine()
-        assert rust_openssl.capture_error_stack() == []
-
     def test_version_mismatch(self):
         with pytest.raises(ImportError):
             _verify_package_version("nottherightversion")
 
     def test_legacy_provider_error(self):
         with pytest.raises(RuntimeError):
             _legacy_provider_error(False)
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/fixtures_dh.py` & `cryptography-41.0.0/tests/hazmat/primitives/fixtures_dh.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/fixtures_dsa.py` & `cryptography-41.0.0/tests/hazmat/primitives/fixtures_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/fixtures_ec.py` & `cryptography-41.0.0/tests/hazmat/primitives/fixtures_ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/fixtures_rsa.py` & `cryptography-41.0.0/tests/hazmat/primitives/fixtures_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_3des.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_3des.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_aead.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_aes.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_aes.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,17 +57,15 @@
         tweak = b"\x00" * 16
         cipher = base.Cipher(algorithms.AES(key), modes.XTS(tweak))
         enc = cipher.encryptor()
         with pytest.raises(ValueError):
             enc.update(b"0" * 15)
 
     @pytest.mark.supported(
-        only_if=lambda backend: (
-            backend._lib.CRYPTOGRAPHY_OPENSSL_111D_OR_GREATER
-        ),
+        only_if=lambda backend: (not backend._lib.CRYPTOGRAPHY_IS_LIBRESSL),
         skip_message="duplicate key encryption error added in OpenSSL 1.1.1d",
     )
     def test_xts_no_duplicate_keys_encryption(self, backend):
         key = bytes(range(16)) * 2
         tweak = b"\x00" * 16
         cipher = base.Cipher(algorithms.AES(key), modes.XTS(tweak))
         with pytest.raises(ValueError, match="duplicated keys"):
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_aes_gcm.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_aes_gcm.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_arc4.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_arc4.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_asym_utils.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_asym_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_block.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_block.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_blowfish.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_blowfish.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_camellia.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_camellia.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_cast5.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_cast5.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_chacha20.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_chacha20.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_ciphers.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_cmac.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_concatkdf.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_concatkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_constant_time.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_constant_time.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_dh.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_dh.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         with pytest.raises(ValueError):
             dh.generate_parameters(2, 511, backend)
 
     def test_unsupported_generator_generate_dh(self, backend):
         with pytest.raises(ValueError):
             dh.generate_parameters(7, 512, backend)
 
-    def test_large_key_generate_dh(self):
+    def test_large_key_generate_dh(self, backend):
         with pytest.raises(ValueError):
             dh.generate_parameters(2, 1 << 30)
 
     @pytest.mark.skip_fips(reason="non-FIPS parameters")
     def test_dh_parameters_supported(self, backend):
         valid_p = int(
             b"907c7211ae61aaaba1825ff53b6cb71ac6df9f1a424c033f4a0a41ac42fad3a9"
@@ -460,14 +460,39 @@
         key2 = private2.private_key(backend)
         symkey1 = key1.exchange(public2.public_key(backend))
         symkey2 = key2.exchange(public1.public_key(backend))
 
         assert int.from_bytes(symkey1, "big") == int(vector["z"], 16)
         assert int.from_bytes(symkey2, "big") == int(vector["z"], 16)
 
+    @pytest.mark.supported(
+        only_if=lambda backend: backend.dh_x942_serialization_supported(),
+        skip_message="DH X9.42 not supported",
+    )
+    def test_public_key_equality(self, backend):
+        key_bytes = load_vectors_from_file(
+            os.path.join("asymmetric", "DH", "dhpub.pem"),
+            lambda pemfile: pemfile.read(),
+            mode="rb",
+        )
+        key_bytes_2 = load_vectors_from_file(
+            os.path.join("asymmetric", "DH", "dhpub_rfc5114_2.pem"),
+            lambda pemfile: pemfile.read(),
+            mode="rb",
+        )
+        key1 = serialization.load_pem_public_key(key_bytes)
+        key2 = serialization.load_pem_public_key(key_bytes)
+        key3 = serialization.load_pem_public_key(key_bytes_2)
+        assert key1 == key2
+        assert key1 != key3
+        assert key1 != object()
+
+        with pytest.raises(TypeError):
+            key1 < key2  # type: ignore[operator]
+
 
 @pytest.mark.supported(
     only_if=lambda backend: backend.dh_supported(),
     skip_message="DH not supported",
 )
 class TestDHPrivateKeySerialization:
     @pytest.mark.parametrize(
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_dsa.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_dsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,14 +380,28 @@
                     g=pn.public_numbers.parameter_numbers.g,
                 ),
                 y=pn.public_numbers.y,
             ),
             x=pn.x,
         ).private_key(backend)
 
+    def test_public_key_equality(self, backend):
+        key_bytes = load_vectors_from_file(
+            os.path.join("asymmetric", "PKCS8", "unenc-dsa-pkcs8.pem"),
+            lambda pemfile: pemfile.read().encode(),
+        )
+        key1 = serialization.load_pem_private_key(key_bytes, None).public_key()
+        key2 = serialization.load_pem_private_key(key_bytes, None).public_key()
+        key3 = DSA_KEY_2048.private_key().public_key()
+        assert key1 == key2
+        assert key1 != key3
+        assert key1 != object()
+        with pytest.raises(TypeError):
+            key1 < key2  # type: ignore[operator]
+
 
 @pytest.mark.supported(
     only_if=lambda backend: backend.dsa_supported(),
     skip_message="Does not support DSA.",
 )
 class TestDSAVerification:
     def test_dsa_verification(self, backend, subtests):
@@ -695,14 +709,18 @@
     @pytest.mark.parametrize(
         ("encoding", "fmt"),
         [
             (serialization.Encoding.Raw, serialization.PrivateFormat.PKCS8),
             (serialization.Encoding.DER, serialization.PrivateFormat.Raw),
             (serialization.Encoding.Raw, serialization.PrivateFormat.Raw),
             (serialization.Encoding.X962, serialization.PrivateFormat.PKCS8),
+            (
+                serialization.Encoding.SMIME,
+                serialization.PrivateFormat.TraditionalOpenSSL,
+            ),
         ],
     )
     def test_private_bytes_rejects_invalid(self, encoding, fmt, backend):
         key = DSA_KEY_1024.private_key(backend)
         with pytest.raises(ValueError):
             key.private_bytes(encoding, fmt, serialization.NoEncryption())
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_ec.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_ec.py`

 * *Files 1% similar despite different names*

```diff
@@ -561,15 +561,15 @@
         public_key = private_key.public_key()
         with pytest.raises(ValueError):
             public_key.verify(
                 b"\x00" * 32, data, ec.ECDSA(Prehashed(hashes.SHA256()))
             )
 
 
-class TestECNumbersEquality:
+class TestECEquality:
     def test_public_numbers_eq(self):
         pub = ec.EllipticCurvePublicNumbers(1, 2, ec.SECP192R1())
         assert pub == ec.EllipticCurvePublicNumbers(1, 2, ec.SECP192R1())
 
     def test_public_numbers_ne(self):
         pub = ec.EllipticCurvePublicNumbers(1, 2, ec.SECP192R1())
         assert pub != ec.EllipticCurvePublicNumbers(1, 2, ec.SECP384R1())
@@ -597,14 +597,27 @@
             1, ec.EllipticCurvePublicNumbers(1, 3, ec.SECP192R1())
         )
         assert priv != ec.EllipticCurvePrivateNumbers(
             1, ec.EllipticCurvePublicNumbers(1, 2, ec.SECP521R1())
         )
         assert priv != object()
 
+    def test_public_key_equality(self, backend):
+        _skip_curve_unsupported(backend, ec.SECP256R1())
+        key_bytes = load_vectors_from_file(
+            os.path.join("asymmetric", "PKCS8", "ec_private_key.pem"),
+            lambda pemfile: pemfile.read().encode(),
+        )
+        key1 = serialization.load_pem_private_key(key_bytes, None).public_key()
+        key2 = serialization.load_pem_private_key(key_bytes, None).public_key()
+        key3 = ec.generate_private_key(ec.SECP256R1()).public_key()
+        assert key1 == key2
+        assert key1 != key3
+        assert key1 != object()
+
 
 class TestECSerialization:
     @pytest.mark.parametrize(
         ("fmt", "password"),
         itertools.product(
             [
                 serialization.PrivateFormat.TraditionalOpenSSL,
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_ed25519.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_ed25519.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cryptography.exceptions import InvalidSignature, _Reasons
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.ed25519 import (
     Ed25519PrivateKey,
     Ed25519PublicKey,
 )
 
+from ...doubles import DummyKeySerializationEncryption
 from ...utils import load_vectors_from_file, raises_unsupported_algorithm
 
 
 def load_ed25519_vectors(vector_data):
     """
     djb's ed25519 vectors are structured as a colon delimited array:
         0: secret key (32 bytes) + public key (32 bytes)
@@ -152,35 +153,48 @@
         with pytest.raises(ValueError):
             Ed25519PrivateKey.from_private_bytes(b"a" * 31)
         with pytest.raises(ValueError):
             Ed25519PrivateKey.from_private_bytes(b"a" * 33)
 
     def test_invalid_private_bytes(self, backend):
         key = Ed25519PrivateKey.generate()
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.Raw,
                 None,  # type: ignore[arg-type]
             )
+        with pytest.raises(ValueError):
+            key.private_bytes(
+                serialization.Encoding.Raw,
+                serialization.PrivateFormat.Raw,
+                DummyKeySerializationEncryption(),
+            )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.PKCS8,
-                None,  # type: ignore[arg-type]
+                DummyKeySerializationEncryption(),
             )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.PEM,
                 serialization.PrivateFormat.Raw,
                 serialization.NoEncryption(),
             )
 
+        with pytest.raises(ValueError):
+            key.private_bytes(
+                serialization.Encoding.DER,
+                serialization.PrivateFormat.OpenSSH,
+                serialization.NoEncryption(),
+            )
+
     def test_invalid_public_bytes(self, backend):
         key = Ed25519PrivateKey.generate().public_key()
         with pytest.raises(ValueError):
             key.public_bytes(
                 serialization.Encoding.Raw,
                 serialization.PublicFormat.SubjectPublicKeyInfo,
             )
@@ -191,14 +205,19 @@
             )
 
         with pytest.raises(ValueError):
             key.public_bytes(
                 serialization.Encoding.PEM, serialization.PublicFormat.Raw
             )
 
+        with pytest.raises(ValueError):
+            key.public_bytes(
+                serialization.Encoding.DER, serialization.PublicFormat.OpenSSH
+            )
+
     @pytest.mark.parametrize(
         ("encoding", "fmt", "encryption", "passwd", "load_func"),
         [
             (
                 serialization.Encoding.PEM,
                 serialization.PrivateFormat.PKCS8,
                 serialization.BestAvailableEncryption(b"password"),
@@ -243,7 +262,28 @@
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.Raw,
                 serialization.NoEncryption(),
             )
             == private_bytes
         )
+
+
+@pytest.mark.supported(
+    only_if=lambda backend: backend.ed25519_supported(),
+    skip_message="Requires OpenSSL with Ed25519 support",
+)
+def test_public_key_equality(backend):
+    key_bytes = load_vectors_from_file(
+        os.path.join("asymmetric", "Ed25519", "ed25519-pkcs8.der"),
+        lambda derfile: derfile.read(),
+        mode="rb",
+    )
+    key1 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key2 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key3 = Ed25519PrivateKey.generate().public_key()
+    assert key1 == key2
+    assert key1 != key3
+    assert key1 != object()
+
+    with pytest.raises(TypeError):
+        key1 < key2  # type: ignore[operator]
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_ed448.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_ed448.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cryptography.exceptions import InvalidSignature, _Reasons
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.ed448 import (
     Ed448PrivateKey,
     Ed448PublicKey,
 )
 
+from ...doubles import DummyKeySerializationEncryption
 from ...utils import (
     load_nist_vectors,
     load_vectors_from_file,
     raises_unsupported_algorithm,
 )
 
 
@@ -188,26 +189,32 @@
         with pytest.raises(ValueError):
             Ed448PrivateKey.from_private_bytes(b"a" * 56)
         with pytest.raises(ValueError):
             Ed448PrivateKey.from_private_bytes(b"a" * 58)
 
     def test_invalid_private_bytes(self, backend):
         key = Ed448PrivateKey.generate()
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.Raw,
                 None,  # type: ignore[arg-type]
             )
+        with pytest.raises(ValueError):
+            key.private_bytes(
+                serialization.Encoding.Raw,
+                serialization.PrivateFormat.Raw,
+                DummyKeySerializationEncryption(),
+            )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.PKCS8,
-                None,  # type: ignore[arg-type]
+                DummyKeySerializationEncryption(),
             )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.PEM,
                 serialization.PrivateFormat.Raw,
                 serialization.NoEncryption(),
@@ -256,7 +263,28 @@
             "f9e5c44c54ab23a2eb14f947e167b990b080863e28b399380f30db6e54d5d1406"
             "d23378ffde11b1fb81b2b438a3b8e8aa7f7f4e1befcc905023fab5a5465053844"
             "f04cf0c1b51d84760f869588687f57500"
         )
         key = Ed448PublicKey.from_public_bytes(public_bytes)
         with pytest.raises(InvalidSignature):
             key.verify(signature, b"8")
+
+
+@pytest.mark.supported(
+    only_if=lambda backend: backend.ed448_supported(),
+    skip_message="Requires OpenSSL with Ed448 support",
+)
+def test_public_key_equality(backend):
+    key_bytes = load_vectors_from_file(
+        os.path.join("asymmetric", "Ed448", "ed448-pkcs8.der"),
+        lambda derfile: derfile.read(),
+        mode="rb",
+    )
+    key1 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key2 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key3 = Ed448PrivateKey.generate().public_key()
+    assert key1 == key2
+    assert key1 != key3
+    assert key1 != object()
+
+    with pytest.raises(TypeError):
+        key1 < key2  # type: ignore[operator]
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_hash_vectors.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_hash_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_hashes.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_hashes.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_hkdf.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_hkdf_vectors.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_hkdf_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_hmac.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_hmac.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,7 +84,12 @@
     def test_buffer_protocol(self, backend):
         key = bytearray(b"2b7e151628aed2a6abf7158809cf4f3c")
         h = hmac.HMAC(key, hashes.SHA256(), backend)
         h.update(bytearray(b"6bc1bee22e409f96e93d7e117393172a"))
         assert h.finalize() == binascii.unhexlify(
             b"a1bf7169c56a501c6585190ff4f07cad6e492a3ee187c0372614fb444b9fc3f0"
         )
+
+    def test_algorithm(self):
+        alg = hashes.SHA256()
+        h = hmac.HMAC(b"123456", alg)
+        assert h.algorithm is alg
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_hmac_vectors.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_hmac_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_idea.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_kbkdf.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_kbkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_keywrap.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_padding.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_padding.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_pbkdf2hmac.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_pkcs12.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_pkcs12.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_pkcs7.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_pkcs7.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,15 +803,15 @@
         certs = load_vectors_from_file(
             os.path.join("pkcs7", "amazon-roots.der"),
             lambda derfile: pkcs7.load_der_pkcs7_certificates(derfile.read()),
             mode="rb",
         )
         with pytest.raises(TypeError):
             pkcs7.serialize_certificates(
-                "not a list of certs",  # type: ignore[arg-type]
+                object(),  # type: ignore[arg-type]
                 serialization.Encoding.PEM,
             )
 
         with pytest.raises(TypeError):
             pkcs7.serialize_certificates([], serialization.Encoding.PEM)
 
         with pytest.raises(TypeError):
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_poly1305.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_poly1305.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_rsa.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_rsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -2759,7 +2759,19 @@
     )
     def test_public_bytes_rejects_invalid(
         self, rsa_key_2048: rsa.RSAPrivateKey, encoding, fmt, backend
     ):
         key = rsa_key_2048.public_key()
         with pytest.raises(ValueError):
             key.public_bytes(encoding, fmt)
+
+    def test_public_key_equality(self, rsa_key_2048: rsa.RSAPrivateKey):
+        key1 = rsa_key_2048.public_key()
+        key2 = RSA_KEY_2048.private_key(
+            unsafe_skip_rsa_key_validation=True
+        ).public_key()
+        key3 = RSA_KEY_2048_ALT.private_key(
+            unsafe_skip_rsa_key_validation=True
+        ).public_key()
+        assert key1 == key2
+        assert key1 != key3
+        assert key1 != object()
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_scrypt.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_scrypt.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_seed.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_serialization.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,14 +391,18 @@
             mode="rb",
         )
         assert key
         assert isinstance(key, ec.EllipticCurvePublicKey)
         assert key.curve.name == "secp256r1"
         assert key.curve.key_size == 256
 
+    @pytest.mark.supported(
+        only_if=lambda backend: backend.dh_supported(),
+        skip_message="DH not supported",
+    )
     def test_wrong_parameters_format(self, backend):
         param_data = b"---- NOT A KEY ----\n"
 
         with pytest.raises(ValueError):
             load_der_parameters(param_data, backend)
 
 
@@ -730,14 +734,18 @@
 
     def test_wrong_public_format(self, backend):
         key_data = b"---- NOT A KEY ----\n"
 
         with pytest.raises(ValueError):
             load_pem_public_key(key_data, backend)
 
+    @pytest.mark.supported(
+        only_if=lambda backend: backend.dh_supported(),
+        skip_message="DH not supported",
+    )
     def test_wrong_parameters_format(self, backend):
         param_data = b"---- NOT A KEY ----\n"
 
         with pytest.raises(ValueError):
             load_pem_parameters(param_data, backend)
 
     def test_corrupt_traditional_format(self, backend):
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_sm4.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_sm4.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_ssh.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_ssh.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import base64
 import datetime
 import os
 
 import pytest
 
 from cryptography import utils
-from cryptography.exceptions import InvalidSignature
+from cryptography.exceptions import InvalidSignature, InvalidTag
 from cryptography.hazmat.primitives.asymmetric import (
     dsa,
     ec,
     ed25519,
     rsa,
 )
 from cryptography.hazmat.primitives.serialization import (
@@ -149,14 +149,15 @@
             ("rsa-psw.key",),
             ("dsa-nopsw.key",),
             ("dsa-psw.key",),
             ("ecdsa-nopsw.key",),
             ("ecdsa-psw.key",),
             ("ed25519-nopsw.key",),
             ("ed25519-psw.key",),
+            ("ed25519-aesgcm-psw.key",),
         ],
     )
     def test_load_ssh_private_key(self, key_file, backend):
         if "ed25519" in key_file and not backend.ed25519_supported():
             pytest.skip("Requires OpenSSL with Ed25519 support")
         if "-psw" in key_file and not ssh._bcrypt_supported:
             pytest.skip("Requires bcrypt module")
@@ -240,14 +241,56 @@
             )
 
         # make sure multi-line base64 is used
         maxline = max(map(len, priv_data2.split(b"\n")))
         assert maxline < 80
 
     @pytest.mark.supported(
+        only_if=lambda backend: backend.ed25519_supported(),
+        skip_message="Requires Ed25519 support",
+    )
+    @pytest.mark.supported(
+        only_if=lambda backend: ssh._bcrypt_supported,
+        skip_message="Requires that bcrypt exists",
+    )
+    def test_load_ssh_private_key_invalid_tag(self, backend):
+        priv_data = bytearray(
+            load_vectors_from_file(
+                os.path.join(
+                    "asymmetric", "OpenSSH", "ed25519-aesgcm-psw.key"
+                ),
+                lambda f: f.read(),
+                mode="rb",
+            )
+        )
+        # mutate one byte to break the tag
+        priv_data[-38] = 82
+        with pytest.raises(InvalidTag):
+            load_ssh_private_key(priv_data, b"password")
+
+    @pytest.mark.supported(
+        only_if=lambda backend: backend.ed25519_supported(),
+        skip_message="Requires Ed25519 support",
+    )
+    @pytest.mark.supported(
+        only_if=lambda backend: ssh._bcrypt_supported,
+        skip_message="Requires that bcrypt exists",
+    )
+    def test_load_ssh_private_key_tag_incorrect_length(self, backend):
+        priv_data = load_vectors_from_file(
+            os.path.join("asymmetric", "OpenSSH", "ed25519-aesgcm-psw.key"),
+            lambda f: f.read(),
+            mode="rb",
+        )
+        # clip out a byte
+        broken_data = priv_data[:-37] + priv_data[-38:]
+        with pytest.raises(ValueError):
+            load_ssh_private_key(broken_data, b"password")
+
+    @pytest.mark.supported(
         only_if=lambda backend: ssh._bcrypt_supported,
         skip_message="Requires that bcrypt exists",
     )
     def test_bcrypt_encryption(self, backend):
         private_key = ec.generate_private_key(ec.SECP256R1(), backend)
         pub1 = private_key.public_key().public_bytes(
             Encoding.OpenSSH, PublicFormat.OpenSSH
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_x25519.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_x25519.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cryptography.exceptions import _Reasons
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.x25519 import (
     X25519PrivateKey,
     X25519PublicKey,
 )
 
+from ...doubles import DummyKeySerializationEncryption
 from ...utils import (
     load_nist_vectors,
     load_vectors_from_file,
     raises_unsupported_algorithm,
 )
 
 
@@ -191,26 +192,32 @@
             X25519PrivateKey.from_private_bytes(b"a" * 31)
 
         with pytest.raises(ValueError):
             X25519PrivateKey.from_private_bytes(b"a" * 33)
 
     def test_invalid_private_bytes(self, backend):
         key = X25519PrivateKey.generate()
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.Raw,
                 None,  # type: ignore[arg-type]
             )
+        with pytest.raises(ValueError):
+            key.private_bytes(
+                serialization.Encoding.Raw,
+                serialization.PrivateFormat.Raw,
+                DummyKeySerializationEncryption(),
+            )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.PKCS8,
-                None,  # type: ignore[arg-type]
+                DummyKeySerializationEncryption(),
             )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.PEM,
                 serialization.PrivateFormat.Raw,
                 serialization.NoEncryption(),
@@ -243,14 +250,21 @@
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.SMIME,
                 serialization.PrivateFormat.PKCS8,
                 serialization.NoEncryption(),
             )
 
+        with pytest.raises(ValueError):
+            key.private_bytes(
+                serialization.Encoding.PEM,
+                serialization.PrivateFormat.TraditionalOpenSSL,
+                serialization.NoEncryption(),
+            )
+
     def test_invalid_public_bytes(self, backend):
         key = X25519PrivateKey.generate().public_key()
         with pytest.raises(ValueError):
             key.public_bytes(
                 serialization.Encoding.Raw,
                 serialization.PublicFormat.SubjectPublicKeyInfo,
             )
@@ -313,7 +327,27 @@
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.Raw,
                 serialization.NoEncryption(),
             )
             == private_bytes
         )
+
+
+@pytest.mark.supported(
+    only_if=lambda backend: backend.x25519_supported(),
+    skip_message="Requires OpenSSL with X25519 support",
+)
+def test_public_key_equality(backend):
+    key_bytes = load_vectors_from_file(
+        os.path.join("asymmetric", "X25519", "x25519-pkcs8.der"),
+        lambda derfile: derfile.read(),
+        mode="rb",
+    )
+    key1 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key2 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key3 = X25519PrivateKey.generate().public_key()
+    assert key1 == key2
+    assert key1 != key3
+    assert key1 != object()
+    with pytest.raises(TypeError):
+        key1 < key2  # type: ignore[operator]
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_x448.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_x448.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from cryptography.exceptions import _Reasons
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric.x448 import (
     X448PrivateKey,
     X448PublicKey,
 )
 
+from ...doubles import DummyKeySerializationEncryption
 from ...utils import (
     load_nist_vectors,
     load_vectors_from_file,
     raises_unsupported_algorithm,
 )
 
 
@@ -196,26 +197,32 @@
             X448PrivateKey.from_private_bytes(b"a" * 55)
 
         with pytest.raises(ValueError):
             X448PrivateKey.from_private_bytes(b"a" * 57)
 
     def test_invalid_private_bytes(self, backend):
         key = X448PrivateKey.generate()
-        with pytest.raises(ValueError):
+        with pytest.raises(TypeError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.Raw,
                 None,  # type: ignore[arg-type]
             )
+        with pytest.raises(ValueError):
+            key.private_bytes(
+                serialization.Encoding.Raw,
+                serialization.PrivateFormat.Raw,
+                DummyKeySerializationEncryption(),
+            )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.PKCS8,
-                None,  # type: ignore[arg-type]
+                DummyKeySerializationEncryption(),
             )
 
         with pytest.raises(ValueError):
             key.private_bytes(
                 serialization.Encoding.PEM,
                 serialization.PrivateFormat.Raw,
                 serialization.NoEncryption(),
@@ -249,7 +256,27 @@
             key.private_bytes(
                 serialization.Encoding.Raw,
                 serialization.PrivateFormat.Raw,
                 serialization.NoEncryption(),
             )
             == private_bytes
         )
+
+
+@pytest.mark.supported(
+    only_if=lambda backend: backend.x448_supported(),
+    skip_message="Requires OpenSSL with X448 support",
+)
+def test_public_key_equality(backend):
+    key_bytes = load_vectors_from_file(
+        os.path.join("asymmetric", "X448", "x448-pkcs8.der"),
+        lambda derfile: derfile.read(),
+        mode="rb",
+    )
+    key1 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key2 = serialization.load_der_private_key(key_bytes, None).public_key()
+    key3 = X448PrivateKey.generate().public_key()
+    assert key1 == key2
+    assert key1 != key3
+    assert key1 != object()
+    with pytest.raises(TypeError):
+        key1 < key2  # type: ignore[operator]
```

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_x963_vectors.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_x963_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/test_x963kdf.py` & `cryptography-41.0.0/tests/hazmat/primitives/test_x963kdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/twofactor/test_hotp.py` & `cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_hotp.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/twofactor/test_totp.py` & `cryptography-41.0.0/tests/hazmat/primitives/twofactor/test_totp.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/hazmat/primitives/utils.py` & `cryptography-41.0.0/tests/hazmat/primitives/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,14 @@
 
 
 def base_hash_test(backend, algorithm, digest_size):
     m = hashes.Hash(algorithm, backend=backend)
     assert m.algorithm.digest_size == digest_size
     m_copy = m.copy()
     assert m != m_copy
-    assert m._ctx != m_copy._ctx
 
     m.update(b"abc")
     copy = m.copy()
     copy.update(b"123")
     m.update(b"123")
     assert copy.finalize() == m.finalize()
 
@@ -226,15 +225,14 @@
 
 
 def base_hmac_test(backend, algorithm):
     key = b"ab"
     h = hmac.HMAC(binascii.unhexlify(key), algorithm, backend=backend)
     h_copy = h.copy()
     assert h != h_copy
-    assert h._ctx != h_copy._ctx
 
 
 def generate_hmac_test(param_loader, path, file_names, algorithm):
     def test_hmac(self, backend, subtests):
         for params in _load_all_params(path, file_names, param_loader):
             with subtests.test():
                 hmac_test(backend, algorithm, params)
```

### Comparing `cryptography-40.0.2/tests/hazmat/test_oid.py` & `cryptography-41.0.0/tests/hazmat/test_oid.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/test_cryptography_utils.py` & `cryptography-41.0.0/tests/test_cryptography_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/test_fernet.py` & `cryptography-41.0.0/tests/test_fernet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 
 import base64
-import calendar
+import datetime
 import json
 import os
 import time
 
-import iso8601
 import pretend
 import pytest
 
 import cryptography_vectors
 from cryptography.fernet import Fernet, InvalidToken, MultiFernet
 from cryptography.hazmat.primitives.ciphers import algorithms, modes
 
@@ -42,29 +41,29 @@
         ("secret", "now", "iv", "src", "token"),
         "generate.json",
     )
     def test_generate(self, secret, now, iv, src, token, backend):
         f = Fernet(secret.encode("ascii"), backend=backend)
         actual_token = f._encrypt_from_parts(
             src.encode("ascii"),
-            calendar.timegm(iso8601.parse_date(now).utctimetuple()),
+            int(datetime.datetime.fromisoformat(now).timestamp()),
             bytes(iv),
         )
         assert actual_token == token.encode("ascii")
 
     @json_parametrize(
         ("secret", "now", "src", "ttl_sec", "token"),
         "verify.json",
     )
     def test_verify(
         self, secret, now, src, ttl_sec, token, backend, monkeypatch
     ):
         # secret & token are both str
         f = Fernet(secret.encode("ascii"), backend=backend)
-        current_time = calendar.timegm(iso8601.parse_date(now).utctimetuple())
+        current_time = int(datetime.datetime.fromisoformat(now).timestamp())
         payload = f.decrypt_at_time(
             token,  # str
             ttl=ttl_sec,
             current_time=current_time,
         )
         assert payload == src.encode("ascii")
 
@@ -82,15 +81,15 @@
 
         payload = f.decrypt(token.encode("ascii"), ttl=ttl_sec)  # bytes
         assert payload == src.encode("ascii")
 
     @json_parametrize(("secret", "token", "now", "ttl_sec"), "invalid.json")
     def test_invalid(self, secret, token, now, ttl_sec, backend, monkeypatch):
         f = Fernet(secret.encode("ascii"), backend=backend)
-        current_time = calendar.timegm(iso8601.parse_date(now).utctimetuple())
+        current_time = int(datetime.datetime.fromisoformat(now).timestamp())
         with pytest.raises(InvalidToken):
             f.decrypt_at_time(
                 token.encode("ascii"),
                 ttl=ttl_sec,
                 current_time=current_time,
             )
         monkeypatch.setattr(time, "time", lambda: current_time)
```

### Comparing `cryptography-40.0.2/tests/test_meta.py` & `cryptography-41.0.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/test_rust_utils.py` & `cryptography-41.0.0/tests/test_rust_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/test_utils.py` & `cryptography-41.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/test_warnings.py` & `cryptography-41.0.0/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/utils.py` & `cryptography-41.0.0/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 @contextmanager
 def raises_unsupported_algorithm(reason):
     with pytest.raises(UnsupportedAlgorithm) as exc_info:
         yield exc_info
 
-    assert exc_info.value._reason is reason
+    assert exc_info.value._reason == reason
 
 
 T = typing.TypeVar("T")
 
 
 def load_vectors_from_file(
     filename, loader: typing.Callable[..., T], mode="r"
@@ -239,17 +239,14 @@
 
             public_key_vector = collections.defaultdict(list)
             private_key_vector = collections.defaultdict(list)
             key = None
             attr = None
 
         if private_key_vector is None or public_key_vector is None:
-            # Random garbage to defeat CPython's peephole optimizer so that
-            # coverage records correctly: https://bugs.python.org/issue2506
-            1 + 1
             continue
 
         if line.startswith("# Private key"):
             key = private_key_vector
         elif line.startswith("# Public key"):
             key = public_key_vector
         elif line.startswith("# Modulus:"):
```

### Comparing `cryptography-40.0.2/tests/wycheproof/test_aes.py` & `cryptography-41.0.0/tests/wycheproof/test_aes.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_chacha20poly1305.py` & `cryptography-41.0.0/tests/wycheproof/test_chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_cmac.py` & `cryptography-41.0.0/tests/wycheproof/test_cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_dsa.py` & `cryptography-41.0.0/tests/wycheproof/test_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_ecdh.py` & `cryptography-41.0.0/tests/wycheproof/test_ecdh.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_ecdsa.py` & `cryptography-41.0.0/tests/wycheproof/test_ecdsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_eddsa.py` & `cryptography-41.0.0/tests/wycheproof/test_eddsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_hkdf.py` & `cryptography-41.0.0/tests/wycheproof/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_hmac.py` & `cryptography-41.0.0/tests/wycheproof/test_hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_keywrap.py` & `cryptography-41.0.0/tests/wycheproof/test_keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_rsa.py` & `cryptography-41.0.0/tests/wycheproof/test_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_x25519.py` & `cryptography-41.0.0/tests/wycheproof/test_x25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/test_x448.py` & `cryptography-41.0.0/tests/wycheproof/test_x448.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/wycheproof/utils.py` & `cryptography-41.0.0/tests/wycheproof/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/x509/test_name.py` & `cryptography-41.0.0/tests/x509/test_name.py`

 * *Files identical despite different names*

### Comparing `cryptography-40.0.2/tests/x509/test_ocsp.py` & `cryptography-41.0.0/tests/x509/test_ocsp.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,26 @@
         assert len(req.extensions) == 1
         ext = req.extensions[0]
         assert ext.critical is False
         assert ext.value == x509.OCSPNonce(
             b"{\x80Z\x1d7&\xb8\xb8OH\xd2\xf8\xbf\xd7-\xfd"
         )
 
+    def test_load_request_with_acceptable_responses(self):
+        req = _load_data(
+            os.path.join("x509", "ocsp", "req-acceptable-responses.der"),
+            ocsp.load_der_ocsp_request,
+        )
+        assert len(req.extensions) == 1
+        ext = req.extensions[0]
+        assert ext.critical is False
+        assert ext.value == x509.OCSPAcceptableResponses(
+            [x509.ObjectIdentifier("1.3.6.1.5.5.7.48.1.1")]
+        )
+
     def test_load_request_with_unknown_extension(self):
         req = _load_data(
             os.path.join("x509", "ocsp", "req-ext-unknown-oid.der"),
             ocsp.load_der_ocsp_request,
         )
         assert len(req.extensions) == 1
         ext = req.extensions[0]
```

### Comparing `cryptography-40.0.2/tests/x509/test_x509.py` & `cryptography-41.0.0/tests/x509/test_x509.py`

 * *Files 5% similar despite different names*

```diff
@@ -725,37 +725,109 @@
         # make sure get_revoked_certificate_by_serial_number doesn't affect
         # ordering after being invoked
         crl.get_revoked_certificate_by_serial_number(500)
         assert crl[0].serial_number == 2
         assert crl[2].serial_number == 3
 
 
+@pytest.mark.supported(
+    only_if=lambda backend: (
+        not backend._lib.CRYPTOGRAPHY_IS_LIBRESSL
+        and not backend._lib.CRYPTOGRAPHY_IS_BORINGSSL
+        and not backend._lib.CRYPTOGRAPHY_OPENSSL_LESS_THAN_111E
+    ),
+    skip_message="Does not support RSA PSS loading",
+)
 class TestRSAPSSCertificate:
-    @pytest.mark.supported(
-        only_if=lambda backend: (
-            not backend._lib.CRYPTOGRAPHY_IS_LIBRESSL
-            and not backend._lib.CRYPTOGRAPHY_IS_BORINGSSL
-            and not backend._lib.CRYPTOGRAPHY_OPENSSL_LESS_THAN_111E
-        ),
-        skip_message="Does not support RSA PSS loading",
-    )
     def test_load_cert_pub_key(self, backend):
         cert = _load_cert(
             os.path.join("x509", "custom", "rsa_pss_cert.pem"),
             x509.load_pem_x509_certificate,
         )
         assert isinstance(cert, x509.Certificate)
         expected_pub_key = _load_cert(
             os.path.join("asymmetric", "PKCS8", "rsa_pss_2048_pub.der"),
             serialization.load_der_public_key,
         )
         assert isinstance(expected_pub_key, rsa.RSAPublicKey)
         pub_key = cert.public_key()
         assert isinstance(pub_key, rsa.RSAPublicKey)
-        assert pub_key.public_numbers() == expected_pub_key.public_numbers()
+        assert pub_key == expected_pub_key
+        pss = cert.signature_algorithm_parameters
+        assert isinstance(pss, padding.PSS)
+        assert isinstance(pss._mgf, padding.MGF1)
+        assert isinstance(pss._mgf._algorithm, hashes.SHA256)
+        assert pss._salt_length == 222
+        assert isinstance(cert.signature_hash_algorithm, hashes.SHA256)
+        pub_key.verify(
+            cert.signature,
+            cert.tbs_certificate_bytes,
+            pss,
+            cert.signature_hash_algorithm,
+        )
+
+    def test_load_pss_cert_no_null(self, backend):
+        """
+        This test verifies that PSS certs where the hash algorithm
+        identifiers have no trailing null still load properly. LibreSSL
+        generates certs like this.
+        """
+        cert = _load_cert(
+            os.path.join("x509", "custom", "rsa_pss_sha256_no_null.pem"),
+            x509.load_pem_x509_certificate,
+        )
+        assert isinstance(cert, x509.Certificate)
+        pss = cert.signature_algorithm_parameters
+        assert isinstance(pss, padding.PSS)
+        assert isinstance(pss._mgf, padding.MGF1)
+        assert isinstance(pss._mgf._algorithm, hashes.SHA256)
+        assert isinstance(cert.signature_hash_algorithm, hashes.SHA256)
+
+    def test_load_pss_sha1_mgf1_sha1(self, backend):
+        cert = _load_cert(
+            os.path.join("x509", "ee-pss-sha1-cert.pem"),
+            x509.load_pem_x509_certificate,
+        )
+        assert isinstance(cert, x509.Certificate)
+        pub_key = cert.public_key()
+        assert isinstance(pub_key, rsa.RSAPublicKey)
+        pss = cert.signature_algorithm_parameters
+        assert isinstance(pss, padding.PSS)
+        assert isinstance(pss._mgf, padding.MGF1)
+        assert isinstance(pss._mgf._algorithm, hashes.SHA1)
+        assert pss._salt_length == 20
+        assert isinstance(cert.signature_hash_algorithm, hashes.SHA1)
+
+    def test_invalid_mgf(self, backend):
+        cert = _load_cert(
+            os.path.join("x509", "custom", "rsa_pss_cert_invalid_mgf.der"),
+            x509.load_der_x509_certificate,
+        )
+        with pytest.raises(ValueError):
+            cert.signature_algorithm_parameters
+
+    def test_unsupported_mgf_hash(self, backend):
+        cert = _load_cert(
+            os.path.join(
+                "x509", "custom", "rsa_pss_cert_unsupported_mgf_hash.der"
+            ),
+            x509.load_der_x509_certificate,
+        )
+        with pytest.raises(UnsupportedAlgorithm):
+            cert.signature_algorithm_parameters
+
+    def test_no_sig_params(self, backend):
+        cert = _load_cert(
+            os.path.join("x509", "custom", "rsa_pss_cert_no_sig_params.der"),
+            x509.load_der_x509_certificate,
+        )
+        with pytest.raises(ValueError):
+            cert.signature_algorithm_parameters
+        with pytest.raises(ValueError):
+            cert.signature_hash_algorithm
 
 
 class TestRSACertificate:
     def test_load_pem_cert(self, backend):
         cert = _load_cert(
             os.path.join("x509", "custom", "post2000utctime.pem"),
             x509.load_pem_x509_certificate,
@@ -764,14 +836,36 @@
         assert cert.serial_number == 11559813051657483483
         fingerprint = binascii.hexlify(cert.fingerprint(hashes.SHA1()))
         assert fingerprint == b"2b619ed04bfc9c3b08eb677d272192286a0947a8"
         assert isinstance(cert.signature_hash_algorithm, hashes.SHA1)
         assert (
             cert.signature_algorithm_oid == SignatureAlgorithmOID.RSA_WITH_SHA1
         )
+        assert isinstance(
+            cert.signature_algorithm_parameters, padding.PKCS1v15
+        )
+
+    def test_check_pkcs1_signature_algorithm_parameters(self, backend):
+        cert = _load_cert(
+            os.path.join("x509", "custom", "ca", "rsa_ca.pem"),
+            x509.load_pem_x509_certificate,
+        )
+        assert isinstance(cert, x509.Certificate)
+        assert isinstance(
+            cert.signature_algorithm_parameters, padding.PKCS1v15
+        )
+        pk = cert.public_key()
+        assert isinstance(pk, rsa.RSAPublicKey)
+        assert cert.signature_hash_algorithm is not None
+        pk.verify(
+            cert.signature,
+            cert.tbs_certificate_bytes,
+            cert.signature_algorithm_parameters,
+            cert.signature_hash_algorithm,
+        )
 
     def test_load_legacy_pem_header(self, backend):
         cert = _load_cert(
             os.path.join("x509", "cryptography.io.old_header.pem"),
             x509.load_pem_x509_certificate,
         )
         assert isinstance(cert, x509.Certificate)
@@ -934,14 +1028,28 @@
         public_key.verify(
             cert.signature,
             cert.tbs_certificate_bytes,
             padding.PKCS1v15(),
             cert.signature_hash_algorithm,
         )
 
+    def test_tbs_precertificate_bytes_duplicate_extensions_raises(
+        self, backend
+    ):
+        cert = _load_cert(
+            os.path.join("x509", "custom", "two_basic_constraints.pem"),
+            x509.load_pem_x509_certificate,
+        )
+
+        with pytest.raises(
+            x509.DuplicateExtension,
+            match="Duplicate 2.5.29.19 extension found",
+        ):
+            cert.tbs_precertificate_bytes
+
     def test_tbs_precertificate_bytes_no_extensions_raises(self, backend):
         cert = _load_cert(
             os.path.join("x509", "v1_cert.pem"),
             x509.load_pem_x509_certificate,
         )
 
         with pytest.raises(
@@ -1246,14 +1354,33 @@
             _load_cert(
                 os.path.join("x509", "custom", "invalid_version.pem"),
                 x509.load_pem_x509_certificate,
             )
 
         assert exc.value.parsed_version == 7
 
+    def test_invalid_visiblestring_in_explicit_text(self, backend):
+        cert = _load_cert(
+            os.path.join(
+                "x509",
+                "belgian-eid-invalid-visiblestring.pem",
+            ),
+            x509.load_pem_x509_certificate,
+        )
+        with pytest.warns(utils.DeprecatedIn41):
+            cp = cert.extensions.get_extension_for_class(
+                x509.CertificatePolicies
+            ).value
+        assert isinstance(cp, x509.CertificatePolicies)
+        assert cp[0].policy_qualifiers[1].explicit_text == (
+            "Gebruik onderworpen aan aansprakelijkheidsbeperkingen, zie CPS "
+            "- Usage soumis à des limitations de responsabilité, voir CPS - "
+            "Verwendung unterliegt Haftungsbeschränkungen, gemäss CPS"
+        )
+
     def test_eq(self, backend):
         cert = _load_cert(
             os.path.join("x509", "custom", "post2000utctime.pem"),
             x509.load_pem_x509_certificate,
         )
         cert2 = _load_cert(
             os.path.join("x509", "custom", "post2000utctime.pem"),
@@ -1444,14 +1571,58 @@
         )
         ext = cert.extensions.get_extension_for_class(x509.TLSFeature)
         assert ext.critical is False
         assert ext.value == x509.TLSFeature(
             [x509.TLSFeatureType.status_request]
         )
 
+    def test_verify_directly_issued_by_rsa_pss(
+        self, rsa_key_2048: rsa.RSAPrivateKey
+    ):
+        subject_private_key = RSA_KEY_2048_ALT.private_key(
+            unsafe_skip_rsa_key_validation=True
+        )
+
+        builder = (
+            x509.CertificateBuilder()
+            .subject_name(
+                x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, "PyCA CA")])
+            )
+            .issuer_name(
+                x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, "PyCA CA")])
+            )
+            .public_key(rsa_key_2048.public_key())
+            .serial_number(1)
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2030, 1, 1))
+        )
+        ca = builder.sign(rsa_key_2048, hashes.SHA256())
+        builder = (
+            x509.CertificateBuilder()
+            .subject_name(
+                x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, "leaf")])
+            )
+            .issuer_name(
+                x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, "PyCA CA")])
+            )
+            .public_key(subject_private_key.public_key())
+            .serial_number(100)
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2025, 1, 1))
+        )
+        cert = builder.sign(
+            rsa_key_2048,
+            hashes.SHA256(),
+            rsa_padding=padding.PSS(
+                padding.MGF1(hashes.SHA256()),
+                salt_length=padding.PSS.DIGEST_LENGTH,
+            ),
+        )
+        cert.verify_directly_issued_by(ca)
+
     def test_verify_directly_issued_by_rsa(
         self, rsa_key_2048: rsa.RSAPrivateKey
     ):
         issuer_private_key = rsa_key_2048
         subject_private_key = RSA_KEY_2048_ALT.private_key(
             unsafe_skip_rsa_key_validation=True
         )
@@ -2305,14 +2476,203 @@
             cert.public_bytes(serialization.Encoding.DER)
         )
         # UTC TIME
         assert parsed.not_before_tag == 0x17
         # GENERALIZED TIME
         assert parsed.not_after_tag == 0x18
 
+    def test_rdns_preserve_iteration_order(
+        self, rsa_key_2048: rsa.RSAPrivateKey, backend
+    ):
+        """
+        This test checks that RDN ordering is consistent when loading
+        data from a certificate. Since the underlying RDN is an ASN.1
+        set these values get lexicographically ordered on encode and
+        the parsed value won't necessarily be in the same order as
+        the originally provided list. However, we want to make sure
+        that the order is always consistent since it confuses people
+        when it isn't.
+        """
+        name = x509.Name(
+            [
+                x509.RelativeDistinguishedName(
+                    [
+                        x509.NameAttribute(NameOID.TITLE, "Test"),
+                        x509.NameAttribute(NameOID.COMMON_NAME, "Multivalue"),
+                        x509.NameAttribute(NameOID.SURNAME, "RDNs"),
+                    ]
+                ),
+            ]
+        )
+
+        cert = (
+            x509.CertificateBuilder()
+            .serial_number(1)
+            .issuer_name(name)
+            .subject_name(name)
+            .public_key(rsa_key_2048.public_key())
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2038, 1, 1))
+            .sign(rsa_key_2048, hashes.SHA256(), backend)
+        )
+        loaded_cert = x509.load_pem_x509_certificate(
+            cert.public_bytes(encoding=serialization.Encoding.PEM)
+        )
+        assert next(iter(loaded_cert.subject.rdns[0])) == x509.NameAttribute(
+            NameOID.SURNAME, "RDNs"
+        )
+
+    @pytest.mark.parametrize(
+        ("alg", "mgf_alg"),
+        [
+            (hashes.SHA512(), hashes.SHA256()),
+            (hashes.SHA3_512(), hashes.SHA3_256()),
+        ],
+    )
+    def test_sign_pss(
+        self, rsa_key_2048: rsa.RSAPrivateKey, alg, mgf_alg, backend
+    ):
+        if not backend.signature_hash_supported(alg):
+            pytest.skip(f"{alg} signature not supported")
+        builder = (
+            x509.CertificateBuilder()
+            .subject_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .issuer_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .public_key(rsa_key_2048.public_key())
+            .serial_number(777)
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2038, 1, 1))
+        )
+        pss = padding.PSS(
+            mgf=padding.MGF1(mgf_alg), salt_length=alg.digest_size
+        )
+        cert = builder.sign(rsa_key_2048, alg, rsa_padding=pss)
+        pk = cert.public_key()
+        assert isinstance(pk, rsa.RSAPublicKey)
+        assert isinstance(cert.signature_hash_algorithm, type(alg))
+        cert_params = cert.signature_algorithm_parameters
+        assert isinstance(cert_params, padding.PSS)
+        assert cert_params._salt_length == pss._salt_length
+        assert isinstance(cert_params._mgf, padding.MGF1)
+        assert isinstance(cert_params._mgf._algorithm, type(mgf_alg))
+        pk.verify(
+            cert.signature,
+            cert.tbs_certificate_bytes,
+            cert_params,
+            alg,
+        )
+
+    @pytest.mark.parametrize(
+        ("padding_len", "computed_len"),
+        [
+            (padding.PSS.MAX_LENGTH, 222),
+            (padding.PSS.DIGEST_LENGTH, 32),
+        ],
+    )
+    def test_sign_pss_length_options(
+        self,
+        rsa_key_2048: rsa.RSAPrivateKey,
+        padding_len,
+        computed_len,
+        backend,
+    ):
+        builder = (
+            x509.CertificateBuilder()
+            .subject_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .issuer_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .public_key(rsa_key_2048.public_key())
+            .serial_number(777)
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2038, 1, 1))
+        )
+        pss = padding.PSS(
+            mgf=padding.MGF1(hashes.SHA256()), salt_length=padding_len
+        )
+        cert = builder.sign(rsa_key_2048, hashes.SHA256(), rsa_padding=pss)
+        assert isinstance(cert.signature_algorithm_parameters, padding.PSS)
+        assert cert.signature_algorithm_parameters._salt_length == computed_len
+
+    def test_sign_pss_auto_unsupported(
+        self, rsa_key_2048: rsa.RSAPrivateKey, backend
+    ):
+        builder = (
+            x509.CertificateBuilder()
+            .subject_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .issuer_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .public_key(rsa_key_2048.public_key())
+            .serial_number(777)
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2038, 1, 1))
+        )
+        pss = padding.PSS(
+            mgf=padding.MGF1(hashes.SHA256()), salt_length=padding.PSS.AUTO
+        )
+        with pytest.raises(TypeError):
+            builder.sign(rsa_key_2048, hashes.SHA256(), rsa_padding=pss)
+
+    def test_sign_invalid_padding(
+        self, rsa_key_2048: rsa.RSAPrivateKey, backend
+    ):
+        builder = (
+            x509.CertificateBuilder()
+            .subject_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .issuer_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .public_key(rsa_key_2048.public_key())
+            .serial_number(777)
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2038, 1, 1))
+        )
+        with pytest.raises(TypeError):
+            builder.sign(
+                rsa_key_2048,
+                hashes.SHA256(),
+                rsa_padding=b"notapadding",  # type: ignore[arg-type]
+            )
+        eckey = ec.generate_private_key(ec.SECP256R1())
+        with pytest.raises(TypeError):
+            builder.sign(
+                eckey, hashes.SHA256(), rsa_padding=padding.PKCS1v15()
+            )
+
+    def test_sign_pss_hash_none(
+        self, rsa_key_2048: rsa.RSAPrivateKey, backend
+    ):
+        builder = (
+            x509.CertificateBuilder()
+            .subject_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .issuer_name(
+                x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
+            )
+            .public_key(rsa_key_2048.public_key())
+            .serial_number(777)
+            .not_valid_before(datetime.datetime(2020, 1, 1))
+            .not_valid_after(datetime.datetime(2038, 1, 1))
+        )
+        pss = padding.PSS(mgf=padding.MGF1(hashes.SHA256()), salt_length=32)
+        with pytest.raises(TypeError):
+            builder.sign(rsa_key_2048, None, rsa_padding=pss)
+
     def test_no_subject_name(self, rsa_key_2048: rsa.RSAPrivateKey, backend):
         subject_private_key = rsa_key_2048
         builder = (
             x509.CertificateBuilder()
             .serial_number(777)
             .issuer_name(
                 x509.Name([x509.NameAttribute(NameOID.COUNTRY_NAME, "US")])
@@ -4576,14 +4936,15 @@
         cert = _load_cert(
             os.path.join("x509", "custom", "dsa_selfsigned_ca.pem"),
             x509.load_pem_x509_certificate,
         )
         assert isinstance(cert.signature_hash_algorithm, hashes.SHA1)
         public_key = cert.public_key()
         assert isinstance(public_key, dsa.DSAPublicKey)
+        assert cert.signature_algorithm_parameters is None
         num = public_key.public_numbers()
         assert num.y == int(
             "4c08bfe5f2d76649c80acf7d431f6ae2124b217abc8c9f6aca776ddfa94"
             "53b6656f13e543684cd5f6431a314377d2abfa068b7080cb8ddc065afc2"
             "dea559f0b584c97a2b235b9b69b46bc6de1aed422a6f341832618bcaae2"
             "198aba388099dafb05ff0b5efecb3b0ae169a62e1c72022af50ae68af3b"
             "033c18e6eec1f7df4692c456ccafb79cc7e08da0a5786e9816ceda651d6"
@@ -4824,14 +5185,23 @@
         )
         assert num.y == int(
             "ec0770f5cf842e40839ce83f416d3badd3a4145936789d0343ee10136c7"
             "2deae88a7a16bb543ce67dc23ff031ca3e23e",
             16,
         )
         assert isinstance(num.curve, ec.SECP384R1)
+        assert isinstance(cert.signature_algorithm_parameters, ec.ECDSA)
+        assert isinstance(
+            cert.signature_algorithm_parameters.algorithm, hashes.SHA384
+        )
+        public_key.verify(
+            cert.signature,
+            cert.tbs_certificate_bytes,
+            cert.signature_algorithm_parameters,
+        )
 
     def test_load_bitstring_dn(self, backend):
         cert = _load_cert(
             os.path.join("x509", "scottishpower-bitstring-dn.pem"),
             x509.load_pem_x509_certificate,
         )
         assert cert.subject == x509.Name(
@@ -4857,14 +5227,30 @@
             x509.load_pem_x509_certificate,
         )
         with pytest.raises(ValueError, match="Long-form"):
             cert.subject
         with pytest.raises(ValueError, match="Long-form"):
             cert.issuer
 
+    def test_ms_certificate_template(self, backend):
+        cert = _load_cert(
+            os.path.join("x509", "custom", "ms-certificate-template.pem"),
+            x509.load_pem_x509_certificate,
+        )
+        ext = cert.extensions.get_extension_for_class(
+            x509.MSCertificateTemplate
+        )
+        tpl = ext.value
+        assert isinstance(tpl, x509.MSCertificateTemplate)
+        assert tpl == x509.MSCertificateTemplate(
+            template_id=x509.ObjectIdentifier("1.2.3.4.5.6.7.8.9.0"),
+            major_version=1,
+            minor_version=None,
+        )
+
     def test_signature(self, backend):
         cert = _load_cert(
             os.path.join("x509", "ecdsa_root.pem"),
             x509.load_pem_x509_certificate,
         )
         assert cert.signature == binascii.unhexlify(
             b"3065023100adbcf26c3f124ad12d39c30a099773f488368c8827bbe6888d5085"
@@ -5551,14 +5937,15 @@
         public_key = cert.public_key()
         assert isinstance(public_key, ed25519.Ed25519PublicKey)
         public_key.verify(cert.signature, cert.tbs_certificate_bytes)
         assert isinstance(cert, x509.Certificate)
         assert cert.serial_number == 9579446940964433301
         assert cert.signature_hash_algorithm is None
         assert cert.signature_algorithm_oid == SignatureAlgorithmOID.ED25519
+        assert cert.signature_algorithm_parameters is None
 
     def test_deepcopy(self, backend):
         cert = _load_cert(
             os.path.join("x509", "ed25519", "root-ed25519.pem"),
             x509.load_pem_x509_certificate,
         )
         assert copy.deepcopy(cert) is cert
@@ -5596,14 +5983,15 @@
         public_key = cert.public_key()
         assert isinstance(public_key, ed448.Ed448PublicKey)
         public_key.verify(cert.signature, cert.tbs_certificate_bytes)
         assert isinstance(cert, x509.Certificate)
         assert cert.serial_number == 448
         assert cert.signature_hash_algorithm is None
         assert cert.signature_algorithm_oid == SignatureAlgorithmOID.ED448
+        assert cert.signature_algorithm_parameters is None
 
     def test_verify_directly_issued_by_ed448(self, backend):
         issuer_private_key = ed448.Ed448PrivateKey.generate()
         subject_private_key = ed448.Ed448PrivateKey.generate()
         ca, cert = _generate_ca_and_leaf(
             issuer_private_key, subject_private_key
         )
```

### Comparing `cryptography-40.0.2/tests/x509/test_x509_crlbuilder.py` & `cryptography-41.0.0/tests/x509/test_x509_crlbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,14 +520,18 @@
                 private_key,
                 object(),  # type:ignore[arg-type]
                 backend,
             )
         with pytest.raises(ValueError):
             builder.sign(private_key, hashes.SHA256(), backend)
 
+    @pytest.mark.supported(
+        only_if=lambda backend: backend.dsa_supported(),
+        skip_message="Requires OpenSSL with DSA support",
+    )
     def test_sign_dsa_key(self, backend):
         private_key = DSA_KEY_2048.private_key(backend)
         invalidity_date = x509.InvalidityDate(
             datetime.datetime(2002, 1, 1, 0, 0)
         )
         ian = x509.IssuerAlternativeName(
             [x509.UniformResourceIdentifier("https://cryptography.io")]
```

### Comparing `cryptography-40.0.2/tests/x509/test_x509_ext.py` & `cryptography-41.0.0/tests/x509/test_x509_ext.py`

 * *Files 0% similar despite different names*

```diff
@@ -6128,14 +6128,164 @@
         assert hash(nonce1) != hash(nonce3)
 
     def test_public_bytes(self):
         ext = x509.OCSPNonce(b"0" * 5)
         assert ext.public_bytes() == b"\x04\x0500000"
 
 
+class TestOCSPAcceptableResponses:
+    def test_invalid_types(self):
+        with pytest.raises(TypeError):
+            x509.OCSPAcceptableResponses(38)  # type:ignore[arg-type]
+        with pytest.raises(TypeError):
+            x509.OCSPAcceptableResponses([38])  # type:ignore[list-item]
+
+    def test_eq(self):
+        acceptable_responses1 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.3")]
+        )
+        acceptable_responses2 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.3")]
+        )
+        assert acceptable_responses1 == acceptable_responses2
+
+    def test_ne(self):
+        acceptable_responses1 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.3")]
+        )
+        acceptable_responses2 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.4")]
+        )
+        assert acceptable_responses1 != acceptable_responses2
+        assert acceptable_responses1 != object()
+
+    def test_repr(self):
+        acceptable_responses = x509.OCSPAcceptableResponses([])
+        assert (
+            repr(acceptable_responses)
+            == "<OCSPAcceptableResponses(responses=[])>"
+        )
+
+    def test_hash(self):
+        acceptable_responses1 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.3")]
+        )
+        acceptable_responses2 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.3")]
+        )
+        acceptable_responses3 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.4")]
+        )
+
+        assert hash(acceptable_responses1) == hash(acceptable_responses2)
+        assert hash(acceptable_responses1) != hash(acceptable_responses3)
+
+    def test_iter(self):
+        acceptable_responses1 = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.2.3")]
+        )
+
+        assert list(acceptable_responses1) == [ObjectIdentifier("1.2.3")]
+
+    def test_public_bytes(self):
+        ext = x509.OCSPAcceptableResponses([])
+        assert ext.public_bytes() == b"\x30\x00"
+
+        ext = x509.OCSPAcceptableResponses(
+            [ObjectIdentifier("1.3.6.1.5.5.7.48.1.1")]
+        )
+        assert (
+            ext.public_bytes()
+            == b"\x30\x0b\x06\t+\x06\x01\x05\x05\x07\x30\x01\x01"
+        )
+
+
+class TestMSCertificateTemplate:
+    def test_invalid_type(self):
+        with pytest.raises(TypeError):
+            x509.MSCertificateTemplate(
+                "notanoid", None, None  # type:ignore[arg-type]
+            )
+        oid = x509.ObjectIdentifier("1.2.3.4")
+        with pytest.raises(TypeError):
+            x509.MSCertificateTemplate(
+                oid, "notanint", None  # type:ignore[arg-type]
+            )
+        with pytest.raises(TypeError):
+            x509.MSCertificateTemplate(
+                oid, None, "notanint"  # type:ignore[arg-type]
+            )
+
+    def test_eq(self):
+        template1 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, None
+        )
+        template2 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, None
+        )
+        assert template1 == template2
+
+    def test_ne(self):
+        template1 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, None
+        )
+        template2 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), 1, None
+        )
+        template3 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, 1
+        )
+        template4 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3"), None, None
+        )
+        assert template1 != template2
+        assert template1 != template3
+        assert template1 != template4
+        assert template1 != object()
+
+    def test_repr(self):
+        template = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, None
+        )
+        assert repr(template) == (
+            "<MSCertificateTemplate(template_id=<ObjectIdentifier(oid=1.2.3.4,"
+            " name=Unknown OID)>, major_version=None, minor_version=None)>"
+        )
+
+    def test_hash(self):
+        template1 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, None
+        )
+        template2 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, None
+        )
+        template3 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, 1
+        )
+        template4 = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3"), None, None
+        )
+
+        assert hash(template1) == hash(template2)
+        assert hash(template1) != hash(template3)
+        assert hash(template1) != hash(template4)
+
+    def test_public_bytes(self):
+        ext = x509.MSCertificateTemplate(
+            ObjectIdentifier("1.2.3.4"), None, None
+        )
+        assert ext.public_bytes() == b"0\x05\x06\x03*\x03\x04"
+
+        ext = x509.MSCertificateTemplate(ObjectIdentifier("1.2.3.4"), 1, 0)
+        assert (
+            ext.public_bytes()
+            == b"0\x0b\x06\x03*\x03\x04\x02\x01\x01\x02\x01\x00"
+        )
+
+
 def test_all_extension_oid_members_have_names_defined():
     for oid in dir(ExtensionOID):
         if oid.startswith("__"):
             continue
         assert getattr(ExtensionOID, oid) in _OID_NAMES
```

### Comparing `cryptography-40.0.2/tests/x509/test_x509_revokedcertbuilder.py` & `cryptography-41.0.0/tests/x509/test_x509_revokedcertbuilder.py`

 * *Files identical despite different names*

