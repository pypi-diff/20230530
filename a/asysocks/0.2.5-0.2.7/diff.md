# Comparing `tmp/asysocks-0.2.5.tar.gz` & `tmp/asysocks-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asysocks-0.2.5.tar", last modified: Thu Jan 19 23:50:13 2023, max compression
+gzip compressed data, was "asysocks-0.2.7.tar", last modified: Tue May 30 13:35:56 2023, max compression
```

## Comparing `asysocks-0.2.5.tar` & `asysocks-0.2.7.tar`

### file list

```diff
@@ -1,100 +1,105 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.808628 asysocks-0.2.5/
--rw-rw-r--   0 root         (0) root         (0)     1064 2021-10-28 11:03:58.000000 asysocks-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      349 2023-01-19 23:50:13.808628 asysocks-0.2.5/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3590 2022-01-26 20:28:40.000000 asysocks-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.796628 asysocks-0.2.5/asysocks/
--rw-rw-r--   0 root         (0) root         (0)      332 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      130 2023-01-19 23:47:51.000000 asysocks-0.2.5/asysocks/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.796628 asysocks-0.2.5/asysocks/authentication/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/authentication/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9639 2022-03-14 19:18:55.000000 asysocks-0.2.5/asysocks/certmanager.py
--rw-rw-r--   0 root         (0) root         (0)    24988 2022-05-18 09:44:11.000000 asysocks-0.2.5/asysocks/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.796628 asysocks-0.2.5/asysocks/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1820 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/common/aiowrappers.py
--rw-rw-r--   0 root         (0) root         (0)     7618 2022-03-14 19:19:17.000000 asysocks-0.2.5/asysocks/common/clienturl.py
--rw-rw-r--   0 root         (0) root         (0)      694 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/common/comms.py
--rw-rw-r--   0 root         (0) root         (0)      578 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/common/constants.py
--rw-rw-r--   0 root         (0) root         (0)       92 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/common/credentials.py
--rw-rw-r--   0 root         (0) root         (0)     1113 2022-01-28 18:56:27.000000 asysocks-0.2.5/asysocks/common/target.py
--rw-rw-r--   0 root         (0) root         (0)      801 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/common/trafficlog.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.800628 asysocks-0.2.5/asysocks/examples/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/examples/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8866 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/examples/socksbrute.py
--rw-rw-r--   0 root         (0) root         (0)     8844 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/examples/socksportscan.py
--rw-rw-r--   0 root         (0) root         (0)     2399 2022-03-14 19:19:23.000000 asysocks-0.2.5/asysocks/examples/socksproxy.py
--rw-rw-r--   0 root         (0) root         (0)     3861 2022-03-14 19:19:30.000000 asysocks-0.2.5/asysocks/examples/sockssec.py
--rw-rw-r--   0 root         (0) root         (0)     2429 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/examples/sockstunnel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.800628 asysocks-0.2.5/asysocks/intercepting/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/intercepting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      397 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/intercepting/default_intercept_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.800628 asysocks-0.2.5/asysocks/intercepting/monitors/
--rw-rw-r--   0 root         (0) root         (0)      294 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/intercepting/monitors/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2600 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/intercepting/monitors/base.py
--rw-rw-r--   0 root         (0) root         (0)     1554 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/intercepting/monitors/rawlogging.py
--rw-rw-r--   0 root         (0) root         (0)     8205 2022-03-14 19:19:49.000000 asysocks-0.2.5/asysocks/intercepting/monitors/sslbase.py
--rw-rw-r--   0 root         (0) root         (0)     2995 2022-03-14 19:19:38.000000 asysocks-0.2.5/asysocks/intercepting/server.py
--rw-rw-r--   0 root         (0) root         (0)     1636 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/intercepting/target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.800628 asysocks-0.2.5/asysocks/network/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/network/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1396 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/network/queue.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/network/tcp.py
--rw-rw-r--   0 root         (0) root         (0)     4353 2022-08-29 10:44:26.000000 asysocks-0.2.5/asysocks/network/wsnet.py
--rw-rw-r--   0 root         (0) root         (0)     4552 2022-01-28 18:46:14.000000 asysocks-0.2.5/asysocks/network/wsnetws.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.804628 asysocks-0.2.5/asysocks/protocol/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/protocol/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2845 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/protocol/http.py
--rw-rw-r--   0 root         (0) root         (0)     3282 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/protocol/socks4.py
--rw-rw-r--   0 root         (0) root         (0)     3913 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/protocol/socks4a.py
--rw-rw-r--   0 root         (0) root         (0)    20361 2022-08-05 20:19:29.000000 asysocks-0.2.5/asysocks/protocol/socks5.py
--rw-rw-r--   0 root         (0) root         (0)    12824 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/security.py
--rw-rw-r--   0 root         (0) root         (0)    18022 2022-10-10 18:04:25.000000 asysocks-0.2.5/asysocks/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.804628 asysocks-0.2.5/asysocks/test/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-29 10:44:12.000000 asysocks-0.2.5/asysocks/test/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      872 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/test/listener_test.py
--rw-rw-r--   0 root         (0) root         (0)     1200 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/test/queue_test.py
--rw-rw-r--   0 root         (0) root         (0)     3261 2022-03-14 19:19:56.000000 asysocks-0.2.5/asysocks/test/ssl_test.py
--rw-rw-r--   0 root         (0) root         (0)      460 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/test/test_url_param.py
--rw-rw-r--   0 root         (0) root         (0)     3044 2022-08-29 10:57:00.000000 asysocks-0.2.5/asysocks/test/wsnettest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.804628 asysocks-0.2.5/asysocks/unicomm/
--rw-rw-r--   0 root         (0) root         (0)      270 2022-08-04 21:05:28.000000 asysocks-0.2.5/asysocks/unicomm/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15102 2022-11-28 23:11:30.000000 asysocks-0.2.5/asysocks/unicomm/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.804628 asysocks-0.2.5/asysocks/unicomm/common/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-04 20:50:41.000000 asysocks-0.2.5/asysocks/unicomm/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2346 2022-10-10 18:16:42.000000 asysocks-0.2.5/asysocks/unicomm/common/connection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.804628 asysocks-0.2.5/asysocks/unicomm/common/packetizers/
--rw-rw-r--   0 root         (0) root         (0)     2571 2022-09-03 13:17:06.000000 asysocks-0.2.5/asysocks/unicomm/common/packetizers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2578 2022-08-29 11:15:35.000000 asysocks-0.2.5/asysocks/unicomm/common/packetizers/ssl.py
--rw-rw-r--   0 root         (0) root         (0)     7986 2023-01-18 20:44:53.000000 asysocks-0.2.5/asysocks/unicomm/common/proxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.808628 asysocks-0.2.5/asysocks/unicomm/common/scanner/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-16 10:57:14.000000 asysocks-0.2.5/asysocks/unicomm/common/scanner/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3137 2022-08-21 23:42:23.000000 asysocks-0.2.5/asysocks/unicomm/common/scanner/common.py
--rw-rw-r--   0 root         (0) root         (0)     5181 2022-08-21 16:22:57.000000 asysocks-0.2.5/asysocks/unicomm/common/scanner/scanner.py
--rw-rw-r--   0 root         (0) root         (0)     4039 2022-08-21 20:24:43.000000 asysocks-0.2.5/asysocks/unicomm/common/scanner/targetgen.py
--rw-rw-r--   0 root         (0) root         (0)     5985 2023-01-19 23:46:22.000000 asysocks-0.2.5/asysocks/unicomm/common/target.py
--rw-rw-r--   0 root         (0) root         (0)     6172 2023-01-19 12:11:20.000000 asysocks-0.2.5/asysocks/unicomm/common/unissl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.808628 asysocks-0.2.5/asysocks/unicomm/protocol/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-05 20:18:38.000000 asysocks-0.2.5/asysocks/unicomm/protocol/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2845 2022-08-05 20:18:38.000000 asysocks-0.2.5/asysocks/unicomm/protocol/http.py
--rw-rw-r--   0 root         (0) root         (0)     3198 2022-08-15 17:21:21.000000 asysocks-0.2.5/asysocks/unicomm/protocol/quic.py
--rw-rw-r--   0 root         (0) root         (0)     3208 2022-08-06 18:04:05.000000 asysocks-0.2.5/asysocks/unicomm/protocol/socks4.py
--rw-rw-r--   0 root         (0) root         (0)     3864 2022-08-06 18:07:28.000000 asysocks-0.2.5/asysocks/unicomm/protocol/socks4a.py
--rw-rw-r--   0 root         (0) root         (0)    20360 2022-10-10 17:00:35.000000 asysocks-0.2.5/asysocks/unicomm/protocol/socks5.py
--rw-rw-r--   0 root         (0) root         (0)     9519 2022-10-11 08:38:07.000000 asysocks-0.2.5/asysocks/unicomm/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.808628 asysocks-0.2.5/asysocks/unicomm/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-08-15 19:07:06.000000 asysocks-0.2.5/asysocks/unicomm/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      113 2022-08-15 19:06:31.000000 asysocks-0.2.5/asysocks/unicomm/utils/paramprocessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.808628 asysocks-0.2.5/asysocks/utils/
--rw-rw-r--   0 root         (0) root         (0)        0 2021-10-28 11:03:58.000000 asysocks-0.2.5/asysocks/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6385 2022-03-07 20:37:37.000000 asysocks-0.2.5/asysocks/utils/mbedtlswrapper.py
--rw-rw-r--   0 root         (0) root         (0)     6361 2022-03-14 19:20:12.000000 asysocks-0.2.5/asysocks/utils/sslwrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-19 23:50:13.796628 asysocks-0.2.5/asysocks.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-01-19 23:50:13.000000 asysocks-0.2.5/asysocks.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2492 2023-01-19 23:50:13.000000 asysocks-0.2.5/asysocks.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-19 23:50:13.000000 asysocks-0.2.5/asysocks.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-01-19 23:50:13.000000 asysocks-0.2.5/asysocks.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-19 23:50:13.000000 asysocks-0.2.5/asysocks.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-01-19 23:50:13.000000 asysocks-0.2.5/asysocks.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-19 23:50:13.000000 asysocks-0.2.5/asysocks.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-19 23:50:13.808628 asysocks-0.2.5/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1376 2021-10-28 11:03:58.000000 asysocks-0.2.5/setup.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.728197 asysocks-0.2.7/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1077 2023-03-05 19:48:52.000000 asysocks-0.2.7/LICENSE
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      349 2023-05-30 13:35:56.728197 asysocks-0.2.7/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3590 2023-03-05 19:48:52.000000 asysocks-0.2.7/README.md
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.696197 asysocks-0.2.7/asysocks/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      332 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      130 2023-05-05 16:27:03.000000 asysocks-0.2.7/asysocks/_version.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.696197 asysocks-0.2.7/asysocks/authentication/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/authentication/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     9639 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/certmanager.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    24988 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/client.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.700197 asysocks-0.2.7/asysocks/common/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1820 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/aiowrappers.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7618 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/clienturl.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      694 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/comms.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      578 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/constants.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       92 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/credentials.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1113 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/target.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      801 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/common/trafficlog.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.700197 asysocks-0.2.7/asysocks/examples/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/examples/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8866 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/examples/socksbrute.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8844 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/examples/socksportscan.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2399 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/examples/socksproxy.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3861 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/examples/sockssec.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2429 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/examples/sockstunnel.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.700197 asysocks-0.2.7/asysocks/intercepting/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      397 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/default_intercept_table.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.700197 asysocks-0.2.7/asysocks/intercepting/monitors/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      294 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/monitors/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2600 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/monitors/base.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1554 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/monitors/rawlogging.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     8205 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/monitors/sslbase.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2995 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/server.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1636 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/intercepting/target.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.700197 asysocks-0.2.7/asysocks/network/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/network/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1396 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/network/queue.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/network/tcp.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4353 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/network/wsnet.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4552 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/network/wsnetws.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.700197 asysocks-0.2.7/asysocks/protocol/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/protocol/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2845 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/protocol/http.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3282 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/protocol/socks4.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3913 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/protocol/socks4a.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    20361 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/protocol/socks5.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    12824 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/security.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    18022 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/server.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.704197 asysocks-0.2.7/asysocks/test/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/test/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      872 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/test/listener_test.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1200 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/test/queue_test.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3261 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/test/ssl_test.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      460 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/test/test_url_param.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3044 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/test/wsnettest.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.724197 asysocks-0.2.7/asysocks/unicomm/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      270 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    15102 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/client.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.724197 asysocks-0.2.7/asysocks/unicomm/common/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/common/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2474 2023-04-24 13:31:06.000000 asysocks-0.2.7/asysocks/unicomm/common/connection.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.724197 asysocks-0.2.7/asysocks/unicomm/common/packetizers/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2571 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/common/packetizers/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2603 2023-04-27 17:15:02.000000 asysocks-0.2.7/asysocks/unicomm/common/packetizers/ssl.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     7986 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/common/proxy.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.724197 asysocks-0.2.7/asysocks/unicomm/common/scanner/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/common/scanner/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3137 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/common/scanner/common.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     5236 2023-04-07 15:27:59.000000 asysocks-0.2.7/asysocks/unicomm/common/scanner/scanner.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     4039 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/common/scanner/targetgen.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6164 2023-04-27 21:31:04.000000 asysocks-0.2.7/asysocks/unicomm/common/target.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6581 2023-04-27 21:40:38.000000 asysocks-0.2.7/asysocks/unicomm/common/unissl.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.728197 asysocks-0.2.7/asysocks/unicomm/protocol/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/protocol/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2845 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/protocol/http.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3198 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/protocol/quic.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.728197 asysocks-0.2.7/asysocks/unicomm/protocol/server/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-04-21 21:40:08.000000 asysocks-0.2.7/asysocks/unicomm/protocol/server/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      506 2023-04-24 11:51:04.000000 asysocks-0.2.7/asysocks/unicomm/protocol/server/udp.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3208 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/protocol/socks4.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3864 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/protocol/socks4a.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    20360 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/protocol/socks5.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)    13894 2023-04-27 22:15:46.000000 asysocks-0.2.7/asysocks/unicomm/server.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.728197 asysocks-0.2.7/asysocks/unicomm/utils/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/utils/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     3695 2023-04-27 21:23:52.000000 asysocks-0.2.7/asysocks/unicomm/utils/genselfsigned.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      113 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/unicomm/utils/paramprocessor.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.728197 asysocks-0.2.7/asysocks/utils/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        0 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/utils/__init__.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6385 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/utils/mbedtlswrapper.py
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     6361 2023-03-05 19:48:52.000000 asysocks-0.2.7/asysocks/utils/sslwrapper.py
+drwxrwxr-x   0 webdev    (1000) webdev    (1000)        0 2023-05-30 13:35:56.696197 asysocks-0.2.7/asysocks.egg-info/
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      349 2023-05-30 13:35:56.000000 asysocks-0.2.7/asysocks.egg-info/PKG-INFO
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     2632 2023-05-30 13:35:56.000000 asysocks-0.2.7/asysocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 13:35:56.000000 asysocks-0.2.7/asysocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)      272 2023-05-30 13:35:56.000000 asysocks-0.2.7/asysocks.egg-info/entry_points.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       11 2023-05-30 13:35:56.000000 asysocks-0.2.7/asysocks.egg-info/requires.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        9 2023-05-30 13:35:56.000000 asysocks-0.2.7/asysocks.egg-info/top_level.txt
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)        1 2023-05-30 13:35:56.000000 asysocks-0.2.7/asysocks.egg-info/zip-safe
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       88 2023-03-05 19:48:52.000000 asysocks-0.2.7/pyproject.toml
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)       38 2023-05-30 13:35:56.728197 asysocks-0.2.7/setup.cfg
+-rw-rw-r--   0 webdev    (1000) webdev    (1000)     1376 2023-03-05 19:48:52.000000 asysocks-0.2.7/setup.py
```

### Comparing `asysocks-0.2.5/LICENSE` & `asysocks-0.2.7/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 skelsec
+Copyright (c) 2020 Tamas Jos (@skelsec)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `asysocks-0.2.5/README.md` & `asysocks-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/certmanager.py` & `asysocks-0.2.7/asysocks/certmanager.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/client.py` & `asysocks-0.2.7/asysocks/client.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/common/aiowrappers.py` & `asysocks-0.2.7/asysocks/common/aiowrappers.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/common/clienturl.py` & `asysocks-0.2.7/asysocks/common/clienturl.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/common/comms.py` & `asysocks-0.2.7/asysocks/common/comms.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/common/constants.py` & `asysocks-0.2.7/asysocks/common/constants.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/common/target.py` & `asysocks-0.2.7/asysocks/common/target.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/common/trafficlog.py` & `asysocks-0.2.7/asysocks/common/trafficlog.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/examples/socksbrute.py` & `asysocks-0.2.7/asysocks/examples/socksbrute.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/examples/socksportscan.py` & `asysocks-0.2.7/asysocks/examples/socksportscan.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/examples/socksproxy.py` & `asysocks-0.2.7/asysocks/examples/socksproxy.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/examples/sockssec.py` & `asysocks-0.2.7/asysocks/examples/sockssec.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/examples/sockstunnel.py` & `asysocks-0.2.7/asysocks/examples/sockstunnel.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/intercepting/monitors/base.py` & `asysocks-0.2.7/asysocks/intercepting/monitors/base.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/intercepting/monitors/rawlogging.py` & `asysocks-0.2.7/asysocks/intercepting/monitors/rawlogging.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/intercepting/monitors/sslbase.py` & `asysocks-0.2.7/asysocks/intercepting/monitors/sslbase.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/intercepting/server.py` & `asysocks-0.2.7/asysocks/intercepting/server.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/intercepting/target.py` & `asysocks-0.2.7/asysocks/intercepting/target.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/network/queue.py` & `asysocks-0.2.7/asysocks/network/queue.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/network/wsnet.py` & `asysocks-0.2.7/asysocks/network/wsnet.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/network/wsnetws.py` & `asysocks-0.2.7/asysocks/network/wsnetws.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/protocol/http.py` & `asysocks-0.2.7/asysocks/protocol/http.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/protocol/socks4.py` & `asysocks-0.2.7/asysocks/protocol/socks4.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/protocol/socks4a.py` & `asysocks-0.2.7/asysocks/protocol/socks4a.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/protocol/socks5.py` & `asysocks-0.2.7/asysocks/protocol/socks5.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/security.py` & `asysocks-0.2.7/asysocks/security.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/server.py` & `asysocks-0.2.7/asysocks/server.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/test/listener_test.py` & `asysocks-0.2.7/asysocks/test/listener_test.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/test/queue_test.py` & `asysocks-0.2.7/asysocks/test/queue_test.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/test/ssl_test.py` & `asysocks-0.2.7/asysocks/test/ssl_test.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/test/wsnettest.py` & `asysocks-0.2.7/asysocks/test/wsnettest.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/client.py` & `asysocks-0.2.7/asysocks/unicomm/client.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/connection.py` & `asysocks-0.2.7/asysocks/unicomm/common/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,8 +77,15 @@
 	async def stream(self):
 		if not isinstance(self.packetizer, StreamPacketizer):
 			raise Exception('This function onaly available when StreamPacketizer is used!')
 		while True:
 			data = await self.reader.read(self.packetizer.buffer_size)
 			await self.packetizer.data_in(data)
 			if data == b'':
-				break
+				break
+
+
+class UniUDPConnection:
+	def __init__(self, socket, data, addr):
+		self.socket = socket
+		self.data = data
+		self.addr = addr
```

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/packetizers/__init__.py` & `asysocks-0.2.7/asysocks/unicomm/common/packetizers/__init__.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/packetizers/ssl.py` & `asysocks-0.2.7/asysocks/unicomm/common/packetizers/ssl.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 	
 	def get_peer_certificate(self):
 		return self.tls_obj.getpeercert(binary_form=True)
 	
 	def packetizer_control(self, *args, **kwargs):
 		self.packetizer.packetizer_control(*args, **kwargs)
 
-	async def do_handshake(self, reader, writer):
+	async def do_handshake(self, reader, writer, server_side=False):
 		self.tls_in_buff = ssl.MemoryBIO()
 		self.tls_out_buff = ssl.MemoryBIO()
-		self.tls_obj = self.ssl_ctx.wrap_bio(self.tls_in_buff, self.tls_out_buff, server_side=False) # , server_hostname = self.monitor.dst_hostname
+		self.tls_obj = self.ssl_ctx.wrap_bio(self.tls_in_buff, self.tls_out_buff, server_side=server_side) # , server_hostname = self.monitor.dst_hostname
 
 		ctr = 0
 		while True:
 			ctr += 1
 			try:
 				self.tls_obj.do_handshake()
 			except ssl.SSLWantReadError:
```

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/proxy.py` & `asysocks-0.2.7/asysocks/unicomm/common/proxy.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/scanner/common.py` & `asysocks-0.2.7/asysocks/unicomm/common/scanner/common.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/scanner/scanner.py` & `asysocks-0.2.7/asysocks/unicomm/common/scanner/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 		self.executors = executors
 		if isinstance(self.executors, list) is False:
 			self.executors = [self.executors]
 		if isinstance(self.target_generators, list) is False:
 			self.target_generators = [self.target_generators]
 
 	async def worker(self):
-		while True:
+		while not asyncio.current_task().cancelled():
 			x = await self.__targetgen.__anext__()
 			if x is None:
 				return
 			targetid, target = x
 			for executor in self.executors:
 				try:
 					await asyncio.wait_for(executor.run(targetid, target, self.out_queue), self.host_timeout)
@@ -131,14 +131,15 @@
 							else:
 								fhandles[rtype] = open(os.path.join(out_file, '%s_%s%s' %(rtype, self.scantime,'.tsv')), 'w', newline = '')
 						fhandles[rtype].write(result.to_line()+'\r\n')
 
 		except Exception as e:
 			print('SCANNER CRITICAL ERROR %s' % str(e))
 		finally:
+			await self.stop()
 			for k in fhandles:
 				try:
 					fhandles[k].close()
 				except:
 					pass
 async def amain():
 	try:
```

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/scanner/targetgen.py` & `asysocks-0.2.7/asysocks/unicomm/common/scanner/targetgen.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/target.py` & `asysocks-0.2.7/asysocks/unicomm/common/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	CLIENT_TCP = 1
 	CLIENT_SSL_TCP = 2
 	CLIENT_UDP = 3
 	CLIENT_DTLS = 4
 	CLIENT_QUIC = 5
 	SERVER_TCP = 6
 	SERVER_SSL_TCP = 7
+	SERVER_UDP = 8
 
 unitarget_url_params = {
 	'dc' : str_one,
 	'timeout' : int_one,
 	'serverip' : str_one,
 	'dns' : str_one,
 }
@@ -94,18 +95,21 @@
 				'\tproxysslkey_password - str - proxy SSL/TLS key password\n'
 				
 
 
 	def get_newtarget(self, ip, port, hostname = None):
 		return UniTarget(ip, port, self.protocol, self.timeout, ssl_ctx = self.ssl_ctx, hostname = hostname, dc_ip = self.dc_ip, domain = self.domain, proxies=copy.deepcopy(self.proxies))
 
-	def get_ssl_context(self):
-		if self.ssl_ctx is not None:
-			return self.ssl_ctx.get_ssl_context()
-		return UniSSL.get_noverify_context()
+	def get_ssl_context(self, protocol = None):
+		if self.ssl_ctx is None:
+			is_server = True if self.protocol in [UniProto.SERVER_TCP, UniProto.SERVER_SSL_TCP, UniProto.SERVER_UDP] else False
+			self.ssl_ctx = UniSSL.get_noverify_context(is_server)
+		
+		return self.ssl_ctx.get_ssl_context(protocol)
+		
 
 	def get_hostname(self):
 		return self.hostname
 	
 	def set_hostname_or_ip(self, ip):
 		try:
 			self.ip = str(ipaddress.ip_address(ip))
```

### Comparing `asysocks-0.2.5/asysocks/unicomm/common/unissl.py` & `asysocks-0.2.7/asysocks/unicomm/common/unissl.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	'cert' : ('certfile', [str]),
 	'key' : ('keyfile', [str]),
 	'password' : ('password', [str]),
 	'verify' : ('verify', [bool]),
 }
 
 class UniSSL:
+	"""This class was necessary to be able to create duplicates of ssl contexts, which is not possible with the ssl.SSLContext class."""
 	def __init__(self, certfile:str = None, keyfile:str = None, cacert:str = None, password:str = None, verify:bool = False):
 		self.protocol = ssl.PROTOCOL_TLS
 		self.cacert:str = cacert
 		self.keyfile:str = keyfile
 		self.certfile:str = certfile
 		self.password:str = password
 		self.verify:bool = verify
@@ -106,25 +107,29 @@
 		if len(add_certs) > 0:
 			self.__cacertfilename = 'cacert_%s' % suffix
 			with open(self.__cacertfilename, 'wb') as f:
 				for ca in add_certs:
 					f.write(ca.public_bytes(Encoding.PEM))
 
 	@staticmethod
-	def get_noverify_context(protocol = ssl.PROTOCOL_TLS_CLIENT):
-		ssl_ctx = ssl.SSLContext(protocol)
-		ssl_ctx.check_hostname = False
-		ssl_ctx.verify_mode = ssl.CERT_NONE
-		return ssl_ctx
+	def get_noverify_context(is_server=False, hostname = 'localhost'):
+		"""Returns a generic SSL context that does not verify the certificate."""
+		if is_server is True:
+			from asysocks.unicomm.utils.genselfsigned import generate_selfsigned_cert
+			server_certfile, server_keyfile = generate_selfsigned_cert(hostname)
+			return UniSSL(server_certfile, server_keyfile, None, verify=False)
+		
+		return UniSSL(verify=False)			
 	
 	def get_ssl_context(self, protocol = ssl.PROTOCOL_TLS_CLIENT):
 		try:
 			self.__startup()
 			ssl_ctx = ssl.SSLContext(protocol)
-			ssl_ctx.load_cert_chain(certfile=self.__certfilename, keyfile=self.__keyfilename, password=self.password)
+			if self.__certfilename is not None:
+				ssl_ctx.load_cert_chain(certfile=self.__certfilename, keyfile=self.__keyfilename, password=self.password)
 			
 			if self.verify is False:
 				ssl_ctx.check_hostname = False
 				ssl_ctx.verify_mode = ssl.CERT_NONE
 			else:
 				if self.cacert is not None:
 					ssl_ctx.load_verify_locations(cafile=self.__cacertfilename)
```

### Comparing `asysocks-0.2.5/asysocks/unicomm/protocol/http.py` & `asysocks-0.2.7/asysocks/unicomm/protocol/http.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/protocol/quic.py` & `asysocks-0.2.7/asysocks/unicomm/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/protocol/socks4.py` & `asysocks-0.2.7/asysocks/unicomm/protocol/socks4.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/protocol/socks4a.py` & `asysocks-0.2.7/asysocks/unicomm/protocol/socks4a.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/unicomm/protocol/socks5.py` & `asysocks-0.2.7/asysocks/unicomm/protocol/socks5.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/utils/mbedtlswrapper.py` & `asysocks-0.2.7/asysocks/utils/mbedtlswrapper.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks/utils/sslwrapper.py` & `asysocks-0.2.7/asysocks/utils/sslwrapper.py`

 * *Files identical despite different names*

### Comparing `asysocks-0.2.5/asysocks.egg-info/SOURCES.txt` & `asysocks-0.2.7/asysocks.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 asysocks/__init__.py
 asysocks/_version.py
 asysocks/certmanager.py
 asysocks/client.py
 asysocks/security.py
 asysocks/server.py
@@ -69,12 +70,15 @@
 asysocks/unicomm/common/scanner/targetgen.py
 asysocks/unicomm/protocol/__init__.py
 asysocks/unicomm/protocol/http.py
 asysocks/unicomm/protocol/quic.py
 asysocks/unicomm/protocol/socks4.py
 asysocks/unicomm/protocol/socks4a.py
 asysocks/unicomm/protocol/socks5.py
+asysocks/unicomm/protocol/server/__init__.py
+asysocks/unicomm/protocol/server/udp.py
 asysocks/unicomm/utils/__init__.py
+asysocks/unicomm/utils/genselfsigned.py
 asysocks/unicomm/utils/paramprocessor.py
 asysocks/utils/__init__.py
 asysocks/utils/mbedtlswrapper.py
 asysocks/utils/sslwrapper.py
```

### Comparing `asysocks-0.2.5/setup.py` & `asysocks-0.2.7/setup.py`

 * *Files identical despite different names*

