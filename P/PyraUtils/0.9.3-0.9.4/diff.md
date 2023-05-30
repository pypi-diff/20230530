# Comparing `tmp/PyraUtils-0.9.3.tar.gz` & `tmp/PyraUtils-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyraUtils-0.9.3.tar", last modified: Fri May 26 08:10:09 2023, max compression
+gzip compressed data, was "PyraUtils-0.9.4.tar", last modified: Tue May 30 10:10:36 2023, max compression
```

## Comparing `PyraUtils-0.9.3.tar` & `PyraUtils-0.9.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.699196 PyraUtils-0.9.3/
--rw-rw-rw-   0        0        0      161 2023-05-11 08:15:40.000000 PyraUtils-0.9.3/AUTHORS.rst
--rw-rw-rw-   0        0        0     3666 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/HISTORY.rst
--rw-rw-rw-   0        0        0    11558 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1691 2023-05-26 08:10:09.699196 PyraUtils-0.9.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.617557 PyraUtils-0.9.3/PyraUtils/
--rw-rw-rw-   0        0        0      884 2023-05-26 08:10:05.000000 PyraUtils-0.9.3/PyraUtils/__init__.py
--rw-rw-rw-   0        0        0      427 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/PyraUtils/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.639559 PyraUtils-0.9.3/PyraUtils/common/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/common/__init__.py
--rw-rw-rw-   0        0        0     8511 2023-05-25 03:48:30.000000 PyraUtils-0.9.3/PyraUtils/common/_file.py
--rw-rw-rw-   0        0        0     1250 2023-05-17 03:59:30.000000 PyraUtils-0.9.3/PyraUtils/common/_ipaddress.py
--rw-rw-rw-   0        0        0     3988 2023-05-25 08:55:44.000000 PyraUtils-0.9.3/PyraUtils/common/_json.py
--rw-rw-rw-   0        0        0     1624 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/common/_shelve.py
--rw-rw-rw-   0        0        0    15416 2023-05-25 06:32:04.000000 PyraUtils-0.9.3/PyraUtils/common/_strings.py
--rw-rw-rw-   0        0        0     1878 2023-05-24 08:29:38.000000 PyraUtils-0.9.3/PyraUtils/common/_time.py
--rw-rw-rw-   0        0        0     3636 2023-04-10 07:43:32.000000 PyraUtils-0.9.3/PyraUtils/common/cert.py
--rw-rw-rw-   0        0        0     4641 2023-05-26 08:06:54.000000 PyraUtils-0.9.3/PyraUtils/common/download.py
--rw-rw-rw-   0        0        0     2271 2023-05-24 10:21:11.000000 PyraUtils-0.9.3/PyraUtils/common/password.py
--rw-rw-rw-   0        0        0     3856 2023-05-24 10:37:41.000000 PyraUtils-0.9.3/PyraUtils/common/rsync.py
--rw-rw-rw-   0        0        0     3119 2023-05-25 03:55:22.000000 PyraUtils-0.9.3/PyraUtils/common/signature.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.641560 PyraUtils-0.9.3/PyraUtils/db/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/db/__init__.py
--rw-rw-rw-   0        0        0     4414 2023-05-26 08:07:21.000000 PyraUtils-0.9.3/PyraUtils/db/_sqlalchemy.py
--rw-rw-rw-   0        0        0     2636 2023-05-25 08:44:56.000000 PyraUtils-0.9.3/PyraUtils/db/_sqlite3.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.644560 PyraUtils-0.9.3/PyraUtils/hash/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/hash/__init__.py
--rw-rw-rw-   0        0        0     4852 2023-05-24 11:13:34.000000 PyraUtils-0.9.3/PyraUtils/hash/_hashlib.py
--rw-rw-rw-   0        0        0     1587 2023-05-25 01:11:37.000000 PyraUtils-0.9.3/PyraUtils/hash/_hmac.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.648558 PyraUtils-0.9.3/PyraUtils/http/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/http/__init__.py
--rw-rw-rw-   0        0        0     5314 2023-05-26 08:07:39.000000 PyraUtils-0.9.3/PyraUtils/http/_httpx.py
--rw-rw-rw-   0        0        0     5291 2023-05-26 08:07:55.000000 PyraUtils-0.9.3/PyraUtils/http/_request.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.649557 PyraUtils-0.9.3/PyraUtils/log/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.651558 PyraUtils-0.9.3/PyraUtils/log/logger/
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/log/logger/__init__.py
--rw-rw-rw-   0        0        0     7733 2023-05-24 10:07:44.000000 PyraUtils-0.9.3/PyraUtils/log/logger/_logging.py
--rw-rw-rw-   0        0        0     1701 2023-05-11 09:53:45.000000 PyraUtils-0.9.3/PyraUtils/log/logger/_loguru.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.652558 PyraUtils-0.9.3/PyraUtils/service/
--rw-rw-rw-   0        0        0      754 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.655557 PyraUtils-0.9.3/PyraUtils/service/work_wechat/
--rw-rw-rw-   0        0        0     3079 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/service/work_wechat/AbstractApi.py
--rw-rw-rw-   0        0        0     3313 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/service/work_wechat/CorpApi.py
--rw-rw-rw-   0        0        0     7057 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/service/work_wechat/CorpApiType.py
--rw-rw-rw-   0        0        0    11253 2023-04-10 07:08:41.000000 PyraUtils-0.9.3/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py
--rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/PyraUtils/service/work_wechat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.632556 PyraUtils-0.9.3/PyraUtils.egg-info/
--rw-rw-rw-   0        0        0     1691 2023-05-26 08:10:09.000000 PyraUtils-0.9.3/PyraUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2023-05-26 08:10:09.000000 PyraUtils-0.9.3/PyraUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 08:10:09.000000 PyraUtils-0.9.3/PyraUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-25 10:07:15.000000 PyraUtils-0.9.3/PyraUtils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      361 2023-05-26 08:10:09.000000 PyraUtils-0.9.3/PyraUtils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-26 08:10:09.000000 PyraUtils-0.9.3/PyraUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-05-25 10:04:40.000000 PyraUtils-0.9.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.697192 PyraUtils-0.9.3/docs/
--rw-rw-rw-   0        0        0      632 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/authors.rst
--rw-rw-rw-   0        0        0     4961 2023-05-11 08:11:29.000000 PyraUtils-0.9.3/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/history.rst
--rw-rw-rw-   0        0        0      328 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/index.rst
--rw-rw-rw-   0        0        0     1173 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/installation.rst
--rwxrwxrwx   0        0        0      809 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/readme.rst
--rw-rw-rw-   0        0        0       84 2023-04-13 07:49:46.000000 PyraUtils-0.9.3/docs/usage.rst
--rw-rw-rw-   0        0        0      209 2023-05-12 07:01:34.000000 PyraUtils-0.9.3/pyproject.toml
--rw-rw-rw-   0        0        0     1913 2023-05-26 08:10:09.700195 PyraUtils-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0     1663 2022-04-21 03:55:13.000000 PyraUtils-0.9.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 08:10:09.698193 PyraUtils-0.9.3/tests/
--rw-rw-rw-   0        0        0     1065 2023-05-15 10:46:43.000000 PyraUtils-0.9.3/tests/test_download.py
--rw-rw-rw-   0        0        0      271 2023-05-25 07:23:03.000000 PyraUtils-0.9.3/tests/test_file.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.677339 PyraUtils-0.9.4/
+-rw-rw-rw-   0        0        0      161 2023-05-11 08:15:40.000000 PyraUtils-0.9.4/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3666 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/HISTORY.rst
+-rw-rw-rw-   0        0        0    11558 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1691 2023-05-30 10:10:36.678339 PyraUtils-0.9.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.588672 PyraUtils-0.9.4/PyraUtils/
+-rw-rw-rw-   0        0        0      884 2023-05-30 10:08:48.000000 PyraUtils-0.9.4/PyraUtils/__init__.py
+-rw-rw-rw-   0        0        0      427 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/PyraUtils/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.617162 PyraUtils-0.9.4/PyraUtils/common/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/common/__init__.py
+-rw-rw-rw-   0        0        0     8511 2023-05-25 03:48:30.000000 PyraUtils-0.9.4/PyraUtils/common/_file.py
+-rw-rw-rw-   0        0        0     1250 2023-05-17 03:59:30.000000 PyraUtils-0.9.4/PyraUtils/common/_ipaddress.py
+-rw-rw-rw-   0        0        0     3988 2023-05-25 08:55:44.000000 PyraUtils-0.9.4/PyraUtils/common/_json.py
+-rw-rw-rw-   0        0        0     1624 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/common/_shelve.py
+-rw-rw-rw-   0        0        0    15416 2023-05-25 06:32:04.000000 PyraUtils-0.9.4/PyraUtils/common/_strings.py
+-rw-rw-rw-   0        0        0     1878 2023-05-24 08:29:38.000000 PyraUtils-0.9.4/PyraUtils/common/_time.py
+-rw-rw-rw-   0        0        0     3636 2023-04-10 07:43:32.000000 PyraUtils-0.9.4/PyraUtils/common/cert.py
+-rw-rw-rw-   0        0        0     4653 2023-05-26 08:44:07.000000 PyraUtils-0.9.4/PyraUtils/common/download.py
+-rw-rw-rw-   0        0        0     2271 2023-05-24 10:21:11.000000 PyraUtils-0.9.4/PyraUtils/common/password.py
+-rw-rw-rw-   0        0        0     3856 2023-05-24 10:37:41.000000 PyraUtils-0.9.4/PyraUtils/common/rsync.py
+-rw-rw-rw-   0        0        0     3119 2023-05-25 03:55:22.000000 PyraUtils-0.9.4/PyraUtils/common/signature.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.619161 PyraUtils-0.9.4/PyraUtils/db/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/db/__init__.py
+-rw-rw-rw-   0        0        0     4418 2023-05-26 08:21:55.000000 PyraUtils-0.9.4/PyraUtils/db/_sqlalchemy.py
+-rw-rw-rw-   0        0        0     2636 2023-05-25 08:44:56.000000 PyraUtils-0.9.4/PyraUtils/db/_sqlite3.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.621163 PyraUtils-0.9.4/PyraUtils/hash/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/hash/__init__.py
+-rw-rw-rw-   0        0        0     4852 2023-05-24 11:13:34.000000 PyraUtils-0.9.4/PyraUtils/hash/_hashlib.py
+-rw-rw-rw-   0        0        0     1587 2023-05-25 01:11:37.000000 PyraUtils-0.9.4/PyraUtils/hash/_hmac.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.622163 PyraUtils-0.9.4/PyraUtils/http/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/http/__init__.py
+-rw-rw-rw-   0        0        0     5320 2023-05-26 08:43:25.000000 PyraUtils-0.9.4/PyraUtils/http/_httpx.py
+-rw-rw-rw-   0        0        0     5295 2023-05-26 08:42:52.000000 PyraUtils-0.9.4/PyraUtils/http/_request.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.623164 PyraUtils-0.9.4/PyraUtils/log/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.625162 PyraUtils-0.9.4/PyraUtils/log/logger/
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/log/logger/__init__.py
+-rw-rw-rw-   0        0        0     7733 2023-05-24 10:07:44.000000 PyraUtils-0.9.4/PyraUtils/log/logger/_logging.py
+-rw-rw-rw-   0        0        0     1701 2023-05-11 09:53:45.000000 PyraUtils-0.9.4/PyraUtils/log/logger/_loguru.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.625162 PyraUtils-0.9.4/PyraUtils/service/
+-rw-rw-rw-   0        0        0      754 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/service/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.628163 PyraUtils-0.9.4/PyraUtils/service/work_wechat/
+-rw-rw-rw-   0        0        0     3079 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/service/work_wechat/AbstractApi.py
+-rw-rw-rw-   0        0        0     3313 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/service/work_wechat/CorpApi.py
+-rw-rw-rw-   0        0        0     7057 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/service/work_wechat/CorpApiType.py
+-rw-rw-rw-   0        0        0    11253 2023-04-10 07:08:41.000000 PyraUtils-0.9.4/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py
+-rw-rw-rw-   0        0        0      756 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/PyraUtils/service/work_wechat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.609162 PyraUtils-0.9.4/PyraUtils.egg-info/
+-rw-rw-rw-   0        0        0     1691 2023-05-30 10:10:36.000000 PyraUtils-0.9.4/PyraUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-05-30 10:10:36.000000 PyraUtils-0.9.4/PyraUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 10:10:36.000000 PyraUtils-0.9.4/PyraUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-25 10:07:15.000000 PyraUtils-0.9.4/PyraUtils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      361 2023-05-30 10:10:36.000000 PyraUtils-0.9.4/PyraUtils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 10:10:36.000000 PyraUtils-0.9.4/PyraUtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-05-25 10:04:40.000000 PyraUtils-0.9.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.675336 PyraUtils-0.9.4/docs/
+-rw-rw-rw-   0        0        0      632 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/authors.rst
+-rw-rw-rw-   0        0        0     4961 2023-05-11 08:11:29.000000 PyraUtils-0.9.4/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/history.rst
+-rw-rw-rw-   0        0        0      328 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/index.rst
+-rw-rw-rw-   0        0        0     1173 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/installation.rst
+-rwxrwxrwx   0        0        0      809 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/readme.rst
+-rw-rw-rw-   0        0        0       84 2023-04-13 07:49:46.000000 PyraUtils-0.9.4/docs/usage.rst
+-rw-rw-rw-   0        0        0      209 2023-05-12 07:01:34.000000 PyraUtils-0.9.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1913 2023-05-30 10:10:36.683341 PyraUtils-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2022-04-21 03:55:13.000000 PyraUtils-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:10:36.677339 PyraUtils-0.9.4/tests/
+-rw-rw-rw-   0        0        0     1065 2023-05-15 10:46:43.000000 PyraUtils-0.9.4/tests/test_download.py
+-rw-rw-rw-   0        0        0      271 2023-05-25 07:23:03.000000 PyraUtils-0.9.4/tests/test_file.py
```

### Comparing `PyraUtils-0.9.3/CONTRIBUTING.rst` & `PyraUtils-0.9.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/LICENSE` & `PyraUtils-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PKG-INFO` & `PyraUtils-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyraUtils
-Version: 0.9.3
+Version: 0.9.4
 Summary: Common development utils.
 Home-page: https://www.920430.com/
 Author: pyra
 Author-email: ops@920430.com
 License: APACHE LICENSE, VERSION 2.0
 Project-URL: Documentation, https://www.920430.com/
 Project-URL: Release notes, https://www.920430.com/
```

### Comparing `PyraUtils-0.9.3/PyraUtils/__init__.py` & `PyraUtils-0.9.4/PyraUtils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
  * ```` ':.          ':::::::::'                  ::::..
  *                    '.:::::'                    ':'````..
 """
 
 
 __author__ = """PyraUtils"""
 __email__ = 'ops@920430.com'
-__version__ = '0.9.3'
+__version__ = '0.9.4'
```

### Comparing `PyraUtils-0.9.3/PyraUtils/common/__init__.py` & `PyraUtils-0.9.4/PyraUtils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/_file.py` & `PyraUtils-0.9.4/PyraUtils/common/_file.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/_ipaddress.py` & `PyraUtils-0.9.4/PyraUtils/common/_ipaddress.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/_json.py` & `PyraUtils-0.9.4/PyraUtils/common/_json.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/_shelve.py` & `PyraUtils-0.9.4/PyraUtils/common/_shelve.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/_strings.py` & `PyraUtils-0.9.4/PyraUtils/common/_strings.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/_time.py` & `PyraUtils-0.9.4/PyraUtils/common/_time.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/cert.py` & `PyraUtils-0.9.4/PyraUtils/common/cert.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/download.py` & `PyraUtils-0.9.4/PyraUtils/common/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,40 +27,40 @@
     def dl_01(url:str, dl_path:str, **kwargs) -> None:
         '''
         使用requests实现下载
         '''
         print(url)
         with open(dl_path, "wb") as f:
             try:
-                resp = requests.get(url, kwargs)
+                resp = requests.get(url, **kwargs)
                 f.write(resp.content)
             except (requests.HTTPError, requests.Timeout,
                     requests.exceptions.URLRequired) as err:
                 logger.error(err)
 
     @staticmethod
     def dl_02(url:str, dl_path:str, **kwargs) -> None:
         '''
         使用urllib3实现下载
         '''
         # 创建连接池管理器
         http = urllib3.PoolManager()
          # 发送请求并获取响应
-        response = http.request('GET', url, kwargs)
+        response = http.request('GET', url, **kwargs)
         # 读取响应内容并保存到文件中
         with open(dl_path, 'wb') as f:
             f.write(response.data)
 
 
     @staticmethod
     def dl_03(url:str, dl_path:str, **kwargs) -> None:
         '''
         使用requests实现下载,同时增加对特定情况下的判断
         '''
-        with closing(requests.get(url, kwargs)) as resp:
+        with closing(requests.get(url, **kwargs)) as resp:
             # 判断下载链接是否异常
             resp_code = resp.status_code
             if 299 < resp_code or resp_code < 200:
                 logger.warning('returnCode %s %s' % (resp_code, url))
 
             # 判断下载文件是否为0
             content_length = int(resp.headers.get('content-length', '0'))
@@ -77,15 +77,15 @@
     @staticmethod
     def dl_04(url:str, dl_path:str, **kwargs) -> None:
         '''
         使用requests实现下载,大文件专用
         '''
         with open(dl_path, "wb") as f:
             try:
-                resp = requests.get(url, kwargs)
+                resp = requests.get(url, **kwargs)
                 for chunk in resp.iter_content(chunk_size=1024,): 
                     f.write(chunk)
             except (requests.HTTPError, requests.Timeout,
                     requests.exceptions.URLRequired) as err:
                 logger.error(err)
 
 class DownloadProgressUtil:
@@ -97,15 +97,15 @@
     @staticmethod
     def dl_01(url, dl_path, **kwargs):
         '''
         进度条
         '''
         with open(dl_path, 'wb') as out_file:
             # 需要把kwargs作为一个字典传递给stream()方法，而不是一个位置参数
-            with httpx.stream("GET", url, kwargs) as resp:
+            with httpx.stream("GET", url, **kwargs) as resp:
                 total = int(resp.headers["Content-Length"])
 
                 with tqdm(total=total, unit_scale=True, unit_divisor=1024, unit="B") as progress:
                     num_bytes_downloaded = resp.num_bytes_downloaded
                     for chunk in resp.iter_bytes():
                         out_file.write(chunk)
                         progress.update(resp.num_bytes_downloaded - num_bytes_downloaded)
@@ -115,15 +115,15 @@
     @staticmethod
     def dl_02(url, dl_path, **kwargs):
         '''
         使用rich实现进度条
         '''
         with open(dl_path, 'wb') as out_file:
             # 需要把kwargs作为一个字典传递给stream()方法，而不是一个位置参数
-            with httpx.stream("GET", url, kwargs) as resp:
+            with httpx.stream("GET", url, **kwargs) as resp:
                 total = int(resp.headers["Content-Length"])
 
                 with rich.progress.Progress(
                     "[progress.percentage]{task.percentage:>3.0f}%",
                     rich.progress.BarColumn(bar_width=None),
                     rich.progress.DownloadColumn(),
                     rich.progress.TransferSpeedColumn(),) as progress:
```

### Comparing `PyraUtils-0.9.3/PyraUtils/common/password.py` & `PyraUtils-0.9.4/PyraUtils/common/password.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/rsync.py` & `PyraUtils-0.9.4/PyraUtils/common/rsync.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/common/signature.py` & `PyraUtils-0.9.4/PyraUtils/common/signature.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/db/__init__.py` & `PyraUtils-0.9.4/PyraUtils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/db/_sqlalchemy.py` & `PyraUtils-0.9.4/PyraUtils/db/_sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         session.close()
     
     def query(self, cls, **kwargs):
         # 查询对象
         # 创建会话对象
         session = self.Session()
         # 查询对象
-        result = session.query(cls).filter_by(kwargs).all()
+        result = session.query(cls).filter_by(**kwargs).all()
         # 关闭会话
         session.close()
         # 返回结果
         return result
     
     def update(self, cls, condition, **kwargs):
         # 更新对象
@@ -125,15 +125,15 @@
         session.close()
     
     def delete(self, cls, **kwargs):
         # 删除对象
         # 创建会话对象
         session = self.Session()
         # 查询对象
-        obj = session.query(cls).filter_by(kwargs).first()
+        obj = session.query(cls).filter_by(**kwargs).first()
         if obj:
             # 删除对象
             session.delete(obj)
             # 提交事务
             session.commit()
             print('Delete success')
         else:
```

### Comparing `PyraUtils-0.9.3/PyraUtils/db/_sqlite3.py` & `PyraUtils-0.9.4/PyraUtils/db/_sqlite3.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/hash/__init__.py` & `PyraUtils-0.9.4/PyraUtils/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/hash/_hashlib.py` & `PyraUtils-0.9.4/PyraUtils/hash/_hashlib.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/hash/_hmac.py` & `PyraUtils-0.9.4/PyraUtils/hash/_hmac.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/http/__init__.py` & `PyraUtils-0.9.4/PyraUtils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/http/_httpx.py` & `PyraUtils-0.9.4/PyraUtils/http/_httpx.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
         返回类型:
             bytes or str
         """
 
         try:
             with httpx.Client(timeout=kwargs.get('timeout')) as client:
-                resp = client.request(method, url, kwargs)
+                resp = client.request(method, url, **kwargs)
         except httpx.RequestError as err:
             raise err
 
         resp.raise_for_status()
         return resp.content
 
 
@@ -107,16 +107,16 @@
         self.limits = httpx.Limits(max_keepalive_connections=max_keepalive,
                                    max_connections=max_connections,
                                    keepalive_expiry=keepalive_expiry)
 
     def httpx_method(self, method, url, **kwargs) -> httpx.Response:
         with httpx.Client(http2=self.http2, proxies=self.proxies,
                           timeout=self.timeout, limits=self.limits) as client:
-            resp = client.request(method, url, kwargs)
+            resp = client.request(method, url, **kwargs)
         return resp
 
 
     async def async_method(self, method, url, **kwargs) -> httpx.Response:
         async with httpx.AsyncClient(http2=self.http2, proxies=self.proxies,
                                      timeout=self.timeout, limits=self.limits) as client:
-            resp = await client.request(method, url, kwargs)
+            resp = await client.request(method, url, **kwargs)
         return resp
```

### Comparing `PyraUtils-0.9.3/PyraUtils/http/_request.py` & `PyraUtils-0.9.4/PyraUtils/http/_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         返回:
             Response object
 
         返回类型:
             requests.Response
         """
         try:
-            resp = requests.request(method, url, kwargs)
+            resp = requests.request(method, url, **kwargs)
         except (requests.ConnectionError, requests.HTTPError,
                 requests.Timeout, requests.URLRequired) as err:
             raise RuntimeError(err)
         return resp
 
 
 class RequestsSessionUtil:
@@ -95,10 +95,10 @@
         返回类型:
             requests.Response
         """
         with requests.Session() as s:
             max_retries = requests.adapters.HTTPAdapter(max_retries=self.max_retries)
             s.mount('https://', max_retries)
             s.mount('http://', max_retries)
-            resp = s.request(method, url, kwargs)
+            resp = s.request(method, url, **kwargs)
         return resp
```

### Comparing `PyraUtils-0.9.3/PyraUtils/log/__init__.py` & `PyraUtils-0.9.4/PyraUtils/log/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/log/logger/__init__.py` & `PyraUtils-0.9.4/PyraUtils/log/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/log/logger/_logging.py` & `PyraUtils-0.9.4/PyraUtils/log/logger/_logging.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/log/logger/_loguru.py` & `PyraUtils-0.9.4/PyraUtils/log/logger/_loguru.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/service/__init__.py` & `PyraUtils-0.9.4/PyraUtils/service/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/service/work_wechat/AbstractApi.py` & `PyraUtils-0.9.4/PyraUtils/service/work_wechat/AbstractApi.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/service/work_wechat/CorpApi.py` & `PyraUtils-0.9.4/PyraUtils/service/work_wechat/CorpApi.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/service/work_wechat/CorpApiType.py` & `PyraUtils-0.9.4/PyraUtils/service/work_wechat/CorpApiType.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py` & `PyraUtils-0.9.4/PyraUtils/service/work_wechat/WXBizMsgCrypt3.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils/service/work_wechat/__init__.py` & `PyraUtils-0.9.4/PyraUtils/service/work_wechat/__init__.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/PyraUtils.egg-info/PKG-INFO` & `PyraUtils-0.9.4/PyraUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyraUtils
-Version: 0.9.3
+Version: 0.9.4
 Summary: Common development utils.
 Home-page: https://www.920430.com/
 Author: pyra
 Author-email: ops@920430.com
 License: APACHE LICENSE, VERSION 2.0
 Project-URL: Documentation, https://www.920430.com/
 Project-URL: Release notes, https://www.920430.com/
```

### Comparing `PyraUtils-0.9.3/PyraUtils.egg-info/SOURCES.txt` & `PyraUtils-0.9.4/PyraUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/docs/Makefile` & `PyraUtils-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/docs/conf.py` & `PyraUtils-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/docs/installation.rst` & `PyraUtils-0.9.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/docs/make.bat` & `PyraUtils-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/setup.cfg` & `PyraUtils-0.9.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 00000580: 616e 6420 7079 7468 6f6e 5f76 6572 7369  and python_versi
 00000590: 6f6e 206e 6f74 2069 6e20 2733 2e30 2c20  on not in '3.0, 
 000005a0: 332e 312c 2033 2e32 2c20 332e 332c 2033  3.1, 3.2, 3.3, 3
 000005b0: 2e34 2c20 332e 3527 0d0a 0970 7963 7279  .4, 3.5'...pycry
 000005c0: 7074 6f64 6f6d 653d 3d33 2e31 322e 300d  ptodome==3.12.0.
 000005d0: 0a09 7572 6c6c 6962 333d 3d32 2e30 2e32  ..urllib3==2.0.2
 000005e0: 0d0a 096c 6f67 7572 753d 3d30 2e37 2e30  ...loguru==0.7.0
-000005f0: 0d0a 096e 756d 7079 3d3d 312e 3133 2e31  ...numpy==1.13.1
+000005f0: 0d0a 096e 756d 7079 3d3d 312e 3234 2e33  ...numpy==1.24.3
 00000600: 0d0a 0973 7973 7273 796e 633d 3d31 2e31  ...sysrsync==1.1
 00000610: 2e31 0d0a 0977 6865 656c 3d3d 302e 3430  .1...wheel==0.40
 00000620: 2e30 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  .0....[flake8]..
 00000630: 6578 636c 7564 6520 3d20 6275 696c 642c  exclude = build,
 00000640: 2e67 6974 2c2e 746f 782c 2e2f 7465 7374  .git,.tox,./test
 00000650: 732f 2e65 6e76 2c50 6970 6669 6c65 2c50  s/.env,Pipfile,P
 00000660: 6970 6669 6c65 2e6c 6f63 6b2c 2e76 656e  ipfile.lock,.ven
```

### Comparing `PyraUtils-0.9.3/setup.py` & `PyraUtils-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `PyraUtils-0.9.3/tests/test_download.py` & `PyraUtils-0.9.4/tests/test_download.py`

 * *Files identical despite different names*

