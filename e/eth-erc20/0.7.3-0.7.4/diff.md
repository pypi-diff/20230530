# Comparing `tmp/eth-erc20-0.7.3.tar.gz` & `tmp/eth-erc20-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-erc20-0.7.3.tar", last modified: Sun Mar 26 07:09:10 2023, max compression
+gzip compressed data, was "eth-erc20-0.7.4.tar", last modified: Tue May 30 16:38:31 2023, max compression
```

## Comparing `eth-erc20-0.7.3.tar` & `eth-erc20-0.7.4.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.696661 eth-erc20-0.7.3/
--rw-r--r--   0 lash      (1000) lash      (1000)     1551 2023-03-22 12:35:51.000000 eth-erc20-0.7.3/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:00:05.000000 eth-erc20-0.7.3/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      153 2023-02-14 06:40:00.000000 eth-erc20-0.7.3/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-03-26 07:09:10.696661 eth-erc20-0.7.3/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 08:00:13.000000 eth-erc20-0.7.3/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 08:03:07.000000 eth-erc20-0.7.3/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/eth_erc20/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2021-05-02 11:58:48.000000 eth-erc20-0.7.3/eth_erc20/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/eth_erc20/data/
--rw-r--r--   0 lash      (1000) lash      (1000)     2605 2021-05-02 12:53:06.000000 eth-erc20-0.7.3/eth_erc20/data/ERC20.json
--rw-r--r--   0 lash      (1000) lash      (1000)     8888 2022-11-23 16:04:50.000000 eth-erc20-0.7.3/eth_erc20/erc20.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/eth_erc20/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     3703 2023-02-19 16:09:00.000000 eth-erc20-0.7.3/eth_erc20/runnable/balance.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3804 2023-02-13 06:39:32.000000 eth-erc20-0.7.3/eth_erc20/runnable/info.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3700 2022-11-06 10:30:18.000000 eth-erc20-0.7.3/eth_erc20/runnable/transfer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/eth_erc20.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-03-26 07:09:10.000000 eth-erc20-0.7.3/eth_erc20.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1067 2023-03-26 07:09:10.000000 eth-erc20-0.7.3/eth_erc20.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-26 07:09:10.000000 eth-erc20-0.7.3/eth_erc20.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      288 2023-03-26 07:09:10.000000 eth-erc20-0.7.3/eth_erc20.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-03-26 07:09:10.000000 eth-erc20-0.7.3/eth_erc20.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-03-26 07:09:10.000000 eth-erc20-0.7.3/eth_erc20.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/giftable_erc20_token/
--rw-r--r--   0 lash      (1000) lash      (1000)      119 2023-02-14 06:40:00.000000 eth-erc20-0.7.3/giftable_erc20_token/__init__.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/giftable_erc20_token/data/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-02-13 13:41:54.000000 eth-erc20-0.7.3/giftable_erc20_token/data/.chainlib
--rw-r--r--   0 lash      (1000) lash      (1000)    18930 2023-03-26 07:09:01.000000 eth-erc20-0.7.3/giftable_erc20_token/data/GiftableToken.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     6791 2023-03-26 07:09:01.000000 eth-erc20-0.7.3/giftable_erc20_token/data/GiftableToken.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2021-02-24 16:44:15.000000 eth-erc20-0.7.3/giftable_erc20_token/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5239 2023-03-21 20:26:30.000000 eth-erc20-0.7.3/giftable_erc20_token/factory.py
--rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-13 12:12:59.000000 eth-erc20-0.7.3/giftable_erc20_token/gen.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/giftable_erc20_token/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2803 2023-01-24 15:09:24.000000 eth-erc20-0.7.3/giftable_erc20_token/runnable/gift.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3431 2023-01-24 15:53:09.000000 eth-erc20-0.7.3/giftable_erc20_token/runnable/minter.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3255 2023-02-21 18:21:49.000000 eth-erc20-0.7.3/giftable_erc20_token/runnable/publish.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.696661 eth-erc20-0.7.3/giftable_erc20_token/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-21 17:44:31.000000 eth-erc20-0.7.3/giftable_erc20_token/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1677 2023-02-21 18:13:15.000000 eth-erc20-0.7.3/giftable_erc20_token/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-03-22 10:40:04.000000 eth-erc20-0.7.3/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1445 2023-03-26 07:09:10.696661 eth-erc20-0.7.3/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      666 2021-04-04 12:48:14.000000 eth-erc20-0.7.3/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.693328 eth-erc20-0.7.3/static_token/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.696661 eth-erc20-0.7.3/static_token/data/
--rw-r--r--   0 lash      (1000) lash      (1000)    11366 2023-03-02 11:29:39.000000 eth-erc20-0.7.3/static_token/data/StaticToken.bin
--rw-r--r--   0 lash      (1000) lash      (1000)     3288 2023-03-02 11:29:39.000000 eth-erc20-0.7.3/static_token/data/StaticToken.json
--rw-r--r--   0 lash      (1000) lash      (1000)       66 2022-04-22 18:28:18.000000 eth-erc20-0.7.3/static_token/data/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)       51 2021-05-02 12:00:59.000000 eth-erc20-0.7.3/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-03-26 07:09:10.696661 eth-erc20-0.7.3/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)      266 2023-02-23 08:04:58.000000 eth-erc20-0.7.3/tests/test_erc20_interface.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4318 2023-02-22 10:16:13.000000 eth-erc20-0.7.3/tests/test_giftable.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1642 2023-05-30 16:38:03.000000 eth-erc20-0.7.4/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 08:00:05.000000 eth-erc20-0.7.4/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      153 2023-02-14 06:40:00.000000 eth-erc20-0.7.4/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      869 2022-11-14 08:00:13.000000 eth-erc20-0.7.4/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 08:03:07.000000 eth-erc20-0.7.4/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2021-05-02 11:58:48.000000 eth-erc20-0.7.4/eth_erc20/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2605 2021-05-02 12:53:06.000000 eth-erc20-0.7.4/eth_erc20/data/ERC20.json
+-rw-r--r--   0 lash      (1000) lash      (1000)     8888 2022-11-23 16:04:50.000000 eth-erc20-0.7.4/eth_erc20/erc20.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3703 2023-02-19 16:09:00.000000 eth-erc20-0.7.4/eth_erc20/runnable/balance.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3804 2023-02-13 06:39:32.000000 eth-erc20-0.7.4/eth_erc20/runnable/info.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3700 2022-11-06 10:30:18.000000 eth-erc20-0.7.4/eth_erc20/runnable/transfer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-23 08:04:29.000000 eth-erc20-0.7.4/eth_erc20/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6489 2023-02-23 08:03:36.000000 eth-erc20-0.7.4/eth_erc20/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/eth_erc20.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      786 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1125 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      288 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       44 2023-05-30 16:38:31.000000 eth-erc20-0.7.4/eth_erc20.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/
+-rw-r--r--   0 lash      (1000) lash      (1000)      119 2023-02-14 06:40:00.000000 eth-erc20-0.7.4/giftable_erc20_token/__init__.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2023-05-08 04:03:57.000000 eth-erc20-0.7.4/giftable_erc20_token/data/.chainlib
+-rw-r--r--   0 lash      (1000) lash      (1000)    18930 2023-03-26 07:09:01.000000 eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     6791 2023-03-26 07:09:01.000000 eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2021-02-24 16:44:15.000000 eth-erc20-0.7.4/giftable_erc20_token/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5307 2023-05-30 16:30:35.000000 eth-erc20-0.7.4/giftable_erc20_token/factory.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      108 2023-02-13 12:12:59.000000 eth-erc20-0.7.4/giftable_erc20_token/gen.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2803 2023-01-24 15:09:24.000000 eth-erc20-0.7.4/giftable_erc20_token/runnable/gift.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3431 2023-01-24 15:53:09.000000 eth-erc20-0.7.4/giftable_erc20_token/runnable/minter.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3255 2023-02-21 18:21:49.000000 eth-erc20-0.7.4/giftable_erc20_token/runnable/publish.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/giftable_erc20_token/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-02-21 17:44:31.000000 eth-erc20-0.7.4/giftable_erc20_token/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1677 2023-05-05 07:48:30.000000 eth-erc20-0.7.4/giftable_erc20_token/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       69 2023-03-22 10:40:04.000000 eth-erc20-0.7.4/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1465 2023-05-30 16:38:31.866638 eth-erc20-0.7.4/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2021-04-04 12:48:14.000000 eth-erc20-0.7.4/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/static_token/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/static_token/data/
+-rw-r--r--   0 lash      (1000) lash      (1000)    11366 2023-03-02 11:29:39.000000 eth-erc20-0.7.4/static_token/data/StaticToken.bin
+-rw-r--r--   0 lash      (1000) lash      (1000)     3288 2023-03-02 11:29:39.000000 eth-erc20-0.7.4/static_token/data/StaticToken.json
+-rw-r--r--   0 lash      (1000) lash      (1000)       66 2022-04-22 18:28:18.000000 eth-erc20-0.7.4/static_token/data/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       51 2021-05-02 12:00:59.000000 eth-erc20-0.7.4/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-30 16:38:31.863305 eth-erc20-0.7.4/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)      266 2023-02-23 08:04:58.000000 eth-erc20-0.7.4/tests/test_erc20_interface.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4318 2023-02-22 10:16:13.000000 eth-erc20-0.7.4/tests/test_giftable.py
```

### Comparing `eth-erc20-0.7.3/CHANGELOG` & `eth-erc20-0.7.4/CHANGELOG`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+* 0.7.4
+	- Add missing unittest module to python package
+* 0.7.3
+	- Add ERC5679Ext20 fills
 * 0.7.2
 	- Update python classifiers
 	- Upgrade to beta
 * 0.7.1
 	- Upgrade deps
 * 0.7.0
 	- Implement proper burner interface method
```

### Comparing `eth-erc20-0.7.3/LICENSE` & `eth-erc20-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/PKG-INFO` & `eth-erc20-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc20
-Version: 0.7.3
+Version: 0.7.4
 Summary: ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 Home-page: https://git.defalsify.org/eth-erc20
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,ethereum,token,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-erc20-0.7.3/WAIVER` & `eth-erc20-0.7.4/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/WAIVER.asc` & `eth-erc20-0.7.4/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/eth_erc20/data/ERC20.json` & `eth-erc20-0.7.4/eth_erc20/data/ERC20.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/eth_erc20/erc20.py` & `eth-erc20-0.7.4/eth_erc20/erc20.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/eth_erc20/runnable/balance.py` & `eth-erc20-0.7.4/eth_erc20/runnable/balance.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/eth_erc20/runnable/info.py` & `eth-erc20-0.7.4/eth_erc20/runnable/info.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/eth_erc20/runnable/transfer.py` & `eth-erc20-0.7.4/eth_erc20/runnable/transfer.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/eth_erc20.egg-info/PKG-INFO` & `eth-erc20-0.7.4/eth_erc20.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-erc20
-Version: 0.7.3
+Version: 0.7.4
 Summary: ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 Home-page: https://git.defalsify.org/eth-erc20
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,ethereum,token,blockchain,cryptocurrency
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-erc20-0.7.3/eth_erc20.egg-info/SOURCES.txt` & `eth-erc20-0.7.4/eth_erc20.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 eth_erc20.egg-info/entry_points.txt
 eth_erc20.egg-info/requires.txt
 eth_erc20.egg-info/top_level.txt
 eth_erc20/data/ERC20.json
 eth_erc20/runnable/balance.py
 eth_erc20/runnable/info.py
 eth_erc20/runnable/transfer.py
+eth_erc20/unittest/__init__.py
+eth_erc20/unittest/base.py
 giftable_erc20_token/__init__.py
 giftable_erc20_token/factory.py
 giftable_erc20_token/gen.py
 giftable_erc20_token/data/.chainlib
 giftable_erc20_token/data/GiftableToken.bin
 giftable_erc20_token/data/GiftableToken.json
 giftable_erc20_token/data/__init__.py
```

### Comparing `eth-erc20-0.7.3/giftable_erc20_token/data/GiftableToken.bin` & `eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.bin`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/giftable_erc20_token/data/GiftableToken.json` & `eth-erc20-0.7.4/giftable_erc20_token/data/GiftableToken.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/giftable_erc20_token/factory.py` & `eth-erc20-0.7.4/giftable_erc20_token/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,17 @@
             expire = 0
         code = GiftableToken.bytecode(version=version)
         enc = ABIContractEncoder()
         enc.string(name)
         enc.string(symbol)
         enc.uint256(decimals)
         enc.uint256(expire)
-        code += enc.get()
+        args = enc.get()
+        code += args
+        logg.debug('constructor code: ' + args)
         return code
 
 
     @staticmethod
     def gas(code=None):
         return 2000000
```

### Comparing `eth-erc20-0.7.3/giftable_erc20_token/runnable/gift.py` & `eth-erc20-0.7.4/giftable_erc20_token/runnable/gift.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/giftable_erc20_token/runnable/minter.py` & `eth-erc20-0.7.4/giftable_erc20_token/runnable/minter.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/giftable_erc20_token/runnable/publish.py` & `eth-erc20-0.7.4/giftable_erc20_token/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/giftable_erc20_token/unittest/base.py` & `eth-erc20-0.7.4/giftable_erc20_token/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/setup.cfg` & `eth-erc20-0.7.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-erc20
-version = 0.7.3
+version = 0.7.4
 description = ERC20 interface and simple contract with deployment script that lets any address mint and gift itself tokens.
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-erc20
 keywords = 
 	dlt
 	ethereum
@@ -31,14 +31,15 @@
 	giftable_erc20_token
 	giftable_erc20_token.runnable
 	giftable_erc20_token.unittest
 	giftable_erc20_token.data
 	eth_erc20
 	eth_erc20.data
 	eth_erc20.runnable
+	eth_erc20.unittest
 	static_token.data
 
 [options.package_data]
 * = 
 	data/GiftableToken.json
 	data/GiftableToken.bin
 	data/StaticToken.json
```

### Comparing `eth-erc20-0.7.3/setup.py` & `eth-erc20-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/static_token/data/StaticToken.bin` & `eth-erc20-0.7.4/static_token/data/StaticToken.bin`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/static_token/data/StaticToken.json` & `eth-erc20-0.7.4/static_token/data/StaticToken.json`

 * *Files identical despite different names*

### Comparing `eth-erc20-0.7.3/tests/test_giftable.py` & `eth-erc20-0.7.4/tests/test_giftable.py`

 * *Files identical despite different names*

