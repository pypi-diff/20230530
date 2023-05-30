# Comparing `tmp/yog-2.2.1.tar.gz` & `tmp/yog-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.2.1.tar", max compression
+gzip compressed data, was "yog-2.2.2.tar", max compression
```

## Comparing `yog-2.2.1.tar` & `yog-2.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.1/README.md
--rw-r--r--   0        0        0      541 2023-05-30 01:34:07.618585 yog-2.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.1/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.1/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.1/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.1/yog/host/__init__.py
--rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.1/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.1/yog/host/main.py
--rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.1/yog/host/manage.py
--rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.1/yog/host/necronomicon.py
--rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.1/yog/host/os_utils.py
--rw-r--r--   0        0        0    12646 2023-05-30 01:33:34.834403 yog-2.2.1/yog/host/pki.py
--rw-r--r--   0        0        0      775 2023-05-30 01:33:34.817736 yog-2.2.1/yog/host/pki_model.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.1/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.1/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.1/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.1/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.1/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.1/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.1/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.1/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.1/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.1/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.1/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.1/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    11024 2023-05-30 01:28:33.283278 yog-2.2.1/yog/ssh_utils.py
--rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.2/README.md
+-rw-r--r--   0        0        0      541 2023-05-30 01:38:39.692291 yog-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.2/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.2/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.2/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.2/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.2/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.2/yog/host/main.py
+-rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.2/yog/host/manage.py
+-rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.2/yog/host/necronomicon.py
+-rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.2/yog/host/os_utils.py
+-rw-r--r--   0        0        0    12656 2023-05-30 01:38:07.588127 yog-2.2.2/yog/host/pki.py
+-rw-r--r--   0        0        0      752 2023-05-30 01:36:44.675981 yog-2.2.2/yog/host/pki_model.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.2/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.2/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.2/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.2/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.2/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.2/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.2/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.2/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.2/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.2/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.2/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.2/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    11024 2023-05-30 01:28:33.283278 yog-2.2.2/yog/ssh_utils.py
+-rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.2/PKG-INFO
```

### Comparing `yog-2.2.1/README.md` & `yog-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/pyproject.toml` & `yog-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.2.1"
+version = "2.2.2"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
```

### Comparing `yog-2.2.1/yog/git_utils.py` & `yog-2.2.2/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/host/docker_attrs.py` & `yog-2.2.2/yog/host/docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/host/manage.py` & `yog-2.2.2/yog/host/manage.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/host/necronomicon.py` & `yog-2.2.2/yog/host/necronomicon.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/host/os_utils.py` & `yog-2.2.2/yog/host/os_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/host/pki.py` & `yog-2.2.2/yog/host/pki.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def cert_names(self) -> t.List[str]:
         e: x509.SubjectAlternativeName = self.crt().extensions.get_extension_for_class(x509.SubjectAlternativeName).value
         return e.get_values_for_type(x509.DNSName)
 
     def issuer_cn(self) -> str:
         return self.crt().issuer.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
 
-    def write(self, ssh: SSHClient, path: str, owner: t.Optional[Owner], perms: t.Optional[Perms]):
+    def write(self, ssh: SSHClient, path: str, owner: t.Optional[Owner]=None, perms: t.Optional[Perms]=None):
         mkdirp(ssh, path, "root")
         for km in self.materials():
             put(ssh, os.path.join(path, km.fname), km.body,
                 user=owner.user if owner else None,
                 group=owner.group if owner else None,
                 mode=("600" if km.mattype == "private" else perms.to_chmod_expr() if perms else "644"))
         put(ssh, os.path.join(path, "issuer_serial.txt"), str(self.issuer_serial), "root")
```

### Comparing `yog-2.2.1/yog/host/pki_model.py` & `yog-2.2.2/yog/host/pki_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     elif s.endswith("d"):
         return int(s[:-1])
     else:
         raise ValueError(f"Invalid validity period: needs to end in y or d: {s}")
 
 
 def load_caentry(raw: t.Any) -> CAEntry:
-    return CAEntry(raw["ident"], parse_hostpath(raw["storage"]), parse_validity_period(str(raw["validity_period"])))
+    return CAEntry(raw["ident"], parse_hostpath(raw["storage"]), str(raw["validity_period"]))
 
 
 def load_cas(path: str) -> t.List[CAEntry]:
     with open(path, "r") as fin:
         raw = yaml.safe_load(fin.read())
     return [load_caentry(re) for re in raw]
```

### Comparing `yog-2.2.1/yog/host/test_docker_attrs.py` & `yog-2.2.2/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/logging_utils.py` & `yog-2.2.2/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/repo/main.py` & `yog-2.2.2/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/res/docker_test.yml` & `yog-2.2.2/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/yog/ssh_utils.py` & `yog-2.2.2/yog/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.1/PKG-INFO` & `yog-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yog
-Version: 2.2.1
+Version: 2.2.2
 Summary: The Gate and Key
 License: AGPLv3
 Author: Josh Hertlein
 Author-email: jmhertlein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

