# Comparing `tmp/yog-2.2.0.tar.gz` & `tmp/yog-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.2.0.tar", max compression
+gzip compressed data, was "yog-2.2.1.tar", max compression
```

## Comparing `yog-2.2.0.tar` & `yog-2.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.0/README.md
--rw-r--r--   0        0        0      541 2023-05-30 01:28:33.283278 yog-2.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.0/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.0/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.0/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.0/yog/host/__init__.py
--rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.0/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.0/yog/host/main.py
--rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/manage.py
--rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/necronomicon.py
--rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/os_utils.py
--rw-r--r--   0        0        0    12621 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/pki.py
--rw-r--r--   0        0        0      775 2023-05-30 01:28:33.283278 yog-2.2.0/yog/host/pki_model.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.0/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.0/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.0/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.0/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.0/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.0/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.0/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.0/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.0/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.0/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      185 2023-02-22 04:11:12.414451 yog-2.2.0/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.0/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    11024 2023-05-30 01:28:33.283278 yog-2.2.0/yog/ssh_utils.py
--rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.1/README.md
+-rw-r--r--   0        0        0      541 2023-05-30 01:34:07.618585 yog-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.1/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.1/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.1/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.1/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.1/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.1/yog/host/main.py
+-rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.1/yog/host/manage.py
+-rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.1/yog/host/necronomicon.py
+-rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.1/yog/host/os_utils.py
+-rw-r--r--   0        0        0    12646 2023-05-30 01:33:34.834403 yog-2.2.1/yog/host/pki.py
+-rw-r--r--   0        0        0      775 2023-05-30 01:33:34.817736 yog-2.2.1/yog/host/pki_model.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.1/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.1/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.1/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.1/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.1/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.1/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.1/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.1/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.1/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.1/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.1/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.1/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    11024 2023-05-30 01:28:33.283278 yog-2.2.1/yog/ssh_utils.py
+-rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.1/PKG-INFO
```

### Comparing `yog-2.2.0/README.md` & `yog-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/pyproject.toml` & `yog-2.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.2.0"
+version = "2.2.1"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
```

### Comparing `yog-2.2.0/yog/git_utils.py` & `yog-2.2.1/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/host/docker_attrs.py` & `yog-2.2.1/yog/host/docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/host/manage.py` & `yog-2.2.1/yog/host/manage.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/host/necronomicon.py` & `yog-2.2.1/yog/host/necronomicon.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/host/os_utils.py` & `yog-2.2.1/yog/host/os_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/host/pki.py` & `yog-2.2.1/yog/host/pki.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     builder = builder.subject_name(x509.Name([
         x509.NameAttribute(NameOID.COMMON_NAME, ca.ident),
     ]))
     builder = builder.issuer_name(x509.Name([
         x509.NameAttribute(NameOID.COMMON_NAME, ca.ident),
     ]))
     builder = builder.not_valid_before(datetime.datetime.utcnow())
-    builder = builder.not_valid_after(datetime.datetime.utcnow()+datetime.timedelta(days=ca.validity_days))
+    builder = builder.not_valid_after(datetime.datetime.utcnow()+datetime.timedelta(days=parse_validity_period(ca.validity_period)))
     serial_no = uuid.uuid4()
     builder = builder.serial_number(int(serial_no))
     builder = builder.public_key(public_key)
     builder = builder.add_extension(
         x509.BasicConstraints(ca=True, path_length=None), critical=True,
     )
     certificate = builder.sign(
```

### Comparing `yog-2.2.0/yog/host/pki_model.py` & `yog-2.2.1/yog/host/pki_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from yog.model_utils import HostPathStr, parse_hostpath
 
 
 class CAEntry(t.NamedTuple):
     ident: str
     storage: HostPathStr
-    validity_period: int
+    validity_period: str
 
 
 def parse_validity_period(s: str) -> int:
     if s.endswith("y"):
         return 365 * int(s[:-1])
     elif s.endswith("d"):
         return int(s[:-1])
```

### Comparing `yog-2.2.0/yog/host/test_docker_attrs.py` & `yog-2.2.1/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/logging_utils.py` & `yog-2.2.1/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/repo/main.py` & `yog-2.2.1/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/res/docker_test.yml` & `yog-2.2.1/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/yog/ssh_utils.py` & `yog-2.2.1/yog/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.0/PKG-INFO` & `yog-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yog
-Version: 2.2.0
+Version: 2.2.1
 Summary: The Gate and Key
 License: AGPLv3
 Author: Josh Hertlein
 Author-email: jmhertlein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

