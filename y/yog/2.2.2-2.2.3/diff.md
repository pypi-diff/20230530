# Comparing `tmp/yog-2.2.2.tar.gz` & `tmp/yog-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.2.2.tar", max compression
+gzip compressed data, was "yog-2.2.3.tar", max compression
```

## Comparing `yog-2.2.2.tar` & `yog-2.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.2/README.md
--rw-r--r--   0        0        0      541 2023-05-30 01:38:39.692291 yog-2.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.2/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.2/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.2/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.2/yog/host/__init__.py
--rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.2/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.2/yog/host/main.py
--rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.2/yog/host/manage.py
--rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.2/yog/host/necronomicon.py
--rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.2/yog/host/os_utils.py
--rw-r--r--   0        0        0    12656 2023-05-30 01:38:07.588127 yog-2.2.2/yog/host/pki.py
--rw-r--r--   0        0        0      752 2023-05-30 01:36:44.675981 yog-2.2.2/yog/host/pki_model.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.2/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.2/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.2/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.2/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.2/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.2/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.2/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.2/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.2/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.2/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.2/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.2/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    11024 2023-05-30 01:28:33.283278 yog-2.2.2/yog/ssh_utils.py
--rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.3/README.md
+-rw-r--r--   0        0        0      541 2023-05-30 01:54:05.386243 yog-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.3/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.3/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.3/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.3/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.3/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.3/yog/host/main.py
+-rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.3/yog/host/manage.py
+-rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.3/yog/host/necronomicon.py
+-rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.3/yog/host/os_utils.py
+-rw-r--r--   0        0        0    12672 2023-05-30 01:53:37.105511 yog-2.2.3/yog/host/pki.py
+-rw-r--r--   0        0        0      752 2023-05-30 01:36:44.675981 yog-2.2.3/yog/host/pki_model.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.3/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.3/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.3/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.3/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.3/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.3/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.3/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.3/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.3/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.3/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.3/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.3/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    11032 2023-05-30 01:53:37.125512 yog-2.2.3/yog/ssh_utils.py
+-rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.3/PKG-INFO
```

### Comparing `yog-2.2.2/README.md` & `yog-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/pyproject.toml` & `yog-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.2.2"
+version = "2.2.3"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
```

### Comparing `yog-2.2.2/yog/git_utils.py` & `yog-2.2.3/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/host/docker_attrs.py` & `yog-2.2.3/yog/host/docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/host/manage.py` & `yog-2.2.3/yog/host/manage.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/host/necronomicon.py` & `yog-2.2.3/yog/host/necronomicon.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/host/os_utils.py` & `yog-2.2.3/yog/host/os_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/host/pki.py` & `yog-2.2.3/yog/host/pki.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
                 log.debug("expiry too far out")
             elif cert.subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value != ce.names[0]:
                 generate = True
                 log.debug("CN != cert CN")
             elif ca_data.serial != cur_trust.issuer_serial:
                 generate = True
                 log.debug("CA serial != cert issuer serial")
-            elif ce.chown and any(ce.chown != m.owner for m in cur_trust.materials() if m.mattype != "private"):
+            elif ce.chown and any(Owner.from_str(ce.chown) != m.owner for m in cur_trust.materials() if m.mattype != "private"):
                 generate = True
                 log.debug("chown != current ownership")
             elif ce.chmod and any(Perms(*RWXBits.from_stat(ce.chmod)) != m.perms for m in cur_trust.materials() if m.mattype != "private"):
                 generate = True
                 log.debug("chmod != current perms")
         except ValueError:
             generate = True
```

### Comparing `yog-2.2.2/yog/host/pki_model.py` & `yog-2.2.3/yog/host/pki_model.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/host/test_docker_attrs.py` & `yog-2.2.3/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/logging_utils.py` & `yog-2.2.3/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/repo/main.py` & `yog-2.2.3/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/res/docker_test.yml` & `yog-2.2.3/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.2.2/yog/ssh_utils.py` & `yog-2.2.3/yog/ssh_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     cmd = _as_user(cmd, user)
     check_call(ssh, cmd)
 
 
 def stat(ssh: SSHClient, path: str) -> t.Tuple[Owner, Perms]:
     path = shlex.quote(path)
     # stat -c '%A %U:%G'
-    raw = check_output(ssh, f"stat -c {shlex.quote('%A %U:%G')} {path}")[0][0]
+    raw = check_output(ssh, f"stat -c {shlex.quote('%A %U:%G')} {path}")[0][0].strip()
     log.debug(f"stat: {path}: {raw}")
     perms, owner = raw.split(" ", 1)
     perms = perms[-9:]
 
     return Owner.from_str(owner), Perms(*RWXBits.from_stat(perms))
```

### Comparing `yog-2.2.2/PKG-INFO` & `yog-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yog
-Version: 2.2.2
+Version: 2.2.3
 Summary: The Gate and Key
 License: AGPLv3
 Author: Josh Hertlein
 Author-email: jmhertlein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

