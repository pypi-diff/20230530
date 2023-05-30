# Comparing `tmp/asyauth-0.0.8.tar.gz` & `tmp/asyauth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyauth-0.0.8.tar", last modified: Sat Nov 26 20:54:31 2022, max compression
+gzip compressed data, was "asyauth-0.0.9.tar", last modified: Sun Nov 27 22:15:50 2022, max compression
```

## Comparing `asyauth-0.0.8.tar` & `asyauth-0.0.9.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.644238 asyauth-0.0.8/
--rw-rw-r--   0 root         (0) root         (0)     1064 2022-08-24 21:27:42.000000 asyauth-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      469 2022-11-26 20:54:31.644238 asyauth-0.0.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        9 2022-08-24 21:27:42.000000 asyauth-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.616238 asyauth-0.0.8/asyauth/
--rw-rw-r--   0 root         (0) root         (0)      357 2022-08-13 17:54:19.000000 asyauth-0.0.8/asyauth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      129 2022-11-26 19:36:45.000000 asyauth-0.0.8/asyauth/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.616238 asyauth-0.0.8/asyauth/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 16:49:33.000000 asyauth-0.0.8/asyauth/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1702 2022-10-13 20:01:37.000000 asyauth-0.0.8/asyauth/common/clientauthalgo.py
--rw-rw-r--   0 root         (0) root         (0)      959 2022-10-13 19:23:31.000000 asyauth-0.0.8/asyauth/common/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.616238 asyauth-0.0.8/asyauth/common/credentials/
--rw-rw-r--   0 root         (0) root         (0)     5460 2022-11-18 18:54:16.000000 asyauth-0.0.8/asyauth/common/credentials/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1019 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/credentials/credssp.py
--rw-rw-r--   0 root         (0) root         (0)     6502 2022-11-26 19:36:45.000000 asyauth-0.0.8/asyauth/common/credentials/kerberos.py
--rw-rw-r--   0 root         (0) root         (0)     3220 2022-11-26 19:36:45.000000 asyauth-0.0.8/asyauth/common/credentials/ntlm.py
--rw-rw-r--   0 root         (0) root         (0)     1310 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/credentials/spnego.py
--rw-rw-r--   0 root         (0) root         (0)     1314 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/credentials/spnegoex.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.620238 asyauth-0.0.8/asyauth/common/subprotocols/
--rw-rw-r--   0 root         (0) root         (0)     1134 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/subprotocols/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      529 2022-10-14 19:14:23.000000 asyauth-0.0.8/asyauth/common/subprotocols/custom.py
--rw-rw-r--   0 root         (0) root         (0)      312 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/subprotocols/native.py
--rw-rw-r--   0 root         (0) root         (0)      421 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/subprotocols/sspi.py
--rw-rw-r--   0 root         (0) root         (0)     1434 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/subprotocols/sspiproxy.py
--rw-rw-r--   0 root         (0) root         (0)      309 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/common/subprotocols/wsnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.624238 asyauth-0.0.8/asyauth/common/winapi/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 17:51:18.000000 asyauth-0.0.8/asyauth/common/winapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    17344 2022-10-05 21:52:44.000000 asyauth-0.0.8/asyauth/common/winapi/constants.py
--rw-rw-r--   0 root         (0) root         (0)    12418 2022-10-05 21:52:44.000000 asyauth-0.0.8/asyauth/common/winapi/functiondefs.py
--rw-rw-r--   0 root         (0) root         (0)     1413 2022-10-05 21:52:44.000000 asyauth-0.0.8/asyauth/common/winapi/token.py
--rw-rw-r--   0 root         (0) root         (0)     2902 2022-10-05 21:52:44.000000 asyauth-0.0.8/asyauth/common/winapi/winsspi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.624238 asyauth-0.0.8/asyauth/protocols/
--rw-rw-r--   0 root         (0) root         (0)     1259 2022-08-12 23:03:35.000000 asyauth-0.0.8/asyauth/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.624238 asyauth-0.0.8/asyauth/protocols/credssp/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/credssp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.624238 asyauth-0.0.8/asyauth/protocols/credssp/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 13:15:53.000000 asyauth-0.0.8/asyauth/protocols/credssp/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5869 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/credssp/client/native.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.624238 asyauth-0.0.8/asyauth/protocols/credssp/messages/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/credssp/messages/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4460 2022-08-11 16:40:26.000000 asyauth-0.0.8/asyauth/protocols/credssp/messages/asn1_structs.py
--rw-rw-r--   0 root         (0) root         (0)     4014 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/credssp/messages/remcredguard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.624238 asyauth-0.0.8/asyauth/protocols/kerberos/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/kerberos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.628238 asyauth-0.0.8/asyauth/protocols/kerberos/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-12 22:50:09.000000 asyauth-0.0.8/asyauth/protocols/kerberos/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7483 2022-10-05 21:52:44.000000 asyauth-0.0.8/asyauth/protocols/kerberos/client/native.py
--rw-rw-r--   0 root         (0) root         (0)     3706 2022-10-05 21:52:44.000000 asyauth-0.0.8/asyauth/protocols/kerberos/client/sspi.py
--rw-rw-r--   0 root         (0) root         (0)     4848 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/kerberos/client/sspiproxy.py
--rw-rw-r--   0 root         (0) root         (0)     4712 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/kerberos/client/wsnet.py
--rw-rw-r--   0 root         (0) root         (0)    15484 2022-08-14 22:55:02.000000 asyauth-0.0.8/asyauth/protocols/kerberos/gssapi.py
--rw-rw-r--   0 root         (0) root         (0)    12420 2022-08-14 22:55:23.000000 asyauth-0.0.8/asyauth/protocols/kerberos/gssapismb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.628238 asyauth-0.0.8/asyauth/protocols/ntlm/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.632238 asyauth-0.0.8/asyauth/protocols/ntlm/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-12 22:43:20.000000 asyauth-0.0.8/asyauth/protocols/ntlm/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15672 2022-10-13 19:41:35.000000 asyauth-0.0.8/asyauth/protocols/ntlm/client/native.py
--rw-rw-r--   0 root         (0) root         (0)     3329 2022-10-05 21:52:44.000000 asyauth-0.0.8/asyauth/protocols/ntlm/client/sspi.py
--rw-rw-r--   0 root         (0) root         (0)     2546 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/client/sspiproxy.py
--rw-rw-r--   0 root         (0) root         (0)     2420 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/client/wsnet.py
--rw-rw-r--   0 root         (0) root         (0)    18300 2022-11-18 19:14:04.000000 asyauth-0.0.8/asyauth/protocols/ntlm/creds_calc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.632238 asyauth-0.0.8/asyauth/protocols/ntlm/messages/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/messages/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9287 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/messages/authenticate.py
--rw-rw-r--   0 root         (0) root         (0)     4869 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/messages/challenge.py
--rw-rw-r--   0 root         (0) root         (0)     5714 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/messages/negotiate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.636238 asyauth-0.0.8/asyauth/protocols/ntlm/structures/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4298 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/avpair.py
--rw-rw-r--   0 root         (0) root         (0)     6847 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/challenge_response.py
--rw-rw-r--   0 root         (0) root         (0)      851 2022-08-12 22:46:16.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/fields.py
--rw-rw-r--   0 root         (0) root         (0)     9340 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/negotiate_flags.py
--rw-rw-r--   0 root         (0) root         (0)      907 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/ntlmssp_message_signature.py
--rw-rw-r--   0 root         (0) root         (0)     1052 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/ntlmssp_message_signature_noext.py
--rw-rw-r--   0 root         (0) root         (0)     4560 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/serverinfo.py
--rw-rw-r--   0 root         (0) root         (0)     4231 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/structures/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.636238 asyauth-0.0.8/asyauth/protocols/ntlm/templates/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/ntlm/templates/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4159 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/templates/client.py
--rw-rw-r--   0 root         (0) root         (0)     2048 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/ntlm/templates/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.636238 asyauth-0.0.8/asyauth/protocols/spnego/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/spnego/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.640238 asyauth-0.0.8/asyauth/protocols/spnego/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-12 22:39:25.000000 asyauth-0.0.8/asyauth/protocols/spnego/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10863 2022-10-14 18:52:21.000000 asyauth-0.0.8/asyauth/protocols/spnego/client/native.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.640238 asyauth-0.0.8/asyauth/protocols/spnego/messages/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 20:12:30.000000 asyauth-0.0.8/asyauth/protocols/spnego/messages/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4292 2022-01-19 22:38:05.000000 asyauth-0.0.8/asyauth/protocols/spnego/messages/asn1_structs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.640238 asyauth-0.0.8/asyauth/protocols/spnegoex/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-15 09:10:58.000000 asyauth-0.0.8/asyauth/protocols/spnegoex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.640238 asyauth-0.0.8/asyauth/protocols/spnegoex/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-15 09:11:30.000000 asyauth-0.0.8/asyauth/protocols/spnegoex/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5343 2022-08-24 21:17:24.000000 asyauth-0.0.8/asyauth/protocols/spnegoex/client/native.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.640238 asyauth-0.0.8/asyauth/protocols/spnegoex/protocol/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 asyauth-0.0.8/asyauth/protocols/spnegoex/protocol/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19156 2021-10-28 11:02:11.000000 asyauth-0.0.8/asyauth/protocols/spnegoex/protocol/messages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.644238 asyauth-0.0.8/asyauth/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-24 21:19:45.000000 asyauth-0.0.8/asyauth/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1117 2022-08-13 17:35:19.000000 asyauth-0.0.8/asyauth/utils/hexdump.py
--rw-rw-r--   0 root         (0) root         (0)      158 2022-08-15 21:40:15.000000 asyauth-0.0.8/asyauth/utils/paramprocessor.py
--rw-rw-r--   0 root         (0) root         (0)      522 2022-08-12 22:47:23.000000 asyauth-0.0.8/asyauth/utils/timestamp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-26 20:54:31.616238 asyauth-0.0.8/asyauth.egg-info/
--rw-r--r--   0 root         (0) root         (0)      469 2022-11-26 20:54:31.000000 asyauth-0.0.8/asyauth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3218 2022-11-26 20:54:31.000000 asyauth-0.0.8/asyauth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 20:54:31.000000 asyauth-0.0.8/asyauth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-26 20:54:31.000000 asyauth-0.0.8/asyauth.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       71 2022-11-26 20:54:31.000000 asyauth-0.0.8/asyauth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-26 20:54:31.000000 asyauth-0.0.8/asyauth.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-26 20:54:31.644238 asyauth-0.0.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1220 2022-11-26 20:53:45.000000 asyauth-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/
+-rw-rw-r--   0 root         (0) root         (0)     1064 2022-08-24 21:27:42.000000 asyauth-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      469 2022-11-27 22:15:50.856008 asyauth-0.0.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        9 2022-08-24 21:27:42.000000 asyauth-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.848008 asyauth-0.0.9/asyauth/
+-rw-rw-r--   0 root         (0) root         (0)      357 2022-08-13 17:54:19.000000 asyauth-0.0.9/asyauth/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      129 2022-11-27 22:13:33.000000 asyauth-0.0.9/asyauth/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.848008 asyauth-0.0.9/asyauth/common/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 16:49:33.000000 asyauth-0.0.9/asyauth/common/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1702 2022-10-13 20:01:37.000000 asyauth-0.0.9/asyauth/common/clientauthalgo.py
+-rw-rw-r--   0 root         (0) root         (0)      997 2022-11-27 22:13:12.000000 asyauth-0.0.9/asyauth/common/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.848008 asyauth-0.0.9/asyauth/common/credentials/
+-rw-rw-r--   0 root         (0) root         (0)     5460 2022-11-18 18:54:16.000000 asyauth-0.0.9/asyauth/common/credentials/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1019 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/credentials/credssp.py
+-rw-rw-r--   0 root         (0) root         (0)     6643 2022-11-27 21:54:25.000000 asyauth-0.0.9/asyauth/common/credentials/kerberos.py
+-rw-rw-r--   0 root         (0) root         (0)     3220 2022-11-26 19:36:45.000000 asyauth-0.0.9/asyauth/common/credentials/ntlm.py
+-rw-rw-r--   0 root         (0) root         (0)     1310 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/credentials/spnego.py
+-rw-rw-r--   0 root         (0) root         (0)     1314 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/credentials/spnegoex.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/common/subprotocols/
+-rw-rw-r--   0 root         (0) root         (0)     1134 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/subprotocols/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      529 2022-10-14 19:14:23.000000 asyauth-0.0.9/asyauth/common/subprotocols/custom.py
+-rw-rw-r--   0 root         (0) root         (0)      312 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/subprotocols/native.py
+-rw-rw-r--   0 root         (0) root         (0)      421 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/subprotocols/sspi.py
+-rw-rw-r--   0 root         (0) root         (0)     1434 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/subprotocols/sspiproxy.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/common/subprotocols/wsnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/common/winapi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 17:51:18.000000 asyauth-0.0.9/asyauth/common/winapi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    17344 2022-10-05 21:52:44.000000 asyauth-0.0.9/asyauth/common/winapi/constants.py
+-rw-rw-r--   0 root         (0) root         (0)    12418 2022-10-05 21:52:44.000000 asyauth-0.0.9/asyauth/common/winapi/functiondefs.py
+-rw-rw-r--   0 root         (0) root         (0)     1413 2022-10-05 21:52:44.000000 asyauth-0.0.9/asyauth/common/winapi/token.py
+-rw-rw-r--   0 root         (0) root         (0)     2902 2022-10-05 21:52:44.000000 asyauth-0.0.9/asyauth/common/winapi/winsspi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/
+-rw-rw-r--   0 root         (0) root         (0)     1259 2022-08-12 23:03:35.000000 asyauth-0.0.9/asyauth/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/credssp/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/credssp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/credssp/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 13:15:53.000000 asyauth-0.0.9/asyauth/protocols/credssp/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5869 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/credssp/client/native.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/credssp/messages/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/credssp/messages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4460 2022-08-11 16:40:26.000000 asyauth-0.0.9/asyauth/protocols/credssp/messages/asn1_structs.py
+-rw-rw-r--   0 root         (0) root         (0)     4014 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/credssp/messages/remcredguard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/kerberos/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/kerberos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/kerberos/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-12 22:50:09.000000 asyauth-0.0.9/asyauth/protocols/kerberos/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7483 2022-10-05 21:52:44.000000 asyauth-0.0.9/asyauth/protocols/kerberos/client/native.py
+-rw-rw-r--   0 root         (0) root         (0)     3706 2022-10-05 21:52:44.000000 asyauth-0.0.9/asyauth/protocols/kerberos/client/sspi.py
+-rw-rw-r--   0 root         (0) root         (0)     4848 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/kerberos/client/sspiproxy.py
+-rw-rw-r--   0 root         (0) root         (0)     4712 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/kerberos/client/wsnet.py
+-rw-rw-r--   0 root         (0) root         (0)    15484 2022-08-14 22:55:02.000000 asyauth-0.0.9/asyauth/protocols/kerberos/gssapi.py
+-rw-rw-r--   0 root         (0) root         (0)    12420 2022-08-14 22:55:23.000000 asyauth-0.0.9/asyauth/protocols/kerberos/gssapismb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/ntlm/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/ntlm/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-12 22:43:20.000000 asyauth-0.0.9/asyauth/protocols/ntlm/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15672 2022-10-13 19:41:35.000000 asyauth-0.0.9/asyauth/protocols/ntlm/client/native.py
+-rw-rw-r--   0 root         (0) root         (0)     3329 2022-10-05 21:52:44.000000 asyauth-0.0.9/asyauth/protocols/ntlm/client/sspi.py
+-rw-rw-r--   0 root         (0) root         (0)     2546 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/client/sspiproxy.py
+-rw-rw-r--   0 root         (0) root         (0)     2420 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/client/wsnet.py
+-rw-rw-r--   0 root         (0) root         (0)    18300 2022-11-18 19:14:04.000000 asyauth-0.0.9/asyauth/protocols/ntlm/creds_calc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.852008 asyauth-0.0.9/asyauth/protocols/ntlm/messages/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/messages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9287 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/messages/authenticate.py
+-rw-rw-r--   0 root         (0) root         (0)     4869 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/messages/challenge.py
+-rw-rw-r--   0 root         (0) root         (0)     5714 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/messages/negotiate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/ntlm/structures/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4298 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/avpair.py
+-rw-rw-r--   0 root         (0) root         (0)     6847 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/challenge_response.py
+-rw-rw-r--   0 root         (0) root         (0)      851 2022-08-12 22:46:16.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/fields.py
+-rw-rw-r--   0 root         (0) root         (0)     9340 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/negotiate_flags.py
+-rw-rw-r--   0 root         (0) root         (0)      907 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/ntlmssp_message_signature.py
+-rw-rw-r--   0 root         (0) root         (0)     1052 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/ntlmssp_message_signature_noext.py
+-rw-rw-r--   0 root         (0) root         (0)     4560 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/serverinfo.py
+-rw-rw-r--   0 root         (0) root         (0)     4231 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/structures/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/ntlm/templates/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/ntlm/templates/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4159 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/templates/client.py
+-rw-rw-r--   0 root         (0) root         (0)     2048 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/ntlm/templates/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/spnego/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/spnego/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/spnego/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-12 22:39:25.000000 asyauth-0.0.9/asyauth/protocols/spnego/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10863 2022-10-14 18:52:21.000000 asyauth-0.0.9/asyauth/protocols/spnego/client/native.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/spnego/messages/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-13 20:12:30.000000 asyauth-0.0.9/asyauth/protocols/spnego/messages/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4292 2022-01-19 22:38:05.000000 asyauth-0.0.9/asyauth/protocols/spnego/messages/asn1_structs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/spnegoex/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-15 09:10:58.000000 asyauth-0.0.9/asyauth/protocols/spnegoex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/spnegoex/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-15 09:11:30.000000 asyauth-0.0.9/asyauth/protocols/spnegoex/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5343 2022-08-24 21:17:24.000000 asyauth-0.0.9/asyauth/protocols/spnegoex/client/native.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/protocols/spnegoex/protocol/
+-rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:02:11.000000 asyauth-0.0.9/asyauth/protocols/spnegoex/protocol/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    19156 2021-10-28 11:02:11.000000 asyauth-0.0.9/asyauth/protocols/spnegoex/protocol/messages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.856008 asyauth-0.0.9/asyauth/utils/
+-rw-rw-r--   0 root         (0) root         (0)        0 2022-08-24 21:19:45.000000 asyauth-0.0.9/asyauth/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1117 2022-08-13 17:35:19.000000 asyauth-0.0.9/asyauth/utils/hexdump.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2022-08-15 21:40:15.000000 asyauth-0.0.9/asyauth/utils/paramprocessor.py
+-rw-rw-r--   0 root         (0) root         (0)      522 2022-08-12 22:47:23.000000 asyauth-0.0.9/asyauth/utils/timestamp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-27 22:15:50.848008 asyauth-0.0.9/asyauth.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      469 2022-11-27 22:15:50.000000 asyauth-0.0.9/asyauth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3218 2022-11-27 22:15:50.000000 asyauth-0.0.9/asyauth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-27 22:15:50.000000 asyauth-0.0.9/asyauth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-27 22:15:50.000000 asyauth-0.0.9/asyauth.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       71 2022-11-27 22:15:50.000000 asyauth-0.0.9/asyauth.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2022-11-27 22:15:50.000000 asyauth-0.0.9/asyauth.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-11-27 22:15:50.856008 asyauth-0.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1220 2022-11-26 20:53:45.000000 asyauth-0.0.9/setup.py
```

### Comparing `asyauth-0.0.8/LICENSE` & `asyauth-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/clientauthalgo.py` & `asyauth-0.0.9/asyauth/common/clientauthalgo.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/constants.py` & `asyauth-0.0.9/asyauth/common/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 	CCACHE = 'CCACHE'
 	CCACHEHEX = 'CCACHEHEX'
 	CCACHEB64 = 'CCACHEB64'
 	KEYTAB = 'KEYTAB'
 	KEYTABHEX = 'KEYTABHEX'
 	KEYTABB64 = 'KEYTABB64'
 	PFX = 'PFX'
+	PFXB64 = 'PFXB64'
+	PFXHEX = 'PFXHEX'
 	PFXSTR = 'PFXSTR'
 	PEM = 'PEM'
 	CERTSTORE = 'CERTSTORE'
 	KIRBI = 'KIRBI'
 	KIRBIHEX = 'KIRBIHEX'
 	KIRBIB64 = 'KIRBIB64'
 	DES = 'DES'
```

### Comparing `asyauth-0.0.8/asyauth/common/credentials/__init__.py` & `asyauth-0.0.9/asyauth/common/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/credentials/credssp.py` & `asyauth-0.0.9/asyauth/common/credentials/credssp.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/credentials/kerberos.py` & `asyauth-0.0.9/asyauth/common/credentials/kerberos.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,18 @@
 		basetype, encoding = self.get_basetype_and_encoding()
 		if basetype == asyauthSecret.KEYTAB:
 			return KCRED.from_keytab(self.secret, self.username, self.domain, encoding=encoding)
 		if basetype == asyauthSecret.KIRBI:
 			return KCRED.from_kirbi(self.secret, encoding=encoding)
 		if basetype == asyauthSecret.CCACHE:
 			return KCRED.from_ccache(self.secret, self.username, self.domain, encoding=encoding)
-		if basetype == asyauthSecret.PFXSTR:
+		if basetype == asyauthSecret.PFX:
 			return KCRED.from_pfx(self.keydata, self.secret, self.dh_params, self.altname, self.altdomain, encoding=encoding)
+		if basetype == asyauthSecret.PFXSTR:
+			return KCRED.from_pfx_string(self.keydata, self.secret, self.dh_params, self.altname, self.altdomain)
 
 		res = KCRED()
 		res.username = self.username
 		res.domain = self.domain
 
 		if self.stype in [asyauthSecret.PASSWORD, asyauthSecret.PW, asyauthSecret.PASS]:
 			res.password = self.secret
```

### Comparing `asyauth-0.0.8/asyauth/common/credentials/ntlm.py` & `asyauth-0.0.9/asyauth/common/credentials/ntlm.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/credentials/spnego.py` & `asyauth-0.0.9/asyauth/common/credentials/spnego.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/credentials/spnegoex.py` & `asyauth-0.0.9/asyauth/common/credentials/spnegoex.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/subprotocols/__init__.py` & `asyauth-0.0.9/asyauth/common/subprotocols/__init__.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/subprotocols/custom.py` & `asyauth-0.0.9/asyauth/common/subprotocols/custom.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/subprotocols/sspiproxy.py` & `asyauth-0.0.9/asyauth/common/subprotocols/sspiproxy.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/winapi/constants.py` & `asyauth-0.0.9/asyauth/common/winapi/constants.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/winapi/functiondefs.py` & `asyauth-0.0.9/asyauth/common/winapi/functiondefs.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/winapi/token.py` & `asyauth-0.0.9/asyauth/common/winapi/token.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/common/winapi/winsspi.py` & `asyauth-0.0.9/asyauth/common/winapi/winsspi.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/__init__.py` & `asyauth-0.0.9/asyauth/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/credssp/client/native.py` & `asyauth-0.0.9/asyauth/protocols/credssp/client/native.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/credssp/messages/asn1_structs.py` & `asyauth-0.0.9/asyauth/protocols/credssp/messages/asn1_structs.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/credssp/messages/remcredguard.py` & `asyauth-0.0.9/asyauth/protocols/credssp/messages/remcredguard.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/kerberos/client/native.py` & `asyauth-0.0.9/asyauth/protocols/kerberos/client/native.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/kerberos/client/sspi.py` & `asyauth-0.0.9/asyauth/protocols/kerberos/client/sspi.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/kerberos/client/sspiproxy.py` & `asyauth-0.0.9/asyauth/protocols/kerberos/client/sspiproxy.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/kerberos/client/wsnet.py` & `asyauth-0.0.9/asyauth/protocols/kerberos/client/wsnet.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/kerberos/gssapi.py` & `asyauth-0.0.9/asyauth/protocols/kerberos/gssapi.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/kerberos/gssapismb.py` & `asyauth-0.0.9/asyauth/protocols/kerberos/gssapismb.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/client/native.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/client/native.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/client/sspi.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/client/sspi.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/client/sspiproxy.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/client/sspiproxy.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/client/wsnet.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/client/wsnet.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/creds_calc.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/creds_calc.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/messages/authenticate.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/messages/authenticate.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/messages/challenge.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/messages/challenge.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/messages/negotiate.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/messages/negotiate.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/avpair.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/avpair.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/challenge_response.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/challenge_response.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/fields.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/fields.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/negotiate_flags.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/negotiate_flags.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/ntlmssp_message_signature.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/ntlmssp_message_signature.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/ntlmssp_message_signature_noext.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/ntlmssp_message_signature_noext.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/serverinfo.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/serverinfo.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/structures/version.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/structures/version.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/templates/client.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/templates/client.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/ntlm/templates/server.py` & `asyauth-0.0.9/asyauth/protocols/ntlm/templates/server.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/spnego/client/native.py` & `asyauth-0.0.9/asyauth/protocols/spnego/client/native.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/spnego/messages/asn1_structs.py` & `asyauth-0.0.9/asyauth/protocols/spnego/messages/asn1_structs.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/spnegoex/client/native.py` & `asyauth-0.0.9/asyauth/protocols/spnegoex/client/native.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/protocols/spnegoex/protocol/messages.py` & `asyauth-0.0.9/asyauth/protocols/spnegoex/protocol/messages.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/utils/hexdump.py` & `asyauth-0.0.9/asyauth/utils/hexdump.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth/utils/timestamp.py` & `asyauth-0.0.9/asyauth/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/asyauth.egg-info/SOURCES.txt` & `asyauth-0.0.9/asyauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyauth-0.0.8/setup.py` & `asyauth-0.0.9/setup.py`

 * *Files identical despite different names*

