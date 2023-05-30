# Comparing `tmp/pylibagent-0.1.9.tar.gz` & `tmp/pylibagent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibagent-0.1.9.tar", last modified: Sun Dec 25 20:50:14 2022, max compression
+gzip compressed data, was "pylibagent-0.2.0.tar", last modified: Tue May 30 10:04:26 2023, max compression
```

## Comparing `pylibagent-0.1.9.tar` & `pylibagent-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-12-25 20:50:14.009963 pylibagent-0.1.9/
--rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 pylibagent-0.1.9/LICENSE
--rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2022-12-25 20:50:14.009963 pylibagent-0.1.9/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)     2617 2022-12-05 07:42:14.000000 pylibagent-0.1.9/README.md
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-12-25 20:50:14.005963 pylibagent-0.1.9/pylibagent/
--rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-07-04 09:31:51.000000 pylibagent-0.1.9/pylibagent/__init__.py
--rw-rw-r--   0 joente    (1000) joente    (1000)    11960 2022-12-25 20:48:08.000000 pylibagent-0.1.9/pylibagent/agent.py
--rw-rw-r--   0 joente    (1000) joente    (1000)      823 2022-11-15 14:58:49.000000 pylibagent-0.1.9/pylibagent/check.py
--rw-rw-r--   0 joente    (1000) joente    (1000)     1576 2022-11-18 11:52:45.000000 pylibagent-0.1.9/pylibagent/logger.py
--rw-rw-r--   0 joente    (1000) joente    (1000)       22 2022-12-25 20:49:20.000000 pylibagent-0.1.9/pylibagent/version.py
-drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2022-12-25 20:50:14.005963 pylibagent-0.1.9/pylibagent.egg-info/
--rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2022-12-25 20:50:13.000000 pylibagent-0.1.9/pylibagent.egg-info/PKG-INFO
--rw-rw-r--   0 joente    (1000) joente    (1000)      301 2022-12-25 20:50:13.000000 pylibagent-0.1.9/pylibagent.egg-info/SOURCES.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)        1 2022-12-25 20:50:13.000000 pylibagent-0.1.9/pylibagent.egg-info/dependency_links.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2022-12-25 20:50:13.000000 pylibagent-0.1.9/pylibagent.egg-info/requires.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       11 2022-12-25 20:50:13.000000 pylibagent-0.1.9/pylibagent.egg-info/top_level.txt
--rw-rw-r--   0 joente    (1000) joente    (1000)       38 2022-12-25 20:50:14.009963 pylibagent-0.1.9/setup.cfg
--rw-rw-r--   0 joente    (1000) joente    (1000)     1550 2022-11-16 21:18:12.000000 pylibagent-0.1.9/setup.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.944541 pylibagent-0.2.0/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.932541 pylibagent-0.2.0/.github/
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.936541 pylibagent-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      535 2022-02-17 12:20:07.000000 pylibagent-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 joente    (1000) joente    (1000)      595 2022-02-17 12:20:07.000000 pylibagent-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.940541 pylibagent-0.2.0/.github/workflows/
+-rw-rw-r--   0 joente    (1000) joente    (1000)      685 2022-11-15 21:09:32.000000 pylibagent-0.2.0/.github/workflows/ci.yml
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1799 2022-02-17 09:45:16.000000 pylibagent-0.2.0/.gitignore
+-rw-rw-r--   0 joente    (1000) joente    (1000)    35149 2022-07-05 11:43:02.000000 pylibagent-0.2.0/LICENSE
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2023-05-30 10:04:26.944541 pylibagent-0.2.0/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)     2617 2022-12-05 07:42:14.000000 pylibagent-0.2.0/README.md
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.944541 pylibagent-0.2.0/pylibagent/
+-rw-rw-r--   0 joente    (1000) joente    (1000)        0 2022-07-04 09:31:51.000000 pylibagent-0.2.0/pylibagent/__init__.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)    12918 2023-05-30 09:48:07.000000 pylibagent-0.2.0/pylibagent/agent.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)      823 2022-11-15 14:58:49.000000 pylibagent-0.2.0/pylibagent/check.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1576 2022-11-18 11:52:45.000000 pylibagent-0.2.0/pylibagent/logger.py
+-rw-rw-r--   0 joente    (1000) joente    (1000)       22 2023-05-30 09:48:48.000000 pylibagent-0.2.0/pylibagent/version.py
+drwxrwxr-x   0 joente    (1000) joente    (1000)        0 2023-05-30 10:04:26.944541 pylibagent-0.2.0/pylibagent.egg-info/
+-rw-rw-r--   0 joente    (1000) joente    (1000)     3506 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/PKG-INFO
+-rw-rw-r--   0 joente    (1000) joente    (1000)      433 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/SOURCES.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)        1 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/dependency_links.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/requires.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       11 2023-05-30 10:04:26.000000 pylibagent-0.2.0/pylibagent.egg-info/top_level.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       66 2022-11-16 21:17:54.000000 pylibagent-0.2.0/requirements.txt
+-rw-rw-r--   0 joente    (1000) joente    (1000)       38 2023-05-30 10:04:26.944541 pylibagent-0.2.0/setup.cfg
+-rw-rw-r--   0 joente    (1000) joente    (1000)     1550 2022-11-16 21:18:12.000000 pylibagent-0.2.0/setup.py
```

### Comparing `pylibagent-0.1.9/LICENSE` & `pylibagent-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibagent-0.1.9/PKG-INFO` & `pylibagent-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylibagent
-Version: 0.1.9
+Version: 0.2.0
 Summary: Library for building InfraSonar agents
 Home-page: https://github.com/infrasonar/python-libagent
-Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.1.9
+Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.2.0
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,agent
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pylibagent-0.1.9/README.md` & `pylibagent-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pylibagent-0.1.9/pylibagent/agent.py` & `pylibagent-0.2.0/pylibagent/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,22 +92,43 @@
                 logging.info(f'created agent {name} (Id: {self.asset_id})')
                 return
 
             url = _join(self.api_uri, f'asset/{self.asset_id}')
             async with ClientSession(headers=self._headers) as session:
                 async with session.get(
                         url,
-                        params={'field': 'name'},
+                        params={'fields': 'name', 'collectors': 'key'},
                         ssl=self.verify_ssl) as r:
                     if r.status != 200:
                         msg = await r.text()
                         raise Exception(f'{msg} (error code: {r.status})')
 
                     resp = await r.json()
                     name = resp["name"]
+                    collectors = resp["collectors"]
+
+            for collector in collectors:
+                if collector['key'] == self.key:
+                    break
+            else:
+                # The collector is not assigned yet
+                url = _join(
+                    self.api_uri,
+                    f'asset/{self.asset_id}/collector/{self.key}')
+                try:
+                    async with ClientSession(headers=self._headers) as session:
+                        async with session.post(url, ssl=self.verify_ssl) as r:
+                            if r.status != 204:
+                                msg = await r.text()
+                                raise Exception(
+                                    f'{msg} (error code: {r.status})')
+                except Exception as e:
+                    msg = str(e) or type(e).__name__
+                    logging.error(f'failed to assign collector: {msg}')
+
             logging.info(f'announced agent {name} (Id: {self.asset_id})')
             return
 
         except Exception as e:
             msg = str(e) or type(e).__name__
             logging.error(f'announce failed: {msg}')
             exit(1)
```

### Comparing `pylibagent-0.1.9/pylibagent/check.py` & `pylibagent-0.2.0/pylibagent/check.py`

 * *Files identical despite different names*

### Comparing `pylibagent-0.1.9/pylibagent/logger.py` & `pylibagent-0.2.0/pylibagent/logger.py`

 * *Files identical despite different names*

### Comparing `pylibagent-0.1.9/pylibagent.egg-info/PKG-INFO` & `pylibagent-0.2.0/pylibagent.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pylibagent
-Version: 0.1.9
+Version: 0.2.0
 Summary: Library for building InfraSonar agents
 Home-page: https://github.com/infrasonar/python-libagent
-Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.1.9
+Download-URL: https://github.com/infrasonar/python-libagent/tarball/v0.2.0
 Author: Cesbit
 Author-email: info@cesbit.com
 License: UNKNOWN
 Keywords: monitoring,infrasonar,agent
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pylibagent-0.1.9/setup.py` & `pylibagent-0.2.0/setup.py`

 * *Files identical despite different names*

