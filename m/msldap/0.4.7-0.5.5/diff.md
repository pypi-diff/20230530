# Comparing `tmp/msldap-0.4.7.tar.gz` & `tmp/msldap-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msldap-0.4.7.tar", last modified: Sat Nov 19 11:31:10 2022, max compression
+gzip compressed data, was "msldap-0.5.5.tar", last modified: Tue May 30 15:57:10 2023, max compression
```

## Comparing `msldap-0.4.7.tar` & `msldap-0.5.5.tar`

### file list

```diff
@@ -1,86 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.662161 msldap-0.4.7/
--rw-rw-r--   0 root         (0) root         (0)     3362 2021-10-28 11:03:04.000000 msldap-0.4.7/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       34 2021-10-28 11:03:04.000000 msldap-0.4.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      477 2022-11-19 11:31:10.662161 msldap-0.4.7/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5168 2022-11-19 09:57:38.000000 msldap-0.4.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.650161 msldap-0.4.7/msldap/
--rw-rw-r--   0 root         (0) root         (0)      332 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2480 2022-08-29 22:26:05.000000 msldap-0.4.7/msldap/__main__.py
--rw-rw-r--   0 root         (0) root         (0)      128 2022-11-18 14:09:54.000000 msldap-0.4.7/msldap/_version.py
--rw-rw-r--   0 root         (0) root         (0)    51190 2022-11-18 14:50:35.000000 msldap-0.4.7/msldap/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.654161 msldap-0.4.7/msldap/commons/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/commons/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      655 2022-08-29 22:26:05.000000 msldap-0.4.7/msldap/commons/authbuilder.py
--rw-rw-r--   0 root         (0) root         (0)      109 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/commons/common.py
--rw-rw-r--   0 root         (0) root         (0)     2831 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/commons/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     5988 2022-08-29 22:26:05.000000 msldap-0.4.7/msldap/commons/factory.py
--rw-rw-r--   0 root         (0) root         (0)     4042 2022-11-19 09:52:37.000000 msldap-0.4.7/msldap/commons/target.py
--rw-rw-r--   0 root         (0) root         (0)     2571 2022-08-29 22:26:05.000000 msldap-0.4.7/msldap/commons/utils.py
--rw-rw-r--   0 root         (0) root         (0)    24800 2022-10-05 22:25:50.000000 msldap-0.4.7/msldap/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.654161 msldap-0.4.7/msldap/examples/
--rw-rw-r--   0 root         (0) root         (0)       62 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/examples/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27007 2022-11-18 16:53:32.000000 msldap-0.4.7/msldap/examples/msldapclient.py
--rw-rw-r--   0 root         (0) root         (0)     2409 2022-08-29 22:26:05.000000 msldap-0.4.7/msldap/examples/msldapcompdnslist.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.654161 msldap-0.4.7/msldap/external/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.658161 msldap-0.4.7/msldap/external/aiocmd/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/aiocmd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.658161 msldap-0.4.7/msldap/external/aiocmd/aiocmd/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/aiocmd/aiocmd/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6150 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/aiocmd/aiocmd/aiocmd.py
--rw-rw-r--   0 root         (0) root         (0)     3688 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/aiocmd/aiocmd/nested_completer.py
--rw-rw-r--   0 root         (0) root         (0)      718 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/aiocmd/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.658161 msldap-0.4.7/msldap/external/asciitree/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/asciitree/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.658161 msldap-0.4.7/msldap/external/asciitree/asciitree/
--rw-rw-r--   0 root         (0) root         (0)     2499 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/asciitree/asciitree/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2909 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/asciitree/asciitree/drawing.py
--rw-rw-r--   0 root         (0) root         (0)     1142 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/asciitree/asciitree/traversal.py
--rw-rw-r--   0 root         (0) root         (0)      136 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/asciitree/asciitree/util.py
--rw-rw-r--   0 root         (0) root         (0)      529 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/external/asciitree/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.662161 msldap-0.4.7/msldap/ldap_objects/
--rw-rw-r--   0 root         (0) root         (0)     1685 2022-01-10 19:07:02.000000 msldap-0.4.7/msldap/ldap_objects/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1101 2022-01-10 19:07:02.000000 msldap-0.4.7/msldap/ldap_objects/adca.py
--rw-rw-r--   0 root         (0) root         (0)    17689 2022-01-10 19:07:02.000000 msldap-0.4.7/msldap/ldap_objects/adcertificatetemplate.py
--rw-rw-r--   0 root         (0) root         (0)     9293 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adcomp.py
--rw-rw-r--   0 root         (0) root         (0)     1870 2022-01-10 19:07:02.000000 msldap-0.4.7/msldap/ldap_objects/adenrollmentservice.py
--rw-rw-r--   0 root         (0) root         (0)     2745 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adgpo.py
--rw-rw-r--   0 root         (0) root         (0)     2782 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adgroup.py
--rw-rw-r--   0 root         (0) root         (0)     6631 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adinfo.py
--rw-rw-r--   0 root         (0) root         (0)     3210 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adou.py
--rw-rw-r--   0 root         (0) root         (0)     1581 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adschemaentry.py
--rw-rw-r--   0 root         (0) root         (0)     2213 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adsec.py
--rw-rw-r--   0 root         (0) root         (0)     5339 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/adtrust.py
--rw-rw-r--   0 root         (0) root         (0)    10639 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/aduser.py
--rw-rw-r--   0 root         (0) root         (0)     4569 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/ldap_objects/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.662161 msldap-0.4.7/msldap/network/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/network/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1090 2022-08-29 22:26:05.000000 msldap-0.4.7/msldap/network/packetizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.662161 msldap-0.4.7/msldap/protocol/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      121 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.662161 msldap-0.4.7/msldap/protocol/ldap_filter/
--rw-rw-r--   0 root         (0) root         (0)       58 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/ldap_filter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    12513 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/ldap_filter/filter.py
--rw-rw-r--   0 root         (0) root         (0)    59585 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/ldap_filter/parser.py
--rw-rw-r--   0 root         (0) root         (0)      493 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/ldap_filter/soundex.py
--rw-rw-r--   0 root         (0) root         (0)    11130 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/messages.py
--rw-rw-r--   0 root         (0) root         (0)     2780 2022-03-29 22:29:27.000000 msldap-0.4.7/msldap/protocol/query.py
--rw-rw-r--   0 root         (0) root         (0)    10281 2022-11-18 16:37:17.000000 msldap-0.4.7/msldap/protocol/typeconversion.py
--rw-rw-r--   0 root         (0) root         (0)      547 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/protocol/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.662161 msldap-0.4.7/msldap/wintypes/
--rw-rw-r--   0 root         (0) root         (0)      185 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/wintypes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.662161 msldap-0.4.7/msldap/wintypes/asn1/
--rw-rw-r--   0 root         (0) root         (0)       63 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/wintypes/asn1/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      654 2021-10-28 11:03:04.000000 msldap-0.4.7/msldap/wintypes/asn1/sdflagsrequest.py
--rw-rw-r--   0 root         (0) root         (0)     2327 2022-11-18 16:38:11.000000 msldap-0.4.7/msldap/wintypes/managedpassword.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-19 11:31:10.654161 msldap-0.4.7/msldap.egg-info/
--rw-r--r--   0 root         (0) root         (0)      477 2022-11-19 11:31:10.000000 msldap-0.4.7/msldap.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2083 2022-11-19 11:31:10.000000 msldap-0.4.7/msldap.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-19 11:31:10.000000 msldap-0.4.7/msldap.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2022-11-19 11:31:10.000000 msldap-0.4.7/msldap.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-19 11:31:10.000000 msldap-0.4.7/msldap.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      135 2022-11-19 11:31:10.000000 msldap-0.4.7/msldap.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-11-19 11:31:10.000000 msldap-0.4.7/msldap.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-19 11:31:10.662161 msldap-0.4.7/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1475 2022-11-19 11:26:39.000000 msldap-0.4.7/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.281783 msldap-0.5.5/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3373 2023-03-05 19:48:34.000000 msldap-0.5.5/LICENSE
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       34 2023-03-05 19:48:34.000000 msldap-0.5.5/MANIFEST.in
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      477 2023-05-30 15:57:10.281783 msldap-0.5.5/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5168 2023-03-05 19:48:34.000000 msldap-0.5.5/README.md
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.253783 msldap-0.5.5/msldap/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      332 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2480 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/__main__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      128 2023-04-15 10:24:10.000000 msldap-0.5.5/msldap/_version.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    55417 2023-04-18 07:39:42.000000 msldap-0.5.5/msldap/client.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.257783 msldap-0.5.5/msldap/commons/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/commons/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      698 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/commons/authbuilder.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      134 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/commons/common.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2831 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/commons/exceptions.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5988 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/commons/factory.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4109 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/commons/target.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2571 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/commons/utils.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    27350 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/connection.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.261783 msldap-0.5.5/msldap/examples/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       62 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/examples/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    37734 2023-04-18 10:58:01.000000 msldap-0.5.5/msldap/examples/msldapclient.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2409 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/examples/msldapcompdnslist.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.261783 msldap-0.5.5/msldap/examples/utils/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/examples/utils/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2062 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/examples/utils/completers.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.261783 msldap-0.5.5/msldap/external/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.261783 msldap-0.5.5/msldap/external/aiocmd/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/aiocmd/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.265783 msldap-0.5.5/msldap/external/aiocmd/aiocmd/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/aiocmd/aiocmd/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6150 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/aiocmd/aiocmd/aiocmd.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3688 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/aiocmd/aiocmd/nested_completer.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      718 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/aiocmd/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.265783 msldap-0.5.5/msldap/external/asciitree/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/asciitree/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.265783 msldap-0.5.5/msldap/external/asciitree/asciitree/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2499 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/asciitree/asciitree/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2909 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/asciitree/asciitree/drawing.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1142 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/asciitree/asciitree/traversal.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      136 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/asciitree/asciitree/util.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      529 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/external/asciitree/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.273783 msldap-0.5.5/msldap/ldap_objects/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1804 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1101 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adca.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    17893 2023-04-10 23:28:56.000000 msldap-0.5.5/msldap/ldap_objects/adcertificatetemplate.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9293 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adcomp.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1870 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adenrollmentservice.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7440 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adgmsa.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2745 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adgpo.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2782 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adgroup.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6631 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adinfo.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3210 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adou.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2798 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adschemaentry.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2213 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adsec.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5339 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/adtrust.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    10639 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/aduser.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4569 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/ldap_objects/common.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.273783 msldap-0.5.5/msldap/network/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/network/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1090 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/network/packetizer.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.277783 msldap-0.5.5/msldap/protocol/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      121 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/constants.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.277783 msldap-0.5.5/msldap/protocol/ldap_filter/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       58 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/ldap_filter/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    12513 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/ldap_filter/filter.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    59585 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/ldap_filter/parser.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      493 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/ldap_filter/soundex.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    11130 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/messages.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2780 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/query.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    66882 2023-04-18 07:44:23.000000 msldap-0.5.5/msldap/protocol/typeconversion.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      547 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/protocol/utils.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.277783 msldap-0.5.5/msldap/relay/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-04-25 21:03:33.000000 msldap-0.5.5/msldap/relay/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2704 2023-04-27 22:16:22.000000 msldap-0.5.5/msldap/relay/server.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4040 2023-04-25 21:39:02.000000 msldap-0.5.5/msldap/relay/serverconnection.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.281783 msldap-0.5.5/msldap/wintypes/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      185 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/wintypes/__init__.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.281783 msldap-0.5.5/msldap/wintypes/asn1/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       63 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/wintypes/asn1/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      654 2023-03-05 19:48:34.000000 msldap-0.5.5/msldap/wintypes/asn1/sdflagsrequest.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2811 2023-04-18 14:34:10.000000 msldap-0.5.5/msldap/wintypes/encryptedlaps.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2327 2023-04-18 09:48:58.000000 msldap-0.5.5/msldap/wintypes/managedpassword.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 15:57:10.257783 msldap-0.5.5/msldap.egg-info/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      477 2023-05-30 15:57:10.000000 msldap-0.5.5/msldap.egg-info/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2312 2023-05-30 15:57:10.000000 msldap-0.5.5/msldap.egg-info/SOURCES.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 15:57:10.000000 msldap-0.5.5/msldap.egg-info/dependency_links.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       61 2023-05-30 15:57:10.000000 msldap-0.5.5/msldap.egg-info/entry_points.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 15:57:10.000000 msldap-0.5.5/msldap.egg-info/not-zip-safe
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      117 2023-05-30 15:57:10.000000 msldap-0.5.5/msldap.egg-info/requires.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        7 2023-05-30 15:57:10.000000 msldap-0.5.5/msldap.egg-info/top_level.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       88 2023-03-05 19:48:34.000000 msldap-0.5.5/pyproject.toml
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2023-05-30 15:57:10.281783 msldap-0.5.5/setup.cfg
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1409 2023-05-30 15:52:25.000000 msldap-0.5.5/setup.py
```

### Comparing `msldap-0.4.7/LICENSE` & `msldap-0.5.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 This projects contains two other project written by a 3rd party. 
 All code is licensed under MIT.
 
 License for MSLDAP:
 MIT License
 
-Copyright (c) 2018 Tamas Jos
+Copyright (c) 2018 Tamas Jos (@skelsec)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `msldap-0.4.7/README.md` & `msldap-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/__main__.py` & `msldap-0.5.5/msldap/__main__.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/client.py` & `msldap-0.5.5/msldap/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,30 @@
 #
 # Author:
 #  Tamas Jos (@skelsec)
 #
 
 import copy
 import asyncio
+import string
+import random
+from typing import List, Dict, Tuple
 
 from msldap import logger
 from msldap.commons.common import MSLDAPClientStatus
 from msldap.wintypes.asn1.sdflagsrequest import SDFlagsRequest, SDFlagsRequestValue
 from msldap.protocol.constants import BASE, ALL_ATTRIBUTES, LEVEL
 
 from msldap.protocol.query import escape_filter_chars
 from msldap.connection import MSLDAPClientConnection
 from msldap.protocol.messages import Control
 from msldap.ldap_objects import *
 from msldap.commons.utils import KNOWN_SIDS
+from msldap.commons.target import MSLDAPTarget
+from asyauth.common.credentials import UniCredential
 
 from winacl.dtyp.security_descriptor import SECURITY_DESCRIPTOR
 from winacl.dtyp.ace import ACCESS_ALLOWED_OBJECT_ACE, ADS_ACCESS_MASK
 from winacl.dtyp.sid import SID
 from winacl.dtyp.guid import GUID
 
 class MSLDAPClient:
@@ -35,15 +40,15 @@
 	:type creds: :class:`MSLDAPCredential`
 	:param ldap_query_page_size: 
 	:type ldap_query_page_size: int
 	:return: A dictionary representing the LDAP tree
 	:rtype: dict
 
 	"""
-	def __init__(self, target, creds, connection = None, keepalive = False):
+	def __init__(self, target:MSLDAPTarget, creds:UniCredential, connection = None, keepalive = False):
 		self.creds = creds
 		self.target = target
 		self.keepalive = keepalive
 		self.ldap_query_page_size = 1000
 		if self.target is not None:
 			self.ldap_query_page_size = self.target.ldap_query_page_size
 		
@@ -55,26 +60,27 @@
 		self._ldapinfo = None
 		self._con = connection
 		self.__keepalive_task = None
 		self.keepalive_period = 10
 		self.disconnected_evt = None
 		self._sid_cache = {} #SID -> (domain, user)
 		self._domainsid_cache = {} # SID -> domain
+		
 	
 	async def __aenter__(self):
 		return self
 		
 	async def __aexit__(self, exc_type, exc, traceback):
 		await asyncio.wait_for(self.disconnect(), timeout = 1)
 	
-	async def __keepalive(self):
+	async def __keepalive(self, temptree):
 		try:
 			while not self.disconnected_evt.is_set():
 				if self._con is not None:
-					ldap_filter = r'(distinguishedName=%s)' % self._tree
+					ldap_filter = r'(distinguishedName=%s)' % temptree
 					async for entry, err in self.pagedsearch(ldap_filter, MSADInfo_ATTRS):
 						if err is not None:
 							return None, err
 				await asyncio.sleep(self.keepalive_period)
 
 		
 		except asyncio.CancelledError:
@@ -100,63 +106,63 @@
 		try:
 			self.disconnected_evt = asyncio.Event()
 			if self._con is None:
 				self._con = MSLDAPClientConnection(self.target, self.creds)
 				_, err = await self._con.connect()
 				if err is not None:
 					raise err
-				res, err = await self._con.bind()
-				if err is not None:
-					return False, err
+				if self._con.is_anon is False:
+					res, err = await self._con.bind()
+					if err is not None:
+						return False, err
+				else:
+					logger.debug('Skipping bind for no auth!')
 			res, err = await self._con.get_serverinfo()
 			if err is not None:
 				raise err
 			self._serverinfo = res
 			self._tree = res['defaultNamingContext']
 			self._ldapinfo, err = await self.get_ad_info()
 			if self._con.is_anon is False:
 				if err is not None:
 					raise err
 				self._domainsid_cache[self._ldapinfo.objectSid] = self._ldapinfo.name
 			
 			if self.keepalive is True:
-				self.__keepalive_task = asyncio.create_task(self.__keepalive())
+				self.__keepalive_task = asyncio.create_task(self.__keepalive(res['defaultNamingContext']))
 			return True, None
 		except Exception as e:
 			return False, e
 
 	def get_server_info(self):
 		return self._serverinfo
 
-	async def pagedsearch(self, query, attributes, controls = None, tree = None):
+	async def pagedsearch(self, query:str, attributes:List[str], controls:List[Tuple[str, str, str]] = None, tree:str = None):
 		"""
 		Performs a paged search on the AD, using the filter and attributes as a normal query does.
 			!The LDAP connection MUST be active before invoking this function!
 
 		:param query: LDAP query filter
 		:type query: str
 		:param attributes: List of requested attributes
 		:type attributes: List[str]
 		:param controls: additional controls to be passed in the query
 		:type controls: dict
-		:param level: Recursion level
-		:type level: int
+		:param tree: Base tree to perform the search on
+		:type tree: str
 
 		:return: Async generator which yields (`dict`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`dict`, :class:`Exception`)]
 
 		"""
 		logger.debug('Paged search, filter: %s attributes: %s' % (query, ','.join(attributes)))
 		if self._con.status != MSLDAPClientStatus.RUNNING:
 			if self._con.status == MSLDAPClientStatus.ERROR:
 				print('There was an error in the connection!')
 				return
-			elif self._con.status == MSLDAPClientStatus.ERROR:
-				print('Theconnection is in stopped state!')
-				return
 
 		if tree is None:
 			tree = self._tree
 		if tree is None:
 			raise Exception('BIND first!')
 		t = []
 		for x in attributes:
@@ -188,15 +194,15 @@
 					return
 				if entry['objectName'] == '' and entry['attributes'] == '':
 					#searchresref...
 					continue
 				#print('et %s ' % entry)
 				yield entry, None
 
-	async def get_tree_plot(self, root_dn, level = 2):
+	async def get_tree_plot(self, root_dn:str, level:int = 2):
 		"""
 		Returns a dictionary representing a tree starting from 'dn' containing all subtrees.
 
 		:param root_dn: The start DN of the tree
 		:type root_dn: str
 		:param level: Recursion level
 		:type level: int
@@ -225,15 +231,15 @@
 				#print(entry['attributes']['distinguishedName'])
 				if 'distinguishedName' not in entry['attributes'] or entry['attributes']['distinguishedName'] is None or entry['attributes']['distinguishedName'] == []:
 					continue
 				subtree = await self.get_tree_plot(entry['attributes']['distinguishedName'], level = level -1)
 				tree[entry['attributes']['distinguishedName']] = subtree
 		return {root_dn : tree}
 
-	async def get_all_users(self, attrs = MSADUser_ATTRS):
+	async def get_all_users(self, attrs:List[str] = MSADUser_ATTRS):
 		"""
 		Fetches all user objects available in the LDAP tree and yields them as MSADUser object.
 		
 		:return: Async generator which yields (`MSADUser`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`MSADUser`, :class:`Exception`)]
 		
 		"""
@@ -242,15 +248,15 @@
 		async for entry, err in self.pagedsearch(ldap_filter, attrs):
 			if err is not None:
 				yield None, err
 				return
 			yield MSADUser.from_ldap(entry, self._ldapinfo), None
 		logger.debug('Finished polling for entries!')
 
-	async def get_all_machines(self, attrs = MSADMachine_ATTRS):
+	async def get_all_machines(self, attrs:List[str] = MSADMachine_ATTRS):
 		"""
 		Fetches all machine objects available in the LDAP tree and yields them as MSADMachine object.
 
 		:param attrs: Lists of attributes to request (eg. `['sAMAccountName', 'dNSHostName']`) Default: all attrs.
 		:type attrs: list
 		:return: Async generator which yields (`MSADMachine`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`MSADMachine`, :class:`Exception`)]
@@ -262,15 +268,15 @@
 		async for entry, err in self.pagedsearch(ldap_filter, attrs):
 			if err is not None:
 				yield None, err
 				return
 			yield MSADMachine.from_ldap(entry, self._ldapinfo), None
 		logger.debug('Finished polling for entries!')
 	
-	async def get_all_gpos(self, attrs = MSADGPO_ATTRS):
+	async def get_all_gpos(self, attrs:List[str] = MSADGPO_ATTRS):
 		"""
 		Fetches all GPOs available in the LDAP tree and yields them as MSADGPO object.
 		
 		:return: Async generator which yields (`MSADGPO`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`MSADGPO`, :class:`Exception`)]
 		
 		"""
@@ -290,16 +296,50 @@
 		:rtype: Iterator[(:class:`dict`, :class:`Exception`)]
 		"""
 
 		ldap_filter = r'(sAMAccountType=805306369)'
 		attributes = ['cn','ms-mcs-AdmPwd']
 		async for entry, err in self.pagedsearch(ldap_filter, attributes):
 			yield entry, err
+	
+	async def get_all_laps_windows(self):
+		"""
+		Fetches all LAPS passwords for all machines. This functionality is only available to specific high-privileged users.
 
-	async def get_schemaentry(self, dn):
+		:return: Async generator which yields (`dict`, None) tuple on success or (None, `Exception`) on error
+		:rtype: Iterator[(:class:`dict`, :class:`Exception`)]
+		"""
+
+		ldap_filter = r'(sAMAccountType=805306369)'
+		# first try to get the plaintext password (the new windows laps doesn't necessary encrypt the PWs)
+		attributes = ['cn','msLAPS-Password']
+		async for entry, err in self.pagedsearch(ldap_filter, attributes):
+			yield entry, err
+
+		# now try to get the encrypted password
+		attributes = ['cn','msLAPS-EncryptedPassword']
+		async for entry, err in self.pagedsearch(ldap_filter, attributes):
+			yield entry, err
+		
+		# now try to get the encrypted password history
+		attributes = ['cn','msLAPS-EncryptedPasswordHistory']
+		async for entry, err in self.pagedsearch(ldap_filter, attributes):
+			yield entry, err
+		
+		# now try to get the encrypted DSRM password
+		attributes = ['cn','msLAPS-EncryptedDSRMPassword']
+		async for entry, err in self.pagedsearch(ldap_filter, attributes):
+			yield entry, err
+		
+		# now try to get the encrypted DSRM password history
+		attributes = ['cn','msLAPS-EncryptedDSRMPasswordHistory']
+		async for entry, err in self.pagedsearch(ldap_filter, attributes):
+			yield entry, err
+
+	async def get_schemaentry(self, dn:str):
 		"""
 		Fetches one Schema entriy identified by dn
 
 		:return: (`MSADSchemaEntry`, None) tuple on success or (None, `Exception`) on error
 		:rtype: (:class:`MSADSchemaEntry`, :class:`Exception`)
 		"""
 		logger.debug('Polling Schema entry for %s'% dn)
@@ -346,30 +386,30 @@
 						yield MSADSchemaEntry.from_ldap(entry), None
 						break
 				else:
 					yield None, None
 					
 		logger.debug('Finished polling for entries!')
 
-	async def get_laps(self, sAMAccountName):
+	async def get_laps(self, sAMAccountName:str):
 		"""
 		Fetches the LAPS password for a machine. This functionality is only available to specific high-privileged users.
 		
 		:param sAMAccountName: The username of the machine (eg. `COMP123$`).
 		:type sAMAccountName: str
 		:return: Laps attributes as a `dict`
 		:rtype: (:class:`dict`, :class:`Exception`)
 		"""
 
 		ldap_filter = r'(&(sAMAccountType=805306369)(sAMAccountName=%s))' % sAMAccountName
 		attributes = ['cn','ms-mcs-AdmPwd']
 		async for entry, err in self.pagedsearch(ldap_filter, attributes):
 			return entry, err
 
-	async def get_user(self, sAMAccountName):
+	async def get_user(self, sAMAccountName:str):
 		"""
 		Fetches one user object from the AD, based on the sAMAccountName attribute (read: username) 
 		
 		:param sAMAccountName: The username of the user.
 		:type sAMAccountName: str
 		:return: A tuple with the user as `MSADUser` and an `Exception` is there was any
 		:rtype: (:class:`MSADUser`, :class:`Exception`)
@@ -380,15 +420,15 @@
 			if err is not None:
 				return None, err
 			return MSADUser.from_ldap(entry, self._ldapinfo), None
 		else:
 			return None, None
 		logger.debug('Finished polling for entries!')
 
-	async def get_machine(self, sAMAccountName):
+	async def get_machine(self, sAMAccountName:str):
 		"""
 		Fetches one machine object from the AD, based on the sAMAccountName attribute (read: username) 
 		
 		:param sAMAccountName: The username of the machine.
 		:type sAMAccountName: str
 		:return: A tuple with the user as `MSADMachine` and an `Exception` is there was any
 		:rtype: (:class:`MSADMachine`, :class:`Exception`)
@@ -435,15 +475,15 @@
 		logger.debug('Polling AD for all SPN entries')
 		ldap_filter = r'(&(sAMAccountType=805306369))'
 		attributes = ['objectSid','sAMAccountName', 'servicePrincipalName']
 
 		async for entry, err in self.pagedsearch(ldap_filter, attributes):
 			yield entry, err
 
-	async def get_all_service_users(self, include_machine = False):
+	async def get_all_service_users(self, include_machine:bool = False):
 		"""
 		Fetches all service user objects from the AD, and returns MSADUser object.
 		Service user refers to an user with SPN (servicePrincipalName) attribute set
 
 		:param include_machine: Specifies wether machine accounts should be included in the query
 		:type include_machine: bool
 		
@@ -460,15 +500,15 @@
 		async for entry, err in self.pagedsearch(ldap_filter, MSADUser_ATTRS):
 			if err is not None:
 				yield None, err
 				return
 			yield MSADUser.from_ldap(entry, self._ldapinfo), None
 		logger.debug('Finished polling for entries!')
 
-	async def get_all_knoreq_users(self, include_machine = False):
+	async def get_all_knoreq_users(self, include_machine:bool = False):
 		"""
 		Fetches all user objects with useraccountcontrol DONT_REQ_PREAUTH flag set from the AD, and returns MSADUser object.
 		
 		:param include_machine: Specifies wether machine accounts should be included in the query
 		:type include_machine: bool
 		:return: Async generator which yields (`MSADUser`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`MSADUser`, :class:`Exception`)]
@@ -483,15 +523,15 @@
 		async for entry, err in self.pagedsearch(ldap_filter, MSADUser_ATTRS):
 			if err is not None:
 				yield None, err
 				return
 			yield MSADUser.from_ldap(entry, self._ldapinfo), None
 		logger.debug('Finished polling for entries!')
 			
-	async def get_objectacl_by_dn_p(self, dn, flags = SDFlagsRequest.DACL_SECURITY_INFORMATION|SDFlagsRequest.GROUP_SECURITY_INFORMATION|SDFlagsRequest.OWNER_SECURITY_INFORMATION):
+	async def get_objectacl_by_dn_p(self, dn:str, flags:SDFlagsRequest = SDFlagsRequest.DACL_SECURITY_INFORMATION|SDFlagsRequest.GROUP_SECURITY_INFORMATION|SDFlagsRequest.OWNER_SECURITY_INFORMATION):
 		"""
 		Returns the full or partial Security Descriptor of the object specified by it's DN.
 		The flags indicate which part of the security Descriptor to be returned.
 		By default the full SD info is returned.
 
 		:param object_dn: The object's DN
 		:type object_dn: str
@@ -510,15 +550,15 @@
 		
 		async for entry, err in self.pagedsearch(ldap_filter, attributes, controls = controls):
 			if err is not None:
 				yield None, err
 				return
 			yield MSADSecurityInfo.from_ldap(entry), None
 
-	async def get_objectacl_by_dn(self, dn, flags = SDFlagsRequest.DACL_SECURITY_INFORMATION|SDFlagsRequest.GROUP_SECURITY_INFORMATION|SDFlagsRequest.OWNER_SECURITY_INFORMATION):
+	async def get_objectacl_by_dn(self, dn:str, flags:SDFlagsRequest = SDFlagsRequest.DACL_SECURITY_INFORMATION|SDFlagsRequest.GROUP_SECURITY_INFORMATION|SDFlagsRequest.OWNER_SECURITY_INFORMATION):
 		"""
 		Returns the full or partial Security Descriptor of the object specified by it's DN.
 		The flags indicate which part of the security Descriptor to be returned.
 		By default the full SD info is returned.
 
 		:param object_dn: The object's DN
 		:type object_dn: str
@@ -537,15 +577,15 @@
 		
 		async for entry, err in self.pagedsearch(ldap_filter, attributes, controls = controls):
 			if err is not None:
 				return None, err
 			return entry['attributes'].get('nTSecurityDescriptor'), None
 		return None, None
 
-	async def set_objectacl_by_dn(self, object_dn, data, flags = SDFlagsRequest.DACL_SECURITY_INFORMATION|SDFlagsRequest.GROUP_SECURITY_INFORMATION|SDFlagsRequest.OWNER_SECURITY_INFORMATION):
+	async def set_objectacl_by_dn(self, object_dn:str, data:bytes, flags:SDFlagsRequest = SDFlagsRequest.DACL_SECURITY_INFORMATION|SDFlagsRequest.GROUP_SECURITY_INFORMATION|SDFlagsRequest.OWNER_SECURITY_INFORMATION):
 		"""
 		Updates the security descriptor of the LDAP object
 		
 		:param object_dn: The object's DN
 		:type object_dn: str
 		:param data: The actual data as bytearray to be updated in the Security Descriptor of the specified object 
 		:type data: bytes
@@ -562,19 +602,19 @@
 						'controlType' : b'1.2.840.113556.1.4.801',
 						'controlValue': req_flags.dump(),
 						'criticality' : True,
 					})
 				]
 
 		changes = {
-			'nTSecurityDescriptor': [('replace', [data])]
+			'nTSecurityDescriptor': [('replace', data)]
 		}
 		return await self._con.modify(object_dn, changes, controls = controls)
 		
-	async def get_all_groups(self, attrs = MSADGroup_ATTRS):
+	async def get_all_groups(self, attrs:List[str] = MSADGroup_ATTRS):
 		"""
 		Yields all Groups present in the LDAP tree.  
 		
 		:return: Async generator which yields (`MSADGroup`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`MSADGroup`, :class:`Exception`)]
 		"""
 		ldap_filter = r'(objectClass=group)'
@@ -594,15 +634,15 @@
 		ldap_filter = r'(objectClass=organizationalUnit)'
 		async for entry, err in self.pagedsearch(ldap_filter, MSADOU_ATTRS):
 			if err is not None:
 				yield None, err
 				return
 			yield MSADOU.from_ldap(entry), None
 			
-	async def get_group_by_dn(self, group_dn):
+	async def get_group_by_dn(self, group_dn:str):
 		"""
 		Returns an `MSADGroup` object for the group specified by group_dn
 
 		:param group_dn: The user's DN
 		:type group_dn: str
 		:return: tuple of `MSADGroup` and an `Exception` is there was any
 		:rtype: (:class:`MSADGroup`, :class:`Exception`)
@@ -612,15 +652,15 @@
 		async for entry, err in self.pagedsearch(ldap_filter, MSADGroup_ATTRS):
 			if err is not None:
 				return None, err
 			return MSADGroup.from_ldap(entry), None
 		
 		return None, Exception('Search returned no results!')
 			
-	async def get_user_by_dn(self, user_dn):
+	async def get_user_by_dn(self, user_dn:str):
 		"""
 		Fetches the DN for an object specified by `user_dn`
 
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:return: The user object
 		:rtype: (:class:`MSADUser`, :class:`Exception`)
@@ -628,15 +668,15 @@
 
 		ldap_filter = r'(&(objectClass=user)(distinguishedName=%s))' % user_dn
 		async for entry, err in self.pagedsearch(ldap_filter, MSADUser_ATTRS):
 			if err is not None:
 				return None, err
 			return MSADUser.from_ldap(entry), None
 			
-	async def get_group_members(self, dn, recursive = False):
+	async def get_group_members(self, dn:str, recursive:bool = False):
 		"""
 		Fetches the DN for an object specified by `objectsid`
 
 		:param dn: The object's DN
 		:type dn: str
 		:param recursive: Indicates wether the lookup should recursively affect all groups
 		:type recursive: bool
@@ -653,15 +693,15 @@
 				if isinstance(result, MSADGroup) and recursive:
 					async for user, err in self.get_group_members(result.distinguishedName, recursive = True):
 						yield user, err
 				else:
 					yield result, err
 		
 						
-	async def get_dn_for_objectsid(self, objectsid):
+	async def get_dn_for_objectsid(self, objectsid:str):
 		"""
 		Fetches the DN for an object specified by `objectsid`
 
 		:param objectsid: The object's SID
 		:type objectsid: str
 		:return: The distinguishedName
 		:rtype: (:class:`str`, :class:`Exception`)
@@ -673,15 +713,15 @@
 			if err is not None:
 				return None, err
 			
 			return entry['attributes']['distinguishedName'], None
 		
 		return None, Exception('Search returned no results!')
 
-	async def get_objectsid_for_dn(self, dn):
+	async def get_objectsid_for_dn(self, dn:str):
 		"""
 		Fetches the objectsid for an object specified by `dn`
 
 		:param dn: The object's distinguishedName
 		:type dn: str
 		:return: The SID of the pobject
 		:rtype: (:class:`str`, :class:`Exception`)
@@ -693,15 +733,15 @@
 			if err is not None:
 				return None, err
 			
 			return entry['attributes']['objectSid'], None
 		
 		return None, Exception('Search returned no results!')
 	
-	async def get_tokengroups_user(self, samaccountname):
+	async def get_tokengroups_user(self, samaccountname:str):
 		ldap_filter = r'(sAMAccountName=%s)' % escape_filter_chars(samaccountname)
 		user_dn = None
 		async for entry, err in self.pagedsearch(ldap_filter, ['distinguishedName']):
 			if err is not None:
 				return None, err
 			
 			user_dn = entry['attributes']['distinguishedName']
@@ -713,15 +753,15 @@
 		async for sids, err in self.get_tokengroups(user_dn):
 			if err is not None:
 				return None, err
 			tokengroup.append(sids)
 		
 		return tokengroup, None
 		
-	async def get_tokengroups(self, dn):
+	async def get_tokengroups(self, dn:str):
 		"""
 		Yields SIDs of groups that the given DN is a member of.
 
 		:return: Async generator which yields (`str`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`str`, :class:`Exception`)]
 
 		"""
@@ -831,15 +871,15 @@
 		ldap_filter = r'(objectClass=trustedDomain)'
 		async for entry, err in self.pagedsearch(ldap_filter, attributes = MSADDomainTrust_ATTRS):
 			if err is not None:
 				yield None, err
 				return
 			yield MSADDomainTrust.from_ldap(entry), None
 		
-	async def create_user_dn(self, user_dn, password):
+	async def create_user_dn(self, user_dn:str, password:str):
 		"""
 		Creates a new user object with a password and enables the user so it can be used immediately.
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:param password: The password of the user
 		:type password: str
@@ -871,123 +911,123 @@
 				return False, err
 
 			return True, None
 		except Exception as e:
 			return False, e
 
 
-	async def unlock_user(self, user_dn):
+	async def unlock_user(self, user_dn:str):
 		"""
 		Unlocks the user by clearing the lockoutTime attribute.
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		changes = {
-			'lockoutTime': [('replace', [0])]
+			'lockoutTime': [('replace', 0)]
 		}
 		return await self._con.modify(user_dn, changes)
 
-	async def enable_user(self, user_dn):
+	async def enable_user(self, user_dn:str):
 		"""
 		Sets the user object to enabled by modifying the UserAccountControl attribute.
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		changes = {
-			'userAccountControl': [('replace', [512])]
+			'userAccountControl': [('replace', 512)]
 		}
 		return await self._con.modify(user_dn, changes)
 	
-	async def disable_user(self, user_dn):
+	async def disable_user(self, user_dn:str):
 		"""
 		Sets the user object to disabled by modifying the UserAccountControl attribute.
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		changes = {
-			'userAccountControl': [('replace', [2])]
+			'userAccountControl': [('replace', 2)]
 		}
 		return await self._con.modify(user_dn, changes)
 
-	async def add_user_spn(self, user_dn, spn):
+	async def add_user_spn(self, user_dn:str, spn:str):
 		"""
 		Adds an SPN record to the user object.
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:param spn: The SPN to be added. It must follow the SPN string format specifications.
 		:type spn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		changes = {
-			'servicePrincipalName': [('add', [spn])]
+			'servicePrincipalName': [('add', spn)]
 		}
 		return await self._con.modify(user_dn, changes)
 	
-	async def del_user_spn(self, user_dn, spn):
+	async def del_user_spn(self, user_dn:str, spn:str):
 		"""
 		Adds an SPN record to the user object.
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:param spn: The SPN to be added. It must follow the SPN string format specifications.
 		:type spn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		changes = {
-			'servicePrincipalName': [('delete', [spn])]
+			'servicePrincipalName': [('delete', spn)]
 		}
 		return await self._con.modify(user_dn, changes)
 
-	async def add_additional_hostname(self, user_dn, hostname):
+	async def add_additional_hostname(self, user_dn:str, hostname:str):
 		"""
 		Adds additional hostname to the user object.
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		changes = {
-			'msds-additionaldnshostname': [('add', [hostname])]
+			'msds-additionaldnshostname': [('add', hostname)]
 		}
 		return await self._con.modify(user_dn, changes)
 		
 	
-	async def delete_user(self, user_dn):
+	async def delete_user(self, user_dn:str):
 		"""
 		Deletes the user.
 		This action is destructive!
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		return await self._con.delete(user_dn)
 
-	async def change_password(self, user_dn: str, newpass: str, oldpass = None):
+	async def change_password(self, user_dn: str, newpass: str, oldpass:str = None):
 		"""
 		Changes the password of a user.  
 		If used with a high-privileged account (eg. Domain admin, Account operator...), the old password can be `None` 
 		
 		:param user_dn: The user's DN
 		:type user_dn: str
 		:param newpass: The new password
@@ -998,19 +1038,19 @@
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 		"""
 		changes = {
 			'unicodePwd': []
 		}
 		if oldpass is not None:
-			changes['unicodePwd'].append(('delete', ['"%s"' % oldpass]))
-			changes['unicodePwd'].append(('add', ['"%s"' % newpass]))
+			changes['unicodePwd'].append(('delete', '"%s"' % oldpass))
+			changes['unicodePwd'].append(('add', '"%s"' % newpass))
 		else:
 			#if you are admin...
-			changes['unicodePwd'].append(('replace', ['"%s"' % newpass]))
+			changes['unicodePwd'].append(('replace', '"%s"' % newpass))
 
 		return await self._con.modify(user_dn, changes)
 
 	
 	async def add_user_to_group(self, user_dn: str, group_dn: str):
 		"""
 		Adds a user to a group
@@ -1021,15 +1061,15 @@
 		:type group_dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 
 		"""
 		changes = {
-			'member': [('add', [user_dn])]
+			'member': [('add', user_dn)]
 		}
 		return await self._con.modify(group_dn, changes)
 
 	async def del_user_from_group(self, user_dn: str, group_dn: str):
 		"""
 		Removes user from group
 
@@ -1039,20 +1079,20 @@
 		:type group_dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 
 
 		"""
 		changes = {
-			'member': [('delete', [user_dn])]
+			'member': [('delete', user_dn)]
 		}
 		return await self._con.modify(group_dn, changes)
 		
 
-	async def get_object_by_dn(self, dn, expected_class = None):
+	async def get_object_by_dn(self, dn:str, expected_class = None):
 		ldap_filter = r'(distinguishedName=%s)' % dn
 		async for entry, err in self.pagedsearch(ldap_filter, ALL_ATTRIBUTES):
 			if err is not None:
 				yield None, err
 				return
 			temp = entry['attributes'].get('objectClass')
 			if expected_class:
@@ -1061,15 +1101,15 @@
 			if not temp:
 				yield entry, None
 			elif 'user' in temp:
 				yield MSADUser.from_ldap(entry), None
 			elif 'group' in temp:
 				yield MSADGroup.from_ldap(entry), None
 
-	async def modify(self, dn, changes, controls = None):
+	async def modify(self, dn:str, changes:Dict[str, object], controls:Dict[str, object] = None):
 		"""
 		Performs the modify operation.
 		
 		:param dn: The DN of the object whose attributes are to be modified
 		:type dn: str
 		:param changes: Describes the changes to be made on the object. Must be a dictionary of the following format: {'attribute': [('change_type', [value])]}
 		:type changes: dict
@@ -1077,46 +1117,46 @@
 		:type controls: dict
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 		"""
 		if controls is None:
 			controls = []
 		controls_conv = []
-		for control in controls:		
+		for control in controls:	
 			controls_conv.append(Control(control))
 		return await self._con.modify(dn, changes, controls=controls_conv)
 
 
-	async def add(self, dn, attributes):
+	async def add(self, dn:str, attributes:Dict[str, object]):
 		"""
 		Performs the add operation.
 		
 		:param dn: The DN of the object to be added
 		:type dn: str
 		:param attributes: Attributes to be used in the operation
 		:type attributes: dict
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 		"""
 		
 		return await self._con.add(dn, attributes)
 
-	async def delete(self, dn):
+	async def delete(self, dn:str):
 		"""
 		Performs the delete operation.
 		
 		:param dn: The DN of the object to be deleted
 		:type dn: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
 		"""
 
 		return await self._con.delete(dn)
 
-	async def add_priv_addmember(self, user_dn, group_dn):
+	async def add_priv_addmember(self, user_dn:str, group_dn:str):
 		"""Adds AddMember rights to the user on the group specified by group_dn"""
 		try:
 			#getting SID of target dn
 			user_sid, err = await self.get_objectsid_for_dn(user_dn)
 			if err is not None:
 				raise err
 			
@@ -1134,25 +1174,25 @@
 			ace_1.ObjectType = GUID.from_string('bf9679c0-0de6-11d0-a285-00aa003049e2')
 			ace_1.Mask = ADS_ACCESS_MASK.WRITE_PROP
 			ace_1.AceFlags = 0
 
 			new_sd.Dacl.aces.append(ace_1)
 
 			changes = {
-				'nTSecurityDescriptor' : [('replace', [new_sd.to_bytes()])]
+				'nTSecurityDescriptor' : [('replace', new_sd.to_bytes())]
 			}
 			_, err = await self.modify(group_dn, changes)
 			if err is not None:
 				raise err
 
 			return True, None
 		except Exception as e:
 			return False, e
 
-	async def add_priv_dcsync(self, user_dn, forest_dn = None):
+	async def add_priv_dcsync(self, user_dn:str, forest_dn:str = None):
 		"""Adds DCSync rights to the given user by modifying the forest's Security Descriptor to add GetChanges and GetChangesAll ACE"""
 		try:
 			#getting SID of target dn
 			user_sid, err = await self.get_objectsid_for_dn(user_dn)
 			if err is not None:
 				raise err
 			
@@ -1183,25 +1223,25 @@
 			ace_2.ObjectType = GUID.from_string('1131f6ad-9c07-11d1-f79f-00c04fc2dcd2')
 			ace_2.Mask = ADS_ACCESS_MASK.CONTROL_ACCESS
 			ace_2.AceFlags = 0
 
 			new_sd.Dacl.aces.append(ace_2)
 
 			changes = {
-				'nTSecurityDescriptor' : [('replace', [new_sd.to_bytes()])]
+				'nTSecurityDescriptor' : [('replace', new_sd.to_bytes())]
 			}
 			_, err = await self.modify(forest_dn, changes)
 			if err is not None:
 				raise err
 
 			return True, None
 		except Exception as e:
 			return False, e
 
-	async def change_priv_owner(self, new_owner_sid, target_dn, target_attribute = None):
+	async def change_priv_owner(self, new_owner_sid:str, target_dn:str, target_attribute = None):
 		"""Changes the owner in a Security Descriptor to the new_owner_sid on an LDAP object or on an LDAP object's attribute identified by target_dn and target_attribute. target_attribute can be omitted to change the target_dn's SD's owner"""
 		try:
 			try:
 				new_owner_sid = SID.from_string(new_owner_sid)
 			except:
 				return False, Exception('Incorrect SID')
 
@@ -1223,15 +1263,15 @@
 				else:
 					raise Exception('Target DN not found!')
 
 			new_sd = copy.deepcopy(target_sd)
 			new_sd.Owner = new_owner_sid
 
 			changes = {
-				target_attribute : [('replace', [new_sd.to_bytes()])]
+				target_attribute : [('replace', new_sd.to_bytes())]
 			}
 			_, err = await self.modify(target_dn, changes)
 			if err is not None:
 				raise err
 
 			return True, None
 		except Exception as e:
@@ -1290,15 +1330,15 @@
 					return
 				yield MSADEnrollmentService.from_ldap(entry), None
 			
 		except Exception as e:
 			yield None, e
 			return
 
-	async def list_certificate_templates(self, name = None):
+	async def list_certificate_templates(self, name:str = None):
 		try:
 			req_flags = SDFlagsRequestValue({'Flags' : SDFlagsRequest.DACL_SECURITY_INFORMATION|SDFlagsRequest.GROUP_SECURITY_INFORMATION|SDFlagsRequest.OWNER_SECURITY_INFORMATION})
 			controls = [('1.2.840.113556.1.4.801', True, req_flags.dump())]
 
 			ldap_filter = "(objectCategory=pKICertificateTemplate)"
 			if name is not None:
 				ldap_filter = "(&(objectCategory=pKICertificateTemplate)(name=%s))" % name
@@ -1315,24 +1355,97 @@
 			return
 
 	async def list_gmsa(self):
 		try:
 			ldap_filter = r'(objectClass=msDS-GroupManagedServiceAccount)'
 			async for entry, err in self.pagedsearch(ldap_filter, attributes = ['sAMAccountName','msDS-GroupMSAMembership', 'msDS-ManagedPassword']):
 				if err is not None:
-					yield None, err
+					yield None, None, None, err
 					return
 				yield entry['attributes'].get('sAMAccountName'), entry['attributes'].get('msDS-GroupMSAMembership'), entry['attributes'].get('msDS-ManagedPassword'), None
 
 		except Exception as e:
 			yield None, None, None, e
 			return
 
+	async def get_all_gmsa(self, attributes:list = MSADGMSAUser_ATTRS):
+		try:
+			ldap_filter = r'(objectClass=msDS-GroupManagedServiceAccount)'
+			async for entry, err in self.pagedsearch(ldap_filter, attributes = ALL_ATTRIBUTES):
+				if err is not None:
+					yield None, err
+					return
+				gmsauser = MSADGMSAUser.from_ldap(entry)
+				yield gmsauser, None
+
+		except Exception as e:
+			yield None, e
+			return
+		
+	async def add_computer(self, computername:str = None, password:str = None):
+		try:
+			if computername is None:
+				computername = 'COMP%s$' % ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(4))
+			if computername.endswith('$') is False:
+				computername += '$'
+			if password is None:
+				password = ''.join(random.choice(string.ascii_uppercase + string.digits + '!@#$%+') for _ in range(16))
+			
+			
+			# Create computer object
+			domain = self._ldapinfo.distinguishedName.replace('DC','').replace('=','').replace(',','.')
+			attributes = {
+				'objectClass':  ['top', 'person', 'organizationalPerson', 'user', 'computer'], 
+				#'cn': computername[:-1], 
+				'sAMAccountName': computername,
+				'name': computername[:-1],
+				'servicePrincipalName' : "HOST/{}.{}".format(computername[:-1], domain),
+			}
+			dn = 'CN=%s,CN=Computers,%s' % (computername[:-1], self._ldapinfo.distinguishedName)
+			_, err = await self.add(dn, attributes)
+			if err is not None:
+				raise err
+			
+			# enabling computer account
+			changes = {
+				'userAccountControl': [('replace', 4096)]
+			}
+			_, err = await self._con.modify(dn, changes)
+			if err is not None:
+				raise err
+			
+			# Change password
+			_, err = await self.change_password(dn, password)
+			if err is not None:
+				raise err
+			
+			# Get computer object
+			computer, err = await self.get_machine(computername)
+			if err is not None:
+				raise err
+			
+
+			return computer, password, None
+		except Exception as e:
+			return None, None, e
+		
+	async def change_samaccountname(self, dn:str, samaccountname:str):
+		try:
+			changes = {
+				'sAMAccountName': [('replace', samaccountname)]
+			}
+			_, err = await self._con.modify(dn, changes)
+			if err is not None:
+				raise err
+			return None
+		except Exception as e:
+			return e
+		
 
-	async def resolv_sd(self, sd):
+	async def resolv_sd(self, sd:SECURITY_DESCRIPTOR or bytes):
 		"Resolves all SIDs found in security descriptor, returns lookup table"
 		try:
 			if isinstance(sd, bytes):
 				sd = SECURITY_DESCRIPTOR.from_bytes(sd)
 			
 			lookup_table = {}
 			sids = {}
@@ -1352,15 +1465,15 @@
 				lookup_table[sid] = (domain, username)
 			
 			return lookup_table, None
 
 		except Exception as e:
 			return None, e
 	
-	async def resolv_sid(self, sid, use_cache = True):
+	async def resolv_sid(self, sid:SID or str, use_cache:bool = True):
 		"""Performs a SID lookup for object and returns the domain name and the samaccountname"""
 		try:
 			sid = str(sid).upper()
 			if sid in KNOWN_SIDS:
 				return "BUILTIN", KNOWN_SIDS[sid], None
 			domain = None
 			username = None
```

### Comparing `msldap-0.4.7/msldap/commons/exceptions.py` & `msldap-0.5.5/msldap/commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/commons/factory.py` & `msldap-0.5.5/msldap/commons/factory.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/commons/target.py` & `msldap-0.5.5/msldap/commons/target.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 	:param ldap_query_page_size: Maximum number of elements to fetch in each paged_query call.
 	:type ldap_query_page_size: int
 	:param ldap_query_ratelimit: rate limit of paged queries. This will cause a sleep (in seconds) between fetching of each page of the query
 	:type ldap_query_ratelimit: float
 	:param dc_ip: Ip address of the kerberos server (if kerberos is used)
 	:type dc_ip: str
 	"""
-	def __init__(self, ip, port = 389, protocol = UniProto.CLIENT_TCP, tree = None, proxies = None, timeout = 10, ldap_query_page_size = 1000, ldap_query_ratelimit = 0, dns:str=None, dc_ip:str = None, domain:str = None, hostname:str = None):
-		UniTarget.__init__(self, ip, port, protocol, timeout, hostname = hostname, proxies = proxies, domain = domain, dc_ip = dc_ip, dns=dns)
+	def __init__(self, ip, port = 389, protocol = UniProto.CLIENT_TCP, tree = None, proxies = None, timeout = 10, ldap_query_page_size = 1000, ldap_query_ratelimit = 0, dns:str=None, dc_ip:str = None, domain:str = None, hostname:str = None, ssl_ctx = None):
+		UniTarget.__init__(self, ip, port, protocol, timeout, hostname = hostname, ssl_ctx= ssl_ctx, proxies = proxies, domain = domain, dc_ip = dc_ip, dns=dns)
 		self.tree = tree
 		self.ldap_query_page_size = ldap_query_page_size
 		self.ldap_query_ratelimit = ldap_query_ratelimit
 	
 	def to_target_string(self):
 		return 'ldap/%s@%s' % (self.get_hostname_or_ip(), self.domain)  #ldap/WIN2019AD.test.corp @ TEST.CORP
 
@@ -111,15 +111,16 @@
 			proxies = unitarget.proxies, 
 			timeout = unitarget.timeout, 
 			ldap_query_page_size = pagesize, 
 			ldap_query_ratelimit = rate,
 			dns = unitarget.dns, 
 			dc_ip = unitarget.dc_ip, 
 			domain = unitarget.domain, 
-			hostname = unitarget.hostname
+			hostname = unitarget.hostname,
+			ssl_ctx = unitarget.ssl_ctx,
 		)
 		return target
 
 	
 	def __str__(self):
 		t = '==== MSLDAPTarget ====\r\n'
 		for k in self.__dict__:
```

### Comparing `msldap-0.4.7/msldap/commons/utils.py` & `msldap-0.5.5/msldap/commons/utils.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/connection.py` & `msldap-0.5.5/msldap/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-
+from typing import List, Dict
 
 from msldap import logger
 from msldap.commons.common import MSLDAPClientStatus
 from .commons.target import MSLDAPTarget
 from msldap.protocol.messages import LDAPMessage, BindRequest, \
 	protocolOp, AuthenticationChoice, SaslCredentials, \
 	SearchRequest, AttributeDescription, Filter, Filters, \
@@ -44,23 +44,27 @@
 		self.lasterror = None
 
 		self.message_id = 0
 		self.message_table = {}
 		self.message_table_notify = {}
 		self.encryption_sequence_counter = 0 # this will be set by the inderlying auth algo
 		self.cb_data = None #for channel binding
+
+		if self.credential.protocol == asyauthProtocol.NONE:
+			self.is_anon = True
 	
 	async def __aenter__(self):
 		return self
 		
 	async def __aexit__(self, exc_type, exc, traceback):
 		await asyncio.wait_for(self.disconnect(), timeout = 1)
 
 	async def __handle_incoming(self):
 		try:
+			
 			async for message_data in self.network.read():				
 				#print('Incoming message data: %s' % message_data)
 				if self.bind_ok is True:
 					if self.__encrypt_messages is True:
 						#removing size
 						message_data = message_data[4:]
 						try:
@@ -121,15 +125,15 @@
 			for msgid in self.message_table_notify:
 				self.message_table[msgid] = [e]
 				self.message_table_notify[msgid].set()
 		
 		self.status = MSLDAPClientStatus.STOPPED
 
 
-	async def send_message(self, message):
+	async def send_message(self, message:Dict[str, object]):
 		curr_msg_id = self.message_id
 		self.message_id += 1
 
 		message['messageID'] = curr_msg_id
 		message_data = LDAPMessage(message).dump()
 
 		if self.bind_ok is True:
@@ -145,15 +149,15 @@
 				self.encryption_sequence_counter += 1
 		
 		self.message_table_notify[curr_msg_id] = asyncio.Event()
 		await self.network.write(message_data)
 
 		return curr_msg_id
 
-	async def recv_message(self, message_id):
+	async def recv_message(self, message_id:int):
 		if message_id not in self.message_table_notify:
 			logger.debug('Requested message id %s which is not in the message notify table!' % message_id)
 			return None
 		#print('Waiting for %s' % message_id)
 		await self.message_table_notify[message_id].wait()
 		#print(self.message_table)
 		messages = self.message_table[message_id]
@@ -181,14 +185,15 @@
 			
 			# now processing channel binding options
 			if self.target.protocol == UniProto.CLIENT_SSL_TCP:
 				certdata = self.network.get_peer_certificate()
 				self.cb_data = b'tls-server-end-point:' + sha256(certdata).digest()
 
 			self.handle_incoming_task = asyncio.create_task(self.__handle_incoming())
+			self.status = MSLDAPClientStatus.CONNECTED
 			logger.debug('Connection succsessful!')
 			return True, None
 		except Exception as e:
 			return False, e
 
 	async def disconnect(self):
 		"""
@@ -211,14 +216,15 @@
 	def __bind_success(self):
 		"""
 		Internal function invoked after bind finished. 
 		Instructs the network layer that upcoming messages might be wrapped
 		"""
 		logger.debug('BIND Success!')
 		self.bind_ok = True
+		self.status = MSLDAPClientStatus.RUNNING
 		if self.credential.protocol in [asyauthProtocol.NTLM, asyauthProtocol.KERBEROS, asyauthProtocol.SICILY]:
 			self.__sign_messages = self.auth.signing_needed()
 			self.__encrypt_messages = self.auth.encryption_needed()
 			if self.__encrypt_messages or self.__sign_messages:
 				self.network.packetizer.is_plain_msg = False
 
 	async def bind(self):
@@ -416,22 +422,93 @@
 						continue
 
 					else:
 						return False, LDAPBindException(
 								res['protocolOp']['resultCode'], 
 								res['protocolOp']['diagnosticMessage']
 							)
+			elif self.credential.protocol == asyauthProtocol.SSL:
+				if self.target.protocol == UniProto.CLIENT_SSL_TCP:
+					self.__bind_success()
+					return True, None
+				elif self.target.protocol == UniProto.CLIENT_TCP:
+					_, err = await self.starttls()
+					if err is not None:
+						return False, err
+					
+					sasl = {
+						'mechanism' : 'EXTERNAL'.encode(),
+					}
+					auth = {
+						'sasl' : SaslCredentials(sasl)
+					}
+
+					bindreq = {
+						'version' : 3,
+						'name': b'',
+						'authentication': AuthenticationChoice(auth), 
+					}
+
+					br = { 'bindRequest' : BindRequest( bindreq	)}
+					msg = { 'protocolOp' : protocolOp(br)}
+
+					msg_id = await self.send_message(msg)
+					res = await self.recv_message(msg_id)
+					if isinstance(res[0], Exception):
+						return False, res[0]
+					resp = res[0].native['protocolOp']
+					if resp['resultCode'] != 'success':
+						#startls refused :(
+						return False, LDAPBindException(
+								resp['resultCode'], 
+								resp['diagnosticMessage']
+							)
+					self.__bind_success()
+					return True, None
+				
+				return False, Exception('Not implemented: %s' % self.credential.protocol.name)
 					
 			else:
 				raise Exception('Not implemented authentication method: %s' % self.credential.protocol.name)
+			
 		except Exception as e:
 			await self.disconnect()
 			return False, e
 
-	async def add(self, entry, attributes):
+	async def starttls(self):
+		try:
+			# https://www.ietf.org/rfc/rfc2830.txt
+			ext = {
+				'requestName': b'1.3.6.1.4.1.1466.20037', 
+			}
+			br = { 'extendedReq' : ExtendedRequest(ext)}
+			msg = { 'protocolOp' : protocolOp(br)}
+			msg_id = await self.send_message(msg)
+			res = await self.recv_message(msg_id)
+			if isinstance(res[0], Exception):
+				return False, res[0]
+			resp = res[0].native['protocolOp']
+			if resp['resultCode'] != 'success':
+				#startls refused :(
+				return False, LDAPBindException(
+						resp['resultCode'], 
+						resp['diagnosticMessage']
+					)
+			self.handle_incoming_task.cancel()
+			await asyncio.sleep(0)
+			await self.network.wrap_ssl(self.target.get_ssl_context())
+			self.handle_incoming_task = asyncio.create_task(self.__handle_incoming())
+			self.status = MSLDAPClientStatus.CONNECTED
+			await asyncio.sleep(0)
+			return True, None
+		except Exception as e:
+			print(e)
+			return False, e
+
+	async def add(self, entry:str, attributes:Dict[str, object]):
 		"""
 		Performs the add operation.
 		
 		:param entry: The DN of the object to be added
 		:type entry: str
 		:param attributes: Attributes to be used in the operation
 		:type attributes: dict
@@ -439,14 +516,15 @@
 		:rtype: (:class:`bool`, :class:`Exception`)
 		"""
 		try:
 			req = {
 				'entry' : entry.encode(),
 				'attributes' : encode_attributes(attributes)
 			}
+			logger.debug(req)
 			br = { 'addRequest' : AddRequest(req)}
 			msg = { 'protocolOp' : protocolOp(br)}
 			
 			msg_id = await self.send_message(msg)
 			results = await self.recv_message(msg_id)
 			if isinstance(results[0], Exception):
 				return False, results[0]
@@ -462,15 +540,15 @@
 							message['protocolOp']['diagnosticMessage']
 						)
 
 			return True, None
 		except Exception as e:
 			return False, e
 
-	async def modify(self, entry, changes, controls = None):
+	async def modify(self, entry:str, changes:Dict[str, object], controls:List[Control] = None):
 		"""
 		Performs the modify operation.
 		
 		:param entry: The DN of the object whose attributes are to be modified
 		:type entry: str
 		:param changes: Describes the changes to be made on the object. Must be a dictionary of the following format: {'attribute': [('change_type', [value])]}
 		:type changes: dict
@@ -505,15 +583,15 @@
 							message['protocolOp']['diagnosticMessage']
 						)
 
 			return True, None
 		except Exception as e:
 			return False, e
 
-	async def delete(self, entry):
+	async def delete(self, entry:str):
 		"""
 		Performs the delete operation.
 		
 		:param entry: The DN of the object to be deleted
 		:type entry: str
 		:return: A tuple of (True, None) on success or (False, Exception) on error. 
 		:rtype: (:class:`bool`, :class:`Exception`)
@@ -538,15 +616,15 @@
 							message['protocolOp']['diagnosticMessage']
 						)
 
 			return True, None
 		except Exception as e:
 			return False, e
 	
-	async def search(self, base, query, attributes, search_scope = 2, size_limit = 1000, types_only = False, derefAliases = 0, timeLimit = None, controls = None, return_done = False):
+	async def search(self, base:str, query:str, attributes:List[str], search_scope:int = 2, size_limit:int = 1000, types_only:bool = False, derefAliases:int = 0, timeLimit:int = None, controls:List[Control] = None, return_done:bool = False):
 		"""
 		Performs the search operation.
 		
 		:param base: base tree on which the search should be performed
 		:type base: str
 		:param query: filter query that defines what should be searched for
 		:type query: str
@@ -566,15 +644,15 @@
 		:type controls: List[class:`Control`]
 		:param return_done: Controls wether the final 'done' LDAP message should be returned, or just the actual results
 		:type return_done: bool
 
 		:return: Async generator which yields (`LDAPMessage`, None) tuple on success or (None, `Exception`) on error
 		:rtype: Iterator[(:class:`LDAPMessage`, :class:`Exception`)]
 		"""
-		if self.status != MSLDAPClientStatus.RUNNING:
+		if self.status not in [MSLDAPClientStatus.CONNECTED, MSLDAPClientStatus.RUNNING]:
 			yield None, Exception('Connection not running! Probably encountered an error')
 			return
 		try:
 			if timeLimit is None:
 				timeLimit = 600 #not sure
 
 			flt = query_syntax_converter(query)
@@ -619,15 +697,15 @@
 					continue
 				
 				break
 		
 		except Exception as e:
 			yield (None, e)
 
-	async def pagedsearch(self, base, query, attributes, search_scope = 2, size_limit = 1000, typesOnly = False, derefAliases = 0, timeLimit = None, controls = None, rate_limit = 0):
+	async def pagedsearch(self, base:str, query:str, attributes:List[str], search_scope:int = 2, size_limit:int = 1000, typesOnly:bool = False, derefAliases:bool = 0, timeLimit:int = None, controls:List[Control] = None, rate_limit:int = 0):
 		"""
 		Paged search is the same as the search operation and uses it under the hood. Adds automatic control to read all results in a paged manner.
 		
 		:param base: base tree on which the search should be performed
 		:type base: str
 		:param query: filter query that defines what should be searched for
 		:type query: str
@@ -731,15 +809,15 @@
 					res['protocolOp']['diagnosticMessage']
 				)
 		return res.native['protocolOp']['responseValue'].decode(), None
 		
 
 
 	async def get_serverinfo(self):
-		if self.status != MSLDAPClientStatus.RUNNING:
+		if self.status not in [MSLDAPClientStatus.CONNECTED, MSLDAPClientStatus.RUNNING]:
 			return None, Exception('Connection not running! Probably encountered an error')
 
 		attributes = [
 			b'subschemaSubentry',
     		b'dsServiceName',
     		b'namingContexts',
     		b'defaultNamingContext',
@@ -773,10 +851,8 @@
 
 		msg_id = await self.send_message(msg)
 		res = await self.recv_message(msg_id)
 		res = res[0]
 		if isinstance(res, Exception):
 			return None, res
 		
-		#print('res')
-		#print(res)
 		return convert_attributes(res.native['protocolOp']['attributes']), None
```

### Comparing `msldap-0.4.7/msldap/examples/msldapcompdnslist.py` & `msldap-0.5.5/msldap/examples/msldapcompdnslist.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/external/aiocmd/aiocmd/aiocmd.py` & `msldap-0.5.5/msldap/external/aiocmd/aiocmd/aiocmd.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/external/aiocmd/aiocmd/nested_completer.py` & `msldap-0.5.5/msldap/external/aiocmd/aiocmd/nested_completer.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/external/aiocmd/setup.py` & `msldap-0.5.5/msldap/external/aiocmd/setup.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/external/asciitree/asciitree/__init__.py` & `msldap-0.5.5/msldap/external/asciitree/asciitree/__init__.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/external/asciitree/asciitree/drawing.py` & `msldap-0.5.5/msldap/external/asciitree/asciitree/drawing.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/external/asciitree/asciitree/traversal.py` & `msldap-0.5.5/msldap/external/asciitree/asciitree/traversal.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/external/asciitree/setup.py` & `msldap-0.5.5/msldap/external/asciitree/setup.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/__init__.py` & `msldap-0.5.5/msldap/ldap_objects/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from msldap.ldap_objects.adou import MSADOU, MSADOU_ATTRS
 from msldap.ldap_objects.adgpo import MSADGPO, MSADGPO_ATTRS
 from msldap.ldap_objects.adtrust import MSADDomainTrust, MSADDomainTrust_ATTRS
 from msldap.ldap_objects.adschemaentry import MSADSCHEMAENTRY_ATTRS, MSADSchemaEntry
 from msldap.ldap_objects.adca import MSADCA, MSADCA_ATTRS
 from msldap.ldap_objects.adenrollmentservice import MSADEnrollmentService_ATTRS, MSADEnrollmentService
 from msldap.ldap_objects.adcertificatetemplate import MSADCertificateTemplate, MSADCertificateTemplate_ATTRS
+from msldap.ldap_objects.adgmsa import MSADGMSAUser, MSADGMSAUser_ATTRS
 
 __all__ = [
     'MSADUser', 
     'MSADUser_ATTRS', 
     'MSADUser_TSV_ATTRS', 
     'MSADInfo',
     'MSADInfo_ATTRS',
@@ -42,9 +43,11 @@
     'MSADSchemaEntry',
     'MSADCA',
     'MSADCA_ATTRS',
     'MSADEnrollmentService_ATTRS',
     'MSADEnrollmentService',
     'MSADCertificateTemplate', 
     'MSADCertificateTemplate_ATTRS',
+    'MSADGMSAUser', 
+    'MSADGMSAUser_ATTRS',
 
 ]
```

### Comparing `msldap-0.4.7/msldap/ldap_objects/adca.py` & `msldap-0.5.5/msldap/ldap_objects/adca.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adcertificatetemplate.py` & `msldap-0.5.5/msldap/ldap_objects/adcertificatetemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,17 +349,27 @@
 		if self.enroll_services:
 			t += "Enroll Services: %s\r\n" % ", ".join(self.enroll_services)
 
 		if len(self.vulns) > 0:
 			t += "Vulnerabilities: %s\r\n" % ", ".join(self.vulns)
 		
 		if self.Certificate_Name_Flag is not None:
-			t += "msPKI-Certificate-Name-Flag: %s\r\n" % str(CertificateNameFlag(self.Certificate_Name_Flag)).split('.',1)[1].replace('|',', ')
+			x = str(CertificateNameFlag(self.Certificate_Name_Flag)).split('.',1)
+			if len(x) >= 2:
+				x = x[1].replace('|',', ')
+			else:
+				x = str(self.Certificate_Name_Flag).replace('|',', ')
+			t += "msPKI-Certificate-Name-Flag: %s\r\n" % x
 		if self.Enrollment_Flag is not None:
-			t += "msPKI-Enrollment-Flag: %s\r\n" % str(EnrollmentFlag(self.Enrollment_Flag)).split('.',1)[1].replace('|',', ')
+			x = str(EnrollmentFlag(self.Enrollment_Flag)).split('.',1)
+			if len(x) >= 2:
+				x = x[1].replace('|',', ')
+			else:
+				x = str(self.Enrollment_Flag).replace('|',', ')
+			t += "msPKI-Enrollment-Flag: %s\r\n" % x
 		if self.RA_Signature is not None:
 			t += "msPKI-RA-Signature: %s\r\n" % self.RA_Signature
 		if self.pKIExtendedKeyUsage is not None:
 			t += "pKIExtendedKeyUsage: %s\r\n" % ", ".join([EKUS_NAMES.get(oid, oid) for oid in self.pKIExtendedKeyUsage])
 		if self.Certificate_Application_Policy is not None:
 			t += "msPKI-Certificate-Application-Policy: %s\r\n" % ", ".join([EKUS_NAMES.get(oid, oid) for oid in self.Certificate_Application_Policy])
 		if self.RA_Application_Policies is not None:
```

### Comparing `msldap-0.4.7/msldap/ldap_objects/adcomp.py` & `msldap-0.5.5/msldap/ldap_objects/adcomp.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adenrollmentservice.py` & `msldap-0.5.5/msldap/ldap_objects/adenrollmentservice.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adgpo.py` & `msldap-0.5.5/msldap/ldap_objects/adgpo.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adgroup.py` & `msldap-0.5.5/msldap/ldap_objects/adgroup.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adinfo.py` & `msldap-0.5.5/msldap/ldap_objects/adinfo.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adou.py` & `msldap-0.5.5/msldap/ldap_objects/adou.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adsec.py` & `msldap-0.5.5/msldap/ldap_objects/adsec.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/adtrust.py` & `msldap-0.5.5/msldap/ldap_objects/adtrust.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/aduser.py` & `msldap-0.5.5/msldap/ldap_objects/aduser.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/ldap_objects/common.py` & `msldap-0.5.5/msldap/ldap_objects/common.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/network/packetizer.py` & `msldap-0.5.5/msldap/network/packetizer.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/protocol/ldap_filter/filter.py` & `msldap-0.5.5/msldap/protocol/ldap_filter/filter.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/protocol/ldap_filter/parser.py` & `msldap-0.5.5/msldap/protocol/ldap_filter/parser.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/protocol/messages.py` & `msldap-0.5.5/msldap/protocol/messages.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/protocol/query.py` & `msldap-0.5.5/msldap/protocol/query.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/protocol/utils.py` & `msldap-0.5.5/msldap/protocol/utils.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/wintypes/asn1/sdflagsrequest.py` & `msldap-0.5.5/msldap/wintypes/asn1/sdflagsrequest.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap/wintypes/managedpassword.py` & `msldap-0.5.5/msldap/wintypes/managedpassword.py`

 * *Files identical despite different names*

### Comparing `msldap-0.4.7/msldap.egg-info/SOURCES.txt` & `msldap-0.5.5/msldap.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 msldap/__init__.py
 msldap/__main__.py
 msldap/_version.py
 msldap/client.py
 msldap/connection.py
 msldap.egg-info/PKG-INFO
@@ -20,14 +21,16 @@
 msldap/commons/exceptions.py
 msldap/commons/factory.py
 msldap/commons/target.py
 msldap/commons/utils.py
 msldap/examples/__init__.py
 msldap/examples/msldapclient.py
 msldap/examples/msldapcompdnslist.py
+msldap/examples/utils/__init__.py
+msldap/examples/utils/completers.py
 msldap/external/__init__.py
 msldap/external/aiocmd/__init__.py
 msldap/external/aiocmd/setup.py
 msldap/external/aiocmd/aiocmd/__init__.py
 msldap/external/aiocmd/aiocmd/aiocmd.py
 msldap/external/aiocmd/aiocmd/nested_completer.py
 msldap/external/asciitree/__init__.py
@@ -37,14 +40,15 @@
 msldap/external/asciitree/asciitree/traversal.py
 msldap/external/asciitree/asciitree/util.py
 msldap/ldap_objects/__init__.py
 msldap/ldap_objects/adca.py
 msldap/ldap_objects/adcertificatetemplate.py
 msldap/ldap_objects/adcomp.py
 msldap/ldap_objects/adenrollmentservice.py
+msldap/ldap_objects/adgmsa.py
 msldap/ldap_objects/adgpo.py
 msldap/ldap_objects/adgroup.py
 msldap/ldap_objects/adinfo.py
 msldap/ldap_objects/adou.py
 msldap/ldap_objects/adschemaentry.py
 msldap/ldap_objects/adsec.py
 msldap/ldap_objects/adtrust.py
@@ -58,11 +62,15 @@
 msldap/protocol/query.py
 msldap/protocol/typeconversion.py
 msldap/protocol/utils.py
 msldap/protocol/ldap_filter/__init__.py
 msldap/protocol/ldap_filter/filter.py
 msldap/protocol/ldap_filter/parser.py
 msldap/protocol/ldap_filter/soundex.py
+msldap/relay/__init__.py
+msldap/relay/server.py
+msldap/relay/serverconnection.py
 msldap/wintypes/__init__.py
+msldap/wintypes/encryptedlaps.py
 msldap/wintypes/managedpassword.py
 msldap/wintypes/asn1/__init__.py
 msldap/wintypes/asn1/sdflagsrequest.py
```

### Comparing `msldap-0.4.7/setup.py` & `msldap-0.5.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	version=verstr,
 
 	# Application author details:
 	author="Tamas Jos",
 	author_email="info@skelsecprojects.com",
 
 	# Packages
-	packages=find_packages(),
+	packages=find_packages(exclude=["tests*"]),
 
 	# Include additional files into the package
 	include_package_data=True,
 
 
 	# Details
 	url="https://github.com/skelsec/msldap",
@@ -36,31 +36,29 @@
 	#
 	# license="LICENSE.txt",
 	description="Python library to play with MS LDAP",
 	long_description="Python library to play with MS LDAP",
 
 	# long_description=open("README.txt").read(),
 	python_requires='>=3.7',
-	classifiers=(
+	classifiers=[
 		"Programming Language :: Python :: 3.7",
 		"Programming Language :: Python :: 3.8",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
-	),
+	],
 	install_requires=[
-		'unicrypto>=0.0.9',
-		'asyauth>=0.0.7',
-		'asysocks>=0.2.1',
+		'unicrypto==0.0.10',
+		'asyauth==0.0.14',
+		'asysocks==0.2.7',
 		'asn1crypto>=1.3.0',
-		'minikerberos>=0.3.1',
-		'winacl>=0.1.4',
+		'winacl==0.1.7',
 		'prompt-toolkit>=3.0.2',
 		'tqdm',
 		'wcwidth',
 	],
 	entry_points={
 		'console_scripts': [
 			'msldap = msldap.examples.msldapclient:main',
-			'msldapcompdns = msldap.examples.msldapcompdnslist:main',
 		],
 	}
 )
```

