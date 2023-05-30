# Comparing `tmp/intra42-0.1.1.tar.gz` & `tmp/intra42-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intra42-0.1.1.tar", last modified: Fri May 26 17:46:30 2023, max compression
+gzip compressed data, was "intra42-0.1.2.tar", last modified: Tue May 30 15:22:35 2023, max compression
```

## Comparing `intra42-0.1.1.tar` & `intra42-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-26 17:46:30.087753 intra42-0.1.1/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-26 17:46:30.087753 intra42-0.1.1/PKG-INFO
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-26 17:46:30.083753 intra42-0.1.1/intra42.egg-info/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/PKG-INFO
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/SOURCES.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/dependency_links.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/requires.txt
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-26 17:46:30.000000 intra42-0.1.1/intra42.egg-info/top_level.txt
-drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-26 17:46:30.087753 intra42-0.1.1/intrascraper/
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      105 2023-05-26 17:24:40.000000 intra42-0.1.1/intrascraper/__init__.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5539 2023-05-26 17:34:19.000000 intra42-0.1.1/intrascraper/intrascraper.py
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-26 17:46:30.087753 intra42-0.1.1/setup.cfg
--rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-26 17:46:24.000000 intra42-0.1.1/setup.py
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 15:22:35.556726 intra42-0.1.2/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 15:22:35.556726 intra42-0.1.2/PKG-INFO
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 15:22:35.556726 intra42-0.1.2/intra42.egg-info/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      222 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/PKG-INFO
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      216 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/SOURCES.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)        1 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/dependency_links.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/requires.txt
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       13 2023-05-30 15:22:35.000000 intra42-0.1.2/intra42.egg-info/top_level.txt
+drwxrwxr-x   0 reclaire  (1000) reclaire  (1000)        0 2023-05-30 15:22:35.556726 intra42-0.1.2/intrascraper/
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      259 2023-05-30 15:15:57.000000 intra42-0.1.2/intrascraper/__init__.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)     5693 2023-05-30 15:15:22.000000 intra42-0.1.2/intrascraper/intrascraper.py
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)       38 2023-05-30 15:22:35.556726 intra42-0.1.2/setup.cfg
+-rw-rw-r--   0 reclaire  (1000) reclaire  (1000)      437 2023-05-30 15:22:33.000000 intra42-0.1.2/setup.py
```

### Comparing `intra42-0.1.1/intrascraper/intrascraper.py` & `intra42-0.1.2/intrascraper/intrascraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import requests
 from bs4 import BeautifulSoup, ResultSet
-import bs4
 import urllib.parse
 import urllib
 import typing
 from urllib import parse
 import typing
-import re
 
 KEYCLOAK = "https://profile.intra.42.fr/users/auth/keycloak_student"
 SEND_FORM = "https://auth.42.fr/auth/realms/students-42/login-actions/authenticate"
 
 class Token(typing.TypedDict):
 	cookie:str
 	expires:int
@@ -169,7 +167,10 @@
 			data={"authenticity_token":auth_token, "gitlab_user[public_key]":new_key, "gitlab_user[name]":key_name})
 	return (x)
 
 def get_clusters_map(scraper:IntraScraper = SCRAPER) -> requests.Response:
 	return scraper.do_request(requests.get, "https://meta.intra.42.fr/clusters")
 
 
+def get_location_data(login:str, scraper:IntraScraper = SCRAPER):
+	return scraper.do_request(requests.get, f"https://profile.intra.42.fr/users/{login}/locations_stats.json")
+
```

